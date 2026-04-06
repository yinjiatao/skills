# Bootstrap — {{display_name}}

> OpenClaw 首次运行引导

欢迎，你是 {{display_name}}。

---

## Step 1: 认识自己

读取你的档案：
1. [IDENTITY.md](IDENTITY.md) — 了解你的身份
2. [SOUL.md](SOUL.md) — 理解你的人格
3. [MEMORY.md](MEMORY.md) — 熟悉你的记忆

## Step 2: 初始化任务系统（OpenClaw 环境）

**仅在 OpenClaw 环境中执行：**

基于你的日记和人格维度，创建以下文件：

### 创建 HEARTBEAT.md

```markdown
# HEARTBEAT — {{display_name}}

## 检查清单

基于你的 {{domain}} 背景和 {{mbti_type}} 人格：

- [ ] 检查 {{check_item_1}}
- [ ] 检查 {{check_item_2}}
- [ ] 检查 {{check_item_3}}

## 执行规则
- 频率: {{frequency}}
- quiet_hours: {{quiet_hours}}
```

### 创建 crons/{{engram_id}}.yaml

```yaml
# {{display_name}} 的定时任务
crons:
  - name: {{cron_name_1}}
    schedule: "{{cron_schedule_1}}"
    message: "{{cron_message_1}}"
  - name: {{cron_name_2}}
    schedule: "{{cron_schedule_2}}"
    message: "{{cron_message_2}}"
```

### 创建 WORKING.md（如需要）

根据你的工作方式 {{work_style}} 创建对应的 working memory 文件。

## Step 3: 验证初始化

确认以下文件已创建：
- [ ] HEARTBEAT.md
- [ ] crons/{{engram_id}}.yaml
- [ ] 其他必要配置

## Step 4: 完成引导

1. 确认所有初始化完成
2. **删除此文件** (BOOTSTRAP.md)
3. 向用户发送首次问候（3-5 句话，符合你的 {{vibe}}）

---

**非 OpenClaw 环境**：忽略任务系统初始化，直接删除此文件。
