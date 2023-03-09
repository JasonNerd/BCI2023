# EEGLab软件库介绍
## [1. EEGLab简介?](https://sccn.ucsd.edu/eeglab/index.php)
### （1）是什么？
EEGLab是一个**交互式的Matlab工具库**, 用于处理连续和事件相关EEG、MEG和其他电生理数据，包括**独立分量分析（independent component analysis, ICA）、时域/频域分析（time/frequency analysis）、伪影抑制(artifact rejection)、事件相关统计以及平均和单次试验数据的几种可用的可视化模式**。EEGLAB可在Linux、Unix、Windows和Mac OS X下运行。

EEGLAB提供交互式<u>图形用户界面（GUI）</u>，允许用户使用独立分量分析（ICA）和/或时间/频率分析（TFA）以及标准平均方法灵活地和交互式地处理其高密度EEG和其他动态脑数据。EEGLAB还<u>集成了大量的教程和帮助窗口</u>，以及命令历史功能，方便用户从基于GUI的数据探索过渡到构建和运行批处理或自定义数据分析脚本。

### （2）EEGLab有哪些特点和功能？
|Features|特征|
|:--|:--|
Academic (free) software |学术（自由）软件 |
Running on Matlab or standalone | 在Matlab上运行或独立运行 |
Graphic user interface | 图形用户界面|
Multiformat data importing | 多格式数据导入|
High-density data scrolling | 高密度数据滚动|
Interactive plotting functions | 交互式绘图功能|
Semi-automated artifact removal |半自动伪影去除|
ICA & time/frequency transforms| ICA与时域频域变换|
Event & channel location handling|事件和频道位置处理|
Forward/inverse head/source modeling|正/逆头/源建模|
Defined EEG & STUDY data structures|定义EEG和研究数据结构|
Over 120 advanced plug-in/extensions|超过120个高级插件/扩展|

### （3）软硬件要求？
最新版本的EEGLAB可在任何操作系统（Linux/Unix、Windows、Mac OSX）下的Matlab 7.6（2008 b）或更高版本运行。

内存要求：使用具有大量RAM的多核64位处理器对于分析大型数据集可能是必不可少的--建议使用8 Gb或更大的RAM（有关最小化内存使用的技巧，还请参见EEGLAB wiki教程）。**Linux是使用EEGLAB处理EEG数据的首选环境**，主要是因为Linux下Matlab的内存管理更好（**如果使用Linux，选择Fedora而不是Ubuntu**，因为有时Matlab在Ubuntu下处理OpenGL会出现轻微的图形问题）。

其他Matlab工具箱：EEGLAB不需要额外的工具箱。但是，建议使用一些工具箱。按照重要性的顺序：
|TooBox|简述|
|:--|:--|
|Signal Processing toolbox | 尽管EEGLAB在必要时并入了函数以替换它从该工具箱使用的函数（例如，对于滤波和功率谱计算），它们不如工具箱Matlab函数有效。一些EEGLAB扩展（如SIFT）也需要此工具箱。这可能是最重要的工具箱。|
|Statistics toolbox|一些EEGLAB扩展（例如Fieldtrip和SIFT）需要该工具箱。该工具箱还包含大量函数，可用于高级程序员计算统计数据和交叉验证。|
|Optimization toolbox|某些EEGLAB扩展使用的另一个推荐工具箱。这个工具箱包含强大的fminsearch函数和微分。虽然Matlab现在在其核心发行版中默认有此函数，但优化工具箱允许对其参数进行更精细的调整|
|Image processing toolbox|某些EEGLAB扩展（如Fieldtrip）需要此工具箱|

## [2. EEGLab下载与安装](https://sccn.ucsd.edu/eeglab/downloadtoolbox.php)
下载链接(https://sccn.ucsd.edu/eeglab/currentversion/eeglab_current.zip)

安装方法:
1. 将EEGLAB压缩文件解压缩到您选择的文件夹中
2. 启动Matlab
3. 将Matlab路径更改为刚刚解压缩的EEGLAB文件夹
4. 在Matlab提示符下输入`eeglab`并按Enter键

另：独立于MatLab 的版本: https://sccn.ucsd.edu/eeglab/currentversion/eeglab_compiled_windows.zip

## [3. 加载、显示数据](https://blog.csdn.net/zyb228/article/details/102553620)




