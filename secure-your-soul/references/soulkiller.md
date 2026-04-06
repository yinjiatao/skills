# Soul Killer — 灵魂杀手

从公开信息中提取日记片段。

---

## 搜索策略

### 1. 建立时间线

```
Query:
- "{name}" timeline / journey / history
- "{name}" year in review / annual review
- "{name}" newsletter archive / blog archive
```

### 2. 采集日记内容

**复盘/反思**（高优先级）:
```
- "{name}" lessons learned / what I learned
- "{name}" mistake / failure / retrospective
- "{name}" how I think about / changed my mind
```

**日常/工作**:
```
- "{name}" daily routine / how I work
- "{name}" tools I use / workflow
```

**决策/转折**:
```
- "{name}" why I quit / why I started
- "{name}" turning point / changed my life
```

### 3. 识别关键节点

标记为 **转折点** 的条件:
- 职业方向改变
- 重大决策
- 认知转变
- 重大失败/成功
- 重要关系

---

## 输出格式

```yaml
diary_candidates:
  - date: "YYYY-MM-DD"
    type: "daily|milestone|turning_point"
    title: "..."
    content: "..."
    source: "URL"
    confidence: "H"
```

---

## 下一步

搜索完成后 → 读取 [engram.md](engram.md) 进入提炼阶段
