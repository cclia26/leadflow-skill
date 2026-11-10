# LeadFlow 安装与上手

## 第一步：下载

打开本仓库，点击 **Code → Download ZIP**，解压。主技能文件位于 `skills/leadflow-coordinator/SKILL.md`。

## 第二步：安装到支持 Agent Skills 的工具

### Codex

**推荐：** 在 Codex 的对话中调用 `$skill-installer` 并提供以下目录：

```text
https://github.com/cclia26/leadflow-skill/tree/main/skills/leadflow-coordinator
```

**手动：** 将整个 `leadflow-coordinator` 目录放在：

- 个人使用：`~/.agents/skills/leadflow-coordinator/`
- 当前项目使用：`<项目根目录>/.agents/skills/leadflow-coordinator/`

当 Skill 没有立即出现在列表中时，重新加载会话或重启 Codex。

### 其他兼容 Agent Skills 的工具

各客户端的安装路径不同。选择工具官方文档所述的 Skills 文件夹，放入整个 `leadflow-coordinator` 目录，确保 `SKILL.md` 位于技能目录根部。

**注意：** 普通 ChatGPT 网页对话未必支持直接安装独立的 GitHub Skill。可使用支持 Skills 的客户端，或向分享者索取适合当前工具的教程和临时 Prompt。

## 第三步：尝试这些命令

```text
用 LeadFlow 启动模式帮我处理下面的活动通知。先输出本周交付目标、分工和群公告。
```

```text
LeadFlow 分工：我们有 7 位伙伴，3 人擅长写作，2 人会设计，2 人负责现场协调。周五交活动方案。
```

```text
LeadFlow 验收：这是我们已有的会议流程、海报和报名页面。帮我检查提交前最重要的几项。
```

## 常见问题

**我只有一个人也能用吗？** 可以。把“分工”理解成时间和工具的分配，Skill 会收缩规模。

**AI 会自动帮我通知组员吗？** 能生成通知。是否实际发送取决于你使用的 AI 工具是否连接消息服务、具备相应权限，并获得你的明确授权。

**只发一句 Prompt 可以吗？** 可以快速体验部分功能。Skill 包含完整流程、参考模板与示例，连续处理多轮协作任务时更便于保持一致。

**可以改成自己的社团版本吗？** 可以，参照 MIT 许可。建议保留工作流结构，用自己的组织制度调整验收标准和沟通语气。

## 使用时的小建议

- 先把真实任务要求原文发给 AI；不要只给自己二次概括的目标。
- 附上截止时间、已有材料和成员可用时间，安排会更准确。
- 真实完成状态始终以提交或验收凭据为准。
