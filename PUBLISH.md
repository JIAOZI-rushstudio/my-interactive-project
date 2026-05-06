# 发布到 GitHub Pages

当前目录已经是可发布的静态站点 git 仓库。

## 方式一：安装 GitHub CLI 后发布

安装并登录 GitHub CLI 后，在本目录运行：

```bash
gh auth login
gh repo create radiodonta-ipad-app --public --source=. --remote=origin --push
gh api repos/:owner/radiodonta-ipad-app/pages -f source.branch=main -f source.path=/
```

如果仓库已经存在，则运行：

```bash
git remote add origin https://github.com/你的用户名/radiodonta-ipad-app.git
git push -u origin main
```

然后在 GitHub 仓库的 `Settings -> Pages` 中选择：

- Source: `Deploy from a branch`
- Branch: `main`
- Folder: `/root`

## 方式二：GitHub 网页上传

1. 在 GitHub 创建一个新仓库。
2. 上传本目录中的所有文件和文件夹。
3. 在 `Settings -> Pages` 中启用 Pages，选择 `main / root`。

Pages 发布完成后，iPad Safari 直接打开 GitHub Pages 地址即可运行。
