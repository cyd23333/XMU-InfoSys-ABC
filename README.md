# 厦门大学信息系统从入门到精通
## 记号介绍
各系统账号的格式多为多段文字拼接形成，为了准确描述，定义下面几个记号：

|记号|说明|举例|
|---|---|---|
|`"文字"`|引号引用的文字，直接照抄，不包括引号|`"haha233"` → `haha233`|
|`$(说明文字)`|使用说明文字指代的文字内容替换|如果我的学号是35320182200666，那么`$(学号)` → `35320182200666`|
|`Cat(第一段文字, 第二段文字, ..., 第N段文字)`|依次将第一段文字、第二段文字、...、第N段文字首尾相接，得到一段新的文字，各段文字间无空格/加号等符号|`Cat("666", "haha", "233")` → `666haha233`|

再来几个例子：
+ 如果我的校园卡账号是`12345678`，那么我的图书馆账号是`Cat("0000", $(校园卡账号的前6位数))` → `0000123456`
+ 如果我的Github ID是`yqszxx`，谷歌邮箱的后缀是`gmail.com`，那么我的邮箱是`Cat($(我的Github ID), "@", $(谷歌邮箱的后缀))` → `yqszxx@gmail.com`

## 账号列表
|账号名称|账号|初始密码|修改密码方式|重置密码方式|
|-------|----|--------|----------|-----------|
|统一身份认证账号|`$(学号)`|`$(身份证号后6位)`|点击[这里](https://ids.xmu.edu.cn/authserver/login)登录后，左侧选择`修改密码`|持本人**学生卡、学生证和身份证**到各校区一卡通服务网点（思明校区嘉庚主楼一楼学生事务大厅、图书馆总馆二楼服务总台、学生公寓信息工程分馆服务台、翔安校区图书馆二楼总台、漳州校区一卡通中心）重置密码|
|我的图书馆账号|`Cat("0000", $(校园卡账号的前6位数))`（账号在校园卡的第二行，是个8位数字）|`$(学号)`|点击[这里](https://catalog.xmu.edu.cn/reader/login.php)登录后，点击名字下方的`修改密码`|点击[这里](https://catalog.xmu.edu.cn/reader/redr_mail.php)填写信息后通过邮件重置|
|网络认证账号|`$(学号)`|无，必须重置才能使用|点击[这里](https://p.xmu.edu.cn)，使用**统一身份认证账号**登录后，点击`点击修改校园网（WLAN及VPN通用）密码`按钮修改密码|同修改密码方法|
|邮件系统账号|`Cat($(学号), "@stu.xmu.edu.cn")`|无，必须重置才能使用|点击[这里](https://i2.xmu.edu.cn/)，使用**统一身份认证账号**登录后，点击顶部`邮箱`→`修改邮箱密码`后，点击`修改密码`按钮修改|同修改密码方法|

## 系统介绍
### 校园网
1. 校内计算机教室的计算机都直接连入校园网；
2. 学校教学区域、餐厅均有名为`XMUNET+`的无线网络覆盖，具体连接方法请参阅[这里](https://inc.xmu.edu.cn/17101/list.htm)，其中账号为上文账号列表中的**网络认证账号**；
3. 如需在校外或无法连接`XMUNET+`的场所访问校园网，请使用VPN，具体设置方法请参阅[这里](https://inc.xmu.edu.cn/17097/list.htm)，其中账号为上文账号列表中的**网络认证账号**。

### 统一身份认证
### 图书馆及文献数据库
### 厦大邮箱
### 选课、四六级报名系统
### 教务系统

## 常用链接
### 学校机构
+ 学校官网 https://www.xmu.edu.cn/
+ 教务处 https://jwc.xmu.edu.cn/
+ 学生处 https://xsc.xmu.edu.cn/
+ 国际合作交流处 http://ice.xmu.edu.cn/
+ 信息与网络中心 https://net.xmu.edu.cn/
### 学院
+ 电子科学与技术学院 https://ese.xmu.edu.cn/
