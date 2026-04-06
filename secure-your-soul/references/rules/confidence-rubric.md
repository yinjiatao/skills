# Confidence Rating Rubric

> 置信度评级标准：H (High) / M (Medium) / L (Low) / F (Fact)

---

## Rating Levels

### 🔴 F — Fact (事实)

**Definition**: 无可争议的客观事实，有多个可靠来源交叉验证

**Criteria**:
- 来源可核实（官方记录、公开档案）
- 多独立来源一致
- 无争议或矛盾信息

**Examples**:
- 公开的出生日期
- 公司成立时间
- 公开发表的职位/职称
- 教育背景（学位、学校）
- 直接引用的原话（有出处）

**Usage**:
```yaml
confidence: F
# 用于构建基础身份档案
# 可作为推理的可靠前提
```

---

### 🟢 H — High (高置信度)

**Definition**: 有充分证据支持的推断，逻辑链条清晰，可合理解释

**Criteria**:
- 多个间接证据指向同一结论
- 与已知事实无冲突
- 有直接的日记/访谈证据支持

**Examples**:
- 从多篇博客推断的MBTI类型
- 从行为模式推断的核心价值观
- 从决策历史推断的风险偏好
- 从反复出现的主题推断的深层恐惧

**Evidence Required**:
- 至少3个独立观察点
- 或2个高相关性观察 + 逻辑一致性

**Usage**:
```yaml
confidence: H
# 可用于维度标记
# 可用于生成关键洞察
# 可作为后续分析的基础
```

---

### 🟡 M — Medium (中等置信度)

**Definition**: 有一定证据支持，但存在其他解释可能，需要更多验证

**Criteria**:
- 有支持证据，但不充分
- 存在合理的替代解释
- 证据来源单一或间接

**Examples**:
- 从一篇博客推断的观点（无其他佐证）
- 从第三方描述推断的性格特质
- 从单一事件推断的行为模式
- 基于有限样本的统计推断

**Evidence Required**:
- 1-2个相关观察点
- 或单一强相关证据

**Usage**:
```yaml
confidence: M
# 标记为待验证
# 需要寻找更多证据支持或反驳
# 可作为假设进一步探索
```

---

### 🔵 L — Low (低置信度)

**Definition**: 证据薄弱或矛盾，仅为推测，可能有严重偏差

**Criteria**:
- 单一且弱的证据
- 证据间存在矛盾
- 高度依赖假设和解读

**Examples**:
- 从社交媒体语气推断的情绪状态
- 从照片推断的性格（无其他信息）
- 过度解读的隐喻分析
- 缺乏上下文的孤立言论

**Evidence Required**:
- 间接推测
- 或弱相关观察

**Usage**:
```yaml
confidence: L
# 明确标记为推测
# 不应作为关键决策依据
# 优先寻找更多证据升级
```

---

## Confidence Elevation Rules

### Upgrading (升级)

| From | To | Condition |
|------|----|-----------|
| L | M | 找到第二个独立证据 |
| M | H | 找到第三个独立证据 + 逻辑一致性验证 |
| H | F | 获得直接可核实来源 |

### Downgrading (降级)

| From | To | Condition |
|------|----|-----------|
| F | H | 发现来源有误或存在争议 |
| H | M | 发现矛盾证据或替代解释 |
| M | L | 主要证据被质疑或推翻 |

---

## Evidence Quality Hierarchy

### Tier 1: Direct Evidence (直接证据)
- 本人撰写的日记/博客
- 本人接受的深度访谈
- 本人发布的社交媒体（长文）
- 本人的演讲/讲座内容

### Tier 2: Secondary Evidence (间接证据)
- 亲近者的描述/评价
- 工作伙伴的观察
- 详细的传记材料
- 专业媒体报道

### Tier 3: Circumstantial Evidence (旁证)
- 行为数据（购买、活动）
- 社交媒体互动模式
- 公开的职业轨迹
- 关联事件的时间线

### Tier 4: Inference (推断)
- 从其他维度推导
- 群体统计特征
- 文化背景假设

---

## Application Guidelines

### In Diary Entries
```markdown
**置信度**: H

## 今天发生了什么
描述了在项目中的关键决策...

## 当时的想法
当时认为应该优先考虑长期影响...

## 复盘
### 做得好的
- 坚持了原则
- 考虑了多方利益
```

### In Dimension Analysis
```yaml
engram_data:
  mbti:
    type: INTJ
    confidence: H
    evidence:
      - "博客《我的思考方式》显示Ni洞察模式"
      - "决策历史显示Te组织倾向"
      - "多次表达对概念理论的偏好"
```

### In Final Report
```markdown
## 置信度总结
- F级: 基础身份信息 (5项)
- H级: 核心人格维度 (8项)
- M级: 行为模式推断 (6项)
- L级: 待验证假设 (3项)

**建议**: 优先验证M级维度，收集更多证据升级。
```

---

## Common Pitfalls

### Overconfidence (过度自信)
- ❌ 将单一事件推断视为H级
- ❌ 忽略文化/语境影响
- ❌ 将猜测包装为事实

### Excessive Conservatism (过度保守)
- ❌ 忽视多个弱证据的累积效应
- ❌ 要求过多证据才给予H级
- ❌ 将所有推断都标为L级

### Confirmation Bias (确认偏误)
- ❌ 只关注支持假设的证据
- ❌ 忽视矛盾信息
- ❌ 强行解释不符合的证据

---

> **Golden Rule**: 宁可标低置信度并明确不确定性，也不要高估可靠性。用户可以根据置信度决定如何使用信息。
