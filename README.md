# Research Review Writing Polish

面向研究型论文与综述型论文的 Codex skill。

这个仓库提供一套可直接复用的 skill 目录，用来做：

- 学术英文生成
- 论文段落改写与润色
- 综述段落综合表达
- 摘要压缩与扩写
- Methods / Results / Discussion / Conclusion 的结构化重写
- 基于中文笔记生成审慎、可投稿风格的英文表达

它的核心目标不是“帮你写得更花”，而是：

- 保留科学含义
- 提高逻辑和可读性
- 让段落更符合期刊论文功能
- 控制措辞强度，避免过度宣称
- 让审稿人更容易快速理解

## 方法论来源

本 skill 主要参考 Adrian Wallwork 的《English for Writing Research Papers》。

吸收的重点不是零散句式，而是整套论文写作方法论：

- 不同章节有不同功能，不能混写
- 论文表达首先服务于读者和审稿人
- 清晰、简洁、具体，比“复杂高级”更重要
- 创新点要靠证据和结构体现，不靠夸张形容词
- 文献综述和 review paper 要做综合，而不是堆 citation
- Results 要突出最重要的发现，而不是把表格重念一遍
- Discussion 要解释结果、联系文献、承认边界
- Conclusion 要提供 take-home message，而不是机械重复前文
- 最终润色要围绕 readability、consistency 和 reviewer trust

## 仓库结构

```text
research-review-writing-polish/
|-- SKILL.md
|-- README.md
|-- README.en.md
|-- .gitignore
|-- agents/
|   `-- openai.yaml
|-- references/
|   |-- section-patterns.md
|   |-- review-synthesis-patterns.md
|   |-- academic-tone-checklist.md
|   `-- revision-output-templates.md
`-- examples/
    `-- ...
```

## 各文件作用

### `SKILL.md`

主 skill 定义文件。

负责说明：

- 什么请求应该触发这个 skill
- 任务如何分类
- 哪些事情绝对不能做
- 不同章节应该如何处理
- 默认工作流和输出方式

### `references/section-patterns.md`

章节级写作模式库。

适合处理：

- Abstract
- Introduction
- Literature Review
- Review body
- Methods
- Results
- Discussion
- Conclusions

如果你的问题是“这一节应该怎么写、怎么组织、怎么不像另一节”，先看这个文件。

### `references/review-synthesis-patterns.md`

综述和文献综合写作规则。

适合处理：

- citation 堆砌
- 一篇一篇顺着讲
- 缺少归类、比较、综合
- 综述段落没有主线

如果你的问题是“怎么把文献笔记写成 review prose”，先看这个文件。

### `references/academic-tone-checklist.md`

学术语气和 reviewer-facing 终检清单。

重点检查：

- clarity
- concision
- precision
- contribution visibility
- evidential discipline
- readability
- consistency

如果你的问题是“语言不够像论文，或者太啰嗦、太虚、太满”，先看这个文件。

### `references/revision-output-templates.md`

不同任务的标准输出形状。

适合：

- 纯润色
- 结构重写
- 从要点扩写
- 摘要压缩
- 综述综合改写
- Methods / Results / Discussion / Conclusion 专项重写
- 翻译并润色

如果你想让 skill 输出更稳定、更像一个可复用工作流，先看这个文件。

## 适用场景

这个 skill 最适合你已经有以下材料之一的时候使用：

- 提纲
- 中文或英文草稿
- 文献阅读笔记
- 综述笔记
- 图表解释
- 小节初稿
- 需要压缩或重写的段落

## 不适合的场景

这个 skill 不负责：

- 检索论文
- 下载文献
- 核对引用真伪
- 联网事实核查
- 伪造实验、结果或引用
- 从零设计完整研究方案

## 安装方式

把整个目录放进 Codex 的 skills 目录即可：

```text
$CODEX_HOME/skills/research-review-writing-polish/
```

不要只复制 `SKILL.md`，因为这个 skill 依赖 `references/` 和 `agents/openai.yaml`。

## 快速使用

示例 1：引言润色

```text
Use $research-review-writing-polish to rewrite my introduction draft in more formal academic English without changing the scientific meaning.
```

示例 2：综述综合

```text
Use $research-review-writing-polish to turn my literature notes into a synthesis paragraph for a review paper rather than a paper-by-paper list.
```

示例 3：摘要压缩

```text
Use $research-review-writing-polish to condense this abstract to 200 words while preserving the contribution and limitations.
```

示例 4：中文材料生成英文 Discussion

```text
Use $research-review-writing-polish to generate an English Discussion from my Chinese notes, but keep the claims conservative and limitation-aware.
```

## examples 目录

`examples/` 里放的是可直接参考的输入/输出样例，帮助你理解这个 skill 更适合怎样的材料和怎样的产出。

当前示例覆盖：

- 从研究笔记生成 Discussion
- 从文献笔记生成综述综合段落
- 把过长摘要压缩到目标字数

## 语言说明

- GitHub 首页默认展示中文 `README.md`
- 英文版说明保留在 `README.en.md`

## 后续可扩展项

这个仓库当前先聚焦在 skill 主体，不额外加 license。

后续如果你要继续做成更完整的公开 skill，可以再补：

- `assets/`
- 更多 `examples/`
- 评测样例
- 一组针对具体期刊场景的 prompt recipes
