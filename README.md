# Learning three.js

本文实例都基于 [r157](https://github.com/mrdoob/three.js/releases/tag/r157) 版本进行构建。

`three.js` 是一个简单易用、轻量、跨浏览器、通用的 `JavaScript 3D` 库。目前默认使用 `[WebGL](https://www.khronos.org/webgl/)` 作为底层图形渲染引擎，但此外还可选择 `[WebGPU](https://www.w3.org/TR/webgpu/#intro)`、`SVG` 和 `CSS3D` 进行渲染。


## 快速搭建本地 Web 服务器

### 基于 Python 搭建

```Shell
# 在项目目录下执行命令
cd examples/001-project-structure-demo
python -m SimpleHTTPServer
```

### 基于 NodeJS 搭建

```Shell
npm install -g http-server

# 在项目目录下执行命令
cd examples/001-project-structure-demo
http-server
```

## 下载安装

https://threejs.org/docs/index.html#manual/en/introduction/Installation

### 项目结构

`three.js` 并没有强制项目结构，但是推荐的项目结构如下：

```
# HTML 文件来定义网页骨架
index.html
# JS 文件来定义 three.js 逻辑
main.js
# public 目录来放置静态文件，如模型、音频、纹理等
public/
```

### 基于 NPM 管理所需依赖 & 基于 Vite 管理开发环境

```Shell
# three.js
npm install --save three

# vite
npm install --save-dev vite
```

# 参考

1. https://threejs-journey.com/lessons/local-server#
2. https://vitejs.dev/guide/cli.html
3. https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Understanding_client-side_tools/Package_management