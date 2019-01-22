# qqgroup-visualization

## QQ群关系可视化查询，3D力导向图
![效果图](https://github.com/gstok/qqgroup-visualization/blob/master/img/1.jpg)

![效果图](https://github.com/gstok/qqgroup-visualization/blob/master/img/2.jpg)

## 新的分支[table](https://github.com/gstok/qqgroup-visualization/tree/table)表格方式查询

![效果图](https://github.com/gstok/qqgroup-visualization/blob/master/img/t1.jpg)

## *本项目仅供学习，不提供数据库！*

## 1.配置数据库（需要300GB以上磁盘剩余空间）
+ 该数据库在2018年十月更新，之前的数据库一概不能用
+ 下载并安装SqlServer2008R2(注意，不能是Expores版本，最好是企业版否则会有数据库大小限制)，配置好用户名以及登录密码，如果远程连接数据库的话，需配置数据库允许远程登录（SqlServer数据库配置请自行搜索教程）
+ 下载数据库备份文件
+ 解压下载的压缩包，得到数据库备份文件，恢复数据库备份文件到SqlServer（SqlServer恢复数据库恢复操作请自行搜索教程）

## 2.搭建服务端（需要支持Nodejs的操作系统，CPU1核以上剩余内存1GB以上）
+ 下载安装[Node.js](https://nodejs.org/en/)环境
+ npm全局安装webpack和webpack-dev-server
``` bash
# 全局安装webpack
npm install webpack -g

# 全局安装webpack-dev-server
npm install webpack-dev-server -g
```
## 3.配置数据库连接
+ 进入项目目录下
+ 打开db.json文件
+ 修改其中的数据库连接信息为自己的数据库连接信息（默认的数据库连接信息是我本人的服务器上的数据库，不保证可用）
+ db.json例子
``` json
{
    "server": "服务器地址",
    "database": "数据库名称",
    "user": "请输入用户名",
    "password": "请输入数据库用户密码"
}
```

## 4.运行
+ 进入项目目录下
``` bash
# 安装依赖
npm install

# 运行系统
npm run start
```

## 操作系统要求
+ 因为使用的数据库是SqlServer数据库，所以推荐使用Windows操作系统
+ 当然服务端使用的是Node，如果你连接到的是远程的SqlServer数据库的话，是可以使用任何支持Node的系统的

## 数据库说明
+ 数据库请使用SqlServer2008R2或更新版本的SqlServer
        
## 联系
+ QQ群（常有老司机飙车🚕）：943928860  
![QQ群二维码](https://github.com/gstok/qqgroup-visualization/blob/master/img/groupQRCode.jpg)  
+ 微信号：beijingxuesheng  
![微信号二维码](https://github.com/gstok/qqgroup-visualization/blob/master/img/myWeChatQRCode.jpeg)  

## 请作者吃酸菜鱼🍲
![微信支付](https://github.com/gstok/qqgroup-visualization/blob/master/img/wechatQRCode.png)  
![支付宝支付](https://github.com/gstok/qqgroup-visualization/blob/master/img/alipayQRCode.jpg)  

## 程序员装逼驿站公众号(一起来装逼吧🌚)
![公众号](https://github.com/gstok/qqgroup-visualization/blob/master/img/gzhQRCode.jpg) 

