{{indexmenu_n>30}}

# 监控代理

监控代理是UCloud自主研发并开源的辅助agent程序，在云主机或物理云主机中安装监控代理，能够让资源与云平台监控系统更好的协同工作，以扩展对资源的监控深度，丰富监控指标（如内存、磁盘空间、进程等）。

## 1.版本说明

> 注解 如需使用Linux内网数据上报版本，请重新安装agent；umagent已支持物理云主机，如安装后启动报错，请根据报错信息解决依赖关系。

| 更新时间   | Agent版本 | 更新说明                                                     | 备注 |
| ---------- | --------- | ------------------------------------------------------------ | ---- |
| 2019.08.12 | v1.1.5    | 修复 内核版本高于4.18时无法使用问题                          |      |
| 2018.01.03 | v1.1.4    | 修复 可能产生僵尸进程的bug                                   |      |
| 2017.10.31 | v1.1.3    | 新增 支持物理云采集GPU温度                                   |      |
| 2017.05.15 | v1.1.2    | 优化 Agent采集方式                                           |      |
| 2017.03.07 | v1.1.1    | 新增 加入物理云主机磁盘健康状态检查（0表示正常，1表示异常），支持centos和ubuntu操作系统 |      |
| 2016.11.01 | v1.1.0    | 1、新增 支持内网上报&支持内网下载Agent（**Windows版本更新**）。2、优化 WIndows版本不再需要配置公私钥，安装后启动即生效 |      |
| 2016.05.19 | v1.0.9    | 1、优化 Linux版本支持内网上报功能，uma不再需要外网上报数据。2、支持自动配置，不在需要手动配置 |      |
| 2016.03.25 | v1.0.8    | 1、修复 Windows版本上报阻塞bug。2、优化 Linux版本tcp连接数采集 |      |
| 2016.01.07 | v1.0.7    | 修复 磁盘名称过长导致采集数据错误的bug                       |      |
| 2015.10.29 | v1.0.6    | 1、优化 新版使用C和Python混合编写，无需安装nodejs等依赖库文件。2、优化 简化配置并能够将配置复用，避免了拷贝配置无法供其他主机使用的问题。3、修复 内存泄露问题。4、优化 支持自动更新。5、新增 支持windows操作系统的监控代理 |      |