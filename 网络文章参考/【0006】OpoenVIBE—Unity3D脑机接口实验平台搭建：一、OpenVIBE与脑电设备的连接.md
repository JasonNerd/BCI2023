# OpoenVIBE—Unity3D脑机接口实验平台搭建：一、OpenVIBE与脑电设备的连接
OpenVIBE(OV)是一款用于脑-机接口设置、使用与分析的开源脑电处理软件，其提供丰富的脑电信号处理工具，以可视化的编程方式能够快速的构建脑机接口场景。此外，OV支持Python、Matlab脚本等扩展方式，为融入更多先进的脑电处理算法提供了可能。
OV支持多种设备的接入，具体支持的设备型号可通过OpenVIBE文档查询，我的设备是Emotive EPOC+，通过第三方工具Cykit将其与OV连接。

OpenVIBE与EPOC+的连接
Emotive EPOC+是一款消费级的脑电采集设备，在消费级的脑电采集设备中，信号质量还算不错，但是比较坑的一点是这个设备的开发许可(Epotive Pro)按月收费（起初是8K软妹币/年，现在的收费方式可能有所变化，且具有学生优惠价格），幸好在网上找到了医工荟通过Cykit将OpenVIBE与EPOC+连接的方法，由于比较穷所以果断按照教程白嫖了。

医工荟教程链接：https://cloud.tencent.com/developer/news/337802
目前Cykit已经更到Cykit3了，之前的版本也不再维护，大家可以直接使用新版的Cykit，相比上文中的操作流程有所变动，但是变化不大。Cykit3链接：https://github.com/CymatiCorp/CyKit。

现在Emotive官方提供了设备和OV、Matlab、Unity等连接的方式，如果有Emotive Pro的小伙伴可以直接通过LSL与OV连接，我没有测试过，这里就不放链接了。

补充一点，通过Cykit与OV连接后，OV中显示的是Channel1、Channel2…Channel14，不太方便进行处理，因此需要手动进行通道映射。首先点击Change channel names，然后按照下图顺序进行设置就好啦。
在这里插入图片描述
在这里插入图片描述

参考链接：
https://cloud.tencent.com/developer/news/337802
https://github.com/CymatiCorp/CyKit

