# qqwj-answer

## 效果图

<img width="1618" height="1190" alt="image" src="https://github.com/user-attachments/assets/dffbacb0-7f1c-4ae5-baeb-86b6734f40ff" />

## 项目简介

`qqwj-answer` 是一个基于静态 HTML 的问答答题数据查看器。用户可以输入答题记录 ID，前端通过接口查询答题结果，并在页面上展示用户信息、答题内容及选项结果。

## 主要文件

- `qa_answer_viewer.html`：简洁版问答数据查看页面。
- `qa_answer_viewer1.html`：增强版问答数据查看页面，包含更丰富的页面布局和展示效果。
- `test.html`：示例调试页面，展示如何通过 POST 请求获取答题数据并渲染结果。
- `AGENT.md`：AI 阅读项目时的元信息说明。

## 使用说明

1. 直接打开 `qa_answer_viewer.html` 或 `qa_answer_viewer1.html`。
2. 在输入框中填写答题记录 ID，例如：`33cc555f-056f-4242-a97c-46f3e7d2016f`。
3. 点击“查询”按钮，页面将调用后端接口并呈现答题详情。

## 数据来源

页面中的查询请求使用以下 API：

- `https://xlab.ai-space.net/api/activity/getAnwserInfo/{id}`

该接口会返回包含 `payload.answer`、`payload.third_party_user` 等字段的答题数据，前端页面负责解析并展示这些信息。

## 注意事项

- 该项目仅包含前端静态页面，没有后端接口实现。
- 访问时需要网络可连通 `xlab.ai-space.net`。
- `test.html` 中展示了一个 POST 请求示例，可根据接口要求修改请求参数和请求头。

## 参考文档

查看 `AGENT.md`，获取适合 AI 解析的项目结构和目标说明。

