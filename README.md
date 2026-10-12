# Useful Mint Skills

Free Agent Skills that get real work done with the AI you already use, for people who build with AI but don't write code.

Each Skill is a standard `SKILL.md` folder, the format Claude Code, Codex, Cursor and other agents read. You can also upload one to claude.ai or Cowork.

Tested so far: `launch-check` in Claude Code, Codex and Cursor (October 7). `brand-palette` and `clear-deck` in Claude Code and Codex (October 12); Cursor is not tested yet. Uploading to claude.ai or Cowork is not tested for any of them. Each Skill's page on usefulmint.com has its full test record.

[简体中文](README.zh-CN.md)

| Skill                                                                                                                                           | What you get                                                                                                                                                            | What you bring                                      | Try saying                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------- | ---------------------------------------------- |
| [`launch-check`](https://usefulmint.com/skills/launch-check/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610)   | A plain-language report of what will break before you go live: leaked keys, pages that won't load, missing settings, phone layout problems. Safe fixes after you agree. | Your project and where you plan to publish it       | "Check my site before I launch it."            |
| [`brand-palette`](https://usefulmint.com/skills/brand-palette/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610) | An original five-color palette as editable SVG and CSS values, with contrast numbers for every text pairing.                                                            | Your brand, your audience and the feeling to convey | "Make a color palette for my ceramics studio." |
| [`clear-deck`](https://usefulmint.com/skills/clear-deck/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610)       | A short presentation as editable SVG slides with speaker notes, one claim per slide.                                                                                    | Your notes, the audience and the decision you need  | "Turn these notes into a six-slide proposal."  |

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
- Promise PowerPoint files: `clear-deck` delivers SVG slides and notes, and exports PPTX only when a real presentation library is available.
- Change your project silently: `launch-check` asks before every fix. Real-phone display and live hosting settings still need your own check.

## Next steps

- After `launch-check`: [**Error Rescue**](https://usefulmint.com/skills/error-rescue/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610) (Pro), which reads the error with you and fixes it.

[Browse all Skills](https://usefulmint.com/skills/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610)

## License

MIT. Made by [Useful Mint](https://usefulmint.com/?utm_source=github&utm_medium=readme&utm_campaign=ecosystem_public-skills_202610).
