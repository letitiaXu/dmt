
## **初步了解**
    从打出方形的电钻和水面仿真说开去...
### 对数字媒体基础的学习架构图



课程架构图->软件架构图->基础知识架构图

### 软件架构图
 + 应用层
 + 表示层
 + 业务层
 + 中间层 
 + 网络，数据库，操作系统...
 
tips： 具体情况具体分析
 
## **数字媒体（image & Graphics）**
### 什么是媒体？
所谓媒体，是指传播信息的介质，通俗的说就是宣传平台，能为信息的传播提供平台的就可以称之为媒体。
+ 表示信息的载体：文本，音频，图形，图像，视频等
+ 存储信息的实体：纸张，磁盘，光盘，半导体存储器等

### 媒体的种类
+ 感觉媒体：人类感触信息的形式
+ 表示媒体：为了处理和传输人为创建的形式
+ 显示媒体：表现和获取信息的物理设备
+ 存储媒体：存放表示媒体
+ 传输媒体：传输数据的物理载体

### 关于媒体的发展
+ 第一媒体：报纸，杂志
+ 第二媒体：广播
+ 第三媒体：电视
+ 第四媒体：网络
+ 第五媒体：移动互联网

### web 2.0 & SNS 的发展
web2.0时代：用户创造内容
SNS：social network service 社会性网络服务，六度理论和150法则

### 虚拟竞技和娱乐媒体
各类游戏 
软件&硬件

### 移动互联网——新媒体



三大关键词：连接 互动 传播
三个层面：终端 软件 应用
多种业务模式

### 什么是数字媒体

+ 可感知形式：人-人，人-机交换信息，通过视觉听觉感官等感知信息
+ 数字媒体形式：计算机内部，机-机交换信息，二进制编码形式

### 模数转换

采样 -> 量化 -> 编码

### 自然媒体VS合成媒体
生成属性不同
+ 自然媒体：从自然中通过设备直接采集，数据量大，容易准备，计算简单
+ 合成媒体：通过计算机进行处理合成，数据量小，可编辑性好，虚拟能力强

### 小结：数字媒体的优点&缺点
优点：
+ 可编辑性好
+ 能够进行压缩
+ 与用户交互
+ 提供了自动提取元数据的可能

缺点：
+ 易于复制（版权）
+ 易于修改（信息安全）
+ 需要一定的设备（成本&效率）

### 数字媒体“食物链”
+ 媒体准备
+ 媒体编辑
+ 媒体集成
+ 媒体传输/分发
+ 媒体消费

### 图像
图像拼接 
视觉机理
+ 仿真图
+ 示意图

视觉得出的结论与前期知识有关

### 数字化
模数转换
采样：采样定理 分块
像素：图像的单位元素，即图像是由一个个像素组成的
+ 黑白图 
+ 灰度图
+ 彩色图
 
### 图像的表示
+ 将图像视为一个矩阵
+ 多种存储格式：BMP，JPG，GIF，PNG，PSD

### 颜色模式
+ RGB模式：red green blue
+ HSI模式：Hue Saturation intensity
+ YUV模式：Luminance Chromaticity

### 颜色种类
+ 8位灰度：256
+ 24位真彩色：16777216

### 图像存储
Bytes = Height * Width * bytesperpixel

### 图像处理
+ 图像拼接



+ 图像渐变
从直线方程说开去
f(x) = (1-t)P0 +t*P1      (0<t<1)

+ 标定 bound

### 频域下的图像
+ 高频：边缘 纹理 细节 噪音
+ 低频：区域阴影 渐变

### 图像滤波
+ 高通滤波
+ 低通滤波

### 两种滤波方式
+ 空间滤波
+ 频域滤波

一维卷积 -> 同时行列进行 -> 二维卷积
隐藏信息

### 图像滤波举例：
边缘检测


    从中山大学东校区的3D模型系统说开去
### 一个这样的系统需要如何完成？
+ 模型 
+ 引擎
+ 底层数据库 
+ 网络

### **计算机图形学**
+ 建模
+ 绘制
+ 动画
+ 交互

### 3D建模
+ 建模工具：点->线->面
+ 三维扫描
+ 基于图形，视频，已有模型数据的建模

### 图形
矢量图 
用相关数据确定
符号

### 计算机图形系统
+ 组成



+ 工作流程



### 显示器工作原理
+ 随机扫描

+ 光栅扫描

### 点->线->面
+ 点：单个坐标
+ 线：
    + 直线 
    + 曲线

+ 面：
点线构成面

### 两种直线生成算法
**DDA直线生成算法：**
+ x = x0 + △x   
+ y = y0 + △y
+ 计算简单，但是每一步都需要进行取整



**Breseham直线生成算法：**
+ x每次都增加1
+ 通过s和t的大小比较确定y值
+ 考虑多种情况



### 生成曲线
+ 多条直线->曲线
+ 存储关键点
+ 确定公式，多项式和
    + 样条基函数：曲线的二次导数相等

## **animation动画**
### animation technique
+ user-driven
    + keyframeing 关键帧
    + inverse Kinematics 运动学 and inverse dynamics 动力学
    + Motion capture 动作捕捉
+ Procedural animation
    + Physical simulation 物理模拟
    + Particle systems 粒子系统
    + Crowd behaviors 群体行为
+ Data-driven animation

### keyframe animation 关键帧动画
+ define a set of key pose：[q1,......qt]
+ interpolate 插值 to produce q(t)

### interpolation 插值
+ linear interpolation 线性插值：简单，不连续的速度
+ nonlinear interpolation 非线性插值：光滑的轨迹和连续的速度但是损耗一定的时间
+ Easing 缓动：调整每一帧之间的时间

### Style or Accuracy?
More squash and stretch 更多的形变
+ Direct their attention to what's important
+ resolution of action 动作分解 
+ Extra movements should not detract 减损

### summary of keyframe 关键帧动画
**Pros**：
+ very expressive
+ the choice for most

**Cons**：
+ very labour intensive 劳动密集型
+ hard to Create physical realism 物理现实

**Uses**：potentially everything except complex physical phenomenon 物理现象

### motion capture 动作捕捉
**Pros**：Captures specific style of real people.

**Cons**：
+ Often not expressive enough. 表现力不够
+ Time-consuming and expensive. 浪费时间，昂贵
+ Lots of equipment, space, actors. 设备，空间，演员
+ Manual clean-up. 手动清除
+ Hard to edit. 难以编辑

**Uses**：
+ character animation
+ Medicine

### Procedural Animation 程序动画
**Strengths**：
+ Animation can be generated 'on the fly' 快速
+ Dynamic response to user 动态响应
+ Write-once, use-often 多次使用
+ Algorithms provide accuracy and exhaustive search that animators cannot 精确性和穷举搜索

**Weakness**：
+ We’re not great at boiling human skill down to algorithms 将人类的技能变成算法
+ Difficult to generate 难以产生
+ Expensive to compute 计算代价大
+ Difficult to force system to generate a particular solution 难以驱动一个系统去产生一个特别的解决方法

### Physical simulation物理仿真：牛顿第二定律

**Pros**：
+ Very realistic motion.真实

**Cons**:
+ Very slow. 速度慢
+ Very hard to control. 难以控制
+ Not expressive. 没有表达性

**Uses**:
+ Complex physical phenomena. 复杂的物理现象
+ Special effects. 特殊的效果

### data-driven animation 数据驱动动画
**Pros**:
+ potentially best of all worlds:
+ captures specific style of real actors
+ very flexible 灵活
+ can generate new motion in real-time

**Cons**:
+ requires good data (possibly lots of it) 需要大量的良好的数据

**Uses**:
+ character animation

## **audio声音**
### 声音
+ 声波：人类用耳朵感知声音，耳蜗
+ 模数转换：麦克风
+ 基音&泛音：频率最低的音是基音，其他都称为泛音
+ 表达式 
    
    
     
     + 音调φ：声音的高低     
     + 音色 nw ：混入基础音的泛音
     + 音强 An ：声音的响亮程度，和幅度有关
     
### 音频信号
+ 采样：采样频率 = 2（f2 - f1） 当信号的边界为（f2，f1）
+ 量化：bit

### 信噪比
SNR：信噪比，有用信号与噪声之比
SQNR：Signal-to-quantization-noise ratio 信号-量化噪声比

### 声音数字化的三要素
+ 采样频率
+ 量化位数
+ 声道数

总数据量 = 采样频率 × 量化位数 × 声道数 ÷ 8


### 编码
+ PCM：Pulse Code Modulation 脉冲编码调制
+ DPCM：Differential pulse-code modulation 差分脉冲编码调制
    + 存差，减少了存储位数
+ ADPCM：Adaptive differential pulse-code modulation 自适应差分脉冲编码调制
    + 自适应

### 音频格式
WAV，MP3，WMA，VOC，MIDI等

### MIDI
Musical Instrument Digital Interface 电子乐器数字接口
MIDI合成器产生方式：
+ FM合成器
+ WT合成器 wave table

### 音频设备
+ 声卡
+ 音箱

### 声音识别
找出波形的特征




## **压缩 compression**

    从某黑心医院视频作假说开去
    
### 为什么能够仿出这样的视频？
mpeg格式的文件是场景（scene）和人物（character）分开编码

### 杰尔德定律
吉尔德定律(Gilder's Law)被描述为：在未来25年，主干网的带宽每6个月增长一倍，其增长速度是莫尔定律预测的 CPU 增长速度的3倍并预言将来上网会免费。吉尔德定律的提出者是被称为“数字时代三大思想家”之一的乔治·吉尔德。

### 信息论
研究信息的编码，传输，存储

### information system
+ 信源
+ 信道
+ 信宿

### 信息熵(Entropy)



### 一个事件发生概率大，信息量小
I(x) = log [1/p(x)] = -log p(x)
p(x)是事件出现的概率

### 无损压缩编码算法
**熵编码**
+ Shannon–Fano coding 香农-范诺编码算法
    + 出现次数越多的符号，给它分配的代码位数越少

+ Huffman Coding 哈夫曼编码
    + 出现次数越多的符号，给它分配的代码位数越少

+ 算术编码
    + 根据概率，直接把整个输入的消息编码为一个数
    
**字典编码**
+ 行程码 run-length encoding：统计 数目

### 有损压缩 
+ a close approximation
+ mean square error (MSE) 均方差
+ SNR 信噪比
+ PSNR 峰值信噪比

### VQ(Vector Quantization)
+ 一维 -> 区间



+ 二维 -> 面积





### Transformation 变换
+ time/space -> frequency
+ DFT，FFT，DCT

### zig-zag扫描



低频分量先出现，高频分量后出现，以增加行程中连续“0”的个数

### 视频压缩
**两个维度上的压缩**
+ 图像上
+ 时间上



### 运动补偿
+ 全局运动补偿 
+ 分块运动补偿 

### 运动估计
基本思想是将图像序列的每一帧分成许多互不重叠的宏块，并认为宏块内所有象素的位移量都相同，然后对每个宏块到参考帧某一给定特定搜索范围内根据一定的匹配准则找出与当前块最相似的块
**搜索算法：**
+ 对数搜索
+ 分层搜索

常用准则：MAD平均绝对误差 

Intra frames：I帧，关键帧，帧内编码
Predicted frames frame：P帧，预测帧
Bi-directional predicted frames：B帧，双向预测帧
