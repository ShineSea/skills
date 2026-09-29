# Web PPT Creator Skill

这是一个用于创建和修改网页 PPT 的 Codex skill。它以 Reveal.js、HTML、CSS 和 JavaScript 交付可通过静态 HTTP 服务独立运行的 Web 演示文稿。Skill 使用渐进式加载：入口文件负责模式选择和硬性边界，任务相关的完整规范存放在 `references/`。

## Skill

- [`web-ppt-creator/SKILL.md`](web-ppt-creator/SKILL.md)：入口、模式路由与核心约束
- [`web-ppt-creator/references/content-planning.md`](web-ppt-creator/references/content-planning.md)：内容权威与页面规划
- [`web-ppt-creator/references/visual-design.md`](web-ppt-creator/references/visual-design.md)：叙事、视觉系统与动效
- [`web-ppt-creator/references/implementation-delivery.md`](web-ppt-creator/references/implementation-delivery.md)：网页实现、静态构建与独立交付
- [`web-ppt-creator/references/qa-and-revision.md`](web-ppt-creator/references/qa-and-revision.md)：渲染 QA、修改范围与完成标准
- [`web-ppt-creator/agents/openai.yaml`](web-ppt-creator/agents/openai.yaml)：Codex UI 元数据与默认调用提示

## 使用方式

将 `web-ppt-creator` 目录安装到 Codex skills 目录，或从当前仓库路径加载该 skill。调用示例：

```text
使用 $web-ppt-creator 根据这份方案创建一套网页 PPT。
```

该 skill 只创建网页 PPT，不生成或导出 `.ppt`、`.pptx` 文件。
