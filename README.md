# MedFM
首先在conda中新建一个环境
```Shell
conda create --name openmmlab python=3.9 -y
conda activate openmmlab
```
接着安装pytorch，注意必须安装GPU版本，根据自己的电脑显卡型号选择相应的CUDA安装，再根据CUDA版本安装pytorch，若安装的是CPU版本之后运行代码使用mmcv库会报错显示没有用上CUDA

将所给的MedFM git到自己电脑中，git安装指南：<https://blog.csdn.net/Andone_hsx/article/details/87937329>，遇到问题见评论区解决方案

确保pytorch安装成功后进行下一步安装：
```Shell
pip install mmcls==0.25.0 openmim scipy scikit-learn ftfy regex tqdm
mim install mmcv-full==1.6.0
```
其中第二行代码可能会报错，因此去mmcv-full官网下载whl文件，官网网址：<https://download.openmmlab.com/mmcv/dist/cu111/torch1.9.0/index.html>，下载自己电脑适应的，接着在conda中pip install一下
安装完了mmcv-full之后跑代码依然会报错显示没有mmcv-full库，未解决

剩下的跟着比赛提供的readme文档走

其中config文件的阅读见<https://mmpretrain.readthedocs.io/zh-cn/latest/get_started.html>读懂配置即明白具体原理

