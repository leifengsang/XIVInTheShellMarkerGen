# XivInTheShellMarkerGen

根据FFlogs战斗日志生成[XIV in the Shell](https://xivintheshell.com/)的时间轴

需要在main.py（或markerGen.exe）同目录下创建config.txt配置文件

~~~
{
  "CAST_NAME_LIST": ["超增压急行", "超增压抽雾", "无控急行", "脱轨", "雷转质射线", "无尽狂奔", "雷光一闪", "雷鸣吐息", "前照光", "掉落", "重爆雷", "爆雷"],
  "DAMAGE_NAME_LIST": ["以太炮", "以太冲击波", "冲击波", "重雷", "雷电爆发", "脱轨捶打"],
  "CONVERT_DIC": {"爆雷": "分散", "重爆雷": "分摊", "以太炮": "分散", "以太冲击波": "分摊"},
  "LOGS_ID": "TXN9QjtzBLcFrVKg",
  "FIGHT_ID": 51,
  "FILE_NAME": "极火车marker.txt",
  "API_KEY": ""
}
~~~

* CAST_NAME_LIST：对应敌对**施法**列表
* DAMAGE_NAME_LIST：对应我方**受到伤害**列表
* CONVERT_DIC：将上述名称在导出时替换为指定的名称
* LOGS_ID：logs id，对应下面logs链接中的reports/到?的部分
* FIGHT_ID：战斗id对应下面logs链接中的fight=后的部分
* FILE_NAME：导出的时间轴名称
* API_KEY：V1客户端密钥，在[设置](https://cn.fflogs.com/profile)中获取

示例链接：https://cn.fflogs.com/reports/TXN9QjtzBLcFrVKg?fight=51



部分marker可能需要手动调整

由于副本情况可能比较复杂，Untargetable部分用了Info实现，可以在生成后手动调整为Untargetable段
