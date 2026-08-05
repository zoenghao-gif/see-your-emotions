# 看见情绪

一个一次只问一个短问题的情绪觉察 Skill。

它帮助用户梳理一件具体事情中的：

- 情绪和情绪名称；
- 身体反应；
- 当时闪过的念头；
- 担心或想避免的结果；
- 实际采取的行为；
- 行为暂时保护了什么；
- 可能重复出现的反应模式；
- 用户自己愿意尝试的下一步。

## 它不是什么

「看见情绪」是自我观察和情绪觉察工具，不是：

- 心理诊断工具；
- 心理治疗或医疗服务；
- 危机干预服务；
- 替用户做重大决定的顾问。

它默认只通过问题帮助用户观察，不主动分析、诊断、说服或给建议。

如果出现自伤、伤人、无法保证自身或他人安全，或现实中的紧急危险，应停止普通觉察流程，优先联系当地急救、危机热线、可信任的人或专业机构。

## 快速安装

### 使用统一安装器

需要 Node.js 的环境可以运行：

```bash
npx skills add zoenghao-gif/see-your-emotions --skill see-your-emotions -g
```

也可以指定 Agent：

```bash
npx skills add zoenghao-gif/see-your-emotions \
  --skill see-your-emotions \
  --agent claude-code \
  --agent codex \
  -g
```

### Codex

将 `skills/see-your-emotions/` 放入以下任一位置：

```text
项目级：.agents/skills/see-your-emotions/
用户级：~/.agents/skills/see-your-emotions/
```

也可以使用：

```bash
gh skill install zoenghao-gif/see-your-emotions see-your-emotions \
  --agent codex --scope user
```

### Claude Code

```bash
mkdir -p ~/.claude/skills
cp -R skills/see-your-emotions ~/.claude/skills/
```

安装后可以直接输入：

```text
/see-your-emotions
```

### Kimi Code CLI

优先安装到通用目录：

```text
~/.agents/skills/see-your-emotions/
```

也可以使用 Kimi 支持的用户级目录：

```text
~/.kimi/skills/see-your-emotions/
```

然后输入 `/skill:see-your-emotions`，或者直接描述需要梳理的事情。

### Hermes Agent

可以从 GitHub 直接安装：

```bash
hermes skills install zoenghao-gif/see-your-emotions/skills/see-your-emotions
```

也可以把 `skills/see-your-emotions/` 放入 `~/.hermes/skills/`。

### WorkBuddy / CodeBuddy

优先使用客户端的“技能 / Skills / 导入 Skill”功能，选择本仓库中的：

```text
skills/see-your-emotions/
```

CodeBuddy 项目级目录为：

```text
.codebuddy/skills/see-your-emotions/
```

不同版本的 WorkBuddy 可能使用不同的全局目录，因此建议优先使用界面导入。

## 怎么使用

安装后，可以直接说：

```text
我想做一次情绪觉察。最近让我烦躁的是：临近下班时突然来了一个需要处理的问题。
```

或者明确调用：

```text
使用看见情绪，帮我一次只问一个问题，梳理这件事。
```

对话过程中可以随时说：

- “不知道”；
- “换个问题”；
- “整理一下”；
- “停”；
- “我不想继续了”。

Skill 应尊重这些信号，不为了完成流程而强行追问。

## 版本和许可

当前版本：`v0.1.0`。

本项目以 MIT License 发布，详见 [LICENSE](LICENSE)。

第一版为中文 Skill。它可以被不同 Agent 安装，但实际对话体验主要面向中文用户。

## 相关标准和文档

- [Agent Skills specification](https://agentskills.io/specification)
- [Codex Skills](https://developers.openai.com/codex/skills/)
- [Claude Code Skills](https://code.claude.com/docs/en/skills)
- [Kimi Code CLI Agent Skills](https://moonshotai.github.io/kimi-cli/en/customization/skills.html)
- [Hermes Agent Skills](https://github.com/NousResearch/hermes-agent/blob/main/website/docs/user-guide/features/skills.md)
- [GitHub CLI Skill Install](https://cli.github.com/manual/gh_skill_install)
