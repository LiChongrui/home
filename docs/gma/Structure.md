---
title: 库组织方式
date: 2021-10-29 23:35:00
tags:
 - gma
 - Python
categories:
 - 地理与气象分析库
---
&emsp;&emsp;不同的类型的函数在 gma 中分类构建，**库组织方式**列出了 gma 库的整体组织和构造，供大家了解和参考。

<!-- more -->

::: theorem 函数包和依赖文件的组织关系和说明

- **algorithm**&emsp;&emsp; &emsp;&emsp; ||栅格、矢量操作的**基础算法**
	* raster &emsp;&emsp; &emsp;&emsp; &emsp;&emsp; ——栅格处理， rasp 调用的**算法** 
	* vector &emsp;&emsp; &emsp;&emsp; &emsp;&emsp; ——矢量处理，vesp 调用的**算法**
- **Relation**&emsp;&emsp; &emsp;&emsp; || 关键 **关联参数** 设置
	* error &emsp;&emsp; &emsp;&emsp; &emsp;&emsp; ——输入**参数检查**，错误提示
	* [**key**](Default.html#默认参数) &emsp;&emsp; &emsp;&emsp; &emsp;&emsp; ——栅格/矢量 处理的高阶参数设置，例如**压缩**，**超大 TIFF 支持**等
- [**index**](Function.html#index-指数运算)&emsp;&emsp; &emsp;&emsp; || 遥感、气象的**指数运算**的相关算法
- [**math**](Function.html#math-数学运算)&emsp;&emsp; &emsp;&emsp; || **数学运算**相关算法
- [**osf**](Function.html#osf-系统交互)&emsp;&emsp;&emsp; &emsp;&emsp; || **系统交互**操作
- [**smc**](Function.html#smc-空间杂项)&emsp;&emsp;&emsp; &emsp;&emsp; || **空间杂项**计算
- [**rasp**](Function.html#rasp-栅格处理)&emsp;&emsp; &emsp;&emsp; || **栅格处理**函数包
- [**vesp**](Function.html#vesp-矢量处理)&emsp;&emsp; &emsp;&emsp; || **矢量处理**函数包

:::
