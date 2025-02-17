# hospital-web

## 介绍
该项目是基于Vue+webpack+Vuex+elementUI+scss开发设计的一个后台管理系统；该系统觉得分为医生管
理员和系统管理员；医生管理员能做的事情是查看自己被患者挂号的情况，可以通过日期查看自己出诊时患者
以往的病历以及在出诊时使用管理系统进行点击当前就诊的是哪位患者，并为患者在小程序端查看就诊队列
起到决定性作用；系统管理员主要是对医院、专科、医生、排版等进行所需要的管理如增删查改等；

## 软件架构
该项目是使用Vue+webpack+Vuex进行代码压缩管理等；同时样式使用scss进行编写，前端UI库使用的是
elementUI进行设计的；同时使用webpack代理表进行跨域处理；所有的表格都是通过调用表格组件进行
数据处理的，同时api接口也是经过模块化封装调用；

## 安装教程
1. 首先在当前页面使用克隆将前端代码克隆到编译器中，并使用npm install进行安装依赖；
2. 使用npm run build 便能会在dist文件夹中查看到压缩后的文件；
3. 接着运行前端代码npm run dev；
4. 目前只有账号admin 密码admin；

### npm install 报错，Error: Can't find Python executable "python", you can set the PYTHON env variable.

**解决方案：**

```npm
npm config set sass_binary_site https://npm.taobao.org/mirrors/node-sass/
npm install node-sass
```

## 使用说明
1. 首先每个账号及密码都是系统管理员赋予的，不能自行进行创建；
2. 医生管理员通过输入自己的指定账号和初始化密码进行，只能看到自己的患者和出诊情况，同时可以
进行密码的修改；
3. 医生管理员在出诊当天能对患者进行就诊处理，平时可以查看患者的以往就诊情况，查看过往病历等；
4. 系统管理员能对医院、专科门诊、医生等进行管理，系统管理员的权限最大，根据系统管理员设置的
医院、专科门诊、医生之间的关系环环相扣，之间相互依赖，同时系统管理员还要进行排版等；

