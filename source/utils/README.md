## Introduction
###number
增加了方法bytesToSize；修改了注释

###dom
新增了这个文件，从table.js里提取出getSiblings，保留table.js作为其他组件的辅助工具

###browser
新增

###string
新增

###time
此文件中的getDynamicCls方法，与此文件专注于时间相关操作，不符合，建议适当的时候移出。


###upload
新增

###ajax
新增，修改以下内容：
去掉'../userinfo/'引用，增加一个常量ACCESS_TOKEN，增加一个方法removeAccessToken。
去掉去掉'../config/'引用，增加必须传入的基本配置信息：
const config ={
  code:"dc",
  ajaxPrefix: '/sms/api',
  url:{
    login:"",
     // iframe 父页面
     iframeP: '/pigeon/',
  },
  isRedirectLogin: true,
  useFrontCookie:true
};