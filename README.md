# NOC Points Check

**English** | [中文](#noc-加分自查)

A free lookup page for Express Entry candidates. Enter a NOC code or job title and see two things right away:

- whether the occupation earns the new **high-wage points** (+70, +40 or +20), and
- whether it belongs to a **category-based selection** category with its own invitation rounds.

No login, no tracking, no server. Each page is a single HTML file that runs in your browser.

> **Not affiliated with IRCC or the Government of Canada. Not immigration advice.**
> IRCC decides your NOC from your actual job duties. For your own case, talk to a licensed immigration consultant or lawyer.

## Use it

- English: `https://shunli814.github.io/noc-points-check/`
- 中文: `https://shunli814.github.io/noc-points-check/zh/`

Or download `index.html` (English) or `zh/index.html` (Chinese) and open it in any browser.

## What it does

- **Look up a NOC code.** Shows the high-wage tier, the extra points for Canadian work experience, the points for a qualifying job offer, and any category-based selection categories.
- **Search by job title.** Lists occupations with similar titles on the two official lists.
- **Browse the lists.** Filter by points tier or by category.
- **Not sure of your NOC?** The page includes a prompt you can copy into any AI assistant (ChatGPT, Claude, Gemini and others) together with your job description. Paste the last line of the answer back into the page to see the result.

The prompt tells the AI to classify by job duties rather than job title, to compare neighbouring NOCs that are easy to confuse, and not to lean toward a NOC because it earns points. An AI's answer is a starting point, not a decision.

## The rules in brief

High-wage occupations (in effect from November 3, 2026):

- An occupation is high-wage when its median wage across Canada is at least 1.3 times the average median wage of the overall workforce. It depends on the occupation, not on your own salary.
- At least 12 months of eligible Canadian work experience in a listed occupation adds 70, 40 or 20 points, depending on the tier.
- A qualifying job offer in a listed occupation is worth 100, 70 or 50 points.
- The two are not added together. You get the higher one.

Category-based selection:

- IRCC holds separate invitation rounds for specific categories.
- Being in a category only makes you eligible for those rounds. Whether you are invited still depends on each round's cut-off score and requirements.
- The French-language category does not depend on occupation, so it is not listed on the page.

## Data sources

Both lists are copied from official IRCC pages, last modified **2026-10-16**:

- [High-wage occupations](https://www.canada.ca/en/immigration-refugees-citizenship/services/immigrate-canada/express-entry/check-score/high-wage.html): 186 NOC codes in three tiers
- [Category-based selection](https://www.canada.ca/en/immigration-refugees-citizenship/services/immigrate-canada/express-entry/rounds-invitations/category-based-selection.html): nine occupation categories

The lists can change. If the official pages show a later date, trust them over this page, and please open an issue.

## Limits

- The page covers federal Express Entry only. It does not cover provincial nominee programs.
- It does not calculate a full CRS score or predict draw cut-offs.
- A code that is not on either list is reported as "not listed". The page cannot confirm that an unlisted code is a real NOC code.
- Job title search is a simple keyword match against the official English titles on the two lists.

## Files

```
index.html       English page
zh/index.html    Chinese page
README.md
```

Each page is self-contained: the data, styles and script are all inside the one file.

## Updating the lists

Both pages carry the same data near the top of their `<script>` block: `DATA` (occupations and tiers), `CATS` (category names and requirements) and `CAT_CODES` (which codes belong to which category). When IRCC changes a list, update these in both files and change the date in the page footer and in this README.

---

# NOC 加分自查

[English](#noc-points-check) | **中文**

给 Express Entry 申请人用的免费查询页面。输入 NOC 代码或职业名，马上看到两件事：

- 这个职业有没有新规下的**高薪加分**（+70、+40 或 +20）
- 它是否属于某个**定向抽签类别**，有单独的邀请轮次

不用登录，不收集数据，没有服务器。每个页面就是一个 HTML 文件，在你的浏览器里运行。

> **本项目与 IRCC 及加拿大政府无关，不是移民建议。**
> 你的 NOC 由移民局按实际工作职责认定。个案请咨询持牌移民顾问或律师。

## 怎么用

- 中文版：`https://shunli814.github.io/noc-points-check/zh/`
- English: `https://shunli814.github.io/noc-points-check/`

也可以下载 `zh/index.html`（中文）或 `index.html`（英文），用任何浏览器打开。

## 功能

- **查 NOC 代码**：显示高薪档位、加拿大工作经验的附加分、合格 job offer 的分数，以及所属的定向抽签类别。
- **按职业名搜索**：列出两份官方名单里名称相近的职业，职业名需要用英文。
- **浏览名单**：按加分档位或类别筛选。
- **还不知道自己的 NOC？** 页面里有一段提示词，复制到任意 AI（ChatGPT、Claude、Gemini、DeepSeek、豆包等），加上你的 job description 发送，再把回答的最后一行粘回页面，就能看到结果。

提示词会让 AI 按工作职责而不是头衔来判断，对照容易混淆的相邻 NOC，并且不偏向有加分的 NOC。AI 的回答只是参考，不是认定。

## 规则要点

高薪职业加分（2026 年 11 月 3 日起生效）：

- 高薪与否看职业本身：该 NOC 在全加拿大的工资中位数，达到全体劳动力平均中位数的 1.3 倍以上。不看你个人的工资。
- 在名单内职业累计满 12 个月的合格加拿大工作经验，按档位加 70、40 或 20 分。
- 名单内职业的合格 job offer 得 100、70 或 50 分。
- 两项不叠加，取较高的一项。

定向抽签：

- IRCC 为特定类别单独举行邀请轮次。
- 属于某个类别只代表有资格参加那一类的抽签，是否获邀仍看当轮的分数线和要求。
- 法语类别不看职业，页面里没有列出。

## 数据来源

两份名单都取自 IRCC 官方页面，页面更新日期为 **2026-10-16**：

- [高薪职业名单](https://www.canada.ca/en/immigration-refugees-citizenship/services/immigrate-canada/express-entry/check-score/high-wage.html)：186 个 NOC，分三档
- [定向抽签类别](https://www.canada.ca/en/immigration-refugees-citizenship/services/immigrate-canada/express-entry/rounds-invitations/category-based-selection.html)：九个职业类别

名单可能调整。如果官网的更新日期更晚，请以官网为准，也欢迎提 issue。

## 局限

- 只覆盖联邦 Express Entry，不包括省提名项目。
- 不计算完整的 CRS 总分，不预测抽签分数线。
- 不在两份名单上的代码会显示为"不在名单"。页面无法确认这个代码本身是否真实存在。
- 职业名搜索只是对两份名单里的官方英文名称做关键词匹配。

## 更新名单

两个页面的 `<script>` 开头都有同一份数据：`DATA`（职业和档位）、`CATS`（类别名称和条件）、`CAT_CODES`（代码与类别的对应关系）。IRCC 调整名单时，两个文件都要改，同时更新页面底部和本说明里的日期。
