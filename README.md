# TheBlue · 美观的蓝色系Typora主题

**适用于Typora的蓝色系主题，由[Pink Hsiao](https://github.com/HsiaoDeepie/typora-theme-pink-hsiao)与[Drake](https://github.com/liangjingkanji/DrakeTyporaTheme)主题改编重构。**

**专为长文写作与PDF导出优化，支持鸿蒙黑体与连字代码字体，让你的Markdown编辑界面焕然一新。**



## 样式预览

![StylePreview](https://github.com/CMOS4000/TheBlue/blob/main/img/StylePreview.webp)



## 主题特点

- **美观大方：**采用美观整洁的蓝色系主题，使用多重渐变蓝色渲染不同等级标题，清晰明了，易于分辨。对每种正文变体采用恰到好处的颜色区分，适合长文写作与办公。
- **精致优雅：**对不同字块（如代码块、公式块、图片、表格）应用适当的圆角、阴影与边框，提升精致感与辨识度的同时不会过分打扰。
- **字体舒适：**正文使用[**鸿蒙黑体**](https://developer.huawei.com/images/download/general/HarmonyOS-Sans.zip)，代码块使用[**Maple Mono NF CN**](https://github.com/subframe7536/maple-font/releases/download/v7.9/MapleMono-NF-CN-unhinted.zip)，无论显示器规格都能获得较好的预览体验。外挂WOFF2字体包可开箱即用，但更建议自行安装为系统字体。
- **比例协调：**专门优化放缩功能，虽然默认16px字号显示最佳，但在Typora中无论改变页面比例还是调整字号都不会造成明显的结构错位。
- **打印友好：**优化打印功能，规定各结构标准比例，在Typora中设定页边距后（建议上下边距12，左右边距8），直接导出即可获得一份精美的PDF。特别修复了大部分主题存在的代码块跨页毛边问题、错位问题、公式放缩问题、截断问题。
- **参数易调：**将大部分参数（如主题颜色、结构尺寸、排版位置）作为变量提取到root{}中，用户或开发者可快捷手动调整。将CSS模块化，变量名称语义化，并增加大量注释，主题定制一目了然。



## 调参辅助

如图所示，CSS文件的root{}中配置了大量变量，并进行了参数对齐，附带详细的注释。

![Parameter](https://github.com/CMOS4000/TheBlue/blob/main/img/Parameter.webp)

变量语义化命名遵循规范如下所示。

> **--[scope]-[role]-[property]**

- **scope：**作用域/结构（如theme、font、layout、 spacing、 border、 code）
- **role：**语义/用途（如primary、 h1、 write、 block）
- **property：**属性名（如color、 size、 width、 radius）



## 设计理念

TheBlue设计初衷是为了寻找一份美观、大方、高效、适合办公的Typora主题。

TheBlue最初为[**Pink Hsiao**](https://github.com/HsiaoDeepie/typora-theme-pink-hsiao)框架与[**Drake**](https://github.com/liangjingkanji/DrakeTyporaTheme)代码块的拼接，随后笔者对二者的融合体进行了彻底重构，提取变量并将其规范化以便测试，最终调整到较为合适的比例。

在测试过程中，笔者修复了大量原有的显示问题（比如标题装饰错位、复选框错位、代码块打印毛边等），并采用了更加灵活的CSS实现。

希望这个主题能为您的Typora锦上添花。



## 安装方式

### 方法一：开箱即用

1. 点击**Code——Download ZIP**，下载解压后找到`theblue.css`（样式文件）与`theblue`（外挂字体包）文件夹。
2. 打开Typora，进入**文件——偏好设置——外观——打开主题文件夹**。
3. 将样式文件与字体包放入主题文件夹，重启Typora，在**主题**选项卡中选择**theblue**。

### 方法二：安装字体（推荐）

1. 点击下载[**鸿蒙黑体**](https://developer.huawei.com/images/download/general/HarmonyOS-Sans.zip)（来自华为开发者官网）与[**Maple Mono NF CN**](https://github.com/subframe7536/maple-font/releases/download/v7.9/MapleMono-NF-CN-unhinted.zip)（来自Github），解压后找到所有字体文件并安装。
2. 仅将`theblue.css`（样式文件）放入主题文件夹，重启Typora后在**主题**选项卡中选择**theblue**。
3. 考虑到文件体积，字体包中的WOFF2文件进行了一定程度的压缩，而且外挂字体影响性能，所以更推荐安装字体后直接调用。