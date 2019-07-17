#PyTorch环境搭建

环境：Windows 10 64-bit, Anaconda 2019.03 Python 3.7 version, PyTorch 1.1, PyCharm

##安装

Windows下正常安装Anaconda

按照[PyTorch中文手册](https://github.com/zergtant/pytorch-handbook "PyTorch中文手册")的方法安装PyTorch

正常安装PyCharm

##配置PyCharm

可以参考[这个教程](https://blog.csdn.net/WJ_MeiMei/article/details/84141521 "这个教程")的方法对PyCharm进行配置

打开PyCharm之后，创建一个新项目

在新项目中File->New->Python File创建新文件，可以输入以下代码供测试

```python
    import torch
    print(torch.rand(5,3))
```

保存后File->Settings->Project:*工程名*->Project Interpreter当中点击目录右侧的按钮Add

选择Conda Environment当中的Existing environment，在目录中选择..\Anaconda3\envs\pytorch\python.exe

Run运行，应该输出5行3列的随机矩阵
