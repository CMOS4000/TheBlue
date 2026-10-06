# TheBlue for MarkFlowy

**严格遵循 MarkFlowy 1.0.0 自定义主题规范打造的生产级双模主题（Light / Dark）**

---

## 目录文件说明

* `theblue-markflowy.json`：**MarkFlowy 官方规范主题包**（开箱即用，已集成浅色与暗色全量样式及 61 个设计 Token）

---

## 核心设计与引擎适配

MarkFlowy 采用全新的 Tauri + WebView2 与 Capricorn 渲染器架构，TheBlue 针对其独特底层结构做了深度适配：

1. **浅色与暗色双变体一体化**：
   * 单一 JSON 文件同时包含 `TheBlue Light` 与 `TheBlue Dark` 两个主题变体。
   * 为外围 UI（标题栏、侧边栏、标签页、滚动条、交互焦点）定义了完整的 61 个官方语义 Token，无缝跟随系统深浅模式切换。
2. **扁平化多级引用阶梯渐变（解决色彩溢出）**：
   * 突破 Capricorn 扁平同级 DOM 限制，通过 `linear-gradient` 与 `repeating-linear-gradient` 复合分层背景，在 1em/2em/3em 边界精确控制色标，彻底杜绝外层深色背景向左溢出竖线的缺陷。
   * 引用块连续段落平滑接缝，首尾段落专属倒角，空行白隙彻底消除。
3. **任务列表穿透删除线**：
   * 借助现代 `:has()` 深度穿透选择器，实现勾选任务时精准渗透至 `.capricorn-markdown-list-content` 及内部叶子节点，文字自动变灰并显示 1.2px 删除线。
4. **数学公式排版加粗**：
   * 为 live-preview / MathJax SVG 设定了 `stroke-width: 0.35px` 专属描边加粗，消除公式相比正文字重偏细的问题。
5. **全选区深蓝高反差反白**：
   * 同时适配原生 `::selection` 与 Capricorn 自定义选区 API `::highlight(capricorn-selection)`，保证选中文本呈现深蓝底与纯白文字。
6. **打印与 PDF 导出保护 (@media print)**：
   * 覆盖所有 Capricorn 私有标题类名实现严格防孤行保护。
   * 代码编辑器、公式块、表格等块级元素全面启用 `break-inside: avoid`，严禁跨页截断。
7. **图片样式**：
   * 保持 MarkFlowy 原版响应式默认视觉，不强加额外圆角与投影，更贴合极简办公诉求。

---

## 安装方法

### 1. 安装系统字体（必须）
为保证最佳排版效果与连字特性，请确保本地系统已安装：
* **正文字体**：[华为鸿蒙黑体 (HarmonyOS Sans SC)](https://developer.huawei.com/images/download/general/HarmonyOS-Sans.zip)
* **等宽代码字体**：[Maple Mono NF CN 代码字体](https://github.com/subframe7536/maple-font/releases)

### 2. 导入主题
1. 打开 MarkFlowy 客户端。
2. 进入：**设置 → 扩展 → 自定义主题 (Custom Theme)**。
3. 点击 **导入主题 (Import Theme)**，选择本项目中的 `theblue-markflowy.json` 文件。
4. 导入成功后，在主题列表中启用 **TheBlue** 即可。
