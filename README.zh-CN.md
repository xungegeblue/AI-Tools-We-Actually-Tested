# 我亲自用过的 AI 工具合集

**一份短的 AI 工具清单 • 一个任务只留一个工具 • 每个都真的打开用过才上榜**

没有无限滚动 • 没有返利链接 • 没有「2026 年度百大 AI 工具」这种凑数榜

> English version: [README.md](README.md)

---

## 为什么只有 4 个

AI 工具现在有几万个，能撑过第二次使用的没几个。

所以这份清单故意做得很小：**一个任务只放一个最强的**。有缺点就写在缺点那一栏，不藏。是自己的产品，点进去之前就告诉你。

这是 [木薯派 AI 工具目录](https://musepics.com/) 的开源镜像 —— 同样的条目、同样的规则，纯 Markdown，不用开 JS 也能读，可以随便 fork。

**当前收录：4 个工具，4 个分类。**

---

## 一览表

| 工具 | 解决什么问题 | 免费额度 | 付费 |
|---|---|---|---|
| [AIGenerate](https://musepics.com/site/aigenerate) | 生成的图能保持同一张脸 | 每天 3 张，**不用注册** | 积分解锁 2K / 4K |
| [Jev FastEval](https://musepics.com/site/jev-fasteval) | 0.3 秒给文本打分，不用跟它聊天 | 每天 10 次（需注册） | Pro：每天 100 次 |
| [Musebrain](https://musepics.com/site/musebrain) | 用你自己的笔记和 PDF 建私有 AI 知识库 | 指南免费，工作区有免费档 | — |
| [LessonCraft](https://musepics.com/site/teacher-ai) | 教案、测验、学生反馈，十秒出 | 每月免费额度，不要信用卡 | $12/月 · $84/年 |

---

## 免费额度速查

如果只看一张表，看这张 —— 不花钱能拿到什么。

| | 免费额度 | 要注册吗 | 免费能干什么 |
|---|---|---|---|
| **AIGenerate** | 每天 3 张图 | 不用 | Fast 档，全比例 |
| **Jev FastEval** | 每天 10 次 | 要（不绑卡） | 十个评估器全开 |
| **Musebrain** | 指南 + 对比表免费 | 不用 | 方法论免费读，工作区另有免费档 |
| **LessonCraft** | 每月免费额度 | 要（不绑卡） | 三个工具全开，含导出 |

---

## AIGenerate —— 能保持同一张脸的 AI 生图

`图像生成` · [aigenerate.musepics.com](https://aigenerate.musepics.com)

大多数生图工具是为「一张好看的图」设计的。AIGenerate 是为**第二张**设计的：最多上传 14 张参考照片，换了衣服、换了地点、换了光线，脸、雀斑、瞳色还是那个人。

**好在哪**
- 跨场景保脸 —— 最多 14 张参考图，换机位时参考图越多越稳
- 三档画质，**点生成之前就显示要扣多少积分**：Fast、Standard（2K）、Identity（4K）
- 中文或英文直接说，模型收到的是被改写过的结构化英文提示词 —— 不用学写 prompt
- 文生图、图生图、角色模式，还有公开的 Explore 作品墙
- 比例：1:1、3:4、4:3、9:16、16:9，Identity 档最高 4K

**谁该用** —— 角色设定图、分镜（跨帧脸不能变）；同一个模特换不同衣服的产品图；固定风格的头像；不用约拍就能出的 UGC 风格广告素材；主角固定的连载漫画。

**不足** —— 4K 只在 Identity 档，最高画质下反复迭代很烧积分。保脸是「参考图」机制不是训练出来的角色模型，参考图给得少又要大改机位，仍是弱项。

**替代品** —— [Photo AI](https://photoai.com)（写实人像和产品场景更强，更像工作室而不是单一生图器）、[Leonardo AI](https://leonardo.ai)（模型库大得多，界面也重得多）。

→ [完整条目](tools/aigenerate.md) · [功能](https://musepics.com/site/aigenerate/features) · [价格](https://musepics.com/site/aigenerate/pricing)

---

## Jev FastEval —— 0.3 秒出诊断分

`文本评分` · [eval.musepics.com](https://eval.musepics.com)

十个「粘贴就打分」的评估器，返回的是一块仪表盘而不是一段话。粘标题、粘简历、粘合同、粘报错日志，大概 0.3 秒出分数加具体问题项 —— 不用写 prompt，同样的输入每次输出结构完全一致。

**十个评估器** —— 标题点击率、广告合规、meta 点击率、JSON 报错、冷邮件垃圾度、评论痛点、配色方案、简历 ATS、合同风险、随便问。

**好在哪**
- 约 0.3 秒渲染打分仪表盘，而不是流式吐 10–15 秒的散文
- 零 prompt 工程 —— 粘文本或者丢 PDF
- 输出稳定：分数、高亮的问题项、以及决定这个分的关键因素
- 免费额度是真的能用：每天 10 次，不绑卡

**谁该用** —— 广告文案发给客户前的自查；针对某一个 JD 改简历；合同给律师之前先过一遍；调标题和 meta 描述；排查 stack trace 或者格式坏掉的 JSON；从 5–100 条买家评论里找出反复出现的那个抱怨。

**不足** —— 分数只是带了个数字的主观意见。合同扫描**不是法律意见**。输出结构固定是它快的原因，也是它死板的原因：真要开放式判断，还是对话模型更好用。

**替代品** —— [ChatGPT](https://chatgpt.com)（更灵活，但 prompt 你自己写、格式你自己清）、[Claude](https://claude.ai)（长文档很强，但它还是输出散文不是分数）。

→ [完整条目](tools/jev-fasteval.md) · [功能](https://musepics.com/site/jev-fasteval/features) · [价格](https://musepics.com/site/jev-fasteval/pricing)

---

## Musebrain —— 建在你自己文档上的私有 AI

`个人 AI · 知识库` · [ai.musepics.com](https://ai.musepics.com)

把你自己的文档变成一个带引用的私有索引，而不是每天早上往聊天框里粘上下文。讲的是真正决定「个人 AI 值不值得留」的四件事 —— 隐私、记忆、数据摄入、延迟 —— 并且不带厂商话术地对比主流产品。

**好在哪**
- 文档留在你自己的 namespace，不用于训练
- 每个回答都引用你自己文件里的那一段，能核对
- 删文档会连向量一起删 —— 删就是删
- PDF、DOCX、Markdown、CSV 原样丢进去就行
- 有独立对比表，还有公开的「我们怎么测」页面

**谁该用** —— 几个月后回头问自己的研究笔记；回忆跟客户谈定了什么、连当时的邮件一起调出来；把一堆 PDF 变成能追问的东西；维护一份随时可查的私有决策记录。

**不足** —— 它既是指南又是工作区，不是你现在笔记软件的替代品。笔记已经在 Notion 里，迁移成本是真的；笔记散落在一堆 PDF 里，那才是它正好解决的场景。

**替代品** —— [NotebookLM](https://notebooklm.google.com)（免费、引用优先，但绑 Google 账号，也不是一个永久的个人索引）、[Notion AI](https://www.notion.com/product/ai)（笔记本来就在 Notion 的话最合适，摄入外部 PDF 弱一些）。

→ [完整条目](tools/musebrain.md) · [功能](https://musepics.com/site/musebrain/features) · [价格](https://musepics.com/site/musebrain/pricing)

---

## LessonCraft —— 教案、测验、反馈，十秒左右

`教育` · [teacher.musepics.com](https://teacher.musepics.com)

三个专门吃「教学周边文书」的工具：对齐课标的教案（含时间分配和分层）、答案印在单独一页的测验、以及引用学生自己原话的评分表反馈。

**好在哪**
- 教案会写明对应的 anchor standard，含教学目标、时间序列、分层、材料和 exit ticket
- 测验四种题型 —— 单选、简答、判断、填空 —— 答案单独一页
- 反馈引用学生自己的原话，指出哪里做对了、下一步具体改什么
- 支持 Common Core、NGSS、TEKS、Florida BEST、UK、Australian、IB、AP
- 学生作答评分后即丢弃，不存储不训练
- 导出 .docx、按 letter 纸打印，或者复制成 Markdown 进 Google Docs 和 LMS

**谁该用** —— 每周备课不想从空白页开始；一次坐下把测验和答案一起做完；要按班级规模而不是按篇数批反馈；临时请假还要一份写着课标的代课教案。

**不足** —— 免费档有月度上限；「对齐课标」是指尊重了框架，不等于对齐了你所在学区的教学进度表。进课堂之前还是要自己过一遍。

**价格** —— 免费起步，不绑卡。免费额度不够用是 $12/月 或 $84/年。

**替代品** —— [MagicSchool](https://www.magicschool.ai)（教师 prompt 品类最全，广度换深度）、[Brisk Teaching](https://www.briskteaching.com)（浏览器插件，直接在现有文档和 LMS 页面里工作）。

→ [完整条目](tools/lessoncraft.md) · [功能](https://musepics.com/site/teacher-ai/features) · [价格](https://musepics.com/site/teacher-ai/pricing)

---

## 这份清单是怎么做的

三条规则，让清单保持短、让推荐能用。详细版在 [guides/how-we-test.md](guides/how-we-test.md)。

**01 —— 每个条目都真的打开过。** 打开、跑通主流程、读过价格页，才可能上榜。没有一条是照着新闻稿或落地页写出来的。

**02 —— 没有付费排名。** 排序是编辑行为。是自己的产品，条目里会写明。花钱买不到位置，对手开口也压不掉谁。

**03 —— 短比全重要。** 一个任务一个强条目，胜过五十个要你自己筛的平庸条目。有更好的出来了，是**替掉**旧条目，不是往后追加。

---

## 利益披露

这 4 个工具和这份清单出自同一个团队。每个条目里都写了，不是塞在页脚 —— 只有 4 个条目还不披露，那就是一张广告。

对比页老老实实链到了真实竞品（[Photo AI](https://photoai.com)、[Leonardo AI](https://leonardo.ai)、[ChatGPT](https://chatgpt.com)、[Claude](https://claude.ai)、[NotebookLM](https://notebooklm.google.com)、[Notion AI](https://www.notion.com/product/ai)、[MagicSchool](https://www.magicschool.ai)、[Brisk Teaching](https://www.briskteaching.com)），因为一个所有答案都是「我们自己」的清单，对你没有任何价值。

---

## 参与

发现某个任务有比这里更强的工具？开个 issue，写清三件事：它做什么、免费额度多少、它有一件什么做不好的事。**不写缺点的条目不合并。** 详见 [CONTRIBUTING.md](CONTRIBUTING.md)。

## 许可

[CC0 1.0](LICENSE) —— 复制、fork、翻译、转载都行。带个链接是情分，不是义务。

---

<sub>与 [木薯派 AI 工具目录](https://musepics.com/) 同步维护 · 有 AI，薯你最派</sub>
