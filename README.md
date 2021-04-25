# Inkscape-use-reminder
## 前言
Inkscape是常用的科研作图软件，这里是我重新上传的一份exe文件（1.0.2 version）：
链接：https://pan.baidu.com/s/1OeB646F8I_Y5gqXYYF33Pg 
提取码：vxp0 

本文是在Inkscape中作图中遇到的问题，及其实用小指南，作为个人备忘的同时也帮助大家不要重复造轮子。
## 1.仅在inkscape中添加latex公式，而不使用其他插件
之前发现Extension自带的渲染不行了，就下了个这

1.下载TexText扩展 https://inkscape.org/~jcwinkler/%E2%98%85textext
我重新上传为：
链接：https://pan.baidu.com/s/1RwnoS8j-sO2ZjO-ZvroRUA 
提取码：f99n 

该扩展在git的页面是
Sourcecode: https://github.com/textext/textext

2.windows平台解压压缩包，管理员运行批处理文件。

3.打开inkscape，在扩展-文字中将出现textext选项。这就说明安装已经完成。

## 2.一系列数学插件的安装和使用
### 2.1.基本操作：安装inkscapeMadeEasy扩展，这扩展是使用其他扩展的基础

git地址为https://github.com/fsmMLK/inkscapeMadeEasy

1.直接打包下载，解压之后唯一有用的就是那个latest文件夹。

2.首先打开此文件夹复制里面所有文件（3个.py和一个.tex），再打开inkscape，快捷键ctrl+shift+p打开首选项（在编辑中找也行），之后点击系统，再打开用户扩展的文件夹位置，一般是

![捕获](https://user-images.githubusercontent.com/59023098/115977060-dadcf500-a5a6-11eb-8340-a8a812de9f5d.PNG)


3.如果装了textext，这里会出现它的文件夹。

4.新建一个名为`inkscapeMadeEasy` **要求命名完全一致** 的文件夹，将上述文件复制进去即可。

这里呈现的最终效果大概是这样

![捕获](https://user-images.githubusercontent.com/59023098/115976919-4c1ba880-a5a5-11eb-99f1-298b1a821635.PNG)


有了这个插件，就可以支持如下的诸插件：

![捕获](https://user-images.githubusercontent.com/59023098/115976975-bfbdb580-a5a5-11eb-9b38-58546d1f8727.PNG)


这些插件可以大幅提高作图速度。

**注意：所有的插件安装后要重启inkscape才可用。**

### 2.2.安装和使用cartesianPlotFunction2D扩展

这扩展支持使用LaTeX标注和自定义的步长与标尺，功能相当于2维的 matlab plot功能。

https://github.com/fsmMLK/inkscapeCartesianPlotFunction2D

安装的方法和前面基本一样，同样是打包下载，然后把latest里面的两个文件（.inx和.py）复制出来，在用户扩展的文件夹位置里新建一个文件夹，命名为`cartesianPlotFunction2D`，重启Inkscape，在扩展——fsmMLK——一直点下去就能打开该功能。

这个扩展的渲染速度很慢，不能指望它像Matlab那样秒出图，可以在出图前去做点别的事情。

### 2.3.安装和使用slopeField扩展
这个是向量场的绘图工具，不过只能用于一阶ODE。

https://github.com/fsmMLK/inkscapeSlopeField

安装方法与前面的完全一样，文件夹名为`slopeField`，也在扩展——fsmMLK——plot2D——Cartesian之类的后面找到。


