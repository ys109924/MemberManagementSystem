# 会员管理系统

## 项目说明
该项目为C++课程大作业，无特别参考价值，发布仅供记录，部分功能并不完善。

## 项目依赖
Qt版本：5.12.0或更高
数据库：Sqlite
语言：C++

## 项目架构
会员管理系统使用Qt编写，遵循UI与业务逻辑分离的设计原则。

### 主要模块
- 登录窗口 对应loginwindow.ui，是用户登录连接聊天服务器的界面。
- 注册窗口 对应 registwindow.ui，是用户在相应服务器注册帐号的界面。
- 程序主界面 对应 mainwindow.ui 是程序功能主要界面。
- 其他窗口 包括添加优惠信息窗口，添加活动信息窗口等。

### 系统结构
```mermaid
graph TD

A[系统主界面]-->B[消费管理]
A-->C[会员管理]
A-->D[商品管理]
A-->E[活动营销]
B-->B1[商品消费]
B-->B2[会员充值]
B-->B3[积分兑换]
C-->C1[会员登记]
C-->C2[会员列表]
C-->C3[会员信息]
C-->C4[会员等级]
D-->D1[添加商品]
D-->D2[商品列表]
D-->D3[商品类别]
E-->E1[优惠券管理]
E-->E2[优惠活动管理]
E-->E3[礼品管理]

```


### 文件组织
```
项目目录
├── LICENSE
├── README.md
└── MyMMS
    ├── MyMMS.pro      -- 项目文件
    ├── *.cpp *.h ... -- 源代码文件和头文件
    ├── *.ui      ... -- UI 布局文件
    ├── resources.qrc -- 资源文件
    └── images        -- 图片资源文件夹
        ├── 1.png
        ├── 2.png
        └── ...
```

## 部分界面
![登录界面](MyMMS/images/login.png)

![注册界面](MyMMS/images/regist.png)

![主界面](MyMMS/images/mainwindow.png)

![弹出界面](MyMMS/images/others.png)



