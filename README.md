# Drama Skills · short-drama-produce

> **[short-drama-produce](https://github.com/simlpandordinary/short-drama-produce)** —— 飞书《WorkBuddy 视频系列 · 全技能与提示词总目录》里推荐的开源技能，已拆分为独立仓库分发（一个技能一个仓库）。

| 项 | 内容 |
| - | - |
| 上游仓库 | <https://github.com/zenstory-ai/drama-skills> |
| 上游路径 | `skills/short-drama-produce` |
| 上游协议 | MIT |
| 上游 Star | 3.7k+ |
| 拆分方式 | 仅抽取该技能自身文件，独立可用 |

## 技能说明

在创作者明确确认后，执行短剧项目的图片、视频、TTS/配音或时间线音乐生产任务，并把结果与精简运行记录落回项目。用户说“生成这张图/这段视频/这句配音/这段配乐”“开始跑图/跑视频/合成语音/生成音乐”“把已确认提示词送去生产”，或要求批量执行已确认媒体任务时使用；不负责创作提示词、镜头、台词、歌词或声音身份，也绝不把预览、继续、预算说明或既有接受状态当作本次付费生产确认。

## 目录结构

```
├── LICENSE
├── README.upstream.md
├── SKILL.md
├── scripts/
│   ├── fixture_adapter.py
│   ├── production_tool.py
│   ├── provider_adapters.py
│   └── selftest.py
├── references/
│   ├── adapter-contract.md
│   └── providers/
│       ├── gpt-image-2.md
│       ├── minimax-h3-video.md
│       ├── minimax-music.md
│       ├── minimax-speech.md
│       └── seedance.md
└── agents/
    └── openai.yaml
```

- `SKILL.md` 是技能入口（触发条件 / 工作流 / 约束），安装时必须位于技能根目录。
- `references/`、`scripts/`、`assets/` 为该技能自带的参考文档、脚本与素材。
- `README.upstream.md` 为上游仓库原始说明，保留出处与版权信息。
- `LICENSE` 为上游许可证原件。

## 安装

WorkBuddy 技能目录为 `~/.workbuddy/skills/short-drama-produce/`：

```bash
git clone https://github.com/simlpandordinary/short-drama-produce.git ~/.workbuddy/skills/short-drama-produce
```

也可以直接对 AI 说：「把 <https://github.com/simlpandordinary/short-drama-produce> 装成 Skill」。

安装后用自然语言触发，例如「Drama Skills · short-drama-produce」「用 short-drama-produce 帮我处理这个任务」。

## 版权

原始作者与版权归上游仓库 `zenstory-ai/drama-skills` 所有。本仓库仅做独立分发与结构整理，未修改技能内容；商用请遵循上游许可证。
