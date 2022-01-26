---
title: 函数功能列表
date: 2021-10-29 23:50:00
tags:
 - gma
 - Python
categories:
 - 地理与气象分析库
sticky: 2
---

**&emsp;&emsp;函数功能列表** 列出了 gma 包含的所有可用函数定义和说明，**可以快速了解所有的函数和功能**。如果你需要详细的函数参数说明，请在 Python 中使用 ```help``` 获取函数帮助或参考 [使用指南](UserGuide-index.html)。

<!-- more -->

## index 指数运算

&emsp;&emsp;指数运算函数 **基于 数 或 Numpy 数组**。

 函数 | 引用（简版）| 功能 | 详细解释                          
 :----- | :----- | :----- | :-----
[EVI](UserGuide-index.html#evi) | gma.index.EVI     | 【EVI】     | 增强植被指数                      
[NDBI](UserGuide-index.html#ndbi)| gma.index.NDBI    | 【NDBI】    | 归一化建筑指数                    
[NDWI](UserGuide-index.html#ndwi)  | gma.index.NDWI    | 【NDWI】    | 归一化水指数                      
[NDVI](UserGuide-index.html#ndvi) | gma.index.NDVI    | 【NDVI】    | 归一化植被指数                    
[PM_ET0](UserGuide-index.html#pm-et0) | gma.index.PM_ET0 | 【PM_ET0】 | Penman-Monteith 法作物参考蒸散量 
[TVDI](UserGuide-index.html#tvdi) <Badge text="1.0.2 +"/> | gma.index.TVDI    | 【TVDI】    | 温度植被干旱指数                  

 ## math 数学运算

&emsp;&emsp;数学运算函数基于 **Numpy 数组 或 Pandas 数据帧** 。

| （类）函数          | 引用（简版）                     | 功能               | 详细解释                                                     |
| :------------------ | :------------------------------- | :----------------- | :----------------------------------------------------------- |
| [_DFToNumeric](UserGuide-math.html#dftonumeric)       | gma.math._DFToNumeric         | 【强制转换为数字】 | 强制将 pandas 数据帧中的数据转换数字， 其中不能转换为数字的字符串将被转换为 NAN |
| [FillNoData](UserGuide-math.html#fillnodata)          | gma.math.FillNoData            | 【填充缺失值】     | 对缺失值或异常值值进行插值替换                               |
| [**Smooth.**](UserGuide-math.html#smooth-类)[SavitzkyGolay](UserGuide-math.html#savitzkygolay)             | gma.math.Smooth.SavitzkyGolay | 【SavitzkyGolay】  | 利用SavitzkyGolay方法对数据进行平滑                          |
| [**Smooth.**](UserGuide-math.html#smooth-类)[MovingAverage](UserGuide-math.html#movingaverage)       | gma.math.Smooth.MovingAverage | 【滑动平均】       | 利用滑动平均法对数据进行平滑                                 |
| [**Evaluation.**](UserGuide-math.html#evaluation-类)[RMSE](UserGuide-math.html#rmse)    | gma.math.Evaluation.RMSE      | 【RMSE】           | 均方根误差                                                   |
| [**Evaluation.**](UserGuide-math.html#evaluation-类)[NRMSE](UserGuide-math.html#nrmse)   | gma.math.Evaluation.NRMSE     | 【NRMSE】          | 归一化均方根误差                                             |
| [**Evaluation.**](UserGuide-math.html#evaluation-类)[D](UserGuide-math.html#d)       | gma.math.Evaluation.D         | 【D】              | D指标                                                        |
| [**Evaluation.**](UserGuide-math.html#evaluation-类)[CORR](UserGuide-math.html#corr)       | gma.math.Evaluation.CORR         | 【r，P】           | 相关系数和显著性水平                                         |
| [**Evaluation.**](UserGuide-math.html#evaluation-类)[R2](UserGuide-math.html#r2)      | gma.math.Evaluation.R2        | 【R2】             | 决定系数                                                     |
| [**Evaluation.**](UserGuide-math.html#evaluation-类)[MaxAE](UserGuide-math.html#maxae)   | gma.math.Evaluation.MaxAE     | 【MaxAE】          | 最大绝对误差                                                 |
| [**Evaluation.**](UserGuide-math.html#evaluation-类)[Select](UserGuide-math.html#select)  | gma.math.Evaluation.Select    | 【选择方法】       | 选择Evaluation中需要计算的一个或多个评价指标进行计算         |
| [**Evaluation.**](UserGuide-math.html#evaluation-类)[Methods](UserGuide-math.html#methods) | gma.math.Evaluation.Methods   | 【记录方法】       | 记录Evaluation类中所有的评估方法                             |

 ## osf 系统交互

| （类）函数       | 引用（简版）                | 功能         | 详细解释                                         |
| :--------------- | :-------------------------- | :----------- | :----------------------------------------------- |
| [GetPath](UserGuide-osf.html#getpath)          | gma.osf.GetPath           | 【获取路径】 | 获取目标 路径或路径集合下满足条件的所有文件夹和文件路径                              |
| [Zip](UserGuide-osf.html#zip)            | gma.osf.Zip               | 【压缩】     | 将目标路径下所有文件压缩为 .zip 文件                  |
| [UnZip](UserGuide-osf.html#unzip)            | gma.osf.UnZip             | 【解压缩】   | 解压缩 .zip 文件                                |
| [DateSeries](UserGuide-osf.html#dateseries)       | gma.osf.DateSeries        | 【日期序列】 | 构造一个日期序列列表                               |
| [**Modify.**](UserGuide-osf.html#rename-类)[Rename](UserGuide-osf.html#modify)    | gma.osf.Rename.Modify    | 【修改】     | 将原有文件（夹）名修改为新名                     |
| [**Modify.**](UserGuide-osf.html#rename-类)[Replace](UserGuide-osf.html#replace)  | gma.osf.Rename.Replace   | 【替换】     | 替换原文件（夹）名中字符串后作为新文件（夹）名   |
| [**Modify.**](UserGuide-osf.html#rename-类)[Intercept](UserGuide-osf.html#intercept) | gma.osf.Rename.Intercept | 【截取】     | 截取文件（夹）名中的部分字符串作为新文件（夹）名 |
| [MultiThreading](UserGuide-osf.html#multithreading)<Badge text="1.0.3 +"/> | gma.osf.MultiThreading | 【多线程】 | 创建多个线程，实现同一函数多个参数的同步执行。 |

 ## smc 空间杂项

| 函数 | 引用（简版）| 功能 | 详细解释|                      
| :----- | :----- | :----- | :-----|
|[CALDistanceFromPoint](UserGuide-smc.html#callengthfrompoint)<Badge text="1.0.5 +"/> | gma.smc.CALDistanceFromPoint |【计算距离】|计算输入两点（或多点）之间的距离。|

 ## rasp 栅格处理

| （类）函数                                                   | 引用（简版）                  | 功能                | 详细解释                                                     |
| :----------------------------------------------------------- | :---------------------------- | :------------------ | :----------------------------------------------------------- |
| [BandSynthesis](UserGuide-rasp.html#bandsynthesis)               | gma.rasp.BandSynthesis        | 【文件合并】        | 单波段文件合成多波段文件                                     |
| [BandDecomposition](UserGuide-rasp.html#banddecomposition)       | gma.rasp.BandDecomposition    | 【波段分解】        | 将多波段文件拆分（或提取）为单波段文件                       |
| [Clip](UserGuide-rasp.html#clip)                                 | gma.rasp.Clip                 | 【裁剪】            | 按矢量边界裁剪栅格                                           |
| [ToOtherFormat](UserGuide-rasp.html#tootherformat)               | gma.rasp.ToOtherFormat        | 【格式转换】        | 一种栅格格式转换为另一种栅格格式                             |
| [Mosaic](UserGuide-rasp.html#mosaic)                             | gma.rasp.Mosaic               | 【栅格镶嵌】        | 将多个栅格数据集合并到一个新的栅格数据集中                   |
| [Resample](UserGuide-rasp.html#resample)                         | gma.rasp.Resample             | 【重采样】          | 更改栅格数据的空间分辨率                                     |
| [Reproject](UserGuide-rasp.html#reproject)                       | gma.rasp.Reproject            | 【重投影】          | 将空间数据从一种坐标系投影到另一种坐标系                     |
| [ChangeDataType](UserGuide-rasp.html#changedatatype)             | gma.rasp.ChangeDataType       | 【数据类型转换】    | 转换栅格数据的数据类型                                       |
| [MultiSDSToTif](UserGuide-rasp.html#multisdstotif)               | gma.rasp.MultiSDSToTif        | 【多维数据转GTiff】 | 将含有子数据集的多维数据提取为 GTiff                         |
| [ToVector](UserGuide-rasp.html#tovector)                        | gma.rasp.ToVector             | 【栅格转矢量】      | 将栅格数据转换为矢量数据                                     |
| [WriteRaster](UserGuide-rasp.html#writeraster)                  | gma.rasp.WriteRaster          | 【写出栅格】        | 将数组保存为栅格                                             |
| [GenerateOVR](UserGuide-rasp.html#generateovr)                  | gma.rasp.GenerateOVR          | 【构建栅格金字塔】  | 为GTiff文件构造 .ovr 栅格金字塔，或为其他类型的栅格数据强制构造.ovr金字塔 |
| [OrthophotoCorrection](UserGuide-rasp.html#orthophotocorrection) | gma.rasp.OrthophotoCorrection | 【正射矫正】        | 根据有理多项式系数（RPC）对影像进行正射校正                  |
| [Deformation](UserGuide-rasp.html#deformation)                  | gma.rasp.Deformation          | 【流程化处理】      | 完成镶嵌-裁剪-重采样-重投影-格式转换等其中一个或多个功能     |
| [**Fusion.**](UserGuide-rasp.html#fusion-类)[Pansharpen](UserGuide-rasp.html#pansharpen) | gma.rasp.Fusion.Pansharpen    | 【Pansharpen】      | 对全色影像和多光谱影像基于Pansharpen方法进行融合             |
| [AddColorTable](UserGuide-rasp.html#addcolortable)<Badge text="1.0.1 +"/> | gma.rasp.AddColorTable        | 【添加色彩映射表】  | 为栅格数据添加色彩映射                                       |
| [SplitImage](UserGuide-rasp.html#splitimage)<Badge text="1.0.3 +"/> | gma.rasp.SplitImage           | 【影像切片】        | 将一幅影像切分为特定行列数的小影像。                         |

&emsp;&emsp;此外，gma 提供了 [Open](UserGuide-rasp.html#open) 类实现栅格数据的读取操作，主要栅格数据的操作如下：

| 属性 / 方法    | 引用（简版）                         | 功能                            | 详细解释|
| :------------- | :--------------------------- | :------------------------------ |:-----|
| [Bands](UserGuide-rasp.html#bands)          | gma.rasp.Open.Bands          |【波段数】                  |获取栅格波段数   |
| [Columns](UserGuide-rasp.html#columns)        | gma.rasp.Open.Columns        |  【列数】                  |获取栅格列数（X）   |
| [Rows](UserGuide-rasp.html#rows)          | gma.rasp.Open.Rows           |  【行数】                       |获取栅格行数（Y）|
| [ToArray](UserGuide-rasp.html#toarray)        | gma.rasp.Open.ToArray        | 【转为数组】    | 将栅格数据读取为 Numpy 数组|
| [DataType](UserGuide-rasp.html#datatype)       | gma.rasp.Open.DataType       | 【数据类型】            |获取栅格数据的数据类型|
| [Driver](UserGuide-rasp.html#driver)         | gma.rasp.Open.Driver         |  【栅格驱动】                  |获取栅格数据驱动 |
| [GeoTransform](UserGuide-rasp.html#geotransform)   | gma.rasp.Open.GeoTransform   |  【仿射变换】                 |获取栅格仿射变换  |
| [GetBand](UserGuide-rasp.html#getband)        | gma.rasp.Open.GetBand        | 【获取 Band】        |读取某一波段为 gdal.Band |
| [GetBandToArray](UserGuide-rasp.html#getbandtoarray) | gma.rasp.Open.GetBandToArray |  【转换波段为数组】    |将某一波段读取为 Numpy 数组|
| [GetGDALDataset](UserGuide-rasp.html#getgdaldataset) | gma.rasp.Open.GetGDALDataset | 【获取 GDALDataset】 |读取栅格数据为 gdal.GDALDataset|
| [NoData](UserGuide-rasp.html#nodata)         | gma.rasp.Open.NoData         |  【无效值】                 | 获取栅格无效值|
| [Projection](UserGuide-rasp.html#projection)     | gma.rasp.Open.Projection     |  【坐标系】                   |获取栅格坐标系 |

::: tip 提示

&emsp;&emsp;Open 类的属性/方法在 gma 内部调用，并对名称进行了修改，使其表达的内容更易理解，一定程度上可以代替 gdal.Open。
:::

## vesp 矢量处理

| （类）函数    | 引用（简版）             | 说明             | 解释                                     |
| :------------ | :----------------------- | :--------------- | :--------------------------------------- |
| [Split](UserGuide-vesp.html#split)         | gma.vesp.Split         | 【矢量文件分解】 | 将矢量文件的每个要素拆分为单个文件       |
| [Check](UserGuide-vesp.html#check)         | gma.vesp.Check         | 【检查】         | 检查每个矢量要素的有效性                       |
| [ToRaster](UserGuide-vesp.html#toraster)      | gma.vesp.ToRaster      | 【矢量转栅格】   | 将矢量图层转换为栅格文件                 |
| [Clip](UserGuide-vesp.html#clip)          | gma.vesp.Clip          | 【裁剪】         | 矢量裁剪矢量                             |
| [Erase](UserGuide-vesp.html#erase)         | gma.vesp.Erase         | 【擦除】         | 从第一个矢量中去除与第二个矢量交叉的部分 |
| [Intersection](UserGuide-vesp.html#intersection)  | gma.vesp.Intersection  | 【交集】         | 取两个矢量的交集                         |
| [Union](UserGuide-vesp.html#union)         | gma.vesp.Union         | 【融合】         | 取两个矢量的并集                         |
| [Update](UserGuide-vesp.html#update)        | gma.vesp.Update        | 【更新】         | 用一个矢量更新另一个矢量                 |
| [ToOtherFormat](UserGuide-vesp.html#tootherformat) | gma.vesp.ToOtherFormat | 【格式转换】     | 一种矢量格式转换为另一种矢量格式         |
| [Reproject](UserGuide-vesp.html#reproject)     | gma.vesp.Reproject     | 【重投影】       | 将矢量数据从一种坐标系投影到另一种坐标系                       |
| [SymDifference](UserGuide-vesp.html#symdifference) <Badge text="1.0.4 +"/>    | gma.vesp.SymDifference    | 【交集取反】       | 取两个矢量不相交的部分                       |
