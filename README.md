# TodoList

## 前言


一个简单的<span style="font-weight:800;color:skyblue;font-size:20px">TodoList</span>(📝记录待办事项)小项目，支持云端同步功能(需要注册账号并且登陆)，前端使用<span style="font-weight:800;color:skyblue;font-size:20px">React</span>框架和<span style="font-weight:800;color:skyblue;font-size:20px">Antd</span>组件库构建，后端使用<span style="font-weight:800;color:skyblue;font-size:20px">SSM</span>框架连接<span style="font-weight:800;color:skyblue;font-size:20px">MySQL</span>数据库，<span style="font-weight:600;color:skyblue;font-size:20px">前后端分离</span>的WEB小项目

使用到的设计模式

- 对象传输模式
- 拦截过滤器模式
- MVC模式
- 控制反转模式
- 依赖注入模式

软件架构为

- 分层架构

## 功能

- 不登陆的时候，支持使用本地存储记录待办事项，无需和数据库连接
- 提供注册和登陆选项，注册并登陆后可享用云存储，对待办事项的增删改查都会同步到数据库
- 具体功能：查询，新增，修改，删除，全选，批量删除基本操作

## 技术栈

前端：React

后端：SSM框架

数据库：MySQL(8.0.28)

## 项目运行

**由于前端涉及大量的 ES6/7 等新属性，node 需要 6.0 以上版本**

下载项目

`git clone https://gitee.com/xiaohugitee/todo-list.git`

### 前端

```
cd todo-list/todo_page

npm i

npm run start

```

### 数据库

创建todo数据库，并运行根目录下的`todo.sql`文件创建表

### 后端

使用idea打开`todo_server`文件夹，打开项目的`pom`刷新下载项目所需依赖

安装`Maven Help`插件用来启动项目

<img src="https://gitee.com/xiaohugitee/todo-list/raw/master/pic/mavenhelp.png" alt="image-20221229161656137" style="zoom:50%;float:left" />

右键点击项目选择`run maven`,再选择`tomcat7:run`运行项目即可启动，无需配置tomcat，该项目使用的是maven中的tomcat插件，如果端口冲突可手动修改相关的配置:在pom文件的最下方,如下所示

<img src="https://gitee.com/xiaohugitee/todo-list/raw/master/pic/2022-12-29_20-02-42.png" alt="image-2022-12-29_20-02-42" style="zoom:50%;float:left" />



## 部分截图

> 图片来源于本窗口中的pic文件，部分图片来源于我的github图床，可能加载失败

<img src="https://raw.githubusercontent.com/redyouzi/images-for-blog/main/img02/202212291624352.png" alt="image-20221229162427138" style="zoom:50%;" />

<img src="https://gitee.com/xiaohugitee/todo-list/raw/master/pic/202212291626101.png" alt="image-20221229162633065" style="zoom:50%;" />

<img src="https://gitee.com/xiaohugitee/todo-list/raw/master/pic/202212291627183.png" alt="image-20221229162738126" style="zoom:50%;" />

> 后端对手机号和密码都进行了MD5加密之后存储到数据库，保证了信息的安全

<img src="https://gitee.com/xiaohugitee/todo-list/raw/master/pic/202212291628096.png" alt="image-20221229162827045" style="zoom:50%;" />
