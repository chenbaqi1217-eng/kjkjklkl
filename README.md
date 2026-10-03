# 🖼️ 数字藏品 · 抽卡游戏

一个功能丰富的纯前端数字藏品抽卡养成游戏，包含藏品收集、养成系统、战斗挑战、休闲小游戏等 30+ 独立玩法模块。

> **纯静态网页**：所有逻辑运行在浏览器端，无需后端服务器，可直接部署到 GitHub Pages / Vercel / Netlify 等任意静态托管平台。

## ✨ 特性

- 🎴 **藏品收集**：抽卡获取稀有藏品，支持背包/仓库管理、高级搜索排序
- ⚔️ **多维养成**：命魂、内功、幻兽、辟邪玉、潜能、怪怪卡、圣遗物、符文、八卦等 20+ 养成系统
- 🏰 **战斗挑战**：无限闯塔、攻城略地、副本挑战、马战竞猜、世界BOSS、竞技场
- 🎮 **休闲游戏**：猜猜乐、五子棋、飞行棋、后宫系统
- 📅 **日常系统**：签到、任务、图鉴、称号、排行榜
- 🗑️ **快捷分解**：命魂/内功/幻兽支持按品质、类型、等级筛选批量分解
- 💾 **本地存档**：所有数据存储在浏览器 localStorage，刷新不丢失，支持导入/导出 JSON 备份

## 📂 功能模块

### 藏品养成（21个）
| 页面 | 功能 | 页面 | 功能 |
|------|------|------|------|
| `soul.html` | 👻 命魂系统 | `neigong.html` | ☯️ 内功心法 |
| `pet.html` | 🐉 幻兽殿堂 | `evil-jade.html` | 💠 辟邪玉 |
| `potential.html` | ✨ 潜能系统 | `monster-card.html` | 🃏 怪怪卡 |
| `treasure.html` | 🏺 天宝系统 | `godly.html` | ⚡ 天神恩赐 |
| `calendar.html` | 📅 天道历法 | `decompose.html` | ♻️ 分解熔炼 |
| `reroll.html` | 🔄 洗练重铸 | `mount.html` | 🐎 坐骑系统 |
| `awaken.html` | ⭐ 觉醒转生 | `relic.html` | 🏛️ 圣遗物 |
| `rune.html` | 🔮 符文之语 | `bagua.html` | ☯️ 八卦牌 |
| `wucai.html` | 💎 五彩石 | `spark.html` | ✨ 火花 |
| `prefix.html` | 🏷️ 藏品赋名 | `yihuo.html` | 🔥 异火 |

### 战斗挑战（6个）
`tower.html` 🏰 无限闯塔 · `siege.html` ⚔️ 攻城略地 · `dungeon.html` 🗡️ 副本挑战 · `horse.html` 🏇 马战竞猜 · `world-boss.html` 👹 世界BOSS · `arena.html` ⚔️ 竞技场

### 休闲游戏（4个）
`guess.html` 🎰 猜猜乐 · `gomoku.html` ⚫ 五子棋 · `flight.html` ✈️ 飞行棋 · `harem.html` 🏯 后宫系统

### 日常系统（5个）
`signin.html` 📅 每日签到 · `quest.html` ✅ 每日任务 · `codex.html` 📖 藏品图鉴 · `title.html` 🏅 称号系统 · `rank.html` 🏆 排行榜

### 其他功能（3个）
`market.html` 📈 商城行情 · `shop.html` 🏪 神秘商城 · `story.html` 📚 故事收集

## 🚀 快速开始

### 本地运行
直接用浏览器打开 `index.html` 即可，无需任何构建工具或服务器。

### 部署到 GitHub Pages

1. **创建仓库**：在 GitHub 新建一个仓库（如 `collectible-game`）
2. **上传文件**：将本项目所有文件推送到仓库 main 分支
3. **开启 Pages**：进入仓库 `Settings` → `Pages`
   - Source 选择 `Deploy from a branch`
   - Branch 选择 `main`，目录选择 `/ (root)`
   - 点击 `Save`
4. **访问游戏**：等待约 1 分钟后，访问 `https://<你的用户名>.github.io/<仓库名>/`

> 也可以部署到 Vercel / Netlify / Cloudflare Pages 等平台，直接导入仓库即可，无需额外配置。

## 💾 数据存储说明

- 所有游戏进度（藏品、命魂、内功、幻兽、钻石等）**仅存储在你当前浏览器的 localStorage 中**
- 清除浏览器数据 / 换浏览器 / 换设备会导致存档丢失
- 建议定期使用游戏内「📤 导出」功能备份 JSON 文件，换设备时用「📥 导入」恢复
- GitHub 仓库**不存储任何用户数据**，仅托管静态网页代码

## 📁 项目结构

```
.
├── index.html          # 主入口（藏品总览 + 功能导航）
├── soul.html           # 命魂系统
├── neigong.html        # 内功心法
├── pet.html            # 幻兽殿堂
├── ...                 # 其他 35 个功能页面
├── 404.html            # GitHub Pages 自定义 404 页
├── .gitignore
└── README.md
```

每个功能页面独立加载，打开后自动弹出对应功能面板，顶部「← 返回主页」可回到主入口。所有页面共享同一套 localStorage 存档。

## ⚠️ 注意事项

- 本游戏为纯前端单机游戏，所有随机数在本地生成
- 部分功能（如支付、充值）为模拟演示，不会产生真实交易
- 建议使用 Chrome / Edge / Firefox 等现代浏览器获得最佳体验
- 手机端可正常游玩，部分页面支持自适应布局

## 📄 License

MIT License — 可自由使用、修改、分发。
