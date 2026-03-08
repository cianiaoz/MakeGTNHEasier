Make GTNH Easier

Make GTNH Easier 是一款专为 GregTech New Horizons (GTNH) 整合包开发的轻量化辅助 Mod。本项目旨在通过技术手段简化部分繁琐操作，在不破坏核心生存挑战的前提下，显著提升玩家的开荒与探索效率。

🛠️ 核心功能详解
1. 智能自动化：工具自动切换

双模式切换：

持续检测 (Continuous)：准星指向方块时自动遍历快捷栏，实时计算并切换至挖掘速度最快的工具。

点击触发 (Click)：仅在按下左键挖掘时执行一次切换逻辑。

草丛保护逻辑：针对匠魂 (Tinkers' Construct) 斧头砍草损耗耐久且不加经验的特性，内置黑名单防止误换斧头。

战斗逃逸机制：检测到攻击实体行为时，自动关闭切换功能并发出提示音，防止因工具乱跳导致战斗意外。

2. 预测脚本
实现结构定位：

GT 矿脉预言：模拟矿脉分布（只支持主世界与下界）。注：仅能模拟首次生成结果，非 100% 准确，适用于极度缺乏特定矿产时的应急搜寻。

神秘预言：精准预测使用知识笔记获取“神秘锭”研究的最佳时间点,适用于神秘开局的玩家

星系/匠魂搜索：远程定位月球/火星地牢（Galacticraft）(只测试过月球和火星而已，其他星球没有试过)及史莱姆岛（TConstruct）。

3. 核心扫描系统
异步渲染架构：采用独立线程扫描，在世界中为目标方块绘制3D高亮边框

格雷矿物适配：初步支持 GT 矿物检测（目前仍有小部分兼容性 Bug 待修复）。

白名单管理：内置扫描目标白名单，玩家无法修改

4. 智力游戏辅助
扫雷 (Minesweeper)：自动解算矩阵，清晰标记安全区（Safe）与雷区（Mines）。

点灯 (Game of Light)：自动捕获并记录序列闪烁状态，通过渲染引导玩家完成记忆挑战。

5. 自由视觉
脱体侦察：支持视角脱离角色本体，用于基地布局规划与远距离观察。

动态速控：鼠标滚轮可实时调节飞行速度（0.1x - 10.0x）。

⌨️ 指令与服务器规则

为了兼顾多人游戏环境的公平性

单人模式：所有功能默认全开，不受任何限制。

多人模式：Freecam 与 Target Scanner 默认锁定。若需开启，服务端亦需安装此 Mod，并由管理员(权限2)执行以下指令：

/makegtnheasier list：查看所有功能的授权状态。

/makegtnheasier unlock <feature>：解锁敏感功能（支持 freecam, target_scanner）。

/makegtnheasier lock <feature>：重新锁定功能。

提示：若仅需使用非敏感功能（如自动工具切换、小游戏辅助），仅客户端安装即可。
GUI 操作：默认按 V 键打开主配置界面。

⚠️ 重要说明
稳定性保证：本 Mod 不修改游戏原始逻辑，不添加新物品/方块。如遇任何 Bug，直接移除 Mod 即可恢复，不会损坏存档。

版权与传播：

自由传播：可自由分享，无需标注作者信息。

禁止售卖：严禁以任何形式商业化售卖本 Mod。

关于开源：本项目暂不开源，旨在确保安全逻辑不被轻易篡改。如确有合理需求，作者可提供源码。

免责声明：本项目仅供学习与体验。作者不承担因在服务器中使用本 Mod 而导致的任何封号或处罚责任，请务必在遵守服规的前提下使用。

📺 视频演示
更详细的功能解说与演示，请移步 Bilibili：

👉 点击观看项目演示视频 https://www.bilibili.com/video/BV1NKA1zoEFh/?vd_source=bf82ce50160fa1ff31de0cb03da3e4e5#reply116140193879761

💖 致谢 / Acknowledgements
中文：衷心感谢 GTNH 团队 对这款整合包的付出。更重要的是，感谢你们在维护 1.7.10 MOD 开发环境上所做的巨大努力，让这个经典的 Minecraft 版本在今天依然充满活力。

English: Special thanks to the GTNH team for their incredible dedication. More importantly, we appreciate the immense effort put into maintaining the 1.7.10 development environment, keeping this classic version of Minecraft alive and thriving.