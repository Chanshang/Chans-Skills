# Chan's Skills

个人长期维护的 Agent Skills 集合。Skill 按 Codex 规范放在 .agents/skills/，可随仓库版本管理，并在此仓库中使用。

## 代码库理解与源码学习

| Skill | 用途 | 来源版本 | 许可证 |
|---|---|---|---|
| source-reading | 把大型仓库精读成带源码引用的章节、课程或 HTML 书 | UnknownObject777/chenhao-skills @ 0bd22fe | MIT，原始许可证随文件保存 |
| fireworks-open-eli5 | 将单个概念、模块、工程权衡或事故做成证据标注的离线 HTML 讲解 | UnknownObject777/chenhao-skills @ 0bd22fe | Apache-2.0 |
| codebase-explainer | 解析 Python、JS/TS、Go 导入关系，生成架构说明和交互式 HTML 依赖图 | milad-ahmd/agent-skills @ 81d4841 | MIT，原始许可证随文件保存 |
| how | 对指定模块、功能或流程做结构化架构讲解；复杂问题可分角度探索并综合 | poteto/how @ b1ef429 | MIT，原始许可证随文件保存 |

完整来源路径：
- https://github.com/UnknownObject777/chenhao-skills/tree/0bd22fe4fcb427e5da85204dc5db9daf96548828/source-reading
- https://github.com/UnknownObject777/chenhao-skills/tree/0bd22fe4fcb427e5da85204dc5db9daf96548828/fireworks-open-eli5
- https://github.com/milad-ahmd/agent-skills/tree/81d48414f0c413a32c97524b60386c463c85e6a7/skills/codebase-explainer
- https://github.com/poteto/how/tree/b1ef42969ea7a2bb50aa26c2480274828a0385e7/skills/how

## 安装说明

这些 Skill 同时保存在仓库的 .agents/skills/，并安装到本机 Codex 全局技能目录：
C:/Users/Administrator/.codex/skills/

仓库内版本用于追踪、复查和更新；全局副本用于在其他项目中调用。更新时先检查上游变更和许可证，再同步两处副本。

## 未复制的候选

[show-me](https://github.com/UnknownObject777/chenhao-skills/tree/main/show-me) 可按问题选择调用树、文件树、Mermaid 或 HTML 等视觉表达方式。不过源目录未发现独立许可证，本仓库只保留来源链接，不再分发其原始文件。

## 使用建议

先用 codebase-explainer 看模块和导入关系，再用 source-reading 选择一个真实问题逐章精读；对关键调用链用 fireworks-open-eli5 做可视化。需要快速解释单个模块或请求流程时，可直接使用 how。

代码图只表达静态分析能看到的关系。反射、依赖注入、运行时插件、HTTP/队列跨服务调用等内容仍需回到源码和测试核对。