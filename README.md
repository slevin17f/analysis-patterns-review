# Analysis Patterns Review

用于 Codex 的中文领域建模与评审 Skill。输入一段业务需求或已有模型，得到候选结构、适用条件、失败反例和可复演的验收样例。依据 Martin Fowler 的《Analysis Patterns: Reusable Object Models》整理，内含 12 张能力卡。运行时只需要 Codex 和包内 Markdown 文件。

## 安装

下载仓库并解压，或克隆后进入仓库根目录。把 `skills/analysis-patterns-review` 整个文件夹复制到个人的 `~/.agents/skills/`。团队可将同一文件夹提交至项目的 `.agents/skills/`。

安装后检查 `~/.agents/skills/analysis-patterns-review/SKILL.md` 与同级 `references/` 是否存在。如果 Codex 尚未发现新技能，重启 Codex。

## 使用

> 用 $analysis-patterns-review 评审设备调拨模型。只有 current_owner，调拨单可能晚到。如何分别回答“当时实际归谁”和“当时系统认为归谁”？请给一个现有模型会答错的例子及验收数据。

[能力索引](skills/analysis-patterns-review/references/capability-index.md) · [Codex 技能文档](https://learn.chatgpt.com/docs/build-skills)
