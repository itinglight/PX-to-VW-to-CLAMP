# ✨ PX-to-VW-to-CLAMP Pro

[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/itinglight/px-to-vw-clamp?style=social)](https://github.com/itinglight/px-to-vw-clamp)

一个为现代前端开发者设计的简洁高效工具。它将传统的 **PX** 像素值，实时转换为 **VW** 视口单位，并根据可配置的缩放比例，自动生成**带有最小/最大限制**的 **CSS `clamp()` 函数表达式**。

本项目基于纯 HTML, Tailwind CSS (通过 CDN), 和 Vanilla JavaScript 实现，无需构建依赖，即开即用，方便部署和本地调试。

## 🚀 核心功能与特点

* **📏 实时三向转换:**
    * **PX** → **VW**
    * **PX** → **CLAMP(min, preferred (VW), max (PX))**
* **⚙️ 可配置参数:**
    * **设计稿宽度:** 用户可自定义设计稿宽度（默认 1920px），并自动保存至本地存储。
    * **CLAMP 最小缩放比例:** 可设置 `clamp()` 函数中最小尺寸相对于原始 PX 的比例（默认 80%）。
* **🎨 主题切换:** 支持一键在 **浅色 (Light)** 和 **暗色 (Dark)** 主题间切换，并记住用户选择。
* **📋 常用尺寸列表:** 列出常用 PX 值的 VW 和 CLAMP 转换结果，支持响应式多列展示。
* **🖱️ 一键复制:** 所有计算结果和列表项均可点击，一键复制到剪贴板，并带有友好的顶部居中提示。

## 🛠️ 技术栈

* **HTML5:** 页面结构
* **Tailwind CSS (CDN):** 快速、实用优先的 CSS 框架
* **DaisyUI (CDN):** 基于 Tailwind CSS 的组件库，提供美观的 UI 组件和主题支持。
* **Vanilla JavaScript:** 实现核心计算逻辑、本地存储和交互功能。

## 💻 本地运行

由于本项目是纯 HTML/CSS/JS，运行非常简单：

1.  克隆仓库到本地：
    ```bash
    git clone [https://github.com/itinglight/px-to-vw-clamp.git](https://github.com/itinglight/px-to-vw-clamp.git)
    cd px-to-vw-clamp
    ```
2.  直接用任何现代浏览器打开根目录下的 `index.html` 文件即可。

## 💡 为什么使用 CLAMP？

`clamp(MIN, PREFERRED, MAX)` 是 CSS 提供的强大函数，它解决了纯 VW 缩放的两个主要问题：

1.  **最小限制 (MIN):** 防止在小屏幕上字体或元素尺寸变得过小，影响可读性。
2.  **最大限制 (MAX):** 防止在大屏幕上尺寸变得过大，影响美观和布局。

本项目生成的 CLAMP 表达式为您提供了一个完美的**流体排版**解决方案。

## 🤝 贡献

欢迎所有形式的贡献！无论是新功能建议、Bug 修复还是文档改进，都非常感谢。

1.  **Fork** 本仓库。
2.  创建您的特性分支 (`git checkout -b feature/AmazingFeature`)。
3.  提交您的修改 (`git commit -m 'Add some AmazingFeature'`)。
4.  推送到分支 (`git push origin feature/AmazingFeature`)。
5.  打开 Pull Request。

## 📄 许可证

本项目采用 MIT 许可证。详见 [LICENSE](LICENSE) 文件。

## 👨‍💻 作者

**itinglight**

* [GitHub 主页](https://github.com/itinglight) 