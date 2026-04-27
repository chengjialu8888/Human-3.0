# HUMAN 3.0 Development Assessor

[English README](./README.md)

## 一句话说明

HUMAN 3.0 是一个给“不满足于安慰、效率技巧、人格标签”的人准备的评估与教练框架。它试图给出的是结构性地图，告诉你真正驱动成长、停滞和自我欺骗的到底是什么。

## 来源

这个项目的灵感来源于 Dan Koe 提出的 HUMAN 3.0 prompt 与框架：

- 原始来源：[Prompt: HUMAN 3.0 Self-Discovery & Metatype Test](https://letters.thedankoe.com/p/prompt-human-30-self-discovery-and)

## 为什么值得用

HUMAN 3.0 最打动人的地方，在于它承诺的是大多数自助工具给不了的东西：

- 它不会把你塞进一个人格标签盒子里，而是尝试映射你在 Mind、Body、Spirit、Vocation 四个维度上的真实发展状态。
- 它会揭穿“假性成长”。你可能在一个领域看起来很高级，另一个领域却正在悄悄塌陷。
- 它寻找的是那个制造连锁问题的隐藏瓶颈，而不是让你把精力耗在解决表层症状上。
- 它给的是具体转化路径，不是空泛反思：接下来 30、90、180 天到底做什么。
- 它把 AI 纳入诊断本身，不只把 AI 当效率工具，而是把它看作一种可能加速成长、也可能削弱思维能力的力量。
- 它追求的是“立刻有用”，而不是让你做几个月抽象自我观察之后还不知道下一步怎么走。

## 这个项目能做什么

这个仓库提供了一个 HUMAN 3.0 skill / framework，可以：

- 发起自适应的 HUMAN 3.0 访谈
- 在“首次评估”和“持续教练”两种模式间切换
- 评估 Mind、Body、Spirit、Vocation 四大象限
- 判断可能的发展 level、phase、Metatype 与 Lifestyle Archetype
- 识别假性转化、回退模式与 Glitch 风险
- 把具体生活问题追溯到跨象限的结构性根因
- 直接在对话中输出评估报告
- 在报告后询问是否导出飞书文档
- 为后续咨询保留跨会话长期记忆
- 根据运行环境适配到 Codex、Claude Code 或其他个人 agent

## 兼容性

这个项目不是“只能跑在 Codex 上”，而是“可被多种 agent 使用”。

它最适合具备这些能力的 agent：

- 能遵循较长的 system prompt / skill prompt
- 能一次只问一个问题
- 能维持会话上下文
- 最好支持跨会话记忆
- 最好支持保存或导出报告

所以它天然适配：

- Codex skills
- Claude Code 工作流
- 自定义 personal agent
- 带记忆的聊天 agent
- 本地或托管式咨询助手

## 典型使用场景

用户通常会带着这些状态来到这里：

- `我想做一个真正的发展评估，不想再做人格测试。`
- `我总是在不同人生问题里重复同一个模式。`
- `我高频使用 AI，想知道它是在帮助我成长，还是让我变弱。`
- `我想要一个记得我上次说过什么的教练系统。`

## 它和别的评估工具有什么不同

### 1. 它不把“平衡”当口号

很多表面卡点并不在当前象限，而是由另一个被忽视的象限造成的。它会寻找真正的根因问题。

### 2. 它的目标不是讨好用户

如果一个人只是会讲高级概念、却没有真实落地，这个评估会尽量识别出来。

### 3. 它支持长期追踪

第一次咨询建立基线，后续咨询会主动提取既往记忆，对照执行情况和回退模式，持续更新发展轨迹。

### 4. 它把 AI 当成发展变量

AI 既可能帮助成长，也可能让人外包思考、制造能力幻觉、失去现实锚点。

### 5. 它帮你找“下一个核心问题”

它不只是描述你是什么样的人，而是帮助你找出：哪个问题一旦被解决，会带来最大的连锁式改善。

## 最终你会得到什么

- 一份四象限诊断
- 一个可能的 Metatype 与 Lifestyle Archetype
- 一个被点名的核心问题
- 一个具体到 30/90/180 天的行动方案
- 一组关于回退与自我破坏的预警
- 一套可持续跟进的记忆层

## 适合谁

- 想构建结构化评估流程的教练、顾问、引导师
- 不满足于“效率提升”，而想理解深层发展结构的人
- 高频使用 AI、又担心依赖与失真风险的用户
- 正在搭建长期咨询、反思或成长陪伴系统的创作者

## 快速开始

### 1. 克隆仓库

```bash
git clone https://github.com/chengjialu8888/Human-3.0.git
cd Human-3.0
```

### 2. 查看核心文件

- [SKILL.md](./SKILL.md)：评估 skill 的主操作说明
- [references/human-3-model.md](./references/human-3-model.md)：HUMAN 3.0 模型知识库
- [references/assessment-template.md](./references/assessment-template.md)：输出格式约束
- [references/session-memory.md](./references/session-memory.md)：跨会话记忆工作流
- [references/coaching-patterns.md](./references/coaching-patterns.md)：持续教练与问题诊断层

### 3. 在 Codex 中使用

示例调用：

- `Use $human-3-development-assessor to run a first HUMAN 3.0 assessment.`
- `Use $human-3-development-assessor to continue my follow-up consultation and retrieve prior memory first.`

### 4. 在 Claude Code 中使用

推荐映射方式：

- `SKILL.md` 负责主行为
- `references/human-3-model.md` 负责理论层
- `references/assessment-template.md` 负责输出格式
- `references/session-memory.md` 负责持续记忆
- `references/coaching-patterns.md` 负责问题教练

### 5. 在其他 personal agent 中使用

最简单的接入方式是：

1. 把 [SKILL.md](./SKILL.md) 当作主编排 prompt
2. 把 `references/` 当作按需加载的知识层
3. 把长期记忆流程映射到你自己的存储层
4. 如果没有飞书，就把导出动作替换成你自己的文档系统或笔记系统

框架本身是可迁移的，工具层是可替换的。

## 使用体验示例

这个项目真正拉开差距的，不只是框架本身，而是它的交互方式：

1. 一次只问一个问题
2. 会抓住前后矛盾
3. 会把表层痛点追到结构性根因
4. 直接在对话里给出完整报告
5. 下次继续时还能记得你

示例转化：

- 表层问题：`我总是坚持不了习惯。`
- 结构判断：`你的身体执行失败，背后其实是精神耗竭和心智层面的知行断裂。`
- 下一步动作：`先重建一个在情绪混乱里也能活下来的微型身体实践，再谈更大的优化目标。`

## 仓库结构

```text
.
├── SKILL.md
├── README.md
├── README.zh-CN.md
├── agents/
│   └── openai.yaml
├── assets/
│   └── github-header.svg
├── memory/
│   └── .gitkeep
└── references/
    ├── assessment-template.md
    ├── coaching-patterns.md
    ├── human-3-model.md
    └── session-memory.md
```

## 建议的 GitHub 项目描述

`一个适用于 Codex、Claude Code 与个人 AI Agent 的 HUMAN 3.0 评估与教练框架：支持四象限自适应访谈、根因分析，以及面向长期成长的跨会话记忆。`

## 最后一句

这不是一个“让人感觉良好”的自助包装器，而是一个试图把人类发展过程变得可识别、可行动、也更难自我欺骗的结构化工具。
