# BCI软件平台介绍
脑-机接口能够实现大脑与外界设备的直接通讯。构建一套完整的脑-机接口系统既需要硬件平台也需要软件平台。其中，软件平台涉及刺激呈现、数据读取与预处理、数据分析与解码、在线反馈等多个环节。通用的脑—机交互系统大致由四个模块组成：信号采集模块、信号处理模块、控制器模块和反馈模块。

（1）信号采集模块
脑信号的采集可以采用有创的植入电极方法，也可以采用无创的头皮脑电、功能磁共振成像或者近红外光谱等方法。

（2）信号处理模块
主要包含特征提取和模式识别两个部分。特征提取即找到一种更有效的方法来表达信号中的特征成分，目的是要为进一步的模式分类提供依据。模式识别是对信号进行处理和分析，以便后续进一步地辨认、分类和解释。

（3）控制器模块
控制器模块是将模式分类得到的结果转换成相应的控制命令以实现用户的真实意图，例如移动鼠标或者控制轮椅等。

（4）反馈模块
反馈模块是将被控制对象的状态通过人体的感知系统传递给大脑。现有的基于EEG的脑—机接口系统根据所检测到的电生理信号的不同主要分为以下三类：运动想象脑—机接口、P300脑—机接口和稳态视觉诱发电位（SSVEP）脑—机接口。目前脑—机接口设计主要在软件层面实现，它能与目前常用的脑信号采集设备相连，完成信号采集工作，并在此基础上提供常用脑—机交互实验范式的信号处理软件，并将解读后的脑信号转换成相应的控制命令以实现对外部设备的控制。
![](image/2023-02-28-20-50-53.png)


目前已公开的脑机接口相关软件工具包从应用角度可分为以下几类：第一是用于设计实验任务、构建刺激程序的工具包，主要包括PsychoPy、E-Prime等。第二是用于实现采集设备软硬件联通的工具包。其中，BCI2000软件是一种脑-机接口系统基础研发平台，NeuroScan是与采集硬件配套的集成可编程软件；第三是专精于后期信号处理分析的工具包，包括熟知的EEGLAB、MNE等。


### 参考链接
1. [脑机接口综合性开源软件平台MetaBCI功能介绍及获取方式_脑机接口社区的博客-CSDN博客](https://blog.csdn.net/zyb228/article/details/128017357)

2. [解析热点脑机接口平台_壹脑云的博客-CSDN博客](https://blog.csdn.net/weixin_40052256/article/details/123532583)

3. [解析全球热点脑机接口平台（下）_壹脑云的博客-CSDN博客](https://blog.csdn.net/weixin_40052256/article/details/124211309)

4. [Introduction to BCI: Software Tools to Use](http://learn.neurotechedu.com/introbci_software/)

5. [Center-For-Neurotechnology/CLoSES-RT: A platform for closed-loop intracranial stimulation in humans](https://github.com/Center-For-Neurotechnology/CLoSES-RT)

6. [OpenBCI | Downloads](https://openbci.com/downloads)

7. [SpikeInterface/spikeinterface: A Python-based module for creating flexible and robust spike sorting pipelines.](https://github.com/SpikeInterface/spikeinterface)

8. [Welcome to SpikeInterface’s documentation! — spikeinterface documentation](https://spikeinterface.readthedocs.io/en/latest/)

9. [Hi, MetaBCI. TJU Releases China's First Open Source Software Platform for BCI-Tianjin University:](http://www.tju.edu.cn/english/info/1010/6531.htm)

10. [TBC-TJU/MetaBCI: MetaBCI: China’s first open-source platform for non-invasive brain computer interface. The project of MetaBCI is led by Prof. Minpeng Xu from Tianjin University, China.](https://github.com/TBC-TJU/MetaBCI)

11. [2021年中国脑机接口平台行业概览](https://pdf.dfcfw.com/pdf/H3_AP202201121539917091_1.pdf?1641976029000.pdf)

12. [盘点｜火爆的五家海外脑机接口公司|马斯克|脑机|五家|接口|盘点|癫痫|芯片|大脑|设备|-健康界](https://www.cn-healthcare.com/articlewm/20210930/content-1269415.html)

13. [OpoenVIBE—Unity3D脑机接口实验平台搭建：一、OpenVIBE与脑电设备的连接_少侠只用刀的博客-CSDN博客_openvibe](https://blog.csdn.net/qq_15017307/article/details/116464354)

14. [Acquisition devices and drivers in OpenViBE | OpenViBE](http://openvibe.inria.fr/supported-hardware/)

15. [收藏 | 脑电、脑机接口(BCI)等数据集、书籍、信号处理等相关资源汇总](https://mp.weixin.qq.com/s?__biz=MzI0MTQxNDE5NA==&mid=2247492624&idx=1&sn=b16ccdda19e5ddd23c0b8f08b1281a29&chksm=e9095d4dde7ed45be374b9a92de3a6b286ece095e8897e2b994f8e1ea5df84d614c4cf99d894&scene=178&cur_album_id=2571780432946561027#rd)

16. [Data and Code - CashLab - MGH/Harvard](https://cashlab.mgh.harvard.edu/data-and-code/)

17. [DABI](https://dabi.loni.usc.edu/login?returnUrl=%2Frequest-data%2FU01NS108916)
