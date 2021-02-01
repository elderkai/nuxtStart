# y

> Nuxt.js project

## Build Setup

``` bash
# install dependencies
$ npm install # Or yarn install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, checkout the [Nuxt.js docs](https://github.com/nuxt/nuxt.js).
参考地址：https://www.cnblogs.com/e-cat/p/9134448.html
首先，本机需要有node环境，这边不再阐述（均在命令行进行）。

1.安装vue-cli脚手架

npm install vue-cli -g
查看是否安装成功

vue -V
2.首先创建项目存放位置，即项目名称（盘符自选）

mkdir appName
3.进入项目目录，初始化Nuxt.js项目

cd appName
vue init nuxt/starter
会询问你项目的名称、作者之类的信息，自行填写。

4.安装依赖包

npm install

5.启动服务

npm run dev

目录结构
```
|-- .nuxt                            // Nuxt自动生成，临时的用于编辑的文件，build
|-- assets                           // 用于组织未编译的静态资源入LESS、SASS 或 JavaScript
|-- components                       // 用于自己编写的Vue组件，比如滚动组件，日历组件，分页组件
|-- layouts                          // 布局目录，用于组织应用的布局组件，不可更改。
|-- middleware                       // 用于存放中间件
|-- pages                            // 用于存放写的页面，我们主要的工作区域
|-- plugins                          // 用于存放JavaScript插件的地方
|-- static                           // 用于存放静态资源文件，比如图片
|-- store                            // 用于组织应用的Vuex 状态管理。
|-- .editorconfig                    // 开发工具格式配置
|-- .eslintrc.js                     // ESLint的配置文件，用于检查代码格式
|-- .gitignore                       // 配置git不上传的文件
|-- nuxt.config.json                 // 用于组织Nuxt.js应用的个性化配置，已覆盖默认配置
|-- package-lock.json                // npm自动生成，用于帮助package的统一性设置的，yarn也有相同的操作
|-- package-lock.json                // npm自动生成，用于帮助package的统一性设置的，yarn也有相同的操作
|-- package.json                     // npm包管理配置文件
```
1.配置IP和端口号

修改项目根目录package.json文件（如下图）

![Image text](https://images2018.cnblogs.com/blog/1324387/201806/1324387-20180604171849223-1550445835.png)

Nuxt.js对路由进行了封装，无需像vue一样配置route/index.js，是自动生成的在目录/.nuxt/router.js。

当我们创建完页面，会发现目录/.nuxt/router.js文件已经自动生成路由。多级路由后面再说。

打包：npm run generate

打包后需要在服务器环境才能查看效果哦
