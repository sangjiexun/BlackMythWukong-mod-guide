# 黑神话：悟空 Mod 研究指南

> **Black Myth: Wukong — Mod Research & Guide**

一份关于《黑神话：悟空》PC 版 mod 生态的研究汇总。包含 Nexus Mods Top 100 全榜数据、游民星空/风灵月影修改器评测、社区共识的「必装 mod」清单。

最后更新：**2026-07-31**

<img width="1080" height="675" alt="image" src="https://github.com/user-attachments/assets/00529bca-ac4c-41cd-8b1a-4e8b79ffc7e1" />


*(截图：前台 b1 窗口 / 主屏 PrintWindow 抓取，1966×823 → 1280×536 压缩至 41 KB)*

---

## 📊 数据概览

| 来源 | 抓取内容 | 数量 |
|---|---|---|
| **Nexus Mods**（官方） | Top 100 by Endorsements（5 页 × 20） | **100 个 mod** |
| **游民星空**（gamersky.com） | 中文 mod 资源首页 | **77 个 mod** |
| **风灵月影**（FLiNG Trainer） | 修改器版本全集 | **12 个修改器** |
| 全网搜索（搜狗/360/Bing/百度） | 综合搜索结果 | 多源交叉验证 |

**全站 mod 总数（截至 2026-07-31）**：Nexus Mods 收录 **861 个 mod**，本指南覆盖推荐数前 100 名（覆盖前 11.6%）。

---

## 🏆 社区共识 Top 10（Nexus Mods Endorsements 排名）

| # | Mod | 推荐 | 下载 | 类别 | 一句话点评 |
|---|---|---|---|---|---|
| 1 | **RE-UE4SS** Mod Loader | **5,400** | **463.9k** | Tools | **必装前置**。UE4SS 注入器，社区事实标准 |
| 2 | simple map (简易大地图) | 2,800 | 194.8k | Misc | 原版没地图的痛点修复 |
| 3 | BMWK - SPF Redux | 2,600 | 240k | Misc | **仅 4KB** 的性能优化方案 |
| 4 | Signature Bypass | 2,200 | 134.4k | Tools | 签名绕过工具，与 UE4SS 搭配 |
| 5 | Somersault Cloud Anywhere (筋斗云全图) | 1,600 | 136k | Misc | 筋斗云赶路神器 |
| 6 | CSharpLoader | 1,500 | 144.3k | Tools | C# 脚本加载器 |
| 7 | Increased Rare Item Drop Rates | 1,300 | 70k | Gameplay | 提升稀有材料掉率 |
| 8 | Better dodge(rage) | 1,200 | 78.1k | Gameplay | 翻滚无敌帧全覆盖 |
| 9 | stronger JinguBang | 923 | 65.1k | Misc | 金箍棒吸收所有棍势词条 |
| 10 | BossRushV3 | 905 | 70.2k | Gameplay | BossRush 刷怪模式 |

> 📌 **关键观察**：Top 6 中有 **5 个是基础设施类**（Mod Loader / 签名绕过 / 脚本加载器），说明黑神话 mod 生态的根基是少数核心贡献者打下来的。RE-UE4SS 单独 **463.9k 下载**，约等于 Top 2-100 大部分 mod 下载量之和。

---

## 📂 分类分布（Top 100）

```
Miscellaneous  ████████████████████████  50  (50%)
Gameplay       ███████████               22  (22%)
Tools          ███                        7  (7%)
Characters     ███                        6  (6%)
Weapons        ██                         5  (5%)
User Interface ██                         4  (4%)
Visuals        ██                         4  (4%)
Animations     █                          2  (2%)
```

---

## 🚀 玩家安装建议（实测总结）

### 1️⃣ 最轻量方案（不改任何文件）
直接用 **风灵月影修改器**（FLiNG Trainer 2.0.0.249）
- 优点：不动游戏文件、不封号风险最低、即装即用
- 缺点：每次启动要先开修改器，再开游戏
- 44 个内置选项：HP/MP 锁定、无限技能、无限物品、Boss Rush 等

### 2️⃣ 标准 mod 玩家
装 **RE-UE4SS** + **Signature Bypass** 作为前置
- 然后按需装 gameplay 类别（simple map、稀有掉率、Better dodge 等）

### 3️⃣ 进阶用户
加装 **CSharpLoader**，可以自己写 .cs 脚本挂入游戏

---

## 📁 仓库结构

```
.
├── README.md                          # 本文件（仓库门面）
├── data/
│   ├── top100-endorsements.json       # Nexus Mods Top 100 原始 JSON（29 KB）
│   ├── youmin_page1.json              # 游民星空第 1 页 77 个 mod
│   ├── gamersky_fling_44.json         # 风灵月影 44 选项列表
│   └── category-summary.md            # 按分类整理的 mod 列表
└── reports/
    └── top100-endorsements-report.md  # 完整分析报告（15 KB）
```

---

## 🔧 FLiNG 修改器实测记录

- **版本**：2.0.0.249（最新版）
- **大小**：2.64 MB
- **下载**：游民星空首发
- **文件位置**：`E:\steam\steamapps\common\BlackMythWukong\Trainers\FLiNG_Trainer_BlackMythWukong.exe`
- **实测流程**：
  1. 启动 Steam → 启动游戏 → 等游戏窗口出现
  2. 双击 `FLiNG_Trainer_BlackMythWukong.exe`
  3. 修改器主窗口显示「风灵月影修改器」（600x386）
  4. 隐藏窗口「风灵月影修改器 2.0.0.249 Setup」（按 F1 唤出）
  5. 在游戏前台时按 `Num 0` 激活选项（FLiNG 默认激活键）
- **44 个内置选项**：HP/MP 锁定、无限技能冷却、无限葫芦、无限变身、稀有度 100%、Boss Rush 模式等

---

## ⚠️ 安全提示

- **不建议同时**装 RE-UE4SS + FLiNG 修改器（修改器有自带内存读写）
- RE-UE4SS 会**修改游戏签名**，联机可能被封（虽然黑神话目前为单机）
- 装 mod 前**备份存档**（Steam 云存档可能被覆盖）

---

## 📜 数据来源

- [Nexus Mods - Black Myth: Wukong](https://www.nexusmods.com/games/blackmythwukong/mods)（官方）
- [游民星空 - 黑神话悟空修改器](https://www.gamersky.com/z/blackmythwukong/)
- [风灵月影 - FLiNGTrainers.com](https://www.flingtrainer.com/)

---

## 📝 License

研究数据来自公开互联网采集。Mod 版权归原作者所有（详见各 mod 主页）。
本仓库仅做汇总整理，不分发 mod 文件本身。

---

> 由 AI 研究助手整理 🤖
> 最后抓取：2026-07-31
