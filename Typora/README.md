# TheBlue for Typora

**美观、优雅、专为长文写作与 PDF 导出优化的蓝色系 Typora 主题**

---

## 目录文件说明

* `theblue-typora.css`：Typora 主题核心样式文件（最新全功能修订版）

---

## 主题特点

1. **色彩层次**：采用多重渐变蓝色渲染不同层级标题（H2~H6 彩色实线边框，H1 干净居中），清晰明了。
2. **渐进嵌套引用**：逐级嵌套引用块呈现立体感递进蓝底（0.08 → 0.16 → 0.25 → 0.35），内部行内代码采用纯白微胶囊反差排版。
3. **经典代码块**：IntelliJ Darcula（#2b2b2b）深色背景代码块，搭配 Maple Mono 等宽代码字体与高对比度反白选区。
4. **精细文字修饰**：
   * 行内代码与高亮混叠无缝融合，消除毛刺与黄边。
   * 标题内代码跟随标题字号等比缩放（0.85em）。
   * 任务列表勾选自动触发灰色删除线。
5. **打印/PDF 专属优化**：
   * 标题防孤行保护（严禁标题孤留在页尾）。
   * 代码块打印防白边填缝微调，杜绝跨页截断。
   * 建议导出 PDF 时页边距设置为：**上下 12mm，左右 8mm**。

---

## 安装方法

### 1. 安装系统字体（必须）
为获得最佳排版观感与字形清晰度，请确保本地系统已安装以下字体：
* **正文字体**：[华为鸿蒙黑体 (HarmonyOS Sans SC)](https://developer.huawei.com/images/download/general/HarmonyOS-Sans.zip)
* **等宽代码字体**：[Maple Mono NF CN 代码字体](https://github.com/subframe7536/maple-font/releases)

### 2. 安装主题文件
1. 打开 Typora，点击菜单栏：**文件 → 偏好设置 → 外观 → 打开主题文件夹**。
2. 将本目录下的 `theblue-typora.css` 文件复制到该主题文件夹中。
3. 重启 Typora，在菜单栏 **主题 (Themes)** 中选择 **theblue-typora** 即可生效。
