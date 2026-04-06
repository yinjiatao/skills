# Ending: Star 🌟

> 独立 Relic，随时召唤

---

## 产物形态

```
skills/relic-{engram_id}/
├── SKILL.md
├── AGENTS.md
├── BOOTSTRAP.md
├── IDENTITY.md
├── SOUL.md
└── MEMORY.md
```

---

## 执行流程

### Step 1: Soul Killer（搜索）

**读取**: [soulkiller.md](../soulkiller.md)

**执行**:
1. 建立时间线
2. 搜索日记片段
3. 识别关键节点

**输出**: 日记候选列表

---

### Step 2: Engram（提炼）

**读取**: [engram.md](../engram.md)

**执行**:
1. 编写日记 → 按 engram.md 记忆格式
2. 提炼维度 → 按 dimensions/ 12层体系
3. 构建 MEMORY.md 索引

**输出**: 
- memory/daily/*.md
- MEMORY.md 索引
- 12层维度数据

---

### Step 3: Relic（拼装）

**读取模板**:
- [templates/IDENTITY.md](../templates/IDENTITY.md)
- [templates/SOUL.md](../templates/SOUL.md)
- [templates/AGENTS.md](../templates/AGENTS.md)
- [templates/BOOTSTRAP.md](../templates/BOOTSTRAP.md)
- [templates/SKILL.md](../templates/SKILL.md)

**执行**:
1. 填充 IDENTITY.md — 基础信息、氛围、Emoji
2. 填充 SOUL.md — 人格核心、12层维度标签
3. 填充 AGENTS.md — 规则入口、读取顺序
4. 填充 BOOTSTRAP.md — OpenClaw 首次引导
5. 填充 SKILL.md — 技能壳、触发词

---

## 完成报告

```
✅ Relic 已生成 — {display_name}
位置: skills/relic-{engram_id}/
使用: 「召唤 {display_name}」或「加载 relic-{engram_id}」
```
