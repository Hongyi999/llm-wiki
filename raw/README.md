将你的源文档（文章、论文、笔记、播客 transcripts 等）放在这个文件夹里。
LLM 会读取这些文件，但**永远不会修改文件内容**。

为了保持整洁，源文档按来源组织在子目录下，例如：

- `lenny-podcast/` — Lenny's Podcast 的 transcripts
- （未来可以添加：`paul-graham-essays/`, `hn-posts/`, `arxiv-papers/` 等）

LLM 在生成 wiki 页面时，会使用相对于 `raw/` 的路径来引用源文件，例如
`sources: [lenny-podcast/sean-ellis.md]`。

目录结构可以在用户明确要求下重新组织，但文件内容本身永远是不可变的。
