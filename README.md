# obsidian-Plugin-localization

Obsidian 插件简体中文汉化仓库

## 项目说明

本项目用于收集和维护 Obsidian 社区插件的简体中文（zh-CN）语言文件，帮助中文用户更好地使用各类插件。

## 支持的插件

| 文件夹 | 插件名称 |
|--------|----------|
| copilot/ | Copilot |
| file-explorer-note-count/ | 文件资源管理器笔记计数 |
| file-order/ | 文件排序 |
| file-tree-alternative/ | 替代文件树 |
| obsidian-git/ | Obsidian Git |
| obsidian-hover-editor/ | 悬停编辑器 |
| quickadd/ | 快速添加 |

## 简体中文汉化说明

### 汉化文件位置

每个插件目录下应包含以下文件：

```
插件名称/
├── main.js          # 插件主文件(重点汉化文件)
└── translations/    # 语言文件目录（可选）
    └── zh-CN.json   # 简体中文翻译（可选）
```

### 汉化规范

1. **文件命名**：`main.js`，`zh-CN.json` 或 `zh-CN`（无扩展名）
2. **编码格式**：UTF-8
3. **术语一致性**：
   - Obsidian 官方术语保持统一
   - 常见词汇参考：[Obsidian 中文文档](https://publish.obsidian.md/help/zh)
4. **标点符号**：使用中文标点（全角）
5. **大小写**：保持与原文一致的专有名词大小写

### 常见翻译示例

| 英文 | 中文 |
|------|------|
| plugin | 插件 |
| setting | 设置 |
| command | 命令 |
| hotkey | 快捷键 |
| toggle | 切换 |
| enable/disable | 启用/禁用 |
| note | 笔记 |
| folder | 文件夹 |
| vault | 仓库 |
| workspace | 工作区 |

## 如何参与汉化

1. **Fork 本仓库**
2. **创建分支**：`git checkout -b translate-plugin-name`
3. **添加/修改汉化文件**
4. **提交更改**：`git commit -m "feat: add zh-CN translation for xxx"`
5. **创建 Pull Request**

### 汉化步骤

1. 找到目标插件的 `main.js` 文件
2. 查找所有需要翻译的字符串进行汉化。
3. 创建/编辑 `zh-CN.json` 文件（可选）
4. 遵循 JSON 格式：`"原字符串": "翻译字符串"`（可选）
5. 使用 `zh-CN` 作为语言代码注册翻译（可选）

## 目录结构

```
obsidian-Plugin-localization/
├── README.md           # 本说明文件
├── .gitignore          # Git 忽略配置
└── [插件名]/           # 各插件目录
    ├── main.js         # 插件主文件（主要）
    └── translations/   # 翻译目录（可选）
        └── zh-CN.json  # 简体中文文件（可选）
```

## 注意事项

- 插件更新后可能需要同步更新汉化文件
- 某些插件可能使用不同的翻译加载方式，请参考各插件的具体实现
- 建议使用 JSON 验证工具确保翻译文件格式正确

## 许可证

本项目采用 MIT 许可证。
