# 字迹台 · 截图词频统计

纯静态线上工具。图片和 PDF 在浏览器中通过 PDF.js / Tesseract.js 处理。普通网页链接优先由浏览器直接读取；被跨域限制时，会通过 Jina Reader 提取网页正文。

## 使用

直接打开 `index.html`，或把整个文件夹上传到 Netlify Drop / Cloudflare Pages Direct Upload。

支持 PNG、JPG、WEBP、BMP、PDF，以及任意普通网页、图片或 PDF URL；支持批量 OCR、网页正文提取、完整词频、自定义关键词、来源页面、搜索与 CSV 导出。

PDF 会优先读取内嵌文字；没有文字层的扫描页才会转成图片 OCR。首次 OCR 需要联网加载简体中文与英文语言模型。单个远程图片/PDF 上限 50 MB；Jina Reader 未登录调用受其公开速率限制。
