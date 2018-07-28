# 离线地图显示

------

相关内容说明，分为以下几部分：

> * 支持功能
> * 资源文件配置和使用
> * 运行环境

## 支持功能

加载本地卫星瓦片地图、矢量地图，支持矢量地图显示控制


## 资源文件配置和使用

运行时需要瓦片地图、矢量地图

### 1. 卫星图数据

瓦片地图采用google瓦片地图，内置地图目录为```./Data/TileMap``` 可自行下载并切割，通过配置文件设置瓦片地图路径。如可通过下述连接下载卫星图数据map.iso并加载至虚拟光驱，记录盘符如 ```V:``` 更改配置文件 ```config.ini``` 中卫星图目录配置如下：
```ini
[tile]
path=V:/
```
iso下载 [百度网盘地址](https://pan.baidu.com/s/1lLXLmtKrQhUOH_s1eW7ljA)


### 2. 矢量地图数据

矢量地图数据内置，目录为 ```./Data/VectorMap``` 使用gdal库加载

## 运行环境
需要的运行环境为 Qt5.6 mingw 使用的动态库 ```libgdal.dll``` 需放置到 ```MapDemo.exe``` 相同目录