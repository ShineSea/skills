# Web PPT Creator Skill

这是一个用于创建和修改网页 PPT 的 Codex skill。它以 Reveal.js、HTML、CSS 和 JavaScript 交付可通过 HTTP 访问的 Web 演示文稿，并包含从源文档生成逐页 Markdown 大纲、内容设计、元素级动效以及渲染 QA 的完整要求。

## Skill

- [`web-ppt-creator/SKILL.md`](web-ppt-creator/SKILL.md)：完整提示词与工作流
- [`web-ppt-creator/agents/openai.yaml`](web-ppt-creator/agents/openai.yaml)：Codex UI 元数据与默认调用提示

## 使用方式

将 `web-ppt-creator` 目录安装到 Codex skills 目录，或从当前仓库路径加载该 skill。调用示例：

```text
使用 $web-ppt-creator 根据这份方案创建一套网页 PPT。
```

该 skill 只创建网页 PPT，不生成或导出 `.ppt`、`.pptx` 文件。
