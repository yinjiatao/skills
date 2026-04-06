---
name: secure-your-soul
description: >
  提取人格印迹（Engram），封装为数字人格（Relic）。
  触发词：secure your soul, engram, relic, 提取人格, 学习某人风格,
  封存某人, 人格融合, 数字分身, soulkiller
---

# Secure Your Soul

> Soul Killer → Engram → Relic

将一个人的公开信息提炼为数字人格（Relic）。

---

## 触发后流程

```
-> 向用户询问以下内容：

1. 提供目标人物
2. 选择结局模式

-> 读取流程指引: references/endings/[结局模式].md
-> 按照流程指引执行
```

---

## 结局模式

| 模式 | 说明 | 文件 |
|------|------|------|
| 🌟 Star | 独立 Relic，随时召唤 | [endings/star.md](references/endings/star.md) |
| 🔴 Devil | 融入现有 Agent | [endings/devil.md](references/endings/devil.md) |
| ⚪ Temperance | 完全人格置换 | [endings/temperance.md](references/endings/temperance.md) |

**选择结局后** → 读取对应文件，按指引执行

---

## 参考索引

| 类型 | 路径 | 用途 |
|------|------|------|
| **结局** | [references/endings/](references/endings/) | 核心流程指引 |
| **维度** | [references/dimensions/](references/dimensions/) | 多层级维度画像 |
| **模板** | [references/templates/](references/templates/) | 档案模板 |
| **规则** | [references/rules/](references/rules/) | 置信度、搜索策略等规则 |
| **搜索** | [soulkiller.md](references/soulkiller.md) | 搜索策略 |
| **提炼** | [engram.md](references/engram.md) | 提炼策略 |

---

## 产物结构

所有模式最终输出 Relic：

```
relic-{engram_id}/
├── SKILL.md        ← 技能壳，引导读取 AGENTS.md
├── AGENTS.md       ← 规则入口，引导读取 SOUL/IDENTITY/MEMORY
├── BOOTSTRAP.md    ← OpenClaw 首次引导（如适用）
├── IDENTITY.md     ← 基础信息、氛围、Emoji
├── SOUL.md         ← 人格核心、维度标签
└── MEMORY.md       ← 双层记忆索引
```
