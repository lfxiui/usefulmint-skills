# Useful Mint Skills

Free Agent Skills that get real work done with the AI you already use, for people who build with AI but don't write code.

Each Skill is a standard `SKILL.md` folder, the format Claude Code, Codex, Cursor and other agents read. You can also upload one to claude.ai or Cowork.

Tested so far: `launch-check` in Claude Code, Codex and Cursor (October 7). The other eleven in Claude Code and Codex (October 12–13). Uploading to claude.ai or Cowork is not tested for any of them. Each Skill's page on usefulmint.com has its full test record.

[简体中文](README.zh-CN.md)

| Skill                  | What you get                                                                                                                                                            | What you bring                                               | Try saying                                          |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------ | --------------------------------------------------- |
| [`launch-check`][lc]   | A plain-language report of what will break before you go live: leaked keys, pages that won't load, missing settings, phone layout problems. Safe fixes after you agree. | Your project and where you plan to publish it                | "Check my site before I launch it."                 |
| [`brand-palette`][bp]  | An original five-color palette as editable SVG and CSS values, with contrast numbers for every text pairing.                                                            | Your brand, your audience and the feeling to convey          | "Make a color palette for my ceramics studio."      |
| [`clear-deck`][cd]     | A short presentation as editable SVG slides with speaker notes, one claim per slide.                                                                                    | Your notes, the audience and the decision you need           | "Turn these notes into a six-slide proposal."       |
| [`event-poster`][ep]   | Two distinctly composed event poster directions as editable SVG, with the event details you supplied kept intact.                                                       | Event name, audience, venue, date, time zone and next action | "Make two posters for our Saturday night market."   |
| [`data-story`][ds]     | An editable data card from a small table: proportional charts, explicit units, and the values and calculations beside them.                                             | A small table and the question it should answer              | "Turn this table into a chart for my reading club." |
| [`idea-deck`][id]      | Three editable slides (the idea, the approach, the smallest next step) with concise speaker notes.                                                                      | The proposal and the decision it should support              | "Turn this proposal into three slides."             |
| [`icon-family`][if]    | A cohesive set of original vector icons on a shared grid, checked at 16, 24 and 48px.                                                                                   | The actions to draw and where they appear                    | "Draw an icon set for my habit app."                |
| [`kinetic-type`][kt]   | A kinetic typography opening as editable HTML/CSS, with a real play/pause control and reduced-motion support.                                                           | One message, three short lines and an authorized image       | "Make a 15-second title animation for my launch."   |
| [`sketch-notes`][sn]   | An illustrated knowledge card with editable SVG diagrams and a distinct symbol for each idea.                                                                           | Your notes                                                   | "Turn these notes into an illustrated card."        |
| [`product-poster`][pp] | An original product poster: editable SVG type composed over your own photograph.                                                                                        | An authorized photo and one message                          | "Make a poster from this product photo."            |
| [`portfolio-page`][pf] | A responsive portfolio site as editable HTML/CSS, selected work before biography.                                                                                       | A short bio and images you own                               | "Build a portfolio page from my bio."               |
| [`landing-story`][ls]  | A responsive product introduction page as editable HTML/CSS, designed from your actual brief rather than a template.                                                    | A real brief with your product details                       | "Build a one-page site for my tea studio."          |

[lc]: https://usefulmint.com/skills/launch-check/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610
[bp]: https://usefulmint.com/skills/brand-palette/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610
[cd]: https://usefulmint.com/skills/clear-deck/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610
[ep]: https://usefulmint.com/skills/event-poster/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610
[ds]: https://usefulmint.com/skills/data-story/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610
[id]: https://usefulmint.com/skills/idea-deck/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610
[if]: https://usefulmint.com/skills/icon-family/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610
[kt]: https://usefulmint.com/skills/kinetic-type/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610
[sn]: https://usefulmint.com/skills/sketch-notes/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610
[pp]: https://usefulmint.com/skills/product-poster/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610
[pf]: https://usefulmint.com/skills/portfolio-page/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610
[ls]: https://usefulmint.com/skills/landing-story/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610

## Install

**Claude Code**

```bash
claude plugin marketplace add lfxiui/usefulmint-skills
claude plugin install usefulmint@usefulmint
```

Then describe the task, or type `/usefulmint:launch-check`.

**Codex, Cursor and other agents** (with [`npx skills`](https://github.com/vercel-labs/skills))

```bash
npx skills add lfxiui/usefulmint-skills
```

Add `--skill brand-palette` to install a single Skill.

**claude.ai and Cowork**

Download a Skill's zip from [Releases](https://github.com/lfxiui/usefulmint-skills/releases) and upload it under Skills in Claude's settings.

**No terminal?**

Open the Skill on [usefulmint.com](https://usefulmint.com/skills/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610) and copy its install prompt into your AI. Your AI downloads the Skill and asks before writing anything.

## What these Skills won't do

- Publish, send messages, buy assets or start paid generation without asking you.
- Promise PowerPoint files: `clear-deck` and `idea-deck` deliver SVG slides and notes, and export PPTX only when a real presentation library is available.
- Change your project silently: `launch-check` asks before every fix. Real-phone display and live hosting settings still need your own check.
- Invent facts: no made-up event details, statistics, customers, prices or testimonials.

## Next steps

- After `launch-check`: [**Error Rescue**](https://usefulmint.com/skills/error-rescue/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610) (Pro), which reads the error with you and fixes it.

[Browse all Skills](https://usefulmint.com/skills/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610)

## License

MIT. Made by [Useful Mint](https://usefulmint.com/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610).
