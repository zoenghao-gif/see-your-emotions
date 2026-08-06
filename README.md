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

### 最简单的方式：复制 GitHub 地址

仓库地址：

```text
https://github.com/zoenghao-gif/see-your-emotions
```

如果你的 Agent 有“从 GitHub 导入”“从 URL 安装 Skill”或类似功能，直接粘贴上面的地址即可。

如果它要求你填写具体的 Skill 目录，则使用这个地址：

```text
https://github.com/zoenghao-gif/see-your-emotions/tree/main/skills/see-your-emotions
```

### 使用统一安装器

支持 `npx skills` 的 Agent，可以直接复制下面这一行：

```bash
npx skills add https://github.com/zoenghao-gif/see-your-emotions --skill see-your-emotions -g
```

这个安装器支持 Codex、Claude Code、Kimi、Hermes、CodeBuddy 等多个 Agent。安装完成后，直接对 Agent 说“使用看见情绪”即可。

### 如果 Agent 不支持 URL 导入

将仓库中的 `skills/see-your-emotions/` 文件夹复制到该 Agent 的 Skills 目录即可。不同 Agent 的目录可能不同，因此建议优先使用前面的 GitHub / URL 导入方式。

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
