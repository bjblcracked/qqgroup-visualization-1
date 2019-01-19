# qqgroup-visualization

## QQ群关系可视化查询，3D力导向图
![效果图](https://github.com/gstok/qqgroup-visualization/blob/master/img/1.jpg)

![效果图](https://github.com/gstok/qqgroup-visualization/blob/master/img/2.jpg)

## 新的分支[table](https://github.com/gstok/qqgroup-visualization/tree/table)表格方式查询

![效果图](https://github.com/gstok/qqgroup-visualization/blob/master/img/t1.jpg)

## *本项目不提供数据库*

## 1.配置数据库（需要300GB以上磁盘剩余空间）
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
+ 数据库说明
    + 索引说明
        + 我没有修改数据，只是在QQ号字段以及群号字段上加了索引用来优化查询速度
    + 存储过程说明
        + queryByGroupNum 传入群号查询关联的力导向图数据
        + queryByQQNum 传入QQ号查询关联的力导向图数据
        + queryByQQNumExt 传入QQ号进行二层关联查询，得出力导向图数据
        + queryTableByGroupNum 传入群号查询群成员信息表
        + queryTableByQQNum 传入QQ号查询QQ加群信息表
+ 数据库SHA256
``` 数据库文件SHA256
名称: QQGroup.7z.001
大小: 4290772992 字节 (4092 MiB)
SHA256: F5E2C42140A892E14E56A0B1B839E36E80626B503547738817513513B957FA22

名称: QQGroup.7z.002
大小: 4290772992 字节 (4092 MiB)
SHA256: 6FFD307ED156A48E68E335CD2D3D6A80F447ABAA2BF257A1286444B268FAB1BE

名称: QQGroup.7z.003
大小: 4290772992 字节 (4092 MiB)
SHA256: F2DAFCB3BB4F8B872C36C27935D806AAA30A17D790427516011DFF4995EF11D1

名称: QQGroup.7z.004
大小: 4290772992 字节 (4092 MiB)
SHA256: 9CB364059153A5868306AEAF306B418F54F4C3DE02FD9E9B5C42A37857229AA4

名称: QQGroup.7z.005
大小: 4290772992 字节 (4092 MiB)
SHA256: CA43F7E3D68CCD34C9D449467B0611FBF96603202FA7C5A6BB00D29B953DF606

名称: QQGroup.7z.006
大小: 4290772992 字节 (4092 MiB)
SHA256: 49CF64A9B66D6AEB7681320A5C216EAE1961C005B4700D51525D5F06657171C9

名称: QQGroup.7z.007
大小: 4290772992 字节 (4092 MiB)
SHA256: 78747667D67E7C3D3BC55609342E84272637F32844C7F4D37986702126562CB9

名称: QQGroup.7z.008
大小: 4290772992 字节 (4092 MiB)
SHA256: 2FA3992951648B3185227FEE5121A9C40F41C09DB1E20C970B71047580BA8DAF

名称: QQGroup.7z.009
大小: 4290772992 字节 (4092 MiB)
SHA256: C940F4ABB3BB776B323306D0324998E5ED653CD8FB049B47075B531B70AD1C6B

名称: QQGroup.7z.010
大小: 152463434 字节 (145 MiB)
SHA256: 4DE4E3A0D44FDD4CE9D7EF15747C7516FDFBE10C96BEBDE1D5D98CE501BF1936
```
        
## 联系
+ QQ群（常有老司机飙车🚕）：943928860  
![QQ群二维码](https://github.com/gstok/qqgroup-visualization/blob/master/img/groupQRCode.jpg)  
+ 微信号：beijingxuesheng  
![微信号二维码](https://github.com/gstok/qqgroup-visualization/blob/master/img/myWeChatQRCode.jpeg)  

## 请作者吃酸菜鱼🍲
![微信支付](https://github.com/gstok/qqgroup-visualization/blob/master/img/wechatQRCode.png)  
![支付宝支付](https://github.com/gstok/qqgroup-visualization/blob/master/img/alipayQRCode.jpg)  

## 程序员装逼驿站公众号(一起来装逼吧🌚)
![支付宝支付](https://github.com/gstok/qqgroup-visualization/blob/master/img/gzhQRCode.jpg) 

