## 简介

基于webpack开发，搭建公司的项目，适合PC端的多页面开发。喜欢的话就star🌟一下咯。如有不妥的地方，还请指正，不胜感激。


## 项目背景

因为业务的需要，自己被抽调出来支持另外一个项目。然而，这个项目只有我一个前端，再然而，自己没有跟java的合作过。

他们的技术选型初期是，网页是使用多页面的，前端（我）这边是提供静态的网页给到他们，然后他们使用freemarker来进行数据的写入，然后有什么交互的话我再介入。让后自己就构造出了这么一个实现多页面的`webpack`项目。

昨天进行交流，现在是百分之六十确定上面的方案，不过这样他们后台的工作量就增多，而且好像我也用不到前端的框架。乘着设计还没给设计稿，然后我又新建了一个仓库[vue-cli_multipage](https://github.com/reng99/vue-cli_multipage)，用来探讨一下vue实现多页面应用。

-----------------分割线--------------------

在这两天的搭建[vue-cli_multipage](https://github.com/reng99/vue-cli_multipage)项目中，自己深深感到用vue实现的mpa页面的恶意，混合的东西还是很多，对于多页面来说是个头疼的问题。原谅自己的水平有限，后期回头再看看[vue-cli_multipage](https://github.com/reng99/vue-cli_multipage)。因为在这方面的种种问题，还是使用现在的这个搭建好的`webpack`项目来支持公司的业务（最多要减轻后端压力的话，自己再学点`freemarker`语法），因为`webpack`项目是自己纯手动搭建的，不像`vue-cli`脚手架搭建mpa，出了什么问题那我就有的背锅了。:blush:


## 项目地址

[https://github.com/reng99/webpack](https://github.com/reng99/webpack)



## 使用方法

```

# 下载代码
$ git clone https://github.com/reng99/webpack.git

# 安装依赖
$ npm install

# 开发模式
$ npm run dev

# 检查语法(此步骤可省略，因为在开发的过程中已经检查)
$ npm run lint

# 生产模式
$ npm run build
[注意，在生产模式中，使用到的第三方的资源需要额外在vendor文件夹中按需引用,建议引用相关的CDN(Content Delivery Network 【内容分发网络】)来进行前端优化]

```

## 优化历史(optimation 文件夹中)

1. [提交到github忽略node_modules等文件](./optimization/gitignore.md)

2. [支持es6语法](./optimization/supportEs6.md)

3. [团队ide中editorconfig规范](./optimization/editorconfig.md)

4. [添加服务器外部可以访问](./optimization/devhost.md)

5. [添加eslint规范代码](./optimization/eslint.md)



## plugins选讲

- [webpack-merge](https://npm.taobao.org/package/webpack-merge) --> it provides a `merge` function that concatenates(联系) arrays and merges objects creating a new object.

- [uglifyjs-webpack-plugin](https://doc.webpack-china.org/plugins/uglifyjs-webpack-plugin/) --> uglify js

- [plugin ProvidePlugin](https://webpack.github.io/docs/shimming-modules.html#plugin-provideplugin) --> This plugin makes a module availble as a variable in `every` module is required only you use the variable.


## vendor 引用

- [jQuery](https://jquery.com/) --> jQuery is a fast,small,and feature-rich Javascript library.It makes things like HTML document traversal and manipulation,event handling,and Ajax much simpler with an easy-to-use API that works across a multitude of browers.With a combination of versatility,jQuery has changed the way thar millions of people write Javascript.

- [lodash](https://lodash.com/) --> A modern JavaScript utility library delivering modularity(模块化),performance & extras. 类似[underscore](http://underscorejs.org/)


## 仓库说明

- 本仓库用到的代码是自己学习中总结的

- 本仓库用到的图片是自己在谷歌浏览器上运行的截图

- 本仓库中部分文字引用出自网络，如有侵权，请与我联系--1837895991@qq.com 。我会在第一时间删除。


## 相关参考

- [webpack官网](http://webpack.github.io/)

- [eslint配置](http://eslint.org/docs/user-guide/configuring)

