# XivInTheShellMarkerGen

根据FFlogs战斗日志生成[XIV in the Shell](https://xivintheshell.com/)的时间轴

FFLogs API Key获取方式：[FFLogs设置](https://cn.fflogs.com/profile)

以下是一些参数的用法

* 请求时自动翻译：固定将所有技能名翻译成英文
* 最小间隔：marker之间的最小时间间隔。小于最小间隔的marker会被分到不同的轨道

由于部分FFLogs日志可能存在缺失，Untargetable（不可选中）段生成可能存在异常，如有问题请手动调整

部分战斗开怪后会存在不可选中时间（如O6S），战斗起始时间为实际可选中时间，需要在XIV in the Shell导入时额外配置**载入文件时间偏移**
