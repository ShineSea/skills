# Web PPT Creator Skill

这是一个用于创建和修改网页 PPT 的 Codex skill。它以 Reveal.js、HTML、CSS 和 JavaScript 交付可通过静态 HTTP 服务独立运行的 Web 演示文稿。Skill 使用渐进式加载：入口文件负责模式选择和硬性边界，任务相关的完整规范存放在 `references/`。

## Skill

- [`web-ppt-creator/SKILL.md`](web-ppt-creator/SKILL.md)：入口、输入路由、核心原则与交付要求
- [`web-ppt-creator/references/page-planning.md`](web-ppt-creator/references/page-planning.md)：怎么生成 PPT 页面规划稿（事实底稿、内容地图、内容充分性闸门）
- [`web-ppt-creator/references/ppt-design.md`](web-ppt-creator/references/ppt-design.md)：PPT 具体怎么做（创建/修改模式、逐页设计、Design System、动效、Reveal.js 实现）
- [`web-ppt-creator/references/acceptance.md`](web-ppt-creator/references/acceptance.md)：最终验收（验收步骤与验收标准）
- [`web-ppt-creator/agents/openai.yaml`](web-ppt-creator/agents/openai.yaml)：Codex UI 元数据与默认调用提示

## 使用方式

将 `web-ppt-creator` 目录安装到 Codex skills 目录，或从当前仓库路径加载该 skill。调用示例：

```text
使用 $web-ppt-creator 根据这份方案创建一套网页 PPT。
```

该 skill 只创建网页 PPT，不生成或导出 `.ppt`、`.pptx` 文件。
