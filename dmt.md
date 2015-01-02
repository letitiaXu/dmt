

##**初步了解**
    从打出方形的电钻和水面仿真说开去...
###对数字媒体基础的学习架构图

![](~/02-11-10.jpg)

课程架构图->软件架构图->基础知识架构图

###软件架构图
 + 应用层
 + 表示层
 + 业务层
 + 中间层 
 + 网络，数据库，操作系统...
 
tips： 具体情况具体分析
 
##**数字媒体（image & Graphics）**
###什么是媒体？
所谓媒体，是指传播信息的介质，通俗的说就是宣传平台，能为信息的传播提供平台的就可以称之为媒体。
+ 表示信息的载体：文本，音频，图形，图像，视频等
+ 存储信息的实体：纸张，磁盘，光盘，半导体存储器等

###媒体的种类
+ 感觉媒体：人类感触信息的形式
+ 表示媒体：为了处理和传输人为创建的形式
+ 显示媒体：表现和获取信息的物理设备
+ 存储媒体：存放表示媒体
+ 传输媒体：传输数据的物理载体

###关于媒体的发展
+ 第一媒体：报纸，杂志
+ 第二媒体：广播
+ 第三媒体：电视
+ 第四媒体：网络
+ 第五媒体：移动互联网

###web 2.0 & SNS 的发展
web2.0时代：用户创造内容
SNS：social network service 社会性网络服务，六度理论和150法则

###虚拟竞技和娱乐媒体
各类游戏 
软件&硬件

###移动互联网——新媒体

![](~/02-32-07.jpg)

三大关键词：连接 互动 传播
三个层面：终端 软件 应用
多种业务模式

###什么是数字媒体

+ 可感知形式：人-人，人-机交换信息，通过视觉听觉感官等感知信息
+ 数字媒体形式：计算机内部，机-机交换信息，二进制编码形式

###模数转换

采样 -> 量化 -> 编码

###自然媒体VS合成媒体
生成属性不同
+ 自然媒体：从自然中通过设备直接采集，数据量大，容易准备，计算简单
+ 合成媒体：通过计算机进行处理合成，数据量小，可编辑性好，虚拟能力强

###小结：数字媒体的优点&缺点
优点：
+ 可编辑性好
+ 能够进行压缩
+ 与用户交互
+ 提供了自动提取元数据的可能

缺点：
+ 易于复制（版权）
+ 易于修改（信息安全）
+ 需要一定的设备（成本&效率）

###数字媒体“食物链”
+ 媒体准备
+ 媒体编辑
+ 媒体集成
+ 媒体传输/分发
+ 媒体消费

###图像
图像拼接 
视觉机理
+ 仿真图
+ 示意图

视觉得出的结论与前期知识有关

###数字化
模数转换
采样：采样定理 分块
像素：图像的单位元素，即图像是由一个个像素组成的
+ 黑白图 
+ 灰度图
+ 彩色图
 
###图像的表示
+ 将图像视为一个矩阵
+ 多种存储格式：BMP，JPG，GIF，PNG，PSD

###颜色模式
+ RGB模式：red green blue
+ HSI模式：Hue Saturation intensity
+ YUV模式：Luminance Chromaticity

###颜色种类
+ 8位灰度：256
+ 24位真彩色：16777216

###图像存储
Bytes = Height * Width * bytesperpixel

###图像处理
+ 图像拼接

![](~/QQ图片20150102140107.jpg)

+ 图像渐变
从直线方程说开去
f(x) = (1-t)P0 +t*P1      (0<t<1)

+ 标定 bound

###频域下的图像
+ 高频：边缘 纹理 细节 噪音
+ 低频：区域阴影 渐变

###图像滤波
+ 高通滤波
+ 低通滤波

###两种滤波方式
+ 空间滤波
+ 频域滤波

一维卷积 -> 同时行列 -> 二维卷积
隐藏信息

###图像滤波举例：
边缘检测


    从中山大学东校区的3D模型系统说开去
###一个这样的系统需要如何完成？
+ 模型 
+ 引擎
+ 底层数据库 
+ 网络

###**计算机图形学**
+ 建模
+ 绘制
+ 动画
+ 交互

###3D建模
+ 建模工具：点->线->面
+ 三维扫描
+ 基于图形，视频，已有模型数据的建模

###图形
矢量图 
用相关数据确定
符号

###计算机图形系统
+ 组成

![](~/16-11-07.jpg)

+ 工作流程
![](~/16-03-49.jpg)

###显示器工作原理
+ 随机扫描

+ 光栅扫描

###点->线->面
+ 点：单个坐标
+ 线：
    + 直线 
    + 曲线

+ 面：
点线构成面

###两种直线生成算法
**DDA直线生成算法：**
+ x = x0 + △x   
+ y = y0 + △y
+ 计算简单，但是每一步都需要进行取整

![](~/16-42-04.jpg)

**Breseham直线生成算法：**
+ x每次都增加1
+ 通过s和t的大小比较确定y值
+ 考虑多种情况

![](~/16-36-21.jpg)

###生成曲线
+ 多条直线->曲线
+ 存储关键点
+ 确定公式，多项式和
    + 样条基函数：曲线的二次导数相等

##**animation动画**



