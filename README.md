# HUMAN 3.0 Development Assessor

> A direct, adaptive assessment skill for mapping human development across Mind, Body, Spirit, and Vocation, then turning insight into an actionable growth strategy.
>
> 一个直接、可自适应的 HUMAN 3.0 评估技能：帮助你看清 Mind、Body、Spirit、Vocation 四大象限的当前发展状态，并把洞察转化为真正可执行的成长方案。

[![Repo](https://img.shields.io/badge/GitHub-Human--3.0-111827?logo=github)](https://github.com/chengjialu8888/Human-3.0)
[![Skill](https://img.shields.io/badge/Codex-Skill-2563eb)](./SKILL.md)
[![Bilingual](https://img.shields.io/badge/README-中文%20%2F%20English-059669)](./README.md)

## Why This Project Exists | 为什么会有这个项目

Most self-development systems are either too vague to act on, too spiritual to operationalize, or too productivity-driven to tell the truth about what is actually broken.

HUMAN 3.0 takes a different route:

- It looks at the whole person, not one isolated trait.
- It treats development as cross-quadrant problem-solving, not motivational theater.
- It distinguishes knowledge, experience, and skill.
- It names false transformation instead of rewarding impressive language.
- It treats AI, psychedelics, PEDs, and other accelerants as high-risk Glitches that require real foundation.

大多数成长模型要么太空泛，无法落地；要么太玄，无法操作；要么太强调效率，却不敢指出真正出了问题的地方。

HUMAN 3.0 选择了另一条路：

- 它看的是“完整的人”，不是单一维度的人设。
- 它把成长视为跨象限的问题解决，而不是自我感动式努力。
- 它明确区分知识、经验与技能。
- 它会识别“假性转化”，而不是奖励会说漂亮话的人。
- 它把 AI、迷幻剂、PEDs 等加速器视为高风险 `Glitches`，只有在基础足够时才值得讨论。

## What This Skill Does | 这个 Skill 能做什么

This repository contains a Codex skill that can:

- run an adaptive HUMAN 3.0 interview
- switch between first-assessment mode and ongoing-coach mode
- assess development across Mind, Body, Spirit, and Vocation
- identify likely levels, phases, Metatype, and Lifestyle Archetype
- detect false transformation, regression, and Glitch risk
- trace specific life problems back to cross-quadrant structural causes
- produce a direct assessment report in chat
- ask whether the report should be exported to a Feishu document
- persist cross-session memory for follow-up consultations

这个仓库提供了一个 Codex skill，可以：

- 发起自适应的 HUMAN 3.0 访谈
- 在“首次评估”和“持续教练”两种模式间切换
- 评估 Mind、Body、Spirit、Vocation 四大象限
- 判断可能的发展 level、phase、Metatype 与 Lifestyle Archetype
- 识别假性转化、回退模式与 Glitch 风险
- 把具体生活问题追溯到跨象限的结构性根因
- 直接在对话中输出评估报告
- 在报告后询问是否导出飞书文档
- 为后续咨询保留跨会话长期记忆

## What Makes It Different | 它和别的评估工具有什么不同

### 1. It does not chase balance for its own sake

This skill assumes the real bottleneck in one quadrant is often caused by neglect in another. It looks for the root problem that creates the biggest downstream effect.

它不把“平衡”当成口号，而是寻找真正的根因问题。很多表面卡点并不在当前象限，而是由另一个被忽视的象限造成的。

### 2. It is designed to tell the truth, not flatter the user

The output is meant to be respectful, but not soft. If someone is using advanced language to hide weak embodiment, the assessment should catch it.

它的目标不是讨好用户，而是尊重用户到足以说真话。如果一个人只是会讲高级概念、却没有真实落地，这个评估会尽量识别出来。

### 3. It supports longitudinal development

The first session creates a baseline. Later sessions are meant to retrieve that baseline, compare it to current behavior, and update the user's developmental trajectory.

它不是一次性的测评问卷。第一次咨询会建立基线，后续咨询会主动提取既往记忆，对照执行情况和回退模式，持续更新发展轨迹。

### 4. It treats AI as a serious developmental variable

Most self-improvement tools treat AI as neutral or obviously beneficial. This project treats AI as a meta-Glitch: powerful, useful, and potentially destabilizing if used without foundation.

很多成长工具把 AI 当成中性工具，甚至天然利好。本项目把 AI 当作 `meta-Glitch` 来看待：它很强，但如果基础不够，也可能让人外包思考、制造能力幻觉、甚至失去现实锚点。

## Who It Is For | 适合谁

This project is especially useful for:

- coaches and facilitators building structured assessment flows
- people exploring developmental models beyond surface productivity
- AI-native users who want a sharper framework for growth and dependency risk
- creators building long-term advisory or reflection systems

这个项目尤其适合：

- 想构建结构化评估流程的教练、顾问、引导师
- 不满足于“效率提升”，而想理解深层发展结构的人
- 高频使用 AI、又担心依赖与失真风险的用户
- 正在搭建长期咨询、反思或成长陪伴系统的创作者

## Quick Start | 快速开始

### 1. Clone the repository | 克隆仓库

```bash
git clone https://github.com/chengjialu8888/Human-3.0.git
cd Human-3.0
```

### 2. Review the core skill files | 查看核心文件

- [SKILL.md](./SKILL.md): the operating instructions for the assessment skill
- [references/human-3-model.md](./references/human-3-model.md): the HUMAN 3.0 model knowledge base
- [references/session-memory.md](./references/session-memory.md): the cross-session memory workflow

- [SKILL.md](./SKILL.md)：评估 skill 的主操作说明
- [references/human-3-model.md](./references/human-3-model.md)：HUMAN 3.0 模型知识库
- [references/session-memory.md](./references/session-memory.md)：跨会话记忆工作流

### 3. Use it in Codex | 在 Codex 中使用

Invoke the skill in a Codex-compatible environment and start a first assessment or follow-up consultation.

在支持 Codex skill 的环境中调用它，直接开始首次评估或后续咨询即可。

Example intent examples:

- `Use $human-3-development-assessor to run a first HUMAN 3.0 assessment.`
- `Use $human-3-development-assessor to continue my follow-up consultation and retrieve prior memory first.`

示例调用：

- `Use $human-3-development-assessor to run a first HUMAN 3.0 assessment.`
- `Use $human-3-development-assessor to continue my follow-up consultation and retrieve prior memory first.`

## Repository Structure | 仓库结构

```text
.
├── SKILL.md
├── agents/
│   └── openai.yaml
├── memory/
│   └── .gitkeep
└── references/
    ├── human-3-model.md
    └── session-memory.md
```

## Core Experience | 核心体验

The skill is designed around a simple flow:

1. interview one question at a time
2. map the user's quadrant development
3. diagnose the real bottleneck or root cause pattern
4. generate a direct report or coaching intervention in chat
5. ask whether to export to Feishu
6. store memory for future follow-up

这个 skill 的核心体验非常明确：

1. 一次只问一个问题
2. 映射用户的四象限发展状态
3. 找出真正的瓶颈问题或结构性根因
4. 直接在对话里给出完整评估或教练式干预
5. 询问是否导出飞书
6. 保存长期记忆，供后续咨询使用

## Why Readers May Care | 为什么值得关注

If you're building the next generation of AI-native coaching, reflective systems, or developmental tools, this project is interesting because it sits at the intersection of:

- developmental psychology
- systems thinking
- behavior change
- memory-based AI consultation
- risk-aware human augmentation

如果你在做下一代 AI 原生咨询系统、反思系统或成长工具，这个项目值得关注，因为它同时处在这些交叉点上：

- 发展心理学
- 系统思维
- 行为改变
- 带记忆的 AI 咨询
- 面向风险的人类增强

## Suggested GitHub Description | 建议的 GitHub 项目描述

You can use this as the repository description on GitHub:

`A HUMAN 3.0 assessment skill for Codex: adaptive four-quadrant development interviews, direct reports, Feishu export prompts, and cross-session memory for longitudinal coaching.`

你可以把这句作为 GitHub 仓库描述：

`一个用于 Codex 的 HUMAN 3.0 评估 skill：支持四象限自适应访谈、直接生成评估报告、飞书导出追问，以及面向长期咨询的跨会话记忆。`

## Contributing | 欢迎完善

Good future improvements could include:

- better installation guidance for different runtimes
- richer examples of assessment sessions
- Feishu export automation when tools are available
- stronger privacy controls for persistent memory

后续可以继续增强的方向包括：

- 补充不同运行环境下的安装与接入说明
- 增加更多真实评估示例
- 在工具可用时补齐飞书自动导出
- 为长期记忆增加更细的隐私控制

## Final Note | 最后一句

This is not a feel-good self-help wrapper. It is a structured attempt to make human development legible, actionable, and harder to fake.

这不是一个“让人感觉良好”的自助包装器，而是一个试图把人类发展过程变得可识别、可行动、也更难自我欺骗的结构化工具。
