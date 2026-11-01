# 发布清单 — 从本地目录到 GitHub 仓库

这份文件是给你（维护者）看的操作手册，发布完可以删，也可以留着当备注。

---

## 1. 仓库名

推荐：**`ai-tools-we-tested`**

理由：
- 仓库名里带 `ai-tools`，GitHub 站内搜索和 Google 索引都能命中核心词
- `we-tested` 是差异化，也是这个站唯一的真卖点（每个都打开跑过）
- 不像 `awesome-` 前缀那样有社区规范负担（awesome list 有隐性标准，不合规会被踩）

备选（按需替换，本地目录一起改名即可）：

| 名称 | 适合什么 | 代价 |
|---|---|---|
| `awesome-ai-tools-tested` | 想吃 "awesome ai tools" 的搜索流量 | 会被当 awesome list 审视，需要更严格的条目质量 |
| `ai-tools-short-list` | 强化「短而精」定位 | 搜索词覆盖弱一些 |
| `musepics-directory` | 品牌向，和站点同名 | 几乎没有搜索流量，只适合给老用户找 |

---

## 2. 仓库描述（Description）

填在仓库右上角 About 里，**这是 GitHub 搜索权重最高的字段之一**，别留空。

```
A short, tested list of AI tools — one per job. Every entry was opened, run and priced by hand. No paid placement, no affiliate links, no top-100 padding.
```

中文版可以放在 README 里，Description 保持英文（覆盖英文搜索）。

---

## 3. Topics（标签）

进仓库 → 右上角齿轮 → Topics，逐个粘进去（最多 20 个）：

```
ai-tools  ai  ai-tools-list  ai-directory  awesome-list  generative-ai
ai-image-generator  face-consistency  text-scoring  resume-ats  personal-ai
knowledge-base  education  teacher-tools  lesson-planner  free-ai-tools
ai-resources  llm  prompt-engineering  productivity
```

前 5 个是关键，别漏 `ai-tools` 和 `awesome-list`（后者能进 GitHub 的 awesome 主题聚合页）。

---

## 4. 发布命令

已经装好 `gh` 的话，两条命令搞定：

```bash
cd "C:/Users/Administrator/WorkBuddy/2026-11-01-17-18-22/ai-tools-we-tested"
git init -b main
git add .
git commit -m "feat: initial AI tools directory — 4 entries, tested by hand"
gh repo create ai-tools-we-tested --public --source=. --remote=origin --push \
  --description "A short, tested list of AI tools — one per job. No paid placement, no affiliate links."
```

没装 `gh` 就用网页建空仓库，再：

```bash
git remote add origin https://github.com/<你的用户名>/ai-tools-we-tested.git
git branch -M main
git push -u origin main
```

> 别忘了把仓库 About 里的 **Website** 填成 `https://musepics.com/` — 这是从 GitHub 导流回站点的唯一常驻入口，权重比 README 里的链接高。

---

## 5. 发布后必做的 4 件事

| 动作 | 位置 | 为什么 |
|---|---|---|
| 填 Website 字段 | About → 齿轮 | README 里的链接是 nofollow，About 里的访客入口才是真流量 |
| 传 Social preview 图 | Settings → Social preview | 别人转发链接时有图，点击率差一倍 |
| Pin 到个人主页 | Profile → Customize pins | 新仓库没 star，Pin 是唯一稳定曝光 |
| 选中 4 个 Topics | About → 齿轮 | 缺 topic 等于从聚合页消失 |

---

## 6. 冷启动：前 20 个 star 怎么来

GitHub 不会因为你内容好就推你，前 20 个 star 只能人拉。可行的顺序：

1. **中文社区反哺** — 在你已经发过内容的平台（木薯派论坛、知乎、V2EX、小红书）发一条「我把 AI 工具目录开源了」，附仓库链接。你现有的读者是唯一会立刻点的人。
2. **Reddit 的 r/SideProject 或 r/InternetIsBeautiful** — 注意这两版块反感纯自推，标题必须写成「我做了一个只有 4 个条目的 AI 目录，因为我受够了百大榜单」这种反共识角度，而不是「来看看我的 AI 工具」。
3. **Hacker News 的 Show HN** — 同一天发，标题 `Show HN: An AI directory with four entries`。短清单 + 反内卷叙事是这个社区唯一买账的角度。
4. **不要买 star** — GitHub 会检测，掉权重比没 star 更糟。

前 20 个之后，搜索和 topic 聚合会开始自己带量。

---

## 7. 后续维护节奏

- **每加一个工具，单独一次 commit**，commit message 带上工具名（`feat: add AIGenerate entry`）。GitHub 的 commit 也能被搜到。
- **加工具时同时改 3 个文件**：`README.md`、`README.zh-CN.md`、`tools/<name>.md`。三个都改，长尾页面才会增加。
- **每季度检查一次死链和价格**，改了就提交。活跃仓库的搜索排名明显好于僵尸仓库。
- **README 顶部那句 "Currently listing: 4 tools"** 记得同步，数字对不上会立刻掉信任。

---

## 8. 一句话判断这次有没有效

别只看 star。两周后看这三个数：

- GitHub 仓库页的 **referral traffic**（仓库 → Insights → Traffic）
- musepics.com 的 **Referrers 里是否出现 github.com**
- Google Search Console 里 `site:github.com` 是否已收录这个仓库

如果 GitHub 那边有点击但站上没转化，问题在落地页；如果完全没曝光，问题在命名和 topics。两种问题的解法完全不同，别混着改。
