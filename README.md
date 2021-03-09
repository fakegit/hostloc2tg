### ***hostloc新帖推送机***

###### 简介：

迫于每次有活动都喝不上汤，特意搞了一个自动监视脚本，推送新帖到telegram的机器人，稍后有空补上推送到微信（微信已废，懒得修改了）。

目前已开通了推送频道，可自行点击查看推送效果：https://t.me/hostloc2tg

###### 更新说明

2021.03.09 增加api模式，获取最新帖子和推送新帖分离，最新帖子更新地址：https://cherbim.ml 每次请求会获得最新20个帖子

2020.07.20 网站加了js验证，针对js验证进行更新，采取抓取手机版的方法绕过js验证

###### 使用说明：

本脚本为python3脚本，需依赖环境requests，lxml，torequests，js2py等库，第74行bot api需要改为自己bot api，118行需要修改推送id, 机器人每15秒更新一次

**需要注册tg机器人，若要推送到频道，请将机器人添加到频道，并给予管理员权限**

###### api版本使用方法

安装依赖库 pip3 install requests， 然后修改你自己机器人的bot api token和chat id（代码65 66行），然后后台运行

nohup python3 -u hostloc2tg_api.py >> hostloc.txt 2>&1 &





效果图：

![](https://s1.ax1x.com/2020/07/20/UfQihF.png)


