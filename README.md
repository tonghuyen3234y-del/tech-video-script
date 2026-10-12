# 爆款科技口播文案

一个面向 Codex 的中文科技短视频口播技能：先核实新闻，再输出5个标题、约200字的一段式口播，以及新闻来源链接。

## 使用

安装后输入：

> 用爆款科技口播文案，写这个选题：【你的科技新闻选题】

也可用内部技能名 `$tech-video-script` 调用，并补充语气或长度要求。

## 安装

下载本仓库，将 `tech-video-script` 文件夹复制到 `~/.codex/skills/`。文件结构应为 `~/.codex/skills/tech-video-script/SKILL.md`，之后在支持个人技能的 Codex 会话中调用。

## 能力

- 5个不同角度的标题，推荐1个。
- 默认180—230字口播，整理成一个自然段。
- 优先官方来源，核对媒体报道，提供新闻日期与直接链接。
- 支持结果递进、冲突反转、科技应用、画面吐槽四类结构。
- 无法证实的选题不写成事实；高点击率是创作目标，不承诺流量。

需要运行环境具备联网检索及网页阅读能力。本项目是技能指令，不是独立运行的AI服务；GitHub Pages仅展示介绍与安装说明。

## 项目结构

- `tech-video-script/SKILL.md`：核心工作流
- `tech-video-script/references/style-guide.md`：口播风格指南
- `tech-video-script/agents/openai.yaml`：显示名称与默认提示
- `docs/index.html`：GitHub Pages展示页

## 部署到 GitHub Pages

在仓库 Settings → Pages 中将 Source 设为 GitHub Actions。推送到 `main` 后，Pages工作流会发布 `docs/` 目录。也可手动运行工作流。

## 开源许可

MIT。仓库包含提炼后的写作指南，不包含用户原始参考文案或本地路径。
