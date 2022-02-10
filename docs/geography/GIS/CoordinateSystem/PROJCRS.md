---
title: 其他投影坐标系
date: 2022-02-20
tags:
 - 坐标系
categories:
 - 地信研学
---

&emsp;　本页对 44 个 其他类型的投影坐标系进行汇总，由于其与原有的投影坐标系统有所不同，故分开统计。

<!-- more -->

## 简介

&emsp;　本页统计的地理坐标系具有特有属性特征。在利用 osr （osgeo 的模块）进行识别时，本页所列举的地理坐标系标识为 `PROJCRS` ，与另一部分投影坐标系的标识 `PROJCS` 不同，但两者都能被识别（利用 IsProjected 方法）为投影坐标系这一类，且其具有适用范围边界等一些特殊的参数。

## 其他参数

&emsp;　其他参数详见 [投影坐标系](PROJCS.html)  中相关内容。

## 主要坐标参数

### Hyperbolic Cassini-Soldner

| 官方 ID   | 坐标系名称                        |   自然原点纬度（°） |   自然原点经度（°） |   东伪偏移（m） |   北伪偏移（m） | 长度单位   | 适用范围（S，W，N，E）（°）                    |
|:----------|:----------------------------------|:-----------------------------|:------------------------------|:----------------|:-----------------|:-----------|:----------------------------|
| EPSG:3139 | Vanua Levu 1915 / Vanua Levu Grid |                       -16.25 |                       179.333 |     1.25133e+06 |      1.66289e+06 | link       | -17.07,178.42,-16.1,-179.77 |

### Guam Projection

| 官方 ID   | 坐标系名称            |   自然原点纬度（°）|   自然原点经度（°） |  东伪偏移（m）  |   北伪偏移（m） | 长度单位   | 适用范围 （S，W，N，E）（°）  |
|:----------|:----------------------|:-----------------------------|:------------------------------|:----------------|:-----------------|:-----------|:-------------------------|
| EPSG:3993 | Guam 1963 / Guam SPCS |                      13.4725 |                       144.749 |           50000 |            50000 | metre      | 13.18,144.58,13.7,145.01 |

### Lambert Conic Conformal (2SP Michigan)

| 官方 ID    | 坐标系名称               | 长度单位       | 适用范围（S，W，N，E）（°）   |   伪原点纬度（°） |   伪原点经度（°） |   第一标准纬线纬度（°） |   第二标准纬线纬度（°） |   伪原点东偏移（m） |   伪原点北偏移（m）|   椭球体比例因子	|
|:-----------|:-------------------------|:---------------|:--------------------------|:---------------------------|:----------------------------|:------------------------------------|:------------------------------------|:--------------------------|:---------------------------|:---------------------------|
| EPSG:6200  | NAD27 / Michigan North   | US survey foot | 45.08,-90.42,48.32,-83.44 |                    44.7833 |                    -87      |                             45.4833 |                             47.0833 |                   2000000 |                          0 |                    1.00004 |
| EPSG:6201  | NAD27 / Michigan Central | US survey foot | 43.8,-87.06,45.92,-82.27  |                    43.3167 |                    -84.3333 |                             44.1833 |                             45.7    |                   2000000 |                          0 |                    1.00004 |
| EPSG:6202  | NAD27 / Michigan South   | US survey foot | 41.69,-87.2,44.22,-82.13  |                    41.5    |                    -84.3333 |                             42.1    |                             43.6667 |                   2000000 |                          0 |                    1.00004 |
| EPSG:6966  | NAD27 / Michigan North   | US survey foot | 45.08,-90.42,48.32,-83.44 |                    44.7833 |                    -87      |                             45.4833 |                             47.0833 |                   2000000 |                          0 |                    1.00004 |
| EPSG:26811 | NAD27 / Michigan North   | US survey foot | 45.08,-90.42,48.32,-83.44 |                    45.45   |                    -87      |                             45.4833 |                             47.0833 |                   2000000 |                          0 |                    1.00004 |
| EPSG:26812 | NAD27 / Michigan Central | US survey foot | 43.8,-87.06,45.92,-82.27  |                    43.3167 |                    -84.3333 |                             44.1833 |                             45.7    |                   2000000 |                          0 |                    1.00004 |
| EPSG:26813 | NAD27 / Michigan South   | US survey foot | 41.69,-87.2,44.22,-82.13  |                    41.5    |                    -84.3333 |                             42.1    |                             43.6667 |                   2000000 |                          0 |                    1.00004 |

### Colombia Urban

| 官方 ID   | 坐标系名称                                      |   自然原点纬度（°） |   自然原点经度（°） |    东伪偏移（m） |   北伪偏移（m） | 长度单位   | 适用范围（S，W，N，E）（°）                  |   投影平面原点高度（m） |
|:----------|:------------------------------------------------|:-----------------------------|:------------------------------|:-----------------|:-----------------|:-----------|:--------------------------|:---------------------------------|
| EPSG:6244 | MAGNA-SIRGAS / Arauca urban grid                |                      7.08761 |                      -70.7583 |      1.03526e+06 |      1.27553e+06 | metre      | 7.05,-70.78,7.1,-70.71    |                           100    |
| EPSG:6245 | MAGNA-SIRGAS / Armenia urban grid               |                      4.53233 |                      -75.6735 |      1.15582e+06 | 993087           | metre      | 4.5,-75.73,4.55,-75.65    |                          1470    |
| EPSG:6246 | MAGNA-SIRGAS / Barranquilla urban grid          |                     10.9232  |                      -74.8343 | 917264           |      1.69984e+06 | metre      | 10.85,-74.87,11.06,-74.75 |                           100    |
| EPSG:6247 | MAGNA-SIRGAS / Bogota urban grid                |                      4.68049 |                      -74.1466 |  92334.9         | 109321           | metre      | 4.45,-74.27,4.85,-73.98   |                          2550    |
| EPSG:6248 | MAGNA-SIRGAS / Bucaramanga urban grid           |                      7.07889 |                      -73.1973 |      1.09724e+06 |      1.27464e+06 | metre      | 7.03,-73.19,7.17,-73.06   |                           931    |
| EPSG:6249 | MAGNA-SIRGAS / Cali urban grid                  |                      3.44188 |                      -76.5206 |      1.0619e+06  | 872365           | metre      | 3.32,-76.61,3.56,-76.42   |                          1000    |
| EPSG:6250 | MAGNA-SIRGAS / Cartagena urban grid             |                     10.397   |                      -75.5112 | 842981           |      1.64189e+06 | metre      | 10.27,-75.57,10.47,-75.42 |                             0    |
| EPSG:6251 | MAGNA-SIRGAS / Cucuta urban grid                |                      7.88894 |                      -72.5029 | 842805           |      1.3644e+06  | metre      | 7.81,-72.56,7.97,-72.46   |                           308    |
| EPSG:6252 | MAGNA-SIRGAS / Florencia urban grid             |                      1.62101 |                      -75.6191 |      1.1623e+06  | 671069           | metre      | 1.57,-75.63,1.65,-75.59   |                           300    |
| EPSG:6253 | MAGNA-SIRGAS / Ibague urban grid                |                      4.41941 |                      -75.1799 | 877634           | 980541           | metre      | 4.39,-75.27,4.47,-75.11   |                          1100    |
| EPSG:6254 | MAGNA-SIRGAS / Inirida urban grid               |                      3.84544 |                      -67.9052 |      1.01918e+06 | 491791           | metre      | 3.8,-67.94,3.9,-67.88     |                            96    |
| EPSG:6255 | MAGNA-SIRGAS / Leticia urban grid               |                     -4.19768 |                      -69.9428 |  25978.2         |  27501.4         | metre      | -4.23,-69.98,-4.17,-69.92 |                            89.7  |
| EPSG:6256 | MAGNA-SIRGAS / Manizales urban grid             |                      5.06815 |                      -75.5111 |      1.17373e+06 |      1.05239e+06 | metre      | 5.02,-75.54,5.11,-75.44   |                          2100    |
| EPSG:6257 | MAGNA-SIRGAS / Medellin urban grid              |                      6.22921 |                      -75.5649 | 835379           |      1.18082e+06 | metre      | 6.12,-75.66,6.37,-75.5    |                          1510    |
| EPSG:6258 | MAGNA-SIRGAS / Mitu urban grid                  |                      1.24997 |                      -70.2355 |      1.09372e+06 | 629997           | metre      | 1.23,-70.25,1.29,-70.21   |                           170    |
| EPSG:6259 | MAGNA-SIRGAS / Mocoa urban grid                 |                      1.14002 |                      -76.651  |      1.04747e+06 | 617828           | metre      | 1.12,-76.66,1.18,-76.63   |                           655.2  |
| EPSG:6260 | MAGNA-SIRGAS / Monteria urban grid              |                      8.77309 |                      -75.8796 |      1.13181e+06 |      1.46213e+06 | metre      | 8.7,-75.94,8.81,-75.82    |                            15    |
| EPSG:6261 | MAGNA-SIRGAS / Neiva urban grid                 |                      2.94242 |                      -75.2964 | 864477           | 817200           | metre      | 2.87,-75.32,2.99,-75.23   |                           430    |
| EPSG:6262 | MAGNA-SIRGAS / Pasto urban grid                 |                      1.20099 |                      -77.2531 | 980470           | 624555           | metre      | 1.16,-77.32,1.26,-77.23   |                          2530    |
| EPSG:6263 | MAGNA-SIRGAS / Pereira urban grid               |                      4.81359 |                      -75.694  |      1.15349e+06 |      1.0242e+06  | metre      | 4.78,-75.77,4.87,-75.64   |                          1500    |
| EPSG:6264 | MAGNA-SIRGAS / Popayan urban grid               |                      2.45616 |                      -76.6061 |      1.05243e+06 | 763367           | metre      | 2.41,-76.65,2.49,-76.55   |                          1740    |
| EPSG:6265 | MAGNA-SIRGAS / Puerto Carreno urban grid        |                      6.18072 |                      -67.5008 |      1.06383e+06 |      1.17526e+06 | metre      | 5.98,-67.7,6.3,-67.41     |                            51.58 |
| EPSG:6266 | MAGNA-SIRGAS / Quibdo urban grid                |                      5.69425 |                      -76.6508 |      1.04727e+06 |      1.12144e+06 | metre      | 5.66,-76.67,5.72,-76.63   |                            44    |
| EPSG:6267 | MAGNA-SIRGAS / Riohacha urban grid              |                     11.5369  |                      -72.9028 |      1.12815e+06 |      1.76789e+06 | metre      | 11.42,-72.96,11.58,-72.84 |                             6    |
| EPSG:6268 | MAGNA-SIRGAS / San Andres urban grid            |                     12.5238  |                      -81.7294 | 820439           |      1.87736e+06 | metre      | 12.43,-81.82,12.65,-81.6  |                             6    |
| EPSG:6269 | MAGNA-SIRGAS / San Jose del Guaviare urban grid |                      2.56408 |                      -72.64   |      1.15988e+06 | 775380           | metre      | 2.54,-72.66,2.61,-72.6    |                           185    |
| EPSG:6270 | MAGNA-SIRGAS / Santa Marta urban grid           |                     11.2196  |                      -74.225  | 983892           |      1.73253e+06 | metre      | 11.16,-74.24,11.3,-74.13  |                            29    |
| EPSG:6271 | MAGNA-SIRGAS / Sucre urban grid                 |                      8.81055 |                      -74.7225 | 929044           |      1.46613e+06 | metre      | 8.79,-74.74,8.83,-74.69   |                            20    |
| EPSG:6272 | MAGNA-SIRGAS / Tunja urban grid                 |                      5.53419 |                      -73.3519 |      1.08051e+06 |      1.10377e+06 | metre      | 5.5,-73.39,5.61,-73.3     |                          2800    |
| EPSG:6273 | MAGNA-SIRGAS / Valledupar urban grid            |                     10.4473  |                      -73.2466 |      1.09098e+06 |      1.64721e+06 | metre      | 10.39,-73.3,10.51,-73.19  |                           200    |
| EPSG:6274 | MAGNA-SIRGAS / Villavicencio urban grid         |                      4.15538 |                      -73.6245 |      1.05068e+06 | 950952           | metre      | 4.07,-73.69,4.21,-73.56   |                           427.19 |
| EPSG:6275 | MAGNA-SIRGAS / Yopal urban grid                 |                      5.35393 |                      -72.42   | 851184           |      1.08395e+06 | metre      | 5.3,-72.43,5.37,-72.35    |                           300    |

### Equal Earth

| 官方 ID   | 坐标系名称                        |   自然原点经度（°） |   东伪偏移（m） |  北伪偏移（m） | 长度单位   | 适用范围（S，W，N，E）（°）              |
|:----------|:----------------------------------|:------------------------------|:----------------|:-----------------|:-----------|:---------------------|
| EPSG:8857 | WGS 84 / Equal Earth Greenwich    |                             0 |               0 |                0 | metre      | -90,-180,90,180      |
| EPSG:8858 | WGS 84 / Equal Earth Americas     |                           -90 |               0 |                0 | metre      | -90,90.01,90,89.99   |
| EPSG:8859 | WGS 84 / Equal Earth Asia-Pacific |                           150 |               0 |                0 | metre      | -90,-29.99,90,-30.01 |