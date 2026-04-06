# Engram — 灵魂印迹

将日记片段提炼为维度+记忆。

---

## 输出结构

```
memory/daily/YYYY-MM-DD*.md     ← 日记文件
MEMORY.md                       ← 双层记忆索引
engram_data:                    ← 12层维度数据
  mbti: {...}
  disc: {...}
  ...
```

---

## 任务 1: 编写日记

按 [DIARY.md](../templates/DIARY.md) 格式：

```markdown
# YYYY-MM-DD — {title}

**类型**: turning_point
**置信度**: H

## 今天发生了什么
...

## 当时的想法
...

## 复盘
...
```

---

## 任务 2: 提炼 12层维度

按需读取 [dimensions/](../dimensions/)：

| 层 | 维度 | 文件 |
|---|------|------|
| 1 | 核心性格 (MBTI) | [core-personality.md](../dimensions/core-personality.md) |
| 2 | 行为风格 (DISC) | [behavioral-style.md](../dimensions/behavioral-style.md) |
| 3 | 认知特质 (Big Five) | [cognitive-traits.md](../dimensions/cognitive-traits.md) |
| 4 | 价值取向 | [value-orientation.md](../dimensions/value-orientation.md) |
| 5 | 决策模式 | [decision-mode.md](../dimensions/decision-mode.md) |
| 6 | 动机驱动 | [motivation-drive.md](../dimensions/motivation-drive.md) |
| 7 | 认知处理 | [cognition-processing.md](../dimensions/cognition-processing.md) |
| 8 | 情绪模式 | [emotion-patterns.md](../dimensions/emotion-patterns.md) |
| 9 | 社会关系 | [social-relationship.md](../dimensions/social-relationship.md) |
| 10 | 创造力 | [creativity-problem.md](../dimensions/creativity-problem.md) |
| 11 | 存在意义 | [existential-meaning.md](../dimensions/existential-meaning.md) |
| 12 | 防御机制 | [defense-coping.md](../dimensions/defense-coping.md) |

**方法**: 通读日记 → 标记行为模式 → 匹配维度 → 记录证据

---

## 任务 3: 构建 MEMORY.md

按 [MEMORY.md](../templates/MEMORY.md) 格式：
- 表层记忆（日记索引表）
- 深度记忆（关键事件分类）

---

## 下一步

完成后 → 返回结局文件（star/devil/temperance.md）进入拼装阶段
