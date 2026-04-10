# LLM Wiki 安装指南

基于 Andrej Karpathy 的 LLM Wiki 模式搭建的个人知识库启动包。

## 文件说明

```
CLAUDE.md          ← Claude Code 的指令文件（自动读取）
raw/               ← 放你的原始资料（文章、论文等），LLM 只读不改
raw/assets/        ← 存放下载的图片附件
wiki/index.md      ← 知识库目录，每次 ingest 后自动更新
wiki/log.md        ← 操作日志，按时间记录所有操作
```

## 快速开始

详细的中文步骤请参考你和 Claude 的对话记录。

核心用法只有三个命令（在 Claude Code 中使用）：

1. **Ingest（摄入）**：把新文章放入 `raw/`，然后告诉 Claude Code "处理 raw/xxx.md"
2. **Query（查询）**：直接问 Claude Code 问题，它会搜索 wiki 并给出带引用的回答
3. **Lint（检查）**：让 Claude Code 检查 wiki 的健康状况，发现矛盾和缺失
