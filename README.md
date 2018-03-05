<!-- TOC depthFrom:1 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->

			- [目录结构](目录结构)
			- [规范及约束](#规范及约束)
			- [构建说明](#构建说明)
			- [上线流程](#上线流程)
			- [测试机调试部署](#测试机调试部署)
			- [本地调试方法](#本地调试方法)
			- [数据规范及协议和文档链接](#数据规范及协议和文档链接) 

<!-- /TOC -->----------
#### <i class="icon-folder-open"></i>目录结构
```
.
|- src (源代码目录)
	|- common --目录(通用模块目录，包括js，css等)
	|- components --展示组件目录(可视化组件，包括js、模板、样式、图片等)
		|- header(header组件)
			|- header.js
			|- header.less
	|- containers --容器组件目录(展示组件容器，可以用于redux于组件的绑定)
		|- header(header组件)
			|- header.js
			|- header.less
	|- page --目录(页面目录)
		|-index.html -- 首页
		|-index.js-- 首页js文件
		|-index.scss-- 首页样式
	|- router --目录(webapp路由设置)
		|-index.js-- 路由js文件
	|- store --目录(redux目录包括，store，actin，reducer)
		|-index.js-- store的js文件
		|-action -- action 目录
			|-actions -- 具体的action 目录
			|-types -- action的types 目录
			|-index.js --action 的js文件
		|-reducer-- reducer 目录
			|-index.js --reducer 的js文件
			|-reducers --具体的reducer 的js文件
|- dist --目录(构建后目录，用于上线)
|- dev --目录(调试目录，用于本地调试)
|- node_moudles -- 安装的npm包 可以忽略
|- config -- 打包配置目录
    |- webpack.config.js -- webpack打包基础配置文件
    |- webpack.dev.js -- webpack dev打包配置文件
    |- webpack.prod.js -- webpack build打包配置文件
|- package.json -- 纪录基本信息 包括模块依赖关系
|- README.md -- 项目基本介绍
```

----------

####规范及约束
使用后端blade模板渲染，需要搭建php环境
>使用模块化组织方式，单独的js、css可以为一个模块，可视化组件为一个模块，包括js、css、模板和图片等
>接口地址：http://cwiki.guazi-corp.com/pages/viewpage.action?pageId=11218555
> 产品需求：http://cwiki.guazi-corp.com/pages/viewpage.action?pageId=11209607
####构建说明
初始化
>npm install -d

开发模式
>npm run dev

部署测试机模式
>npm run staging

线上构建模式
>npm run build

####上线流程
>线上域名:

>线上机器:

>部署目录:
####测试机调试部署
####本地调试方法
####数据规范及协议和文档链接
