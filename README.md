> 博客地址：[程序猿刘川枫](http://liujian.cool)
>
> 博客gitHub源码地址：[https://github.com/liujianview/myBlog](https://github.com/liujianview/myBlog)
>
> 博客gitee源码地址：[https://gitee.com/liuchuanfengview/myBlog](https://gitee.com/liuchuanfengview/myBlog)
>
> 欢迎给个star鼓励一下~

## 1.写前感悟

&emsp;&emsp;自打工作以来，一直就想着搭建一个属于自己的个人博客网站，可以记录工作中遇到问题的解决办法，可以记录学习的一些新技术，亦可以记录自己工作生活中的随笔感悟等等。说了这么多，其实就是有了个人博客以后会感觉很牛，哈哈哈哈，一般大佬都有个人博客（优秀的人总是乐忠于分享）。之前在知乎上看过一条段子【程序猿也是可以有女朋友的】，看完后感触挺深，具体内容如下：

> **标题：写博客对程序员很重要吗？**
>
> &emsp;&emsp;之前开了公众号装逼写技术博客，更新了一段时间没人看就不写技术写一些情感、生活、旅游、吃喝玩乐的内容， 反正只要能写的就都写。
>
> &emsp;&emsp;后来相亲认识了一妹子，没多久就好上了，主要是那妹纸太主动了，我没守住底线，沦陷了
>
> &emsp;&emsp;问妹纸为什么主动追我，妹纸说:你的每篇文章我都看了，字里行间感受到了正能量，应该不是那种靠不住的男人，我年纪 也不小了，机会不容错过，于是就使了点套路。
>
> &emsp;&emsp;我之前一直单身，始终找不好女朋友，对我有意思的我不喜欢，我喜欢的对我没感觉。现在能找到个令我满意的女朋友还没费多少 事我想应该有写博客一部分功劳吧。所以我觉得写博客对程序员来说挺重要的。		

&emsp;&emsp;好吧，重点不在于怎么找女朋友。作为一名程序猿，写博客是很好的一种体现，虽然我现在还是菜鸟一枚，但还是想分享些文章，不管有没有人看，坚持就好，也是一种态度。相信多年以后，你会感谢曾经的自己所付出的努力，最终你也会成为那个优秀的人。

## 2.搭建个人博客的选择

&emsp;&emsp;在真正确定搭建本博客网站之前，搜索了很多关于搭建个人博客的方式和思路。譬如现在大部分个人博客网站用的 Wordpress和Hexo框架，这两款博客框架封装的很好，网上教程也很多，分分钟就能搭建好，主题也很多，非常适合新手搭建使用。

&emsp;&emsp;但我并没有直接选择，因为觉得自己动手搭建一个会更好，增长自己项目经验的同时又能随时DIY各种功能，亦可以在博客项目上实践一些没用过的技术，何乐而不为呢？但博主只是后端开发，简单的样式还能调一调，那些炫酷的样式主题还真做不来，就想着网上找一个不错的来进行二次开发。于是我在GitHub和码云上苦苦寻找了一番，终于找到了个不错的，前端页面的尽力修改，后端代码的简单重构以及功能增加，便形成了现在的这个博客，[点此进入我的个人博客](http://liujian.cool)  个人感觉还是不错的，以后还会陆续完善功能，增加使用体验。

## 3.博客功能规划

### 主要功能实现

- 首页有最新文章排版，最新评论留言，每日一言，标签云，网站信息等等
- 文章模块有文章分类，归档，标签等功能，支持点击进入相应文章，都支持评论留言
- 友链支持一些大佬博客链接以及留言互相添加友联等功能
- 更新模块主要记录网站更新的记录，支持留言
- 照片墙模块根据日期展示博主后台上传自己喜欢的图片或游记照片等
- 关于我模块主要介绍博主本身的经历和感悟等
- 登录注册模块：支持QQ一键登录，可用邮箱注册账号登录本博客，忘记密码等
- 个人用户模块：编辑个人资料修改密码，以及评论留言管理，支持悄悄话
- 管理员后台模块：仪表盘展示网站访问信息，文章管理，点赞分类友链图片反馈悄悄话等功能管理

&emsp;&emsp;ps：目前实现了这些功能，后续文章也会着重介绍相关功能的实现，以及我在完善功能时遇到的一些坑和对应解决办法。

## 4.博客页面展示

### 博客首页展示

![](https://img-blog.csdnimg.cn/img_convert/847ad9a0dbe9e7b234eb65f956ca8f63.png)

### 个人主页展示

![](https://img-blog.csdnimg.cn/img_convert/c06661aec1c0d2d1ada201d8d2cd1939.png)

### 博客后台管理展示

![](https://img-blog.csdnimg.cn/img_convert/5b655f288eb2c2edbefae50354ca55b6.png)

## 5.博客项目总体设计

### 本项目中用到的技术框架：

1. web框架：SpringBoot
2. 数据库框架：Mybatis
3. 数据库连接池：阿里Druid
4. 数据库：MySql
5. 分页插件：PageHelper
6. 项目构建工具：Maven
7. 项目缓存选型：Redis
8. 文章编写展示：Editor.md
9. 前端模板：Thymeleaf
10. 安全框架：SpringSecurity

### 本项目所用环境：

1. 开发工具：IDEA
2. 编程语言：JDK1.8,HTML,CSS,JS
3. 数据库：mysql5.6
4. 项目框架：SSM
5. 部署服务器：腾讯云Centos7
6. 图床：七牛云对象存储
7. CDN加速：七牛云CDN

### 本地开发流程：

在文章开头链接下载源码导入IDEA后，修改配置文件中数据库连接信息后，导入项目附带数据库的SQL文件生成所有表结构，项目中用到的七牛云功能需要去七牛云官网实名认证后开通。

## 6.总结

&emsp;&emsp;既然决心搭建博客网站了，就一定好好做，坚持更新，给自己一个目标吧，希望借此能养成认真记录的好习惯。

&emsp;&emsp;接下来会陆续更新搭建博客功能的教程，for example: 使用邮箱注册发送验证码，接入QQ登录，本地图片上传到"七牛云OSS对象存储"图床，增加每日一言功能，增加博客背景鼠标绘制多边形,点击出现爱心功能，增加阿里druid连接池监控功能，增加nginx反向代理，配置网站CDN加速等等功能，欢迎大家拍砖~

&emsp;&emsp;更多精彩功能请关注我的个人博客网站：[http://liujian.cool](http://liujian.cool)

&emsp;&emsp;欢迎关注我的个人公众号：程序猿刘川枫

&emsp;&emsp;![](https://img-blog.csdnimg.cn/img_convert/1944436507a30c7c8541bcc5e4b75969.png)