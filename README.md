MakeGTNHEasierMake
GTNHEasier是一款根据GregTechNewHorizons(GTNH)整合包开发的简易辅助Mod。本项目旨在简化部分操作，提升玩家的开荒效率。
🛠️核心功能详解
1.智能自动化：工具自动切换(AutoSwitchTools)
模式1:持续检测(Continuous)
长按即可自动切换工具，遍历快捷栏，计算对目标方块挖掘速度最快的工具，选出最优解
模式2点击触发(Click)
仅在按下左键时切换一次工具
支持绑定快捷键
草丛保护：针对匠魂(Tinkers'Construct)斧头砍草不加经验却掉耐久的特性，防止在割草时误换斧头。
战斗逃逸机制:检测到攻击实体的时候，自动关闭功能并发出提示音，防止在战斗中因工具乱跳导致意外死亡。
2.预测脚本
矿脉预言：根据格雷矿脉生成规律，直接在内存中模拟矿脉分布，定位特定矿脉，但是只能模拟首次生成的矿脉，因此不是100%正确，只能在主世界和下界使用，如果是在找不到某种矿脉，可以使用这个功能。
神秘预言：预测使用知识笔记可以得到神秘锭研究的特定时间点，用于神秘开局的玩家。
星系/匠魂搜索：对Galacticraft地牢和TConstruct史莱姆岛实现远程定位，Galacticraft地牢只测试过月球和火星。
3.扫描功能
采用异步架构，用于在世界中为目标方块绘制高亮边框，确实是支持格雷科技的矿物，但是对于格雷的矿物支持有点bug
目标方块是那些，内置白名单，玩家无法修改
支持绑定快捷键,开启和关闭内置1s冷却
4.LootGamesHelpers
扫雷：自动解算逻辑矩阵，标记安全区与雷区。
点灯：自动捕获并记录序列闪烁状态，通过渲染引导玩家完成记忆挑战。
5.自由视觉(Freecam)
支持在不移动玩家本体的情况下进行基地规划与远距离侦察。
鼠标滚轮可实时控制飞行速度（0.1x-10.0x）。
支持绑定快捷键
⌨️服务器管理员可用指令(权限等级2)
/makegtnheasier list：查看所有功能的授权与运行状态。
/makegtnheasier unlock <feature>：解锁敏感功能（只支持freecam,target_scanner）。
makegtnheasier lock <feature>：重新锁定功能。
单人游戏所有功能均不受限制，
服务器会限制freecam和扫描功能，如果需要在服务器使用这两个功能，需要服务端也下载此MOD，然后管理员使用命令开启权限。
如果在服务器无使用限制功能的需求，客户端装即可

主配置界面(GUI)默认按V打开
此mod没有任何修改游戏原有逻辑或者添加新东西的存在，因此，如果引发了bug，删除此MOD即可

⚠️ 免责声明
本项目仅供整合包辅助体验使用。作者不承担因在服务器中使用本Mod而导致的任何封号或处罚责任，使用前请先咨询服主。
⚠️ 本MOD可自由传播，传播时无需标注作者信息；但是严禁以任何形式售卖本MOD
⚠️本项目为非开源项目，其核心目的是为了确保多人游戏环境的公平性与安全性，如因特殊原因需要源代码，在诉求合理的前提下，我会提供代码
---

更详细的解说请移步至Bilibili：
https://www.bilibili.com/video/BV1NKA1zoEFh/?vd_source=bf82ce50160fa1ff31de0cb03da3e4e5#reply116140193879761

💖致谢
中文：衷心感谢GTNH团队对这款整合包付出。更重要的是，感谢你们在维护1.7.10MOD开发环境上所做的巨大努力，让这个经典的Minecraft版本在今天依然充满活力和生命力。
English: Thanks to GTNH team for all your hard work on this modpack, And more importantly, thanks for your efforts you've put into maintaining the mod development environment for Minecraft 1.7.10, keeping this classic version alive and thriving to this day.