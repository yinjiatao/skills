# 思维工具路由

## 目录

- [用途](#用途)
- [调度规则](#调度规则)
- [选择顺序](#选择顺序)
- [输出契约](#输出契约)
- [工具索引](#工具索引)

## 用途

在信息足以支持分析后，从现有工具中选择最小、必要的组合。工具用于解释已经确认的问题，不代替发现未知。

## 调度规则

1. 直接处理入口：用户明确指定工具时，直接读取该工具文件；信息缺口不阻止交付时，在结果中标记假设。
2. 认知探索入口：完成问卷、未知地图和必要访谈后，只有当用户选择“使用思维工具解释”或已经具备足够信息时才选工具。
3. 每次选择 **一个核心工具**，用于回答当前最关键的问题。
4. 最多选择 **两个辅助工具**，仅用于补足核心工具覆盖不到的关键维度。
5. 如需把分析转化为执行，可以再选择 **一个行动工具**；行动工具不计入两个辅助工具，但不得因此堆叠完整工具链。
6. 每个工具都必须说明：为什么适用、引用了哪条已确认信息、它要回答什么问题。
7. 只读取被选中的工具文件，不批量加载整个目录。
8. 不按问题类别套用固定工具链；如果一个工具足够，就只用一个。
9. 为完成工具模板而补充的数字、阈值或判断标准必须标为 `[建议值]` 或 `[待确认]`，并与用户已确认信息分开。

## 选择顺序

```text
当前最重要的未知或决策
→ 选择一个核心工具
→ 检查是否存在核心工具无法覆盖的关键维度
→ 必要时增加 0—2 个辅助工具
→ 检查分析是否需要转化为执行步骤
→ 必要时增加一个行动工具并输出可执行方案
```

## 输出契约

```markdown
### 核心工具：[工具名]

- 适用原因：
- 引用的已确认信息：
- 要回答的问题：

### 辅助工具：[工具名]（如需要）

- 适用原因：
- 引用的已确认信息：
- 补充的维度：

### 行动工具：[工具名]（如需要）

- 转化目标：
- 第一项可执行结果：
```

分析中仍未确认的内容必须标记为推断、待验证假设或剩余未知。

工具需要补充参数时，在结果末尾使用：

```markdown
### 待确认的建议值
- [建议值] ……；确认或修改后再作为正式标准。
```

## 工具索引

### 目标管理

| 适用场景 | 工具文件 |
| --- | --- |
| 目标模糊，需要具体化 | [SMART](goal-management/smart.md) |
| 有目标但不行动 | [福格行为模型](goal-management/fogg-model.md) |
| 抓不住重点 | [帕累托法则](goal-management/pareto.md) |
| 需要拆解落地 | [WBS](goal-management/wbs.md) |
| 需要迭代反馈 | [PDCA](goal-management/pdca.md) |
| 需要持续动力 | [飞轮效应](goal-management/flywheel.md) |
| 目标与成果需要对齐 | [OKR](goal-management/okr.md) |
| 大目标需要分阶段 | [目标阶梯](goal-management/goal-ladder.md) |
| 需要从终局倒推 | [逆向规划](goal-management/backward-planning.md) |
| 完美主义卡住了 | [最小可行目标](goal-management/mvg.md) |
| 需要增强承诺感 | [承诺一致性](goal-management/commitment-consistency.md) |
| 接近目标反而松懈 | [目标梯度效应](goal-management/goal-gradient.md) |
| 需要进度可视化 | [甘特图](goal-management/gantt.md) |
| 需要阶段性里程碑 | [里程碑](goal-management/milestone.md) |
| 需要找到核心指标 | [北极星指标](goal-management/north-star.md) |

### 沟通表达

| 适用场景 | 工具文件 |
| --- | --- |
| 需要有效赞美 | [FFC](communication/ffc.md) |
| 表达需要逻辑 | [金字塔原理](communication/pyramid-principle.md) |
| 汇报需要重点 | [PREP](communication/prep.md) |
| 开场需要吸引力 | [SCQA](communication/scqa.md) |
| 需要学会拒绝 | [破唱片法](communication/broken-record.md) |
| 谈判策略 | [红白脸策略](communication/good-cop-bad-cop.md) |
| 跨部门或跨角色沟通 | [乔哈里窗](communication/johari-window.md) |
| 需要共情式安慰 | [共情倾听](communication/empathic-listening.md) |
| 提需求被驳回 | [RIDE](communication/ride.md) |
| 沟通引发冲突 | [非暴力沟通](communication/nvc.md) |
| 需要快速说清价值 | [电梯演讲](communication/elevator-pitch.md) |
| 挖掘深层需求 | [SPIN](communication/spin.md) |
| 增强感染力 | [故事化表达](communication/storytelling.md) |
| 引导对方自己想通 | [苏格拉底提问](communication/socratic-questioning.md) |
| 听到真正诉求 | [3F 倾听](communication/3f-listening.md) |

### 问题分析与决策

| 适用场景 | 工具文件 |
| --- | --- |
| 全面分析问题 | [5W2H](analysis-decision/5w2h.md) |
| 分类不遗漏 | [MECE](analysis-decision/mece.md) |
| 追根溯源 | [5 Why](analysis-decision/5why.md) |
| 多角度决策 | [六顶思考帽](analysis-decision/six-thinking-hats.md) |
| 回到本质 | [第一性原理](analysis-decision/first-principles.md) |
| 评估优劣势 | [SWOT](analysis-decision/swot.md) |
| 检查逻辑 | [三段论](analysis-decision/syllogism.md) |
| 预判风险 | [事前验尸](analysis-decision/pre-mortem.md) |
| 激发创意 | [头脑风暴](analysis-decision/brainstorming.md) |
| 简化问题 | [奥卡姆剃刀](analysis-decision/occams-razor.md) |
| 梳理因果 | [鱼骨图](analysis-decision/fishbone.md) |
| 量化比较方案 | [决策矩阵](analysis-decision/decision-matrix.md) |
| 考虑对手反应 | [博弈论](analysis-decision/game-theory.md) |
| 从失败中学习 | [反事实思维](analysis-decision/counterfactual.md) |
| 减少主观偏见 | [贝叶斯思维](analysis-decision/bayesian-thinking.md) |

### 时间与精力管理

| 适用场景 | 工具文件 |
| --- | --- |
| 区分轻重缓急 | [艾森豪威尔矩阵](time-energy/eisenhower-matrix.md) |
| 克服拖延 | [番茄工作法](time-energy/pomodoro.md) |
| 任务管理混乱 | [GTD](time-energy/gtd.md) |
| 精力不足 | [精力金字塔](time-energy/energy-pyramid.md) |
| 提升批量效率 | [批处理](time-energy/batching.md) |
| 被琐事打断 | [莫法特休息法](time-energy/moffat-rest.md) |
| 长期任务推进 | [时间盒](time-energy/timeboxing.md) |
| 进入专注状态 | [心流](time-energy/flow.md) |
| 会议效率 | [罗伯特议事规则](time-energy/roberts-rules.md) |
| 任务时间膨胀 | [帕金森定律](time-energy/parkinsons-law.md) |
| 先做最难的事 | [吃掉那只青蛙](time-energy/eat-the-frog.md) |
| 小事快速处理 | [两分钟法则](time-energy/two-minute-rule.md) |
| 高强度工作节奏 | [超日节律](time-energy/ultradian-rhythm.md) |
| 减少多任务切换 | [单任务](time-energy/monotasking.md) |
| 追踪时间去向 | [时间日志](time-energy/time-log.md) |

### 学习成长

| 适用场景 | 工具文件 |
| --- | --- |
| 深度理解 | [费曼学习法](learning-growth/feynman.md) |
| 阅读记忆 | [RIA](learning-growth/ria.md) |
| 技能提升 | [刻意练习](learning-growth/deliberate-practice.md) |
| 对抗遗忘 | [艾宾浩斯遗忘曲线](learning-growth/ebbinghaus.md) |
| 知识体系化 | [思维导图](learning-growth/mind-mapping.md) |
| 突破认知局限 | [认知升级](learning-growth/cognitive-upgrade.md) |
| 高效笔记 | [康奈尔笔记法](learning-growth/cornell-notes.md) |
| 深度阅读 | [SQ3R](learning-growth/sq3r.md) |
| 跨书主题研究 | [主题阅读](learning-growth/syntopical-reading.md) |
| 学以致用 | [输出驱动](learning-growth/output-driven.md) |
| 复习节奏 | [间隔重复](learning-growth/spaced-repetition.md) |
| 抽象概念理解 | [双重编码](learning-growth/dual-coding.md) |
| 自我觉察学习盲区 | [元认知](learning-growth/metacognition.md) |
| 突破单一练习瓶颈 | [交错练习](learning-growth/interleaving.md) |
| 举一反三 | [心智模型](learning-growth/mental-models.md) |

### 团队与职业

| 适用场景 | 工具文件 |
| --- | --- |
| 辅导下属 | [GROW](team-career/grow.md) |
| 员工激励 | [双因素理论](team-career/herzberg.md) |
| 职业方向 | [职业锚](team-career/career-anchor.md) |
| 竞争力构建 | [护城河理论](team-career/moat-theory.md) |
| 有效复盘 | [GRAI](team-career/grai.md) |
| 管理风格适配 | [情境领导](team-career/situational-leadership.md) |
| 团队磨合 | [塔克曼模型](team-career/tuckman.md) |
| 职责划分 | [RACI](team-career/raci.md) |
| 团队角色平衡 | [贝尔宾团队角色](team-career/belbin.md) |
| 晋升困境 | [彼得原理](team-career/peter-principle.md) |
| 深层能力评估 | [冰山模型](team-career/iceberg-model.md) |
| 能力边界管理 | [能力圈](team-career/circle-of-competence.md) |
| 深度与广度选择 | [T 型人才](team-career/t-shaped.md) |
| 多层次激励 | [马斯洛需求层次](team-career/maslow.md) |
| 系统性管理思考 | [德鲁克五问](team-career/drucker-five.md) |

### 情绪与心态

| 适用场景 | 工具文件 |
| --- | --- |
| 焦虑内耗 | [ABC 情绪理论](emotion-mindset/abc-emotion.md) |
| 心态调整 | [成长型思维](emotion-mindset/growth-mindset.md) |
| 冲动控制 | [12 秒法则](emotion-mindset/12-second-rule.md) |
| 人际关系 | [互惠原理](emotion-mindset/reciprocity.md) |
| 缺乏自信 | [皮格马利翁效应](emotion-mindset/pygmalion.md) |
| 压力管理 | [正念](emotion-mindset/mindfulness.md) |
| 情绪识别 | [情绪颗粒度](emotion-mindset/emotional-granularity.md) |
| 挫折恢复 | [心理韧性](emotion-mindset/resilience.md) |
| 持久幸福感 | [PERMA](emotion-mindset/perma.md) |
| 内驱力 | [自我决定理论](emotion-mindset/self-determination.md) |
| 面对不可控 | [斯多葛控制二分法](emotion-mindset/stoic-dichotomy.md) |
| 转变负面想法 | [认知重评](emotion-mindset/cognitive-reappraisal.md) |
| 延迟满足 | [延迟满足](emotion-mindset/delayed-gratification.md) |
| 非理性决策 | [心理账户](emotion-mindset/mental-accounting.md) |
| 情绪自察 | [情绪日记](emotion-mindset/emotion-journal.md) |
