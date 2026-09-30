# short-video-script-generator

短视频爆款文案与标题生成技能（Hermes Agent Skill）。

针对给定的短视频，深度解析内容卖点，为抖音、快手、小红书、B站等平台定制差异化的高吸引力文案与标题。

- 技能名（SKILL.md 中的 `name`）：`short-video-script-generator`，与本仓库名一致
- 每个目录 = 一个技能：本仓库根目录只有一个 `SKILL.md`，即一个技能

## 技能包含什么

| 文件 | 说明 |
|---|---|
| `SKILL.md` | 技能主体：卖点提炼 → 多平台文案 → 爆款标题 的三步生成流程，含平台风格规范与避坑指南 |

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
用 short-video-script-generator 技能，为这个视频生成抖音/小红书/B站三套文案和标题
```

## 更新 / 卸载

```bash
hermes skills update short-video-script-generator   # 拉取本仓库更新
hermes skills uninstall short-video-script-generator
```

## License

MIT
