# copywriting-interview

**Make the AI interview you before it writes for you.**

English | [中文](#中文说明)

---

## English

An interview-first copywriting workflow skill for AI agents. When you ask for any content — copy, talking-head scripts, video scripts, topic ideas — the AI doesn't start writing. It first interviews you under a four-scenario protocol to surface your real intent and real material, then delivers a content framework. Works with Claude Code, Codex CLI, and any agent that reads markdown instructions.

### Why

- You say "write me some copy" and the AI just writes → you get a generic draft anyone could post and you never will
- You say "I have no ideas, write whatever" and the AI really writes whatever → the burden of choosing a topic is still on you
- The principle behind this skill: **a misunderstanding costs 10 seconds to fix during the interview, and a whole evening to fix after the draft is written**

### The four-scenario protocol

| Your state | Play | What the AI does |
|---|---|---|
| Have an idea, but vague | **Ask** | One question at a time to dig out the real goal; multiple-choice with trade-offs instead of open questions; ends with a requirement brief you sign off |
| No ideas at all | **Draw cards** | Four material-dredging questions plus provocations — makes you *react* instead of *generate* |
| The AI knows nothing about you | **Fish** | Four cold-start questions, each mining material and profiling you at once; your first answer gets turned into a half-draft immediately to ignite momentum |
| The AI only knows your field | **Locate** | Four positioning questions (time allocation / upstream-downstream / tenure / recent focus) plus reframed feeling-questions that get stories instead of official answers |

Core discipline: one question at a time; a local intelligence pre-read before asking anything (whitelist only: project docs, AI memory, git history — never browser history, chat logs, or email); every fact must be traceable to a source — no fabrication.

### Install

**Claude Code** (one line):

```bash
git clone https://github.com/Vincentzdq/copywriting-interview ~/.claude/skills/copywriting-interview
```

**Codex CLI**:

```bash
git clone https://github.com/Vincentzdq/copywriting-interview ~/.codex/skills/copywriting-interview
```

**claude.ai (web)**: download `copywriting-interview.skill` from this repo and upload it under Settings → Capabilities/Skills.

**Any other agent**: paste the body of `SKILL.md` into your agent's system instructions or persona file (e.g. Hermes' SOUL.md). It's plain markdown.

### Usage

No configuration needed. Tell your AI "I want to post a video", "write me some copy", or "I need to publish this week but have no ideas" — it will start interviewing you instead of start writing.

### Results

Four-scenario automated A/B test: **12/12** assertions passed with the skill vs **7/12** without. Typical baseline failures: dumping 4–5 survey-style questions at once, pushing topic selection back onto a user who has no ideas, and fabricating facts in the draft.

---

## 中文说明

**让 AI 先采访你，再替你写。** 一个文案访谈工作流 skill：接到任何内容创作需求（文案、口播稿、视频脚本、选题）时，AI 不直接动笔，而是先按四场景协议访谈你，把真实需求和真实素材挖出来，再产出内容框架。适用于 Claude Code、Codex CLI，以及任何能读 markdown 说明的 agent。

### 为什么需要它

- 你说"帮我写篇文案"，AI 直接开写 → 得到一篇谁都能发、你不想发的通用稿
- 你说"随便写点什么"，AI 真的随便写 → 选题的负担还是在你身上
- 本 skill 的原则：**理解错误在访谈阶段纠正花 10 秒，在成稿阶段纠正花一晚上**

### 四场景协议

| 你的状态 | 打法 | AI 会做什么 |
|---|---|---|
| 有想法但模糊 | **问他** | 一次一问挖真实目的，选择题代替开放题，产出需求确认书 |
| 完全没想法 | **翻他** | 素材打捞四问 + 刺激物——让你"反应"而不是"生成" |
| AI 对你一无所知 | **钓他** | 冷启动四问，每问既挖素材又画像，答完立刻给半成品点火 |
| AI 只知道你的领域 | **定他** | 定位四问（时间分配/上下游/资历/近况）+ 感受换壳句式 |

核心纪律：一次只问一个问题；开口前先做本地情报预读（白名单：项目文档、AI 记忆、git 历史——不碰浏览器历史/聊天记录/邮件）；所有事实必须可溯源，不能编。

### 安装

**Claude Code**（一行命令）：

```bash
git clone https://github.com/Vincentzdq/copywriting-interview ~/.claude/skills/copywriting-interview
```

**Codex CLI**：

```bash
git clone https://github.com/Vincentzdq/copywriting-interview ~/.codex/skills/copywriting-interview
```

**claude.ai 网页版**：下载本仓库的 `copywriting-interview.skill` 文件，在 设置 → 能力/Skills 里上传。

**其他 agent**：把 `SKILL.md` 的正文贴进你的 agent 的系统指令或人设文件（如 Hermes 的 SOUL.md）即可，内容就是纯 markdown 说明书。

### 使用

装好后无需任何配置。对 AI 说"我想发条视频""帮我写篇文案""这周要更新但没想法"——它会开始采访你，而不是开始写。

### 效果

4 场景自动化对照测试：带 skill 通过率 **12/12**，不带 skill **7/12**。对照组的典型失分：一次抛 4-5 个问卷式问题、把选题负担推回给零想法的用户、以及在成稿中虚构事实。

## License

MIT
