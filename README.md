# suaniao — 可变字体工具

在浏览器中调整字形比例、笔画粗细和画布切分，并导出 SVG 或录制动态效果。

## 使用

1. 输入英文字母、数字或支持的符号。
2. 使用滑轨调整字高、切分位置、最大笔画粗细和粗细焦点。
3. 调整 CANVAS 的列数与行数，或选择预设布局。
4. 点击画布或拖动切分线，改变每个字符的画布比例。
5. 点击 **SVG** 下载矢量文件；点击 **RECORD** 开始录制，再点击 **STOP** 下载 WebM 视频。录制需要浏览器支持 Canvas captureStream 和 MediaRecorder。

页面打开时会随机展示两个字符。所有绘制与导出均在浏览器内完成。

## 本地运行

直接用浏览器打开 `index.html`，或在项目目录运行：

```sh
python3 -m http.server 8000
```

然后访问 <http://localhost:8000>。

## GitHub Pages

这是一个无构建依赖的静态页面。GitHub Pages 的发布来源设为 **Deploy from a branch**，选择 **main** 分支和 **/(root)** 目录。

根目录中的 `.nojekyll` 用于直接发布静态文件。以后推送到 `main` 分支的更新会自动触发部署。
