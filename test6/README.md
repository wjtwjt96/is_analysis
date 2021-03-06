
## 成都大学信息科学与工程学院
|学号|班级|姓名|照片|
|:-------:|:-------------: | :----------:|:---:|
|201510414318|软件(本)15-3|吴江涛|![](./wjt.jpg 'wjt')|

## 1. 概述

  - 基于GitHub的实验管理平台的作用是在线管理实验成绩的Web应用系统。学生和老师的实验内容均存放在GitHUB 页面上。
  - 学生的功能主要有：一是设置自己的GitHub用户名，二是查询自己的实验成绩。学生的GitHub用户名是公开的，但成绩不公开。
  - 老师的功能主要有：一是批改每个学生的成绩，二是查看每个学生的成绩。
  - 老师和学生都能通过本系统的链接方便地跳转到学生的每个GitHUB实验目录，以便批改实验或者查看实验情况。
  - 实验成绩按数字分数计算，每项实验的满分为100分，最低为0分。
  - 系统自动计算每个学生的所有实验的平均分。
  - 本系统实现老师与学生的交互，学生通过平台提交实验，老师通过平台关系学生实验信息
  - 本系统可分为三个用户角色:
       - 游客：只能查看简易信息表，可以访问学生的GitHub账户查看共享的内容
       - 学生用户：可以选择自己喜欢的课程（在老师选课之后），完成实验上床，并查看自己的成绩信息（每个学期），同时可以访问同学的共享内容以及实验内容了，每个用户可以选择一门或多门课程
       - 老师用户：选择自己将要管理的课程，检阅学生的实验，并根据相应评分标准为之打分，每个用户可以选择一门或多门课程
  - 系统内对实验评分，必须按照相应的规则评判，每个实验有多个评分项，最后根据算法算出平均分
  
## 2. 系统总体结构
![](./System.png '系统框架图') 

## 3. 用例图设计[源码](src/UserCase.puml)
![](./UserCase.png '用户用例图') 

## 4. 类图设计[源码](src/UserClass.puml)
![](./UserClass.png '类图') 

## 5.数据库设计
- ### [参见数据库设计](./DesignDatabase.md)

## 6. 用例及界面详细设计
- ### [“学生列表”用例](./用例/学生列表.md),[界面源码](./ui/home.html),[界面](https://wjtwjt96.github.io/is_analysis/test6/ui/home.html)
- ### [“评定成绩”用例](./用例/评定成绩.md),[界面源码](./ui/add_grades.html),[界面](https://wjtwjt96.github.io/is_analysis/test6/ui/add_grades.html)
- ### [“查看成绩”用例](./用例/查看成绩.md),[界面源码](./ui/look_grades.html),[界面](https://wjtwjt96.github.io/is_analysis/test6/ui/look_grades.html)
- ### [“修改密码”用例](./用例/修改密码.md),[界面源码](./ui/modify_password.html),[界面](https://wjtwjt96.github.io/is_analysis/test6/ui/modify_password.html)
- ### [“修改用户信息”用例](./用例/修改用户信息.md),[界面1源码](./ui/modify_users_stu.html),[界面1](https://wjtwjt96.github.io/is_analysis/test6/ui/modify_users_stu.html)&nbsp;[界面2源码](./ui/modify_users_teacher.html),[界面2](https://wjtwjt96.github.io/is_analysis/test6/ui/modify_users_teacher.html)
- ### [“查看用户信息”用例](./用例/查看用户信息.md),[界面1源码](./ui/look_users_stu.html),[界面1](https://wjtwjt96.github.io/is_analysis/test6/ui/look_users_stu.html)&nbsp;&nbsp;[界面2源码](./ui/look_users_tea.html),[界面2](https://wjtwjt96.github.io/is_analysis/test6/ui/look_users_tea.html)
- ### [“选课”用例](./用例/选课.md),[选课界面（老师）源码](./ui/tea_select_course.html),[界面1](https://wjtwjt96.github.io/is_analysis/test6/ui/tea_select_course.html)&nbsp;&nbsp;[选课界面（学生）源码](./ui/stu_select_course.html),[界面2](https://wjtwjt96.github.io/is_analysis/test6/ui/stu_select_course.html)
- ### [“登出”用例](./用例/退出登录.md),[界面源码](./ui/login.html),[界面](https://wjtwjt96.github.io/is_analysis/test6/ui/login.html)
- ### [“登录”用例](./用例/登录.md),[界面源码](./ui/login.html),[界面](https://wjtwjt96.github.io/is_analysis/test6/ui/login.html)
