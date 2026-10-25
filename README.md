# 前任消除器 Ex Eraser

上传合照，点一下要消失的人，AI 在浏览器本地把 TA 抠成手撕纸剪影，再在剪影里写一句话。照片不上传。

纯静态站点：`index.html` 是全部代码；`vision_bundle.js` / `vision_wasm_internal.*` 是 MediaPipe Tasks Vision 运行时（wasm 拆成两段是为了上传限制，页面加载时会拼回去）；`efficientdet_lite0.wasm`、`magic_touch.wasm` 是 Apache-2.0 的检测/抠人模型（内容是 .tflite）。
