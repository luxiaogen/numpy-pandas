# numpy&pandas

## numpy介绍
NumPy 是一个运行速度非常快的数学库，主要用于数组计算，包含：
- 一个强大的N维数组对象 ndarray
- 广播功能函数
- 整合 C/C++/Fortran 代码的工具
- 线性代数、傅里叶变换、随机数生成等功能

> NumPy 通常与 SciPy（Scientific Python）和 Matplotlib（绘图库）一起使用， 这种组合广泛用于替代 MatLab，是一个强大的科学计算环境，有助于我们通过 Python 学习数据科学或者机器学习。
> SciPy 是一个开源的 Python 算法库和数学工具包。
> SciPy 包含的模块有最优化、线性代数、积分、插值、特殊函数、快速傅里叶变换、信号处理和图像处理、常微分方程求解和其他科学与工程中常用的计算。
> Matplotlib 是 Python 编程语言及其数值数学扩展包 NumPy 的可视化操作界面。它为利用通用的图形用户界面工具包，如 Tkinter, wxPython, Qt 或 GTK+ 向应用程序嵌入式绘图提供了应用程序接口（API）。

## Numpy Ndarray对象
- `ndarray`的内部结构

<img src="/Users/luxiaogen/workspace/code/python/numpy+pandas/images/image-20251010154855749.png" alt="image-20251010154855749" style="zoom:30%;" />

> - 一个指向数据（内存或内存映射文件中的一块数据）的指针
> - 数据类型或 dtype，描述在数组中的固定大小值的格子
> - 一个表示数组形状（shape）的元组，表示各维度大小的元组
> - 一个跨度元组（stride），其中的整数指的是为了前进到当前维度下一个元素需要"跨过"的字节数