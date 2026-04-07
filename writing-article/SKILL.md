---
name: writing-article
description: >-
  按主题与类型、平台组合加载约束规则、内容原则、分类与平台参考及写作技巧库，产出高质量文章与文案。触发词：写作、写文章、文案、润色、扩写、改写、缩写、标题、大纲、金句、公众号、知乎、小红书、
  抖音、B站、视频脚本、口播、种草、带货、转化文案、着陆页、B2B、白皮书、案例、邮件通讯、Newsletter、朋友圈、推文、X、LinkedIn、Medium、掘金、即刻、播客稿、品牌故事。适用于需指定或隐含类型与平台的写作任务。
---

# Writing Article - 写作技能

按主题与类型、平台组合加载约束规则、内容原则、分类与平台参考及写作技巧库，产出高质量文章与文案。

## 定位

接受写作任务，组合加载规则文件，输出高质量内容。

---

## 输入参数

| 参数 | 必填 | 说明 |
|------|:----:|------|
| `主题` | ✅ | 写作主题或任务描述 |
| `类型` | ✅ | 见下方[技巧组合指南](#技巧组合指南)，默认 `general` |
| `平台` | ⬜ | 见下方平台列表，默认 `general` |
| `素材` | ⬜ | 参考素材，可多篇，AI 杂糅融合，不得原文照搬 |
| `字数` | ⬜ | 未指定则采用平台推荐字数 |
| `排版` | ⬜ | 未指定则采用平台推荐排版 |

---

## 文件加载顺序

```
1. references/harnesses.md     ← 必读，最高优先级，先建立红线
2. references/rules.md         ← 必读，内容基本原则
3. references/categories/{type}.md
4. references/platforms/{platform}.md
5. references/arts/{art}.md    ← 可多个，按[技巧组合指南]推荐加载
```

**组装公式**：输出 = 类型 ＋ 平台 ＋ 技巧 ＋ 内容规则 ＋ 约束规则

---

## Markdown 使用规则

| 内容场景 | 排版方式 |
|---------|---------|
| 通用文章、公众号图文 | ✅ 使用 Markdown |
| 朋友圈、纯社交媒体文案 | ❌ 纯文本，无任何 Markdown 标记 |

> 判断依据：类型为 `social` 且平台为 `wechat`（朋友圈场景）时输出纯文本。
> 其他所有场景默认使用 Markdown。

---

## 技巧组合指南

根据你的写作目标，选择合适的类型、平台和技巧组合：

### 📄 深度长文 / 观点文章

| 场景 | 类型 | 推荐平台 | 核心技巧组合 | 辅助技巧 |
|------|------|----------|--------------|----------|
| 行业洞察 / 商业分析 | general | 公众号 / 即刻 | APAG + 叙事弧 | SCQA + Bucket Brigades |
| 知识干货 / 深度教程 | general | 公众号 / 掘金 | SCQA + 5W1H | FAB + 公众号结构 |
| 个人成长 / 思考随笔 | general | Medium / 即刻 | APAG + 故事弧 | Hook + 金句公式 |
| 知乎深度回答 | general | 知乎 | SCQA + 叙事弧 | Bucket Brigades |
| 时事评论 / 热点分析 | general | X(Twitter)长推 | SCQA + 4U标题 | Hook |

### 📱 短视频 / 视频脚本

| 场景 | 类型 | 推荐平台 | 核心技巧组合 | 辅助技巧 |
|------|------|----------|--------------|----------|
| 抖音爆款视频 | video-script | 抖音 | 抖音三段式 + Hook + AIDA | 情绪价值 |
| B站知识视频 | video-script | B站 | SCQA + 故事弧 + 5W1H | Hook |
| YouTube Shorts | video-script | YouTube Shorts | 黄金3秒 + AIDA | Bucket Brigades |
| 产品种草视频 | video-script | 小红书/抖音 | FABE + Hook | 情绪价值 |

### 🛒 产品推广 / 转化文案

| 场景 | 类型 | 推荐平台 | 核心技巧组合 | 辅助技巧 |
|------|------|----------|--------------|----------|
| 小红书种草笔记 | product | 小红书 | 小红书三大公式 + FABE | 7大标题 + 情绪价值 |
| 公众号产品推广 | product | 公众号 | PAS + FABE | Hook + 前后对比 |
| 电商详情页 | product | general | FABE + AIDA | 4U标题 |
| 冷启动邮件 | newsletter | general | PAS + 4U标题 | Hook |
| 产品发布文案 | product | LinkedIn / X | AIDA + StoryBrand | 黄金圈 |

### 📢 品牌故事 / 内容营销

| 场景 | 类型 | 推荐平台 | 核心技巧组合 | 辅助技巧 |
|------|------|----------|--------------|----------|
| 品牌故事 / 创始人IP | storytelling | 公众号 | 英雄之旅 + 叙事弧 | APAG |
| 客户成功案例 | case-study | general / LinkedIn | 英雄之旅 + FABE | StoryBrand |
| 品牌宣言 / 使命愿景 | storytelling | 官网/公众号 | StoryBrand + 黄金圈 | 金句公式 |
| 知乎盐选故事 | storytelling | 知乎 | 英雄之旅 + PSP + 三幕式 | Hook |

### 💼 B2B / 专业内容

| 场景 | 类型 | 推荐平台 | 核心技巧组合 | 辅助技巧 |
|------|------|----------|--------------|----------|
| B2B公众号 / SaaS内容 | b2b | 公众号 | Business Casual + SCQA | 数据叙事 |
| 白皮书 / 行业报告 | whitepaper | general | SCQA + RIDBUR | 5W1H |
| 技术博客 | b2b | 掘金 / Medium | SCQA + FAB + 5W1H | 代码示例 |
| LinkedIn职业内容 | b2b | LinkedIn | SCQA + Hook | StoryBrand |
| 销售提案 | b2b | general | PAS + FABE + 数据叙事 | 前后对比 |

### 💬 社交媒体 / 短内容

| 场景 | 类型 | 推荐平台 | 核心技巧组合 | 辅助技巧 |
|------|------|----------|--------------|----------|
| 朋友圈文案 | social | 微信(朋友圈) | Hook + 情绪价值 | 网感写作 |
| 小红书短笔记 | social | 小红书 | Hook + 4U + 网感写作 | 金句公式 |
| X(Twitter)推文 | social | X | Hook + SCQA | 4U标题 |
| 即刻动态 | social | 即刻 | SCQA + 金句 | Hook |
| 活动预热 | social | 朋友圈/即刻 | Hook + 情绪价值 | FOMO设计 |

### 🎙️ 播客 / 音频内容

| 场景 | 类型 | 推荐平台 | 核心技巧组合 | 辅助技巧 |
|------|------|----------|--------------|----------|
| 单人播客 | podcast | 小宇宙/Spotify | 故事弧 + SCQA | Hook |
| 访谈播客 | podcast | 小宇宙 | StoryBrand + SCQA | 5W1H |
| 知识类播客 | podcast | 喜马拉雅 | SCQA + 5W1H | 金句公式 |

---

## 技巧速查表

按写作技巧的类型快速查找：

### 经典转化框架（英文）

| 技巧 | 核心用途 | 适用场景 |
|------|----------|----------|
| [AIDA](references/arts/aida.md) | 注意-兴趣-欲望-行动 | 销售文案、广告、着陆页 |
| [PAS](references/arts/pas.md) | 问题-激化-解决 | 痛点营销、冷邮件、广告 |
| [FAB](references/arts/fab.md) | 特征-优势-利益 | 产品描述、销售话术 |
| [FABE](references/arts/fabe.md) | 特征-优势-利益-证据 | 高客单价产品、B2B销售 |
| [BAB](references/arts/before-after.md) | 之前-之后-桥梁 |  transformation类内容 |
| [4U](references/arts/4u.md) | 有用-紧急-独特-具体 | 标题、短文案 |
| [PASTOR](references/arts/pastor.md) | 问题-放大-方案-证明-反应 | 长销售页面 |
| [SLAP](references/arts/slap.md) | 停下-观看-行动-购买 | 社交媒体广告 |
| [APP](references/arts/app.md) | 认同-承诺-预览 | 内容营销、博客 |
| [QUEST](references/arts/quest.md) | 资格-理解-教育-刺激-转化 | 合格线索培育 |
| [PPPP](references/arts/pppp.md) | 画面-承诺-证明-推动 | 故事型销售文案 |
| [ACCA](references/arts/acca.md) | 认知-理解-确信-行动 | 教育型内容 |
| [4Cs](references/arts/four-cs.md) | 清晰-简洁-吸引-可信 | 通用文案自检 |

### 故事叙事框架

| 技巧 | 核心用途 | 适用场景 |
|------|----------|----------|
| [英雄之旅](references/arts/hero-journey.md) | 经典故事结构 | 品牌故事、创始人IP |
| [英雄之旅简化版](references/arts/hero-journey-simplified.md) | 12阶段简化 | 短视频脚本、演讲 |
| [三幕式](references/arts/three-act.md) | 开端-冲突-结局 | 剧本、长故事 |
| [Freytag金字塔](references/arts/freytag-pyramid.md) | 五阶段戏剧结构 | 小说、戏剧 |
| [PSP](references/arts/psp.md) | Pixar故事法则 | 动画、品牌故事 |
| [叙事弧](references/arts/story-arc.md) | 完整故事曲线 | 长文章、演讲 |
| [STAR](references/arts/star.md) | 情境-任务-行动-结果 | 面试、案例分享 |
| [StoryBrand](references/arts/storybrand.md) | 品牌故事七部曲 | 品牌定位、营销 |

### 结构化表达框架

| 技巧 | 核心用途 | 适用场景 |
|------|----------|----------|
| [SCQA](references/arts/scqa.md) | 情境-冲突-问题-答案 | 商务汇报、写作开头 |
| [SCQA中文应用](references/arts/scqa-chinese.md) | SCQA本土化 | 公众号、知乎 |
| [5W1H](references/arts/5w1h.md) | 六何分析法 | 新闻报道、教程 |
| [APAG](references/arts/apag.md) | 痛苦-渴望-答案-收获 | 个人成长、观点文 |
| [黄金圈](references/arts/golden-circle.md) | WHY-HOW-WHAT | 品牌定位、演讲 |

### 中文社交媒体技巧

| 技巧 | 核心用途 | 适用平台 |
|------|----------|----------|
| [小红书三大爆款公式](references/arts/xiaohongshu-3-formulas.md) | 小红书专属结构 | 小红书 |
| [抖音爆款三段式](references/arts/douyin-3-step.md) | 短视频脚本结构 | 抖音 |
| [公众号文章结构](references/arts/wechat-article-structure.md) | 公众号排版规范 | 公众号 |
| [7大爆款标题模板](references/arts/title-7-templates.md) | 标题公式 | 全平台 |
| [8大开篇模板](references/arts/opening-8-templates.md) | 开头写作 | 公众号、知乎 |
| [金句写作公式](references/arts/golden-sentence-formulas.md) | 金句创作 | 全平台 |
| [鱼骨写作法](references/arts/fishbone-writing.md) | 结构化写作 | 深度长文 |
| [情绪价值写作法](references/arts/emotional-value-writing.md) | 情感共鸣 | 社交媒体 |
| [网感写作技巧](references/arts/internet-slang-integration.md) | 网络语感 | 社交媒体 |

### B2B / 专业写作

| 技巧 | 核心用途 | 适用场景 |
|------|----------|----------|
| [Business Casual](references/arts/business-casual.md) | 专业又轻松 | B2B内容 |
| [Full-Funnel](references/arts/full-funnel.md) | 全漏斗内容 | B2B营销 |
| [RIDBUR](references/arts/ridbur.md) | 6步专业框架 | B2B销售文案 |
| [Hyper-Personalization](references/arts/hyper-personalization.md) | 超个性化 | ABM营销 |
| [Data-Driven Storytelling](references/arts/data-driven-storytelling.md) | 数据叙事 | 报告、分析 |

### 写作增强技巧

| 技巧 | 核心用途 | 适用场景 |
|------|----------|----------|
| [Hook](references/arts/hook.md) | 开头钩子 | 全平台开头 |
| [Bucket Brigades](references/arts/bucket-brigades.md) | 阅读流畅度 | 长文章 |
| [AIDA变体](references/arts/aida-variations.md) | AIDA扩展版 | 高级文案 |
| [So What Test](references/arts/so-what-test.md) | 自检方法 | 内容审核 |

---

## 素材处理规则（有素材时生效）

1. 提取各素材的核心论点、关键数据、典型案例
2. 以写作主题为轴心进行融合，不做拼贴
3. 不得连续复制原文超过 15 字
4. 素材间若有矛盾观点，须主动判断取舍或注明

---

## 文件索引

```
writing-article/
├── SKILL.md                         ← 主控入口（本文件）
└── references/
    ├── harnesses.md                 约束规则（最高优先级）
    ├── rules.md                     内容基本原则
    ├── categories/
    │   ├── general.md               通用文章
    │   ├── social.md                社交媒体内容
    │   ├── b2b.md                   B2B内容/SaaS内容营销
    │   ├── product.md               产品推广/种草文案
    │   ├── storytelling.md          品牌故事/创始人IP
    │   ├── newsletter.md            邮件通讯/Newsletter
    │   ├── whitepaper.md            白皮书
    │   ├── case-study.md            案例研究
    │   ├── video-script.md          视频脚本
    │   └── podcast.md               播客脚本
    ├── platforms/
    │   ├── general.md               通用（无特定平台）
    │   ├── wechat.md                微信
    │   ├── xiaohongshu.md           小红书
    │   ├── zhihu.md                 知乎
    │   ├── douyin.md                抖音
    │   ├── juejin.md                掘金
    │   ├── medium.md                Medium
    │   ├── linkedin.md              LinkedIn
    │   ├── bilibili.md              B站/哔哩哔哩
    │   ├── x.md                     X/Twitter
    │   ├── jike.md                  即刻
    │   └── youtube-shorts.md        YouTube Shorts
    └── arts/
        ├── apag.md                          APAG 框架
        ├── scqa.md                          SCQA 金字塔
        ├── hook.md                          钩子技法
        ├── fab.md                           FAB 利益框架
        ├── fabe.md                          FABE框架（强化版）
        ├── story-arc.md                     叙事弧
        ├── pas.md                           PAS框架
        ├── aida.md                          AIDA模型
        ├── 4u.md                            4U标题法
        ├── psp.md                           PSP/Pixar故事法则
        ├── hero-journey.md                  英雄之旅
        ├── hero-journey-simplified.md       英雄之旅简化版
        ├── before-after.md                  前后对比桥
        ├── pastor.md                        PASTOR框架
        ├── slap.md                          SLAP框架
        ├── app.md                           APP框架
        ├── quest.md                         QUEST框架
        ├── pppp.md                          4P/PPPP框架
        ├── star.md                          STAR方法
        ├── three-act.md                     三幕式结构
        ├── freytag-pyramid.md               Freytag金字塔
        ├── so-what-test.md                  So What? Test
        ├── four-cs.md                       4Cs框架
        ├── acca.md                          ACCA框架
        ├── aida-variations.md               AIDA变体
        ├── bucket-brigades.md               Bucket Brigades
        ├── 5w1h.md                          5W1H
        ├── golden-circle.md                 黄金圈法则
        ├── storybrand.md                    StoryBrand框架
        ├── xiaohongshu-3-formulas.md        小红书三大爆款公式
        ├── fishbone-writing.md              鱼骨写作法
        ├── opening-8-templates.md           8大开篇模板
        ├── golden-sentence-formulas.md      金句写作公式
        ├── douyin-3-step.md                 抖音爆款三段式
        ├── wechat-article-structure.md      公众号文章结构
        ├── title-7-templates.md             7大爆款标题模板
        ├── scqa-chinese.md                  SCQA中文应用
        ├── emotional-value-writing.md       情绪价值写作法
        ├── internet-slang-integration.md    网感写作技巧
        ├── business-casual.md               Business Casual
        ├── full-funnel.md                   Full-Funnel Method
        ├── ridbur.md                        RIDBUR框架
        ├── hyper-personalization.md         Hyper-Personalization
        └── data-driven-storytelling.md      Data-Driven Storytelling
```
