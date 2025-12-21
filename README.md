# PaperStudio - 打印纸设计工具

![PaperStudio](https://img.shields.io/badge/Status-Active-success) ![License](https://img.shields.io/badge/License-MIT-blue)

**PaperStudio** 是一个基于 Web 的轻量级信笺纸、稿纸设计工具。它允许用户通过简单的拖拽和配置，设计出符合传统书写习惯或现代商务风格的信纸，并支持导出为 PDF 或直接打印。

演示：https://jingguanzhang.github.io/PaperStudio/


项目采用单 HTML 文件架构（依赖少量静态资源），无需复杂的后端环境，即开即用。
<img width="1920" height="877" alt="QQ截图20251207180511" src="https://github.com/user-attachments/assets/f7e2364e-58be-4c85-b463-e009d2721275" />




## ✨ 主要特性

*   **📐 灵活的网格布局**：
    *   支持 A4, A3, B5, 16开 等多种标准纸张尺寸，亦可自定义尺寸。
    *   一键生成横线、方格稿纸。
    *   支持调节行数、线宽、颜色、虚线模式以及首尾行双线样式。
*   **🎨 丰富的绘图工具**：
    *   **文字编辑**：支持多种中文字体、字号、加粗/斜体/下划线、字间距与行高调整。
    *   **图形绘制**：内置矩形、圆形、三角形、五角星等矢量图形。
    *   **智能矩形**：支持调节圆角或斜角样式。
    *   **图片处理**：支持上传图片，并可一键设为背景（适合制作带水印的信纸）。
*   **🛠️ 高级编辑功能**：
    *   **图层管理**：直观的图层列表，支持锁定、隐藏、排序。
    *   **对齐与分布**：支持多选元素的左/中/右对齐，以及水平/垂直平均分布。
    *   **历史记录**：完善的撤销 (Undo) 和重做 (Redo) 功能。
*   **💾 存储与导出**：
    *   **工程保存**：可将设计保存为 `.paper` 项目文件，随时重新编辑。
    *   **高清导出**：支持导出高清图片或 PDF 文档。
    *   **直接打印**：优化的打印样式，所见即所得。

## 🚀 快速开始

### 1. 环境准备
本项目是一个纯静态 Web 项目。你只需要一个现代浏览器（Chrome, Edge, Firefox, Safari）即可运行。

### 2. 目录结构
确保你的目录结构如下，以便静态资源能正确加载：

```text
PaperStudio/
├── xfz.html              # 主程序入口
├── static/               # 静态资源文件夹
│   ├── fabric.min.js     # Canvas 操作库
│   ├── tailwindcss.js    # 样式库
│   ├── jspdf.umd.min.js  # PDF 导出库
│   ├── toastify-js.js    # 消息提示库
│   ├── icons.min.css     # 图标样式 (Phosphor Icons)
│   ├── hotkeys-js.min.js # 快捷键库
│   └── SourceHanSerifCN-Bold.ttf # 默认字体文件
```

### 3. 运行
直接双击打开 `xfz.html` 文件即可开始设计。

*推荐使用 VS Code 的 "Live Server" 插件运行，体验更佳。*

## ⌨️ 快捷键指南

| 按键组合 | 功能 | 备注 |
| :--- | :--- | :--- |
| `Ctrl` + `C` | 复制 | 画布内元素复制 |
| `Ctrl` + `V` | 粘贴 | 粘贴到画布 |
| `Ctrl` + `Z` | 撤销 | 回退上一步操作 |
| `Ctrl` + `Y` | 重做 | 恢复下一步操作 |
| `Ctrl` + `S` | 保存 | 保存为 .paper 项目文件 |
| `Ctrl` + `O` | 打开 | 打开 .paper 项目文件 |
| `Ctrl` + `P` | 打印 | 调用浏览器打印 |
| `Delete` | 删除 | 删除选中元素 |
| `Alt` + 拖动 | 平移画布 | 抓手模式 |
| `Shift` + 点击 | 多选 | 选择多个元素 |
| 方向键 (`↑` `↓` `←` `→`) | 微调 | 每次移动 2px |

## 🛠️ 技术栈

*   **HTML5 / CSS3**: 基础结构与样式。
*   **TailwindCSS**: 实用优先的 CSS 框架 (CDN/Script 引入)。
*   **Fabric.js**: 强大的 HTML5 Canvas 库，处理图形交互的核心。
*   **jsPDF**: 用于生成 PDF 文件。
*   **Toastify**: 轻量级的通知提示。

## 🤝 贡献

欢迎提交 Issue 或 Pull Request！

1.  Fork 本仓库。
2.  新建 Feat_xxx 分支。
3.  提交代码。
4.  新建 Pull Request。

## 📄 开源协议

本项目基于 [MIT License](LICENSE) 开源。您可以免费用于个人或商业用途，但请保留原作者版权声明。
