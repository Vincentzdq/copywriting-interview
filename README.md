# copywriting-interview

**让 AI 先采访你，再替你写。** 一个文案访谈工作流 skill：接到任何内容创作需求（文案、口播稿、视频脚本、选题）时，AI 不直接动笔，而是先按四场景协议访谈你，把真实需求和真实素材挖出来，再产出内容框架。

> An interview-first copywriting workflow skill for AI agents: before writing anything, the AI interviews you — one question at a time — to surface your real intent and real material. Works with Claude Code, Codex, and any agent that reads markdown instructions.

## 为什么需要它

- 你说"帮我写篇文案"，AI 直接开写 → 得到一篇谁都能发、你不想发的通用稿
- 你说"随便写点什么"，AI 真的随便写 → 选题的负担还是在你身上
- 本 skill 的原则：**理解错误在访谈阶段纠正花 10 秒，在成稿阶段纠正花一晚上**

## 四场景协议

| 你的状态 | 打法 | AI 会做什么 |
|---|---|---|
| 有想法但模糊 | **问他** | 一次一问挖真实目的，选择题代替开放题，产出需求确认书 |
| 完全没想法 | **翻他** | 素材打捞四问 + 刺激物——让你"反应"而不是"生成" |
| AI 对你一无所知 | **钓他** | 冷启动四问，每问既挖素材又画像，答完立刻给半成品点火 |
| AI 只知道你的领域 | **定他** | 定位四问（时间分配/上下游/资历/近况）+ 感受换壳句式 |

核心纪律：一次只问一个问题；开口前先做本地情报预读（白名单：项目文档、AI 记忆、git 历史——不碰浏览器历史/聊天记录/邮件）；所有事实必须可溯源，不能编。

## 安装

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

## 使用

装好后无需任何配置。对 AI 说"我想发条视频""帮我写篇文案""这周要更新但没想法"——它会开始采访你，而不是开始写。

## 效果

4 场景自动化对照测试：带 skill 通过率 **12/12**，不带 skill **7/12**。对照组的典型失分：一次抛 4-5 个问卷式问题、把选题负担推回给零想法的用户、以及在成稿中虚构事实。

## License

MIT
