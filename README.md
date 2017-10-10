# Puppeteer 个人补丁版

## 项目说明
Puppeteer 缺乏某些 API，自己动手添加一些。这不是一个准备良好维护的公共项目。放在 GitHub 只是为了方便 npm 下载。

[原项目说明文档](./_README_.md)

## API

### Page.goto(url, options)

#### options>waitUntil>contentload

等待页面事件 [DOMContentLoaded](https://developer.mozilla.org/en-US/docs/Web/Events/DOMContentLoaded) 触发时马上返回页面。代码实质是响应 Devtools Protocol 的 [Page.domContentEventFired](https://chromedevtools.github.io/devtools-protocol/tot/Page/#event-domContentEventFired) 事件。
