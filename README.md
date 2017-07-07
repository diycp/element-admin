# 欢迎使用

> 本项目不定时更新。


## 开始构建

``` bash
# 安装依赖
npm install

# 本地调试，浏览器访问：http://localhost:8888
npm run dev

# 生产编译
npm run build

# 报告分析
npm run build --report

# 单元测试
npm run unit
```


## 目录结构

```bash
├── /build/          # 发布目录
├── /config/         # 配置目录
├── /node_modules/   # 依赖模块
├── /src/            # 源码目录
│ ├── /assets/       # 资源文件
│ ├── /components/   # 组件文件
│ ├── /mock/         # 模拟测试
│ ├── /router/       # 路由配置
│ │ └── index.js     # 路由入口
│ ├── /utils/        # 工具函数
│ ├── /view/         # 页面视图
│ ├── app.vue        # 应用组件
│ └── main.js        # 程序入口
├── static/          # 静态资源
├── test/            # 测试目录
│ ├── /e2e/          # e2e 测试
│ ├── /unit/         # 单元测试
├── .babelrc         # Babel 配置
├── .editorconfig    # Editor 配置
├── .eslintignore    # ESLint 忽略文件
├── .eslintrc.js     # ESLint 配置
├── .gitignore       # Git 忽略文件
├── .postcssrc.js    # PostCSS 配置
├── index.html       # 主页入口
├── package.json     # Webpack 配置
└── README.md        # 自述文件
```


## 许可协议

MIT License

Copyright (c) 2017 Vultur

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
