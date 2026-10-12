# 各工具下的运行方式

这个 Skill 可以被支持 Skill 目录的 AI 编程工具读取，也可以作为提示词手动粘贴。

## Claude Code

- 项目级：`.claude/skills/launch-check/SKILL.md`
- 个人级：`~/.claude/skills/launch-check/SKILL.md`
- 触发方式：直接说"帮我做上线前检查"，或输入 `/launch-check`。

## Codex

- 项目级：`.agents/skills/launch-check/SKILL.md`
- 个人级：`~/.agents/skills/launch-check/SKILL.md`
- 触发方式：直接描述需求，例如"我这个网站能上线了吗"。

## Cursor

- 项目级：`.cursor/skills/launch-check/SKILL.md`
- 个人级：`~/.cursor/skills/launch-check/SKILL.md`
- 触发方式：直接描述需求，例如"我想把这个项目发布到网上，帮我检查一遍"。
- 2026-10-07 用 Cursor Agent CLI 2026.10.01（Auto 模型）实测：放进项目级目录后自动触发。
- Cursor 免费账号只能用 Auto 模型；如果出现“Named models unavailable”报错，在模型选择里切回 Auto。

## Lovable、Bolt、v0 等在线平台

- 这些平台没有 Skill 目录，使用 `prompt-version.md`。
- 注意：这些平台的编辑器里通常看不到版本历史，所以"密钥是否被提交过"这一项
  要明确标记为没检查到。

## 通用提示词版

任何工具都可以直接把 `prompt-version.md` 的内容粘贴进对话。它包含同样的检查项，
只是把执行步骤写成了对话指令。

## 安装流程

1. 用户从商品页下载压缩包。
2. 把压缩包（或解压后的文件夹）交给自己的 AI，说"请帮我安装这个 Skill"。
3. AI 会先读一遍内容，再请求写入项目目录的许可，用户点确认即可。

AI 工具出于安全考虑，通常会在写入 Skill 目录前请求确认，部分工具在默认沙箱里还会
禁止联网下载，所以不要依赖"让 AI 自己去网址下载"。

## 安装后怎么验证

装好后向 AI 提问："我这个项目能上线了吗？" 如果 AI 先问项目位置或先读文件，
说明 Skill 已生效。如果 AI 直接开始泛泛而谈，说明没装上。
