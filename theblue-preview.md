---
title: "TheBlue 综合排版测试与效果预览"
author: "TheBlue Team"
date: 2026-10-06
description: 涵盖标准 Markdown 语法展示与复杂混叠兼容性压测的两用测试文档
---

# TheBlue 主题全元素排版预览与兼容性测试

> 本文档专为检验 **TheBlue** 在 **Typora**、**MarkFlowy** 与 **MarkText** 三大平台的视觉保真度与排版兼容性而设计。
> 全文结构分为两部分：
>
> * **第一节**：标准 Markdown 语法全特性展示，覆盖所有常用排版元素与样式；
> * **第二节**：高阶混叠与极限边界兼容性测试，检验多层嵌套、混叠渲染及跨容器表现。

---

# 第一节：标准 Markdown 语法规范展示

本节按照 CommonMark 及 GitHub Flavored Markdown (GFM) 规范，系统性呈现 TheBlue 主题的标准视觉样式。

## 1. 标题层级系统 (Headings)

TheBlue 对各级标题赋予了秩序井然的色彩阶梯与装饰边框：

# 一级主标题 (H1) · 页面居中设计

## 二级章节标题 (H2) · 沉稳纯黑实线装饰竖边

### 三级主要小节 (H3) · TheBlue 深蓝强调竖边 (`#1565c0`)

#### 四级功能小节 (H4) · TheBlue 核心亮蓝竖边 (`#007aff`)

##### 五级子项标题 (H5) · 清新浅蓝装饰竖边 (`#6ec0ff`)

###### 六级说明标题 (H6) · 极淡冰蓝装饰竖边 (`#b3e5fc`)

---

## 2. 正文段落与文本修饰 (Typography & Inline Elements)

正文采用 **HarmonyOS Sans SC** 字体驱动，设定 1.8 倍舒适阅读行高与自然段间距。

这是一个标准正文段落。文字渲染平滑舒适，无论在普通显示器还是高分屏上均具备清晰锐利的边缘呈现。长行文字具有恰当的换行折行保护，阅读节奏紧凑而不压抑。

### 行内修饰元素清单

* **粗体文本 (Bold / Strong)**：**优雅沉稳的加粗文字**，用于突出核心关键词。
* *斜体文本 (Italic / Em)*：*自然倾斜的强调文本*，符合西文及中文标点排版习惯。
* ***粗斜体组合 (Bold + Italic)***：***兼具字重与倾斜的双重强调文本***。
* ~~删除线文本 (Strikethrough)~~：~~已过时或待废弃的文字项~~，搭配高辨识度删除线。
* <u>下划线文本 (Underline)</u>：<u>带有平滑底部描边的文本</u>，用于特别标记。
* 行内代码 (Inline Code)：采用 `const theme = "TheBlue";` 微胶囊浅蓝底色与主题蓝文字。
* 高亮文本 (Mark / Highlight)：<mark>温润淡金底色的重点标记文本</mark>，温润柔和不刺眼。
* 键盘按键 (Keyboard Input)：请按下 <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd> 打开命令面板。
* 超链接文本 (Hyperlink)：[前往 TheBlue 官方仓库](https://github.com/CMOS4000/TheBlue)，呈现优雅紫罗兰色并在悬停时平滑转为高亮主题蓝。
* 脚注标注 (Footnote)：TheBlue 主题支持完善的文末脚注索引[^1]。

[^1]: 这里是脚注的具体说明内容：TheBlue 主题通过纯净本地系统字体提供零延迟渲染。

---

## 3. 列表系统 (Lists)

### 3.1 无序列表 (Unordered List)

* 统一主题色彩的项目符号：
    * 第二层嵌套列表项
        * 第三层嵌套列表项，层级清晰
        * 缩进尺度遵循 2rem 标准规范
    * 返回第二层项目

### 3.2 有序列表 (Ordered List)

1. 第一步：在系统中安装华为鸿蒙黑体与 Maple Mono NF CN 字体
2. 第二步：选择目标平台并将对应主题包导入：
    1. Typora 导入 `theblue-typora.css`
    2. MarkFlowy 导入 `theblue-markflowy.json`
    3. MarkText 导入 `theblue-marktext.css`

### 3.3 任务列表 (Task Lists / Todo)

- [x] 完成 MarkText Cadmium 浅色定制补丁与绿线叠印修复
- [ ] 导出全部平台的实时预览效果长截图

---

## 4. 引用块 (Blockquotes)

### 4.1 单层基础引用

> “简约而不简单，这是设计最高的追求。”
> 
> TheBlue 引用块左侧配有 4px 纯蓝边框（`#007aff`），底色采用 8% 极浅蓝底（`rgba(0, 122, 255, 0.08)`），为长段落带来平整柔和的阅读区隔。

### 4.2 多层渐进阶梯嵌套引用

> 一级引用块：基础淡蓝底色与经典主题蓝边框。
> 
> > 二级引用块：底色深度递进（16%），形成立体的纵深感与层次。
> > 
> > > 三级引用块：底色继续加深（25%），左侧装饰条整齐排布，色阶分明。
> > > 
> > > > 四级极限引用：底色（35%），依然保持出色的正文可读性。

---

## 5. 代码块 (Code Blocks)

代码块统一采用经典的 **IntelliJ Darcula** 深色底色（`#2b2b2b`），代码等宽字体优先选用 **Maple Mono NF CN**，支持清晰的语法着色与高反差白字反白选区。

### 5.1 TypeScript 示例

```typescript
interface ThemeConfig {
  name: string;
  version: string;
  platforms: ('Typora' | 'MarkFlowy' | 'MarkText')[];
  colors: {
    primary: string;
    background: string;
    selection: string;
  };
}

  public activateTheme(platform: ThemeConfig['platforms'][number]): void {
    console.log(`[TheBlue] Successfully loaded for ${platform}!`);
  }
}
```

### 5.2 Python 示例

```python
import math

def calculate_fibonacci_golden_ratio(n: int) -> float:
    """计算斐波那契数列并逼近黄金分割比"""
    if n <= 0:
        return 0.0
    a, b = 0, 1
    for _ in range(n):
        a, b = b, a + b
    ratio = b / a if a != 0 else 0.0
    print(f"Fibonacci({n}) = {b}, Approximated Ratio = {ratio:.6f}")
    return ratio

if __name__ == "__main__":
    calculate_fibonacci_golden_ratio(25)
```

### 5.3 CSS / 样式声明示例

```css
/* TheBlue 设计 Token 定义 */
:root {
  --theme-primary-color: #007aff;
  --theme-dark-color: #1565c0;
  --paper-background-color: #ffffff;
  --code-background-color: #2b2b2b;
  --font-sans-serif: "HarmonyOS Sans SC", sans-serif;
  --font-monospace: "Maple Mono NF CN", monospace;
}
```

---

## 6. 表格排版 (Tables)

TheBlue 表格表头采用浅蓝底色加强显示，支持精准的对齐方式与交替斑马纹。

| 组件分类 | 设计变量名 | 色值 / 规格 | 对齐方式 | 说明备注 |
| :---: | :---: | :---: | :---: | :---: |
| **主色调** | `--theme-primary-color` | `#007aff` | 居中 | 核心交互与强调色 |
| **深蓝强调** | `--theme-dark-color` | `#1565c0` | 居中 | H3 标题竖边色彩 |
| **浅蓝点缀** | `--theme-light-color` | `#6ec0ff` | 居中 | H5 标题竖边色彩 |
| **深色底色** | `--code-background-color` | `#2b2b2b` | 居中 | 经典 IntelliJ Darcula |
| **正文字体** | `--font-sans-serif` | HarmonyOS Sans SC | 左对齐 | 华为全场景黑体 |
| **代码字体** | `--font-monospace` | Maple Mono NF CN | 左对齐 | 带连字特性的 Nerd Font |

---

## 7. 数学公式 (Mathematics)

支持 KaTeX / MathJax 高精度数学排版：

### 7.1 行内公式

质能守恒方程 $E = mc^2$，欧拉恒等式 $e^{i\pi} + 1 = 0$，以及高斯积分 $\int_{-\infty}^{\infty} e^{-x^2} dx = \sqrt{\pi}$。

### 7.2 块级公式

麦克斯韦方程组微分形式：

$$
\begin{aligned}
\nabla \cdot \mathbf{E} &= \frac{\rho}{\varepsilon_0} \\
\nabla \cdot \mathbf{B} &= 0 \\
\nabla \times \mathbf{E} &= -\frac{\partial \mathbf{B}}{\partial t} \\
\nabla \times \mathbf{B} &= \mu_0 \left( \mathbf{J} + \varepsilon_0 \frac{\partial \mathbf{E}}{\partial t} \right)
\end{aligned}
$$

多元正态分布概率密度函数：

$$
f(\mathbf{x}) = \frac{1}{(2\pi)^{k/2} |\mathbf{\Sigma}|^{1/2}} \exp\left( -\frac{1}{2} (\mathbf{x} - \boldsymbol{\mu})^\top \mathbf{\Sigma}^{-1} (\mathbf{x} - \boldsymbol{\mu}) \right)
$$

---

## 8. 图片展示 (Images)

图片自动居中排布，保持适当视口比例与优雅的边缘表现：

![现代建筑立面与明暗几何光影](img/sample.jpg)

<center><em>图 1.1：现代建筑几何立面明暗光影展示示例</em></center>

---

# 第二节：高阶混叠与极限边界兼容性测试

本节专门汇集日常写作与专业技术文档中出现的**复合嵌套、跨容器混叠与极端边界场景**，用于严格检验 TheBlue 在各类 Markdown 渲染引擎下的鲁棒性与兼容表现。

## 1. 标题复合混叠测试

### 标题含行内代码、加粗与徽章：`git commit -m "feat: init"` 与 **Release v1.0.0**

### 包含行内公式的标题：求解薛定谔方程 $i\hbar \frac{\partial}{\partial t} \Psi(\mathbf{r}, t) = \hat{H} \Psi(\mathbf{r}, t)$ 的本征态

#### 包含超链接与删除线的标题：~~弃用草案~~ 改为 [正式规范文档](https://github.com/CMOS4000/TheBlue)

##### 包含高亮标记的标题：测试 <mark>标题内部的高亮标签</mark> 与 `Inline Code`

> **验证要点**：
>
> 1. 标题左侧装饰竖条高度是否随内部嵌套元素（如行内代码、公式、徽标）自适应拉伸？
> 2. 标题内的 `code` 字号是否保持等比缩放（0.85em），避免出现突兀字号断层？
> 3. 行内修饰是否破坏标题自身的单行居中或块级布局？

---

## 2. 引用块深度嵌套与复合容器

### 2.1 引用块内嵌套数学公式

> **经典热力学定律推导**：
>
> 在绝热可逆过程中，理想气体的状态方程满足：
>
> $$
> P V^\gamma = \text{常数}, \quad \text{其中 } \gamma = \frac{C_p}{C_v}
> $$
>
> 由此可推得熵变关系式：$\Delta S = \int \frac{\delta Q_{\text{rev}}}{T} = 0$。

### 2.2 引用块内嵌套多行代码块

> **核心架构逻辑说明**：
> 下方代码展示了引用块内部嵌套标准深色代码块的对比度表现：
>
> ```rust
> #[derive(Debug, Clone)]
> pub struct ThemeToken {
>     pub key: &'static str,
>     pub value: &'static str,
> }
>
> fn main() {
>     let primary = ThemeToken { key: "accent", value: "#007aff" };
>     println!("Loaded token: {:?}", primary);
> }
> ```
>
> 代码块背景应保持独立深色，不被外层浅蓝引用底色透色干扰。

### 2.3 引用块内嵌套任务列表与表格

> 待审核发布清单：
>
> - [x] 验证引用块内的任务勾选效果
> - [ ] 验证引用块内表格边框与背景融合度：
>
> | 检查维度 | 达标判定 | 状态 |
> | :--: | :---: | :---: |
> | 竖线对齐 | 垂直贯通 | PASS |
> | 文本对比度 | 符合 WCAG AA | PASS |

### 2.4 四级嵌套引用 + 行内代码“纯白微胶囊”反差检验

> 一级引用底色（8% 蓝）：测试 `const alpha = 0.08;` 微胶囊反差。
> > 二级引用底色（16% 蓝）：测试 `const alpha = 0.16;` 胶囊纯白底色。
> > > 三级引用底色（25% 蓝）：测试 `const alpha = 0.25;` 在深底上的可读性。
> > > > 四级极限引用（35% 蓝）：测试 `const alpha = 0.35;` 此时行内代码纯白底与深蓝字（`#0062cc`）依然对比鲜明。

---

## 3. 列表深度复合场景

### 3.1 列表中嵌套引用块与代码块

1. **第一阶段：环境准备**
    * 安装核心构建工具链与 Node 运行环境。

      > [!NOTE]
      > 这是一个嵌套在二级列表内部的说明引用块，左侧应保持恰当缩进，不向外侧列表突兀凸出。
2. **第二阶段：配置构建脚本**
    * 编写一键编译任务：

      ```bash
      # 构建并校验主题包
      pnpm install
      pnpm run build --platform=all
      ```
    * 产物将生成在输出目录。
3. **第三阶段：完成与校验**
   
    * 列表项继续正常计数递增，段落与代码块缩进保持对齐。

### 3.2 任务列表内混叠极限元素

- [x] 已完成：包含 `Inline Code`、[超链接](https://github.com/CMOS4000/TheBlue)、**粗体**与 *斜体* 的复合任务。
- [x] 已完成：包含行内数学公式 $\sum_{k=1}^n k^2 = \frac{n(n+1)(2n+1)}{6}$ 的已勾选任务（检查删除线是否穿透整个段落）。
- [ ] 待办项：测试 <mark>高亮文本</mark> 与 `npm run test:compat` 混排在未勾选任务项中的表现。
- [ ] 待办项：在任务列表中插入快捷键提示 <kbd>Alt</kbd> + <kbd>Enter</kbd> 与下标测试 $H_2O$。

---

## 4. 行内修饰极限混叠（高亮 × 代码 × 链接）

* **高亮与行内代码无缝交织**：
    * 普通代码：`npm install theblue`
    * 普通高亮：<mark>这是一段普通的淡金黄色背景高亮文字</mark>
    * 高亮包裹混合文本与代码：<mark>请在终端中执行 `npx create-theblue-app` 安装脚手架</mark>（**关键检验**：代码块两侧是否有黄边毛刺溢出？文字对比度是否达标？）
    * 高亮直接包裹纯行内代码：<mark>`const isPerfect = true;`</mark>（**关键检验**：代码底色透明化融入高亮，文字加深为深蓝 `#0050b3`，消除双重底色毛刺）
    * Markdown 扩展语法高亮包裹代码：==`const isPerfect = true;`==
* **粗体、斜体、删除线与链接多重叠合**：
    * **粗体中的 `code`**：**请重点关注 `options.enableHighDpi` 选项**
    * *斜体中的链接*：*[访问 TheBlue 迁移指南文档](https://github.com/CMOS4000/TheBlue)*
    * ~~删除线中的代码与链接~~：~~废弃的旧方法 `oldEngine.bootstrap()`，参见 [旧版说明](https://github.com)~~
    * ~~直接对数学公式施加删除线~~：~~$E = mc^2$~~ 与 ~~$\Delta S = \int \frac{\delta Q}{T}$~~（单根水平线居中贯穿）
    * <u>下划线中的加粗代码</u>：<u>**`critical_security_patch()`**</u>

---

## 5. 表格极限内容容纳测试

表格单元格内塞入复杂混合元素，检验换行、对齐与行高弹性：

| 状态 | 规范条目与技术代码 | 关键公式 / 表现指标 | 复合标签与操作 |
| :---: | :---: | :---: | :---: |
| ✅ | 规范 A：`@font-face` 纯系统调用 | $\lim_{x \to 0} \frac{\sin x}{x} = 1$ | **通过** · [查看](https://github.com) |
| ⚠️ | 规范 B：标题孤行控制与分页防截断 | `break-inside: avoid;` | <mark>注意边距</mark> |
| 🚀 | 规范 C：嵌套引用色标防溢出 | 阶梯色标 $L_n = 1\text{em} \times n$ | `PASS` <kbd>F12</kbd> |
| ❌ | 规范 D：旧式外挂字体包依赖 | ~~体积约 45MB `.woff2`~~ | **已废除** |

---

## 6. 打印与 PDF 导出分页边界压测 (`@media print`)

> **打印测试指导建议**：
>
> 1. 在各编辑器中选择 **文件 → 导出 → PDF** 或 **打印**；
> 2. 建议页面设置：纸张 **A4**，上下边距 **12mm**，左右边距 **8mm**；
> 3. **检验重点**：
>     * 下方各级标题是否在页面最底端孤立出现（应自动推入下一页顶部）；
>     * 代码块与表格是否被生硬腰斩切断；
>     * 背景色彩在导出 PDF 时是否平整不失真。

### 跨页压力占位块（模拟长内容自然分页）

```python
# 这是一个用于检验代码块跨页与打印防断裂保护的长代码块片段
class PrintOrphanStressTest:
    def __init__(self, document_name: str, margin_vertical: int = 12):
        self.doc_name = document_name
        self.margin_v = margin_vertical
        self.verified_rules = []

    def verify_page_break_rules(self) -> bool:
        self.verified_rules.append("heading: break-after avoid")
        self.verified_rules.append("fences: break-inside avoid")
        self.verified_rules.append("table: break-inside avoid")
        return len(self.verified_rules) == 3

    def print_summary(self):
        print(f"Document: {self.doc_name}")
        for idx, rule in enumerate(self.verified_rules, start=1):
            print(f"  {idx}. {rule}: OK")

test = PrintOrphanStressTest("TheBlue Compatibility Doc")
test.verify_page_break_rules()
test.print_summary()
```

---

<center><strong>🎉 恭喜！若本文档在您的编辑器中全部渲染正常且无错位，说明 TheBlue 主题已完美生效！</strong></center>
