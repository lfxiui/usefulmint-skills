# Useful Mint Skills

免费的 Agent Skill：交给你正在用的 AI，把一件真事做完。为用 AI 做东西、但不写代码的人准备。

每个 Skill 都是标准的 `SKILL.md` 文件夹，Claude Code、Codex、Cursor 等工具都读这种格式；也可以上传到 claude.ai 和 Cowork。

目前的实测：`launch-check` 在 Claude Code、Codex 和 Cursor 里测过（10 月 7 日）；其余十一个在 Claude Code 和 Codex 里测过（10 月 12–13 日）。十二个都还没测过上传到 claude.ai 和 Cowork。完整的实测记录在 usefulmint.com 上各 Skill 的页面里。

[English](README.md)

| Skill                  | 你会拿到                                                                                                         | 你要准备                                 | 可以这样说                         |
| ---------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------- | ---------------------------------- |
| [`launch-check`][lc]   | 一份看得懂的上线前检查报告：泄露的密钥、打不开的页面、缺少的配置、手机上的显示问题。你同意后修掉能安全修的部分。 | 你的项目，以及准备发布到哪里             | “上线前帮我检查一下这个网站。”     |
| [`brand-palette`][bp]  | 一套原创的五色配色，附可编辑的 SVG 和 CSS 颜色值，每组文字搭配都给出对比度数字。                                 | 品牌介绍、用户和希望表达的气质           | “给我的陶艺工作室配一套颜色。”     |
| [`clear-deck`][cd]     | 一份简短的演示：可编辑的 SVG 幻灯片和讲稿，每页只讲一个观点。                                                    | 原始材料、听众，以及希望促成的决定       | “把这些笔记做成 6 页提案。”        |
| [`event-poster`][ep]   | 两个构图完全不同的活动海报方向，可编辑的 SVG，你给的活动信息原样保留。                                           | 活动名称、听众、场地、日期、时区和下一步 | “给周六夜市做两张海报。”           |
| [`data-story`][ds]     | 一张可编辑的数据卡片：按比例画的图表、写清单位，旁边附上原始数值和计算过程。                                     | 一张小表格，以及它要回答的问题           | “把这张表画成读书会用的图。”       |
| [`idea-deck`][id]      | 三页可编辑幻灯片：想法、做法、最小的下一步，配简短讲稿。                                                         | 提案，以及它要促成的决定                 | “把这份提案做成三页。”             |
| [`icon-family`][if]    | 一套同一网格、同一笔画的原创图标，在 16、24、48 像素下都检查过。                                                 | 要画的那些操作，以及它们出现的位置       | “给我的习惯打卡 App 画一套图标。”  |
| [`kinetic-type`][kt]   | 一段可编辑的 HTML/CSS 动态标题，带真正的播放/暂停，并支持减少动效。                                              | 一句话信息、三行短标题和一张有授权的图   | “给我的发布做一段 15 秒标题动效。” |
| [`sketch-notes`][sn]   | 一张带可编辑 SVG 图解的知识卡片，每个观点有自己的符号。                                                          | 你的笔记                                 | “把这些笔记做成一张图解卡片。”     |
| [`product-poster`][pp] | 一张原创产品海报：可编辑的 SVG 文字排版，叠在你自己的照片上。                                                    | 一张有授权的照片和一句卖点               | “用这张产品照做一张海报。”         |
| [`portfolio-page`][pf] | 一个可编辑的 HTML/CSS 作品集网站，先放作品，再放简介。                                                           | 一段简介和属于你的图片                   | “用我的简介做一个作品集页面。”     |
| [`landing-story`][ls]  | 一个可编辑的 HTML/CSS 产品介绍页，按你的真实材料设计，不是套模板。                                               | 一份真实的产品简介                       | “给我的茶工作室做一页网站。”       |

[lc]: https://usefulmint.com/zh/skills/launch-check/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610
[bp]: https://usefulmint.com/zh/skills/brand-palette/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610
[cd]: https://usefulmint.com/zh/skills/clear-deck/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610
[ep]: https://usefulmint.com/zh/skills/event-poster/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610
[ds]: https://usefulmint.com/zh/skills/data-story/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610
[id]: https://usefulmint.com/zh/skills/idea-deck/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610
[if]: https://usefulmint.com/zh/skills/icon-family/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610
[kt]: https://usefulmint.com/zh/skills/kinetic-type/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610
[sn]: https://usefulmint.com/zh/skills/sketch-notes/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610
[pp]: https://usefulmint.com/zh/skills/product-poster/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610
[pf]: https://usefulmint.com/zh/skills/portfolio-page/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610
[ls]: https://usefulmint.com/zh/skills/landing-story/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610

## 安装

**Claude Code**

```bash
claude plugin marketplace add lfxiui/usefulmint-skills
claude plugin install usefulmint@usefulmint
```

之后直接描述任务，或者输入 `/usefulmint:launch-check`。

**Codex、Cursor 和其他工具**（用 [`npx skills`](https://github.com/vercel-labs/skills)）

```bash
npx skills add lfxiui/usefulmint-skills
```

只装一个就加上 `--skill brand-palette`。

在 Codex 里，`/skills` → Enable/Disable Skills 可以关掉一个 Skill。我们在 Codex CLI 0.166.0 上用一个模型实测：关掉以后，只描述任务时 Codex 没有再用上它，但在消息里用 `$` 点名，还是会把它带进来。详见 [Codex 用的 Skill](https://usefulmint.com/zh/skills/codex/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610)。

**claude.ai 和 Cowork**

在 [Releases](https://github.com/lfxiui/usefulmint-skills/releases) 下载某个 Skill 的 zip，然后在 Claude 设置的 Skills 里上传。

**不用终端？**

在 [usefulmint.com](https://usefulmint.com/zh/skills/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610) 打开这个 Skill，把安装话术复制给你的 AI。AI 会自己下载 Skill，写任何东西之前先问你。

## 这些 Skill 不会做什么

- 未经你同意就发布、发消息、买素材或开始付费生成。
- 不承诺 PowerPoint 文件：`clear-deck` 和 `idea-deck` 交付的是 SVG 幻灯片和讲稿，只有在真的有演示库时才导出 PPTX。
- 不偷偷改你的项目：`launch-check` 每次修改前都会问你。真机显示和线上托管设置仍要你自己确认。
- 不编造内容：不会虚构活动信息、统计数字、客户、价格或评价。

## 下一步

- 跑完 `launch-check` 之后：用 [**Error Rescue**](https://usefulmint.com/zh/skills/error-rescue/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610)（Pro）一起读报错并修好。

[浏览全部 Skill](https://usefulmint.com/zh/skills/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610)

## 许可

MIT。由 [Useful Mint](https://usefulmint.com/zh/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610) 制作。
