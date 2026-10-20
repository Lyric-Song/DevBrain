# DevBrain

开发者的「外挂脑子」——把不常做但步骤繁琐、容易忘的操作收成随手可查的工具箱；后期对接 Agent，能够储存Agent或者您创建的自动化脚本快速完成开发任务，Agent将会学习您的自动化脚本并且会持续对脚本的优化分析，提示你可能缺什么、下一步该干什么。

### 要解决什么问题

平时开发或运维时，常会遇到步骤繁琐、频率不高但容易忘的操作，例如：
- 某套复杂的 Docker 部署命令
- 特定框架的初始化配置流程
- 数据库迁移脚本
- 打包部署的固定步骤

DevBrain 目标是：您只需要点一次即可帮助您完成繁琐的任务，快速调出、查看即用。

### 两种执行方式

用户教一次或配一次，之后点一下就能跑：

#### 1. Agent 全自动
- 教一次：Agent 在宿主机上学习用户习惯（例如 Docker 打包怎么做）
- 下次在技能列表点一下：Agent 按该习惯全自动完成操作
- 适合步骤偏界面、环境略有变化、不好写成死脚本的流程

#### 2. 自定义脚本
- 用户自己写好脚本/命令，放到 DevBrain 里
- 点一下直接执行
- 适合已固定的 Docker、迁移、打包等命令流；更快、更可控、更省成本

同一条技能可标记来源（已学习 / 手写脚本）；执行前可预览步骤；危险操作需确认。

### 远期能力（规划）
- 对接 Agent，实时检测用户当前项目情况
- 推断用户可能需要什么，或漏掉了什么
- 在适当时机给出可执行的步骤 / 命令 / checklist
- 技能双模式：Agent 全自动 与 自定义脚本并存，按场景选用

### 现状
仓库刚由 Grok Bot + Cua Driver 在本机演示创建。内容建设中。

### License
TBD

---

**DevBrain** — a developer's "external brain": a handy toolbox for rare but fiddly workflows you keep forgetting. Later it plugs into an Agent that can sense your project state and suggest what you might be missing, and what to do next.

### The problem

In day-to-day development or ops you often hit flows that are tedious, infrequent, and easy to forget, for example:
- Complex Docker deploy command sequences
- Framework init / config rituals
- Database migration scripts
- Fixed build & release steps

Searching or digging through notes every time wastes energy. DevBrain aims to: recall fast, use immediately.

### Two ways to run

Teach or configure once, then one click:

#### 1. Agent fully automatic
- Teach once: the agent learns the user's habit on the host (e.g. how they Docker-package)
- Next time: one click in the skill list → the agent completes it automatically
- Best for UI-heavy or slightly variable flows that are hard to freeze as scripts

#### 2. Custom scripts
- User puts their own scripts/commands into DevBrain
- One click runs them
- Best for fixed Docker / migrate / pack pipelines — faster, more controllable, cheaper

The same skill can be tagged as learned vs handwritten; preview steps before run; confirm dangerous operations.

### Roadmap
- Connect an Agent that watches the current project in real time
- Infer what you might need — or what you skipped
- Surface runnable steps / commands / checklists at the right moment
- Dual-mode skills: Agent auto and custom scripts side by side

### Status
Repo was just created via a Grok Bot + Cua Driver on-machine demo. Content is being built.

### License
TBD
