# Khazix Skills（日本語ローカライズ版）

> **このリポジトリについて**
> これは [KKKKhazix/khazix-skills](https://github.com/KKKKhazix/khazix-skills)（MIT License）の fork です。
> `hv-analysis/` 配下（SKILL.md / scripts / references）を自然な日本語に全訳した **日本語ローカライズ版** を収録しています。
> `khazix-writer/` と `prompts/` は原文（中国語）のままです。

---

数字生命卡兹克的 AI 工具箱。

这里是我自己在用的、经过长期打磨的 Prompts 和 Skills，现在决定把它们完整地、一字不改地开源出来。

两种东西，一个目的：把我积累的方法论变成可复用的工具。

- **Prompts** — 轻量级，复制粘贴到任何 AI 对话或 Deep Research 里就能用
- **Skills** — 重量级，遵循 [Agent Skills](https://agentskills.io) 开放标准的结构化指令集，安装后 Agent 会自动加载

## Prompts

| Prompt | 说明 | 用法 | 讲解 |
|--------|------|------|------|
| [**横纵分析法**](./prompts/横纵分析法.md) | 通用深度研究框架，融合历时-共时分析与竞争战略视角，半小时出一份万字级研究报告 | 复制 Prompt，修改「研究对象」，丢进任何支持 Deep Research 的模型 | [公众号文章](https://mp.weixin.qq.com/s/Y_uRMYBmdLWUPnz_ac7jWA) |

## Skills

| Skill | 说明 | 讲解 |
|-------|------|------|
| [**hv-analysis**](./hv-analysis/) | 縦横分析法の深度研究 Skill（**日本語版**）。ネット経由で自動的に情報を収集し、縦軸で時間の深さ、横軸で競争の広がりを追い、最終的に装丁済みの PDF 研究レポートを出力する | [原著解説（中文）](https://mp.weixin.qq.com/s/Y_uRMYBmdLWUPnz_ac7jWA) |
| [**khazix-writer**](./khazix-writer/) | 卡兹克公众号长文写作 Skill，包含完整的写作风格规则、四层自检体系、内容方法论和风格示例库 | [公众号文章](https://mp.weixin.qq.com/s/AtxGrii_K-nzkwUM9SNhEg) |

### Skill 安装方式

**通过 Agent 安装**

在 Claude Code、Codex、OpenClaw 等支持 Skill 的 Agent 中，直接对话：

```
安装这个 skill：https://github.com/KKKKhazix/khazix-skills
```

**手动安装**

1. 点仓库右上角 **Code → Download ZIP**，或者 `git clone https://github.com/KKKKhazix/khazix-skills.git`
2. 把你想装的 Skill 文件夹（比如 `hv-analysis/`）整个复制到对应工具的 Skills 目录下

各工具的 Skills 安装路径：

| 工具 | 路径 |
|------|------|
| Claude Code | `~/.claude/skills/` |
| OpenClaw | `~/.openclaw/skills/` |
| Codex | `~/.agents/skills/` |

例如装 hv-analysis 到 Claude Code：

```bash
git clone https://github.com/KKKKhazix/khazix-skills.git
cp -r khazix-skills/hv-analysis ~/.claude/skills/
```

## License

[MIT](./LICENSE)
