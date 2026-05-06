# 寒武纪海洋巨型生物科普装置

这是适合部署到 GitHub Pages 并在 iPad Safari 中运行的静态网页版本。

## 使用方式

1. 打开网页。
2. 点击 `GEMINI API`，填写 Google AI Studio 的 Gemini API Key。
3. 在画布上用手指或 Apple Pencil 绘制简笔画。
4. 点击生成，程序会根据线稿生成寒武纪古生物艺术图像并给出形态分析。

API Key 只保存在当前浏览器的 `localStorage` 中，不会写入仓库。

## GitHub Pages 部署

将本目录内容推送到 GitHub 仓库后，在仓库设置中开启 Pages：

- Source: `Deploy from a branch`
- Branch: `main`
- Folder: `/root`

开启后，iPad 可以直接访问 GitHub Pages 地址运行。
