我想改 PRD，有以下几处：

## 改动清单

### 1. [Level 1] Technical Approach
- 现状：有techical approach
- 想改成：移走
- 原因：目前只是产品的决策，不涉及到技术，技术的再写TECHNICAL_DESIGN.md

### 2. [Level 2] TLDR
- 现状： 一次生成双语两份 MD 文件
- 想改方向： 默认生成原本语言，可以选择生成中文的
- 原因：有些时候不用双语的

### 2. [Level 2] Requirements的PDF 转 Markdown
- 现状：把日文 Markdown 保存为文件（文件名格式：{原文件名}.ja.md）
- 想改方向：保存路径可以指定到本地，或者是直接下载
- 原因：有些固定的路径想保存起来，不用反复放

### 2. [Level 3] Requirements的PDF 转 Markdown
- 现状：[ ] 在日文 MD 预览下方提供「翻译为中文」按钮
[ ] 点击后调用 Claude，将日文 MD 翻译成中文 MD
[ ] 翻译完成后在界面显示中文 MD 预览
[ ] 把中文 MD 保存为文件（{原文件名}.zh.md）
[ ] 未点击按钮时，工具不发起任何外部网络请求
- 想改方向：翻译成中文不用preview,只有原文的才用preview，希望是在下载或者保存的时候才选要不要保存成中文，那个时候才保存

### 3. [Level 3] Open Questions
- 现状：翻译用 Anthropic API 直调 vs 复用 Claude Code 订阅？
- 想改成：复用 Claude Code 订阅，因为我目前没有api的
- 原因：因为我目前没有api的权限，只有cli的，这个技术上怎么实现还需要再讨论，先出prd

## 问题：
- 不上传任何遥测 / 日志 / 崩溃数据 是什么意思

## 最后一句
请先告诉我：这些改动有没有互相矛盾？有没有我没想到的级联影响？