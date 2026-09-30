# short-video-script-generator

短视频多平台爆款脚本与标题生成技能（Hermes Agent Skill）v2.0 增强版。

针对给定的短视频，深度解析核心卖点与反差冲突，为抖音、快手、小红书、B站等平台定制高完播率、高点击率、高互动率的完整策划案。

- 技能名（SKILL.md 中的 `name`）：`short-video-script-generator`，与本仓库名一致
- 每个目录 = 一个技能：本仓库根目录只有一个 `SKILL.md`，即一个技能

## v2.0 增强版特性

| 能力 | 说明 |
|---|---|
| 卖点与反差冲突提炼 | 解析视觉高光、冲突反差、情绪落差，输出 1-2 句直击痛点的摘要 |
| 多平台脚本与文案 | 默认 3 平台定制，每套含目标受众画像、平台风格定位、正文文案（≤300 字，无 AI 腔） |
| 黄金 3 秒分镜脚本 | `0-3s Hook` / `3-12s 推进` / `12-15s 爆点` 三段式分镜，保障完播率 |
| BGM / 音效建议 | 音画一体，推荐配乐与反差音效（卡点笑声、急停音效等） |
| 三元冲突标题算法 | `【荒诞/认知冲突】+【具象画面要素】+【口语化报喜/发问】`，杜绝同质化套路 |
| 评论区造梗与控评 | 每平台预设 1-2 条置顶评论/热评梗，提升互动权重 |
| 少样本范例 | Good Case vs Bad Case 对照（产检检出啤酒示例） |
| 质量自查协议 | 输出前强制检查标题套路、前 3 秒 Hook、字数与格式 |

## 安装

### 方式 1：Hermes 命令行（推荐）

```bash
hermes skills install yingmingyapei/short-video-script-generator
```

安装后技能位于 `~/.hermes/skills/short-video-script-generator/`。

### 方式 2：手动 clone

```bash
git clone https://github.com/yingmingyapei/short-video-script-generator.git ~/.hermes/skills/short-video-script-generator
```

### 生效方式

- 新会话自动加载；
- 当前会话内可运行 `/skills install yingmingyapei/short-video-script-generator --now` 立即生效（不带 `--now` 则下次会话生效，这是为了不打断 prompt 缓存）。

## 使用方法

安装后，在 Hermes 中直接把短视频内容（链接、描述或素材）交给 agent，并说「为这个视频写多平台爆款文案」即可触发。也可以显式指定：

```
用 short-video-script-generator 技能，为这个视频生成抖音/小红书/B站三套脚本、黄金3秒分镜、三元冲突标题和评论区造梗
```

## 更新 / 卸载

```bash
hermes skills update short-video-script-generator   # 拉取本仓库更新
hermes skills uninstall short-video-script-generator
```

## License

MIT
