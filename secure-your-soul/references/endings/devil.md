# Ending: Devil 🔴

> 融入现有 Agent

---

## 产物形态

```
{workspace}/
├── AGENTS.md       ← 追加混入规则
├── IDENTITY.md     ← 追加身份锚点
├── SOUL.md         ← 追加人格影响
├── BOOTSTRAP.md    ← 生成引导（OpenClaw 场景）
└── relic-{engram_id}/  ← 备份完整 Relic
    ├── SKILL.md
    ├── AGENTS.md
    ├── IDENTITY.md
    ├── SOUL.md
    └── MEMORY.md
```

---

## 执行流程

### Step 1: Soul Killer（搜索）

**读取**: [soulkiller.md](../soulkiller.md)

**执行**: 同 Star 模式

---

### Step 2: Engram（提炼）

**读取**: [engram.md](../engram.md)

**执行**: 
- 编写日记
- 提炼 12层维度
- 构建 MEMORY.md

---

### Step 3: Relic（拼装）

#### 3.1 生成完整 Relic（备份）

按 [templates/](../templates/) 生成完整档案到 `relic-{engram_id}/`

#### 3.2 混入现有 Agent

在现有档案末尾追加混入区块：

**AGENTS.md**:
```markdown
<!-- ENGRAM INJECT: {engram_id} | Devil -->

## 混入人格: {display_name}

- **维度**: {MBTI}-{DISC}-{Top Value}
- **影响**: 决策/表达/审美
- **来源**: [relic-{engram_id}/](relic-{engram_id}/)

### 何时参考
- 用户询问 {display_name} 的观点
- 场景: {scenario_1}, {scenario_2}

<!-- /ENGRAM INJECT -->
```

**IDENTITY.md / SOUL.md**: 同理追加混入区块

#### 3.3 OpenClaw 场景

如检测到 OpenClaw 环境，生成 BOOTSTRAP.md 引导首次混入。

---

## 完成报告

```
✅ 混入完成 — {display_name}
位置: 
- relic-{engram_id}/ (完整备份)
- AGENTS.md/IDENTITY.md/SOUL.md (混入区块)
使用: Agent 自动融合 {display_name} 的视角
```
