# 邵艾伦（Alan）风格短帖 · Codex Skill

把一个观点写得短、直、有画面。从邵艾伦（Alan，@AlanShao111）的样本分析中提炼短句、反差、自嘲和行动落点，用来写用户自己的原创中文社交内容。

![邵艾伦 AlanShao111 写作风格介绍](assets/style-overview.png)

> 上图由用户提供，展示报告样本中的历史数据与原帖。它是风格说明，不代表本项目获得原作者授权、合作或背书。

## 可以做什么

- 围绕自律、创作、注意力、积累和个人影响力写短帖。
- 把冗长草稿改成一句一行、观点鲜明的社交文案。
- 批量生成不同角度的版本，避免只换词的重复内容。

默认每条约 20–60 字，数量未指定时给 3 个版本。用户自己的长度、数量和语气要求优先。

## 使用示例

```text
使用 $alanshao111-style，围绕“停止空想，先交出第一个作品”写 5 条原创短帖。
```

```text
使用 $alanshao111-style，把下面的草稿改成 3 个版本，每条不超过 60 字，不加 emoji：
[粘贴草稿]
```

原创演示：

> 教程又存了十篇。
>
> 草稿还是零篇。
>
> 今天先把一句话写完，再打开收藏夹。

示例由本项目编写，不是 Alan 的原话。

## 安装到 Windows 的 F 盘

在 PowerShell 中执行：

```powershell
git clone https://github.com/badboywzw/alanshao111-style.git F:\codex\skills\alanshao111-style
powershell -NoProfile -ExecutionPolicy Bypass -File F:\codex\skills\alanshao111-style\install.ps1
```

实际文件默认保存在 `F:\codex\skills\alanshao111-style`，脚本在用户 Skill 发现目录创建目录联接：有 `CODEX_HOME` 时使用其 `skills` 子目录，否则使用 `~\.codex\skills`。脚本不会覆盖已有的不同目录。同一安装可重复执行。

其他位置可通过 `-SkillRoot` 和 `-DiscoveryRoot` 指定。其他系统可把整个仓库复制到自己的 Skill 发现目录，无需运行 Windows 脚本。在新会话中选择该 Skill，或使用上面的 `$alanshao111-style` 提示。

## 文件与来源

| 文件 | 用途 |
|---|---|
| [SKILL.md](SKILL.md) | 触发说明、写作流程、事实边界 |
| [agents/openai.yaml](agents/openai.yaml) | 名称、简介与默认提示 |
| [写作手册](references/writing-playbook.md) | 体裁、改写路径与原创示例 |
| [原始蒸馏报告](references/source-report.md) | 用户提供的研究资料及原帖出处 |
| [install.ps1](install.ps1) | F 盘安装与目录联接 |

报告记录 194 条样本（2026-10-07 至 2026-10-23），带有事件期偏差；本项目没有重新抓取或独立核验报告中的数据。原始报告内的“人格提示词”作为文献保留，不直接执行。

本项目提炼表达方法，不代用作者履历、资产、粉丝数或商业身份，不把生成文本冒充为原帖，也不自动发布内容。原帖、图片和作者标识的权利归各自权利人。
