# 文档服务器手册
该服务器主要功能是,当指定gitbook仓库收到提交时,自动将其部署到web服务器中.

服务器信息和具体部署位置,参见QQ群公告

## 连接服务器
 需要一个SSH连接工具,推荐[MobaXterm](http://mobaxterm.mobatek.net/)

## 步骤
1. 在TssRequirement的organization中创建仓库
2. clone仓库,在 `.git`同级目录执行`gitbook init`
3. 提交
4. http://115.29.184.56:10000/html 中即可查看到编译好的网页
