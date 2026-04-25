# claude-code-report

![类型](https://img.shields.io/badge/%E7%B1%BB%E5%9E%8B-%E9%9D%99%E6%80%81%E6%8A%A5%E5%91%8A-2563eb)
![技术栈](https://img.shields.io/badge/%E6%8A%80%E6%9C%AF%E6%A0%88-HTML%20%7C%20CSS%20%7C%20JavaScript-0f766e)
![状态](https://img.shields.io/badge/%E7%8A%B6%E6%80%81-%E5%8F%AF%E7%9B%B4%E6%8E%A5%E9%98%85%E8%AF%BB-16a34a)
![README](https://img.shields.io/badge/README-%E4%B8%AD%E6%96%87-111827)

面向编程新手的 `Claude Code 源码解读` 静态 HTML 报告，用一页网页讲清 Claude Code 风格 CLI 的核心架构。

## 仓库定位

| 项目 | 说明 |
| --- | --- |
| 分类 | 技术报告 / 源码解读 / 静态网页 |
| 面向对象 | 想快速理解 Claude Code 架构、工具调用、权限和终端交互的新手或内部分享读者 |
| 产物形态 | 单文件 `index.html`，包含页面结构、样式和少量交互脚本 |
| 边界 | 本仓库不是应用源码，也不包含构建流水线；它只维护可直接打开的报告页 |

## 快速开始

直接在浏览器打开报告：

```bash
open index.html
```

或者在仓库根目录启动一个本地静态服务：

```bash
python3 -m http.server 8000
```

然后访问：

```text
http://localhost:8000
```

## 内容亮点

- 以中文解释 Claude Code 风格命令行工具的启动流程、消息循环和工具接口。
- 覆盖权限、记忆、hooks、终端渲染、安全设计和架构取舍等主题。
- 页面自带目录、卡片、代码块、图示和滚动交互。
- 字体组合使用 `Noto Sans SC`、`Inter` 和 `JetBrains Mono`，适合中文技术阅读。

## 项目结构

```text
.
├── README.md   # 仓库说明
└── index.html  # 静态中文报告页
```

## 技术说明

- `index.html` 内联 CSS custom properties、响应式布局和基础动画。
- 页面使用原生 JavaScript 实现目录导航、滚动状态和淡入效果。
- 外部字体通过 Google Fonts 加载；离线环境下会回退到系统字体。

## 维护备注

- 更新报告内容时只需要编辑 `index.html`。
- 如果要发布到静态站点，可以直接托管仓库根目录或单独上传 `index.html`。
- 当前仓库没有测试、打包或部署脚本；请不要假设存在额外运行时。
