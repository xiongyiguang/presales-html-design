---
name: presales-html-design
description: "把已有售前方案或汇报内容制作为一屏一页、可翻页的单文件 HTML 演示。用于分页演示制作与改版；不用于连续长页、通用网站或方案内容策划。"
license: Complete terms in LICENSE.txt
---

# Presales HTML Design

把已提供或已核验的内容转换为分页式 HTML 演示；正文可来自任意已确认来源，不强制先调用内容生成技能。连续阅读长页和交互工作台由 `technical-editorial-web` 负责；PPTX 交付另选对应制作技能。

## macOS 执行说明

- 技能目录内的参考、模板和素材使用相对路径；输出按当前项目或应用的目录约定保存。旧说明中的 Windows 开发路径仅作历史示例，不作为 Mac 的工作路径。
- 需要 Python/Node 时，先通过 `load_workspace_dependencies` 获取当前应用捆绑运行时，不假定系统 `python`、`python3` 或 `node` 已安装。使用当前可用浏览器工具核验最终文件；静态校验不替代实际页面和交互检查。
- HTML 运行与 QA 从本机 HTTP 服务打开，检查后保留可移植文件；客户交付不能依赖这个测试服务。字体使用现有系统字体回退，检查中文实际换行。

## 核心合同

- 来源是事实边界。客户/项目/产品名、数字、状态、条件、责任和披露限制保持原意与原名；不编造案例、Logo 或承诺。
- 制作时先建立章节→页面→保护词/事实块映射，覆盖每个一级章节；内容过密时增加续页，不缩字或悄悄删去关键事实。
- 默认自包含单 HTML，CSS/JS 内联，使用内联 SVG；无字体、图片、框架、CDN 或其他外部运行依赖。
- 一次显示一个直接子 section 页面，稳定页框/页码/品牌导航；支持键盘、单页滚轮、触摸、锚点和 hash。尊重输入控件、焦点与 reduced motion；打印展开全部页面。
- 正文基线 16px，所有可见字不小于 14px，主标题不大于 60px。桌面页不裁切、不内部滚动；移动端按运行规范适配。
- 默认 Richinfo Executive Technical Brief；用户明确样式优先，选定品牌后不混用其他品牌，不因行业或客户名自行换色。

## 制作与读取路由

1. 来源映射/摘要/全文覆盖：读 [source-and-page-mapping](references/source-and-page-mapping.md)。仅做局部视觉调整时沿用已有核验映射，核对受影响内容。
2. 新建或整体改版：读 [default-visual-style](references/default-visual-style.md) 和 [visual-seed-selection](references/visual-seed-selection.md)，选一个主种子；按 [design-review](references/design-review.md) 确定开场与逐页构图理由，复核简短草图后编码。只查看被选中的 HTML 种子，不把样例章节和业务文字带入交付。
3. 新建或修改交互：读 [paged-presentation-runtime](references/paged-presentation-runtime.md)。局部改字不需重新加载未变更的交互细节。
4. 品牌、导航、主视觉或架构图：读 [visual-and-acceptance](references/visual-and-acceptance.md) 对应小节。来源明确有层次时保留层名和能力项，使用分层架构图。
5. 按真实信息关系组织页面，不重复卡片墙，也不按数量轮换版式。同类证据或对比页面可以保持一致结构；开场可用结论、机制、证据、比较或真实路径，服从会议目标与来源。用页面主旨、结构、证据与留白形成层次，直接写客户结论。
6. 交付时执行 [visual-and-acceptance](references/visual-and-acceptance.md) 的 Final Check 和运行参考的验收，按设计计划对照整体截图和阅读尺寸，验证实际最终文件在 1440×900、1366×768 与移动尺寸下的内容覆盖、溢出和导航。局部修改检查影响页，共用样式/交互变化检查所有受影响页面。

输出放入当前项目约定的正式交付目录，映射与检查证据进入 docs/.staging。没有实际渲染或操作验证时说明未验证范围，不把静态结构检查当浏览器验收。
