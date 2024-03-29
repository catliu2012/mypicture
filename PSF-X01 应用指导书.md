# 		                                           XX-XX应用指导书 



<img>![图片描述](https://raw.githubusercontent.com/june0854/june0854.github.io/%E5%9B%BE%E7%89%87/LOGO.bmp)

**版本V1.0** 

**版权©2019** 





##                                                                                                                                                                                                                            	     关于本手册



             本手册介绍了XX-XX应用指导书产品参数，包含以下章节。 

| 章     | **标题**           | **内容**                           |
| :----- | :----------------- | :--------------------------------- |
| 第一章 | 产品简介           | 概述XX-XX的特点和功能应用        |
| 第二章 | 电气特性           | 介绍模块的电气性能基本参数         |
| 第三章 | 模块类型及管脚定义 | 提供模块类型、管脚定义功能说明     |
| 第四章 | 功能描述           | 描述模块功能及具体说明             |
| 第五章 | WIFI射频指标       | 介绍模块的射频指标                 |
| 第六章 | PCB设计            | 提供了模块布局及PCB layout注意事项 |
| 第七章 | 封装信息           | 提供模块封装尺寸图                 |





## 一、  产品简介																																		

​	

               XX-XX是深圳酷宅科技有限公司（简称：酷宅科技）一款基于 SV6166F的超低功耗的Wi-Fi单通道开关模

块，拥有业内极富竞争力的封装尺寸和超低能耗技术，专为移动设备和物联网应用设计，可将用户的物理设备连接

到Wi-Fi无线网络上，进行互联网或局域网通信，实现联网功能。该模块可以作为单个家用电器的开关控制。既可

以通过本地的按键控制，也可以通过连接APP（易微联）远程控制。

        XX-XX可广泛应用于智能电网、智能交通、智能家具、手持设备、工业控制等领域。

​      

   **产品特性**

- 内置 32 位 MCU，可兼作应用处理器 
- 支持无线802.11 b/g/n 标准
- Wi-Fi @2.4 GHz，支持WPA/WPA2安全模式
- 802.11b 模式下+20.5dBm的最大输出功率
- 支持本地硬件开关控制 
- 支持定时器操作
- 支持 Wi-Fi 远程控制 
- 支持兼容配对模式 / 快速配对模式
- 支持OTA升级







## 二、电气特性



####      2.1、额定参数

                                      条件：VDD=3.3V±10%，GND=0V；室温25°C下测试。

|     型号     | 类型                                                     |
| :----------: | :------------------------------------------------------- |
|     型号     | XX-XX                                                  |
|    主芯片    | SV6166F                                                  |
|   硬件接口   | UART，GPIO                                               |
|   工作电压   | 2.7V~3.6V                                                |
| GPIO驱动能力 | Max：12mA                                                |
|   工作电流   | 平均电流：≈80mA，<br>最大工作电流：210mA<br>待机: <200uA |
|   工作温度   | 0℃~45℃                                                   |
|   存储环境   | 温度：-10℃~75℃，相对湿度：20%RH~80%RH                    |
| 无线网络类型 | STA/AP/STA+AP                                            |
|   安全机制   | WEP/WPA-PSK/WPA2-PSK                                     |
|   加密类型   | WEP64/WEP128/TKIP/AES                                    |
|   固件升级   | OTA 远程升级                                             |



####      2.2、Wi-Fi 参数  

                                             条件：VDD=3.3V±10%，GND=0V；室温 25°C 下测试。 

|    类型    | 参数                                                         |
| :--------: | ------------------------------------------------------------ |
|  无线标准  | IEEE 802.11b/g/n                                             |
|  频率范围  | 2.412GHz-2.484GHz                                            |
|  发射功率  | 802.11b: 20±2dBm (@11Mbps)<br>802.11g: 17±2dBm (@54Mbps)<br>802.11n: 14±2dBm (@HT20,MCS7) |
| 接收灵敏度 | 802.11b: -91 dBm (@11Mbps ,CCK)<br>802.11g: -75 dBm (@54Mbps, OFDM)<br>802.11n: -72 dBm (MCS7) |
|  天线类型  | PSF-A01：IPEX接口天线<br>PSF-B01：陶瓷贴片天线               |







## 三、模块类型及管脚定义



#### 3.1、模块类型

            PSF-X01多通道开关模块包含两种型号：PSF-A01、PSF-B01。两种模块的区别只是天线类型的不同，PSF-

A01使用IPEX接口天线，PSF-B01使用陶瓷天线，其他方面没有区别。



![图片描述](https://raw.githubusercontent.com/june0854/june0854.github.io/%E5%9B%BE%E7%89%87/PSF-IPX%E5%A4%A9%E7%BA%BF%E6%8E%A5%E5%8F%A3%E6%A8%A1%E5%9D%97.bmp)

                                                                                     PSF-A01顶视图



![图片描述](https://raw.githubusercontent.com/june0854/june0854.github.io/%E5%9B%BE%E7%89%87/PSF-%E9%99%B6%E7%93%B7%E5%A4%A9%E7%BA%BF%E6%A8%A1%E5%9D%97.bmp)

                                                                                     PSF-B01顶视图



####      3.2、脚位排列顺序

                               PSF-X01模块提供单通道开关控制接口，Wi-Fi指示灯接口，UART串口。



![图片描述](https://raw.githubusercontent.com/june0854/june0854.github.io/%E5%9B%BE%E7%89%87/PSF%E6%A8%A1%E5%9D%97%E9%A1%B6%E8%A7%86%E5%9B%BE.bmp)

                                                                                  模块引脚顶视图



![图片描述](https://raw.githubusercontent.com/june0854/june0854.github.io/%E5%9B%BE%E7%89%87/PSF%E6%A8%A1%E5%9D%97%E4%BD%8E%E8%A7%86%E5%9B%BE.bmp)

                                                                                  模块引脚低视图



####    3.3、管脚定义

                                                                             管脚定义及功能说明

| 管脚 | 名称   | 功能                                                         |
| ---- | ------ | ------------------------------------------------------------ |
| 1    | ANT    | Wi-Fi Antenna注：<br>1：PSF-A01外接IPEX接口天线时不能使用<br>2：PSF-B01不能使用 |
| 2    | ADC    | ADC接口，输入范围：0 – 1V                                    |
| 3    | EN     | 芯片使能端高电平：有效；低电平：关闭。<br>注：外部上拉1~10K电阻，接100nF电容到地。 |
| 4    | GPIO16 | NC                                                           |
| 5    | GPIO14 | NC                                                           |
| 6    | GPIO12 | 继电器开关，高电平有效，上电默认低电平。<br>注：作为开关按键，上电瞬间会有一段时间高电平，需要下拉（1~4.7K）电阻到地。 |
| 7    | STATUS | Wi-Fi状态指示灯，接LED灯串联限流电阻到3V3                    |
| 8    | GPIO15 | 注：芯片配置脚，需要下拉（1~4.7K）电阻到地                   |
| 9    | GPIO2  | 可用作烧写闪存时UART1_TX                                     |
| 10   | GPIO0  | 1、开关引脚，低电平有效<br>2、配网模块                       |
| 11   | GPIO4  | NC                                                           |
| 12   | GND    | GND                                                          |
| 13   | GPIO9  | NC                                                           |
| 14   | GPIO10 | NC                                                           |
| 15   | GPIO11 | NC                                                           |
| 16   | GPIO6  | NC                                                           |
| 17   | GPIO7  | NC                                                           |
| 18   | GPIO8  | NC                                                           |
| 19   | GPIO5  | NC                                                           |
| 20   | GND    | GND                                                          |
| 21   | RX     | 用于烧写Flash时UART_RX                                       |
| 22   | TX     | 用于烧写Flash时UART_TX                                       |
| 23   | 3V3    | 电源                                                         |
| 24   | RST    | 外置复位信号：低电平有效，外部需上拉 10K 电阻到 3.3V，接 100nF电容到地 。 |







## 四、功能描述



#### 4.1、模块功能

            PSF-X01模块可作为一个单通道的开关设备，既可以在本地控制开关，也可以通过APP远程控制开关。以下

       是功能说明：

1. 配置方式：快速配对模式/兼容配对模式 。长按按键（IO0下拉，默认高电平）5s以上进入快速配对模式，

   在此状态下，再长按按键5s以上进入快速配对模式，两种状态都可以配置APP。配置方式具体说明见4.3。

2.   开关：

   a、 正常状态下，单击按键（IO0下拉超过100ms），控制继电器通断（IO12输出高/低电平）。

   a、 配置状态下，单击按键可退出配置状态。

3. 定时：包括单次定时、延时定时、循环定时、重复定时，具体说明见4.5。

4. 上电状态配置：可通过APP端配置上电开关状态开或是关，默认上电关。



#### 4.2、Wi-Fi状态灯闪烁方式说明

            设备端Wi-Fi状态灯的闪烁方式表征设备当前的网络工作状态，具体状态包括以下七种：

![图片描述](https://raw.githubusercontent.com/june0854/june0854.github.io/%E5%9B%BE%E7%89%87/LED%E7%81%AF%E9%97%AA%E7%83%81%E8%AF%B4%E6%98%8E.bmp)

​	                                                        设备状态与Wi-Fi状态灯闪烁方式关系示意图



​	     Wi-Fi状态灯的闪烁特征以2秒为一个周期，如图所示，低电平灯亮，高电平灯灭。各状态详解：

A .  Normal : 设备正常工作，与云服务器连接正常。此时可以通过APP操控设备。在其它任何模式下，

​           都无法通过 APP操控设备。

B .  NO Wifi：设备无法连接到无线路由器。

C .  No Server：设备已经连接上无线路由器，但是无法连接到服务器（就是通常理解下的“无法上网”）。

D . Unregistered：表示设备还没有被绑定到任何账户下。一般的，设备需要与易微联账号绑定才可与云服务器      

      通信。在易微联APP“添加设备”可完成绑定操作。

E .  Upgrade：表示设备正在固件升级。

F .  Setting G1：表示设备正处于兼容配对模式。配置模式用于设备获取移动终端APP提供的加入服务网络的必要

     信息，包括路由器ssid、password和服务器ip、端口号等。

G . Setting G2：表示设备正处于快速配对模式。配置模式用于设备获取移动终端APP提供的加入服务网络的必要

      信息，包括路由器ssid、password和服务器ip、端口号等。两种配置，设备获取相关信息的方式不同，详见下

      节所述。



#### 4.3、Wi-Fi模块的基本工作流程



​	I． 配置

      	      设备模块在未加入局域网时就是一个“信息孤岛”，设备端操作配合易微联APP设置，使设备获取加入服务

网络的必要信息，包括路由器ssid、password和服务器ip、端口号等。模块内置两种配置方式：

​	      1、兼容配对模式：移动终端作为station加入该AP组成局域网实现数据交互。快速配对模式（G状态，

​	      详情见4.2 Wi-Fi状态灯闪烁方式说明）下长按配置按键5S，设备进入兼容配对模式。点击易微联APP

       添 加设备（iOS移动终端需在“设置”菜单内手动连接ssid：ITEAD-10000XXXX， password12345678

       的热Android终端无需此操作），输入家庭路由器的ssid和password，完成设备的上线准备工作。

​	      2、快速配对模式：此方式Wi-Fi模块处于混杂模式（Wi-Fi Promiscuous），通过空快速配对模式：此方

       式Wi-Fi模块处于混杂模式（Wi-Fi Promiscuous），通过空空抓包的形式获取移动终端发出的包含ssid

       和password等信息的加密报文。上节所述A~D任意一个状态内长按配置按键5S，设备进入快速配对模

       式。点击易微联APP添加设备，输入家庭路由器的ssid和password，完成设备的上线配置工作。

​	

​	II． 上线

​	      设备模块从上电到连接服务器，需经历以下流程：

​		1、加入所配置路由器，连接Internet。

​		2、连接服务器。

​		3、注册设备，绑定至易微联账户。

​		4、获取设备应用参数，保持在线 。

​	      以上各个步骤，当连接/获取失败时，均有相应的退避策略和重连接机制，确保设备稳定、实时在线。



​	III． 升级

         模块设备连接升级服务器，下载更新至最新版本固件，实现设备的在线升级。



#### 4.4、定时器功能

​	           定时器功能通过APP配置，定时器分为以下四种:

1. 单次定时器：在指定时间执行操作。

2. 延时定时器：经过所设置的时间执行操作。

3. 循环定时器：周循环执行操作。

4. 重复定时器：日重复执行操作。

    

#### 4.5、定时功能说明

            PSF-X01支持定时器操作，为了方便客户使用以及让其使用在更多的场景下，易微联APP提供了四种定时模

       式：

1. 单次定时：这个是最普通的定时设置，让用户可以设置这个设备的工作日程。比如那一天几点几分启动或者关

   闭，或者每周三几点几分启动或者关闭等。跟闹钟的设置类似，尤其是对重复在某些时刻要运行的设备，定时

   后使用起来非常方便。

2. 延时定时：延时是为了方便用户进行一次性快速的定时操作，比如在多久之后执行启动或者关闭的动作，可以

   非常方便的将某个设备打开后，让它运行一段时间然后关闭。本设备最多支持24小时的延时操作。	

3. 循环定时：对于某些设备，为了可以更方便的在某个场景下使用，易微联推出的循环定时设置，可以让一个设

   备从某个时刻开始，不断循环做一个事情。比如，让鱼缸的打氧泵从现在开始，每一小时启动一次，每次打氧

   20分钟后关闭，然后重复自动循环，保证鱼缸的氧气充足而无需人工干预。	

4. 重复定时：重复定时是方便无需在次日进行同时间设置定时操作。比如，设定上班时间闹钟，时间设置好后，

   选择日期（日期天数为一周可选），闹钟就会在选择的日期内设定的时间开启。







## 五、WIFI射频指标

                                    

                                              条件：VDD=3.3V±10%，GND=0V；室温25°C下测试。

| 描述                               | 最小值 | 典型值 | 最大值 | 单位 |
| :--------------------------------- | :----: | :----: | :----: | :--: |
| 输入频率                           |  2412  |   -    |  2484  | MHz  |
| 输出阻抗                           |   -    |   50   |   -    |  Ω   |
| 输入反射                           |   -    |   -    |  -10   |  dB  |
| 72.2Mbps 下， PA 的输出峰值功率    |  15.5  |  16.5  |  17.5  | dbm  |
| 802.11b 模式下， PA 的输出峰值功率 |  19.5  |  20.5  |  21.5  | dbm  |



#### 	1 . 灵敏度

| 描述                          | 最小值 | 典型值 | 最大值 | 单位mA |
| ----------------------------- | ------ | :----: | ------ | :----: |
| CCK 1Mbps                     |        |  -98   |        |  dBm   |
| CCK 11Mbps                    |        |  -91   |        |  dBm   |
| 6Mbps(1/2BPSK)                |        |  -93   |        |  dBm   |
| 54Mbps(3/4 64-QAM)            |        |  -75   |        |  dBm   |
| HT20，MCS7（65Mbps，72.2Mbps) |        |  -72   |        |  dBm   |



#### 	2 . 邻频抑制

| 描述         | 最小值 | 典型值 | 最大值 | 单位mA |
| ------------ | ------ | :----: | ------ | :----: |
| OFDM，6Mbps  |        |   37   |        |   dB   |
| OFDM，54Mbps |        |   21   |        |   dB   |
| HT20，MCS0   |        |   37   |        |   dB   |
| HT20，MCS7   |        |   20   |        |   dB   |

        注：

            1、72.2Mbps是在802.11n模式下，MCS=7，GI=200uS时测得。

            2、802.11b模式下最高可达+21.5dBm的输出功率。







## 六、PCB设计



       **PCB layout 与模块布局注意事项：**

       1、在PCB layout时注意模块摆放位置，特别是模块的天线部分，尽可能远离干扰源：磁性元件(如马达、电

             感、变压器等)、高频信号器件（如晶振、高频时钟信号等）。

       2、模块摆放位置的PCB上下层尽可能不要走线，做覆铜包地处理，模块天线到模块最近引脚部分的PCB尽可

             能做挖空处理。

       3、模块PCB天线区域及外扩 15 mm 区域需净空（严禁铺铜、⾛线、摆放元件），参考如下图所示：



​	                                                            ![图片描述](https://raw.githubusercontent.com/june0854/june0854.github.io/%E5%9B%BE%E7%89%87/PSF%E6%A8%A1%E5%9D%97%20PCB%20layout%20%E5%A4%A9%E7%BA%BF%E9%83%A8%E5%88%86%E8%AE%BE%E8%AE%A1%E6%8E%92%E6%94%BE%E8%A6%81%E6%B1%82.bmp)



        4、模块的电源（VCC）引脚电容和模块其他引脚电容、电阻尽可能靠近模块引脚摆放，走线路径要短。







## 七、封装信息

​	

             封装尺寸图：

![图片描述](https://raw.githubusercontent.com/june0854/june0854.github.io/%E5%9B%BE%E7%89%87/PSF%E6%A8%A1%E5%9D%97%E5%B0%81%E8%A3%85%E5%B0%BA%E5%AF%B8%E5%9B%BE.bmp)









------





 

   



![图片描述](https://raw.githubusercontent.com/june0854/june0854.github.io/%E5%9B%BE%E7%89%87/%E7%89%88%E6%9D%83%E8%AF%B4%E6%98%8E.bmp )
