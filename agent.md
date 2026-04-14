# AGENT 文档

## 项目目标

此项目为一个问答答题结果查看器，面向人工智能代理读取和理解项目结构。它主要包含静态前端页面，用于通过记录 ID 查询并展示答题数据。

## 主要功能

- 输入答题记录 ID。
- 调用后端 API 获取答题数据。
- 渲染用户信息、答题 ID、题目内容、选项结果和文本答案。
- 支持不同题型展示（单选、填空、问答、多选）。

## 关键入口文件

- `qa_answer_viewer.html`：基础问答结果展示。
- `qa_answer_viewer1.html`：更完整的问答结果展示页面，包含导航栏和卡片布局。
- `test.html`：测试页面，演示如何使用 POST 请求获取接口数据。

## 数据源

- 主要 API: `https://xlab.ai-space.net/api/activity/getAnwserInfo/{id}`
- 接口返回 JSON 数据，关键字段：
  - `payload.answer`：答题内容数组。
  - `payload.third_party_user`：用户信息。
  - `payload.answer_id`：答题记录 ID。
  - `payload.ended_at`：结束时间。
  - `payload.duration`：答题时长。

## AI 解析重点

- 如果需要提取项目用途，重点说明它是一个前端静态展示项目。
- 页面逻辑集中在 `fetchAnswer()` 和 `renderAnswer()`（或类似渲染函数）中。
- 没有复杂构建工具或依赖，项目可直接通过浏览器打开。

## 适用场景

- 作为问答系统数据查看工具。
- 作为前端静态页面示例，展示如何从接口获取并渲染 JSON 数据。
- 方便 AI 代理快速理解项目结构和入口文件位置。