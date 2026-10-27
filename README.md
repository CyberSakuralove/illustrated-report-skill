# Illustrated Report · 图文可读报告 Skill

把项目、研究、实验或机制说明整理成能连续读懂的图文报告。重点是让输入、符号、公式、状态和结论接得上，而不是规定报告必须长成哪一种版式。

## 先看效果

[Transformer 原理图解](https://github.com/CyberSakuralove/transformer-illustrated-guide) 是本 skill 的完整 demo：19 页中文报告，包含 PDF、离线 HTML、可编辑正文与 SVG、重建说明及原始资料入口。

这份 demo 经多轮读者审读后定稿。本仓库将其中反复暴露的问题整理成可迁移的规则，把检查工作前移到首稿交付前；它不代表任意新题材都能自动达到同一质量。

## 它解决什么问题

- 新概念从前文已有对象或计算步骤引出，交代为什么在这里需要它。
- 新符号说明来源、含义和用途，必要时说明形状、单位和计数口径；同一对象保持命名。
- 公式讲清结果用途、运算顺序与关键项的作用，复杂表达先从已知局部推起。
- 阶段、配置、局部与完整过程分清；循环中区分输出产生、下轮消费和状态更新。
- 按关系选择示意图、公式、时序或短表，减少重复文字，保留必要理由。
- 全文执行同一解释标准，并实际渲染检查最终文件。

题材、目录、页数、图表数量、是否举例、输出工具均按任务决定。无需为纯叙事材料另造符号，也无需为满足格式每页画图。

## 使用

将 [illustrated-report/](illustrated-report/) 整个目录放入所用 agent 的 skills 目录，保留 `SKILL.md`、`references/` 与 `agents/` 的相对结构。

可用自然语言指定任务，例如：

> 使用 illustrated-report，把这些材料写成给初学者看的图文报告。先交代输入输出和关键机制，重要符号就地说明，保持前后连续，交付 PDF 和可编辑源文件。

也可以明确指定读者、已有知识、材料范围、语言和文件格式。已有信息足够时直接制作；缺口会改变范围或结论时再澄清。

## 内容

| 文件 | 用途 |
| --- | --- |
| [SKILL.md](illustrated-report/SKILL.md) | 可直接安装的通用规则和首稿闭环 |
| [解释与首稿检查](illustrated-report/references/explanation-review.md) | 复杂符号、状态与章节依赖的检查方法 |
| [图文组织模式](illustrated-report/references/layout-patterns.md) | 表达关系、图文分工和排版修正 |
| [制作与交付](illustrated-report/references/output-workflows.md) | 按输出格式组织源文件、渲染和交付 |
| [从初版到成品的复盘](docs/iteration-lessons.md) | 实际问题、对应规则及其泛化边界 |

本 skill 不绑定特定模型、付费服务、绘图库或报告模板。PDF、Word、HTML、Markdown 等格式使用当前环境适用的能力，事实与结论仍需依据材料核对。
