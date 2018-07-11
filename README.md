##  sunny 后台管理系统开发框架 前端【1.0】

功能介绍：

0，免费开源

1，真正的前后端分离，让专业的人做专业的事情

2，清爽强大的界面 来自HTTP://www.layui.com

3，开发简单，不需要学习新的标准和琐碎的新语法，前台基于layui后台使用thinkphp

4，这是第一个版本，只有简单功能，作者会不断更新

5，感谢界内专业人士提出宝贵意见

##  安装说明
可以把项目文件放在服务器目录的任意文件夹，
然后去config.js 配置后台接口的地址，要求地址必须写到后台框架的public目录下，例如http:///www.example.com/项目名/pbulic/（如果你的后端没有指向到public目录），如果已经指向public目录则直接写http://www.example.com/ ,无论哪种方式写地址时都要在最后加上/
如果你有前台程序，需要在config.js中填入相应的域名就可以在后台通过菜单跳转到前台了，当然了根据你开发的系统类型，这个可选的
配置好后就可以访问 项目所在目录/start/ 如果没有弹窗报错说明接口正常

> 默认的前后端是可以分别放到不同的服务器，在开发中为了解决跨域中session共享的问题，你的每一个ajax请求都要添加一个参数如下:
        xhrFields: {
           withCredentials: true
       }
>如果你不需要跨域就可以忽略
##  后台前端目录结构
    web  WEB部署目录（或者子目录）
    ├─dist                 应用目录
    │  ├─controller        js模块目录
    │  ├─lib               扩展目录
    │  │  ├─extend         扩展js库文件
    │  │  └─ ...           其他文件
    │  ├─style             样式定义文件
    │  │  ├─res            资源文件夹
    │  ├─view              前端界面目录
    │  │  │...             html文件
    │  ├─config.js         前端配置文件
    │  └─index.js          js入口文件
    └─start                前端入口
        ├─layui            layui核心文件
        └─index.html       网站入口html
 
> 前端页面尽量都写到view中
> 具体前端页面的开发请移步www.layui.com 
