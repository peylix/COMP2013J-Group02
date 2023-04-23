# COMP2013J-Group02

## 飞鸽 PigeonWrite

### System Description:
#### 应用简介
这是一个高校内组织通知发送平台，可以让学校内的老师、学生组织和学生个人在平台上统一发放一些小通知，
解决学生需要加入繁多微信群，和微信消息过期的困扰。
1. Part 1: 飞鸽传书
学校及课程通知部分
2. Part 2: 飞鸽落羽
学生组织及学生个人发布通知部分

#### 账户创建部分
每个用户都可以建立一个账户，并且允许修改账号密码。
账号即为注册的教职工及学生的个人号，若个人号不存在则无法注册。
（该信息需从学校的数据库中读取，本项目只创建一个模拟数据库，与真实中的信息无关）

密码必须包含大小写英文字母，英文符号和数字。

个人信息部分：
建立账户后，第一次进入页面，可以自己上传头像。
个人信息从校内数据库自动导入。
不可自行在个人主页更改信息。

#### 飞鸽传书部分：
1. 课程通知：（包含课程表板块，点击进入后可打开对应课程的通知板块）
课程种类从校内数据库获取
老师可在其课程板块内
随笔内容是公共的，可以被所有用户查看
每个用户每天只可写一篇随笔。
每一篇随笔都可以连接到之前的某一篇没有被连接过的随笔。（可以更改）
每篇随笔都可被点赞评论分享
每个用户的随笔的集合被称为一个“随笔序列”（Essay Series），由一个表来储存，其属性（attribute）包括内容、日期、修改日期、连接关系等，
其中日期应为primary key。（待定）

