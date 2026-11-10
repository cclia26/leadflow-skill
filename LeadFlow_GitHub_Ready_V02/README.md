# LeadFlow · AI 协作领队 Skill

**活动策划 · 任务拆解 · 团队分工 · 人机协作 · 验收复盘**

一份给带队者使用的开源 Agent Skill。适合学生组长、活动负责人、社团骨干、工作坊主持人、志愿项目领队及跨专业项目协调人。

> 把一句模糊的任务，变成每个人都知道下一步做什么的协作计划。

**版本：** v0.2 ｜ **语言：** 中文 ｜ **运行方式：** 兼容 Agent Skills 的 AI 工具 ｜ **依赖：** 无

## 这份 Skill 可以做什么？

| 场景 | 你给它什么 | 它帮你产出什么 |
| --- | --- | --- |
| 接到新任务 | 作业通知、目标、截止时间 | 一句话目标、交付清单、保底方案 |
| 活动策划 | 人数、时长、活动目的 | 分段流程、主持提示、应急处理 |
| 任务分工 | 成员条件、意愿、截止时间 | 负责人、具体交付物、交接入口 |
| 推进项目 | 当前进度、卡点 | 优先级、下一步、可直接发群的通知 |
| 临近截止 | 已完成材料、缺口 | 缩减方案、验收要点、提交动作 |
| 项目结束 | 交付与反馈 | 结果复盘、个人贡献与可复用方法 |

## 五步协作流程

**01 定目标 → 02 拆成果 → 03 配协作 → 04 跟进度 → 05 验收复盘**

每一步按任务规模自动调整。负责人保留重大决策，AI负责整理、提醒和草案，成员贡献对应真实产物。

## 立即安装

### A. Codex 等支持 Agent Skills 的工具

**方式1：通过 Skill Installer**

在 Codex 中调用 `$skill-installer`，给它下面的指令：

```text
请从这个 GitHub 目录安装 LeadFlow Skill：
https://github.com/cclia26/leadflow-skill/tree/main/skills/leadflow-coordinator
```

**方式2：手动复制**

1. 点击 GitHub 页面的 **Code → Download ZIP**，解压。
2. 将 `skills/leadflow-coordinator/` 文件夹整体复制到自己的 Skills 目录。
3. 例如 Codex 的个人目录：`~/.agents/skills/leadflow-coordinator/`。
4. 打开 AI 工具，尝试：`用 leadflow-coordinator 帮我安排一场 90 分钟的团队活动。`

不同工具的 Skills 目录与安装方式可能不同，详情请看 [安装与使用说明](docs/GETTING_STARTED.md)。

### B. 暂时没有 Skill 环境

可以联系分享这份 Skill 的伙伴获取安装教程或单句 Prompt。单句 Prompt 适合快速体验；完整 Skill 还包含工作规则、模板和案例，适合持续处理多人任务。

## 一分钟尝试

复制你的实际任务通知，输入：

```text
请使用 leadflow-coordinator 的「启动」模式处理这份任务。
我们有 10 位成员，要在周六前组织一场 90 分钟的新成员活动。
请先确定交付目标，再按成员可用时间拆分任务，给出保底方案和群通知。
```

如果你正在推进已有任务，可以改成：

```text
LeadFlow 推进：目前海报已交、主持稿还没定，明天 18:00 截止。
请告诉我最先处理什么，以及应该怎样通知大家。
```

## 项目结构

```text
leadflow-skill/
├─ README.md
├─ LICENSE
├─ CHANGELOG.md
├─ docs/
│  └─ GETTING_STARTED.md
└─ skills/
   └─ leadflow-coordinator/
      ├─ SKILL.md                     ← 主技能
      └─ references/
         ├─ templates.md              ← 任务卡 / 分工表 / 通知模板
         ├─ examples.md               ← 社团 / 招募 / 跨专业示例
         └─ case-beichen-group1.md    ← 真实协作案例
```

## 来源：第1组的一次真实共创

这套工作流提炼自北辰青年第四期第1组的 2026 年 11 月实践：32 人团队，22 份问卷，19 份倾向交互网站；以产品共创和网站展示为最终载体，通过分工协作完成两款交互原型与一处正式网站。

公开案例只保留协作方法和可核实成果，详见 [真实案例](skills/leadflow-coordinator/references/case-beichen-group1.md)。

## 提供反馈

欢迎通过 **GitHub Issues** 分享使用场景、改进建议和可公开的案例。欢迎 Fork 后提出 Pull Request。提交公开案例时请自行处理隐私与素材许可。

如果这份 Skill 帮你更轻松地带队，欢迎点一下右上角 **Star ⭐**，让更多需要组织活动的人找到它。

## License

MIT License。详见 [LICENSE](LICENSE)。
