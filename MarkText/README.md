# TheBlue for MarkText

**基于 MarkText 官方默认 Cadmium（浅色）主题深度定制与修补的 TheBlue 主题**

---

## 目录文件说明

* `theblue-marktext.css`：MarkText 官方“自定义CSS”专用全量样式包（开箱即用，融合编辑与导出全特性）
* `theblue-marktext.editor.css`：MarkText 编辑界面（Muya 编辑引擎）实时渲染样式补丁
* `theblue-marktext.theme.css`：MarkText 预览区、HTML 导出与 PDF/打印排版样式补丁

---

## 核心设计与定制说明

由于 MarkText 官方自定义主题加载机制尚不完全完善，本主题采取**“精准补丁定制”**策略，在保持官方默认 Cadmium 浅色主题稳定性的同时注入 TheBlue 灵魂：

1. **字体与排版**：
   * 正文采用 HarmonyOS Sans SC（行高 1.8），代码采用 Maple Mono NF CN。
   * H1 干净居中，H2~H6 呈现 TheBlue 标志性 5px 彩色实线装饰竖边。
2. **专属引用块美化与缺陷修复**：
   * 采用 4px 主题蓝竖线边框与 8% 浅蓝底色。
   * **核心缺陷修复**：彻底屏蔽了 MarkText Cadmium 原生绘制的绿色伪元素线条（`blockquote::before`），消除绿线与蓝线错位叠印的 Bug。
   * 引用块内部行内代码采用纯白微胶囊反差排版。
3. **原生悬浮工具栏严格隔离**：
   * 保护 MarkText 的 `.mu-inline-format-toolbar` 快捷格式浮窗与取色器，确保弹窗内部按钮样式与布局不被全局样式污染。
4. **表格智能排版**：
   * 独立成段的表格自动水平居中。
   * 嵌套在列表和引用块内的表格自动保持左对齐缩进，版面层次分明。
5. **IntelliJ Darcula 代码块**：
   * 代码块深色背景（#2b2b2b）搭配 IntelliJ 经典语法着色，选区高对比度反白。
6. **导出与打印保真 (@media print)**：
   * 严格防止标题孤行与代码块截断，保留高保真色彩。

---

## 安装与使用方法

### 1. 安装系统字体（必须）
为保证最佳排版效果与连字特性，请确保本地系统已安装：
* **正文字体**：[华为鸿蒙黑体 (HarmonyOS Sans SC)](https://developer.huawei.com/images/download/general/HarmonyOS-Sans.zip)
* **等宽代码字体**：[Maple Mono NF CN 代码字体](https://github.com/subframe7536/maple-font/releases)

### 2. 应用主题样式
MarkText 支持通过将 CSS 追加/覆盖至官方内置主题的方式生效：

#### 推荐方式（最简便：通过偏好设置「自定义CSS」启用）：
1. 打开 MarkText 客户端，在 **文件 → 偏好设置 → 主题** 中选择 **Light**。
2. 将本目录下的 `theblue-marktext.css` 文件中所有内容复制并粘贴到下方的 **自定义CSS** 输入框中。
3. 重启 MarkText 即可生效。

#### 备选方式（手动覆盖 Cadmium 浅色主题文件）：
1. 找到 MarkText 的主题安装目录：
   * **Windows**：`%APPDATA%\marktext\themes\` 或安装目录下的 `resources\app\dist\themes\`
   * **macOS**：`~/Library/Application Support/marktext/themes/`
   * **Linux**：`~/.config/marktext/themes/`
2. 打开 `cadmium` 浅色主题目录（或新建名为 `theblue` 的主题文件夹）：
   * 将 `theblue-marktext.editor.css` 的内容重命名并应用为 `editor.css`；
   * 将 `theblue-marktext.theme.css` 的内容重命名并应用为 `theme.css`。
3. 重启 MarkText，在偏好设置或主题菜单中选择生效即可。
