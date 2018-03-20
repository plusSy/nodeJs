## NodeJs安装工程:
### 安装nodeJs
- 打开nodeJs官网 `https://nodejs.org/en/` 选择适合自己电脑版本的安装包进行下载,一路回车即可。
- 打开Terminal窗口输入`node -v` 和 `npm -v` 检测安装版本
### 创建一个nodejs工程
- 打开 Terminal 窗口,全局安装 express 模块: `npm install express -g`
- 全局安装 express-generator 模块: `npm install express-generator -g`
- 输入`express --version` 检测是否安装成功
- 新建一个工作文件夹,输入`express helloword` 创建一个 helloword 工程,输出目录为下
```js
      create : helloword
      create : helloword/package.json
      create : helloword/app.js
      create : helloword/public
      create : helloword/routes
      create : helloword/routes/index.js
      create : helloword/routes/users.js
      create : helloword/views
      create : helloword/views/index.jade
      create : helloword/views/layout.jade
      create : helloword/views/error.jade
      create : helloword/bin
      create : helloword/bin/www
      create : helloword/public/javascripts
      create : helloword/public/images
      create : helloword/public/stylesheets
      create : helloword/public/stylesheets/style.css
```
接着执行:`cd helloword && npm install`, npm 会根据 package.json 进行依赖安装,之后项目中会多出 node_moduless 文件夹,里面会有 express 和 jade 两个模块

```
目录介绍:
  bin: 项目的启动文件,也可以放置其他脚本
  node_moduless: 用来存放项目的依赖库
  public: 用来存放项目的静态文件(css, js, img)
  routes: 路由控制器
  views: 视图目录(相当于mvcz中的v)
  app.js: 项目入口及程序启动文件
  package.json: 包描述文件以及开发者信息
---------- 其他目录,自己创建时使用 ----------
  models: 数据模型(相当于mvc中的m)
  controllers: 控制器,对请求的操作(相当于mvc中的c)
  config: 配置目录
  test: 测试目录
  README.md: 项目说明文件
```
### 执行`DEBUG=helloword:* npm start  ||  node app.js`启动项目
### 打开浏览器,输入默认地址:`http://localhost:3000` 页面输出:
```
  Express
  Welcome to Express
```


NodeJsApi手册: https://nodejs.org/dist/latest-v8.x/docs/api

Express4.xAPI中文手册: http://www.expressjs.com.cn/4x/api.com
