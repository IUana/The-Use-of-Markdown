# The-Use-of-Markdown
### 0. 写 Markdown 的第零步

全角标点, 如 `，。？！（）【】：；“”`. 这些标点是不被 Markdown 所认可的, 也是无法转义的. 
应该用半角标点, 如 `,.?!()[]:;""`. 且每个半角标点在文本使用时加上后置空格, 符合英文标点的书写规范, 也更加美观.
在使用中文输入法时按下 `Ctrl` + `.(这是个句号)`, 切换标点的全角与半角. 这样即可中文输入+半角标点.

### 1. 标题 [数个 "#" + 空格 前置]

```
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```
标题会在目录与大纲分级显示, 可以跳转. 

### 2. 强调 [用 "**" 或 "__" 包围]

```
** Hello World!** 
__ Hello World!__
```
或者选中想要强调的文字按下 `Ctrl` + `B`. 

### 3. 斜体 [用 "*" 或 "_" 包围]

```
*再见了，所有的Evangenion* 
_再见了，所有的Evangenion_
```
或者选中想要强调的文字按下 `Ctrl` + `I`. 
(P.S. ***斜体并强调*** [用 "***" 或 "___" 包围])

### 4. 删除线 [用 "~~" 包围]

```
~~再见了，所有的Evangenion~~
```

### 5. *高亮 [用 "==" 包围]
**(此为扩展语法)**
```
==I like Pen, I like pencil.==
```

### 6. 代码 [用 "`" 包围]

```
`sudo rm -rf /*`
```

### 7. 代码块 [按三个 "`" 并敲回车]

````c
```
// 这里就可以开始输入你要的代码了
#include <stdio.h>
int mian()
{
    print（“Hello, world!\n"）;
    retrun O;
}
``` // (这三个"`"文本编辑器会帮你自动补全 一般不用手动输)
````
代码块里可以选择语言, 其会根据语言来自动高亮各个语句. 在选择语言后, ` ``` ` 会变为 ` ```` ` + `对应语言`.

### 8. 引用 [">" + 空格 前置]

```
> 20岁, 是学生.
> > 学生特有的清澈的愚蠢.
```
引用是可以嵌套的.

### 9. 无序列表 ["-" 或  "+" + 空格 前置]

```
- 一颗是枣树
+ 另一颗还是枣树
* (其实这种也可以, 不过由于在 Typora 中很难单个输入, 故不常用)
```
三种前置符都可以, 敲回车会自动补全, 可在 Typora 设置中调整补全的符号, 敲回车后按下 `Tab` 会缩进一级. 

### 10. 有序列表 [数字 + "." + 空格 前置]

```
我来这里就为了三件事:
1. 吃饭
2. 吃饭
3. 还是tm的吃饭!
```
敲回车会自动补全, 敲回车后按下 `Tab` 会缩进一级. 

### 11. *上标 [用 "^" 包围]
**(此为扩展语法)**

```
C语言中int的上限是 2^31^ - 1 = 2147483647
```

### 12. *下标 [用 "~" 包围]
**(此为扩展语法)**

```
H~2~O 是剧毒的!
```

### 13. *注释 ["[^]" 后置]
**(此为扩展语法)**

```
> 今日我们相聚于此, 是为了学习 Markdown 的使用, 它的教程对于全体「观众」而言, 值得足足两个硬币的支持鼓励![^1]

[^1]: 沃兹·基·硕德 改编自「公鸡」普契涅拉.
```

### 14. 链接 [常用 "[ ]" + "( )" 分别包围文本与链接]
**(文内跳转为扩展用法)**

```
[来看看我贫瘠的仓库罢](https://github.com/IUana)
[基础教程: 12. 下标](#12. 下标 [用 "~" 包围])
```
支持网页链接与文内跳转, 按住 `Ctrl` 并 `单击鼠标左键` 即可跳转.

### 15. 任务列表 ["- [ ]" + 空格 前置]

```
TodoList:
- [ ] 吃饭
- [ ] 睡觉
- [x] 打豆豆
```
用 `x` 代替 `[ ]` 中的空格来勾选任务列表. 在 Typora 中可以直接用鼠标左键单击勾选框.

### 16. 表格 [用 "|" 绘制表格边框]

```
| 学号 | 姓名  | 年龄 |
| :--- | :---: | ---: | (引号的位置代表着 左对齐, 居中, 右对齐)
|114514|田所|24|
|1919810|浩三|25|
```
第一行为表头, 并由第二行分割线决定对齐方式与长度, 第三行及之后即表格数据.

### 17. 图片 [直接拖进来或者复制粘贴]

```
![图片](图片的位置)
```

### 18. 分割线 [按三个 "*" 或 "-" 或 "_" 并敲回车]

```
***
--- 
___
// (其实按三个及以上都可以)
```
 `*` 与 `_` 均会自动补全,  `-` 最为方便.

### 19. Emoji表情 [":" 前置]
**(英文输入为扩展语法)**

```
:sweat_smile: 
:drooling_face:
:clown_face:
// (敲回车或者鼠标点击, 后置的":"一般不需要手动输)
```
对于其余普通的 Markdown 文本编辑器, 可以直接将 Emoji 表情复制进来, 这是直接**硬编码**的.
[全Emoji的网站](https://emojipedia.org/apple/).

## 🔥 进阶教程
### 1. 目录 [自动生成]

```
[TOC] (此为 Typora 特有的, 如本文档开头)
```
若使用 VS Code 搭配 Markdown All in One 扩展, 可在 VS Code 的`命令面板` (即 [VS Code Command Palette](https://code.visualstudio.com/docs/getstarted/userinterface#_command-palette)) 输入 `Create Table of Contents` 自动生成目录, 且可在扩展设置中细调目录参数.

### 2. 内联 HTML 代码 [用 "<> </>" 包围]

```
<div style="text-align:center">
  <font style="color:red">我不会 HTML 呜呜呜... 浇浇我</font>
</div>
<center>简单的文字居中</center>
<u>下划线...</u>
```

只要你会写, 你完全可以把 Markdown 当作 **HTML** 来写.
同时, `.md` 文件可以直接导出成一个网页.
下划线可以选中想要下划的文字按下 `Ctrl` + `U`. 

### 3. 内联 $\LaTeX$ 公式 [用 "$" 包围]
**(部分编译器会不识别部分符号)**

```
$\LaTeX$ 是最好用的论文排版语言! 不信你看!

$a^n+b^n=c^n$

$$
%\usepackage{unicode-math}
\displaystyle \ointctrclockwise\mathcal{D}[x(t)]
\sqrt{\frac{\displaystyle3\uppi^2-\sum_{q=0}^{\infty}(z+\hat L)^{q}
\exp(\symrm{i}q^2 \hbar x)}{\displaystyle (\symsfup{Tr}\symbfcal{A})
\left(\symbf\Lambda_{j_1j_2}^{i_1i_2}\Gamma_{i_1i_2}^{j_1j_2}
\hookrightarrow\vec D\cdot \symbf P \right)}}
=\underbrace{\widetilde{\left\langle \frac{\notin \emptyset}
{\varpi\alpha_{k\uparrow}}\middle\vert
\frac{\partial_\mu T_{\mu\nu}}{2}\right\rangle}}_{\mathrm{K}_3
\mathrm{Fe}(\mathrm{CN})_6} ,\forall z \in \mathbb{R}
$$
```

用 `$` 包围为单条公式, 按下两个 `$` 并敲回车即生成公式块.

E.G. 

$a^n+b^n=c^n$

$$
%\usepackage{unicode-math}
\displaystyle \ointctrclockwise\mathcal{D}[x(t)]
\sqrt{\frac{\displaystyle3\uppi^2-\sum_{q=0}^{\infty}(z+\hat L)^{q}
\exp(\symrm{i}q^2 \hbar x)}{\displaystyle (\symsfup{Tr}\symbfcal{A})
\left(\symbf\Lambda_{j_1j_2}^{i_1i_2}\Gamma_{i_1i_2}^{j_1j_2}
\hookrightarrow\vec D\cdot \symbf P \right)}}
=\underbrace{\widetilde{\left\langle \frac{\notin \emptyset}
{\varpi\alpha_{k\uparrow}}\middle\vert
\frac{\partial_\mu T_{\mu\nu}}{2}\right\rangle}}_{\mathrm{K}_3
\mathrm{Fe}(\mathrm{CN})_6} ,\forall z \in \mathbb{R}
$$

### 4. *网络图床

一个 Typora 搭配腾讯云COS/阿里云OSS图床的[例子](https://blog.csdn.net/guo_ridgepole/article/details/108257277).

### 5. *Typora 的常用快捷键

|          按键          |        效果        |          按键          |          效果          |
| :--------------------: | :----------------: | :--------------------: | :--------------------: |
|      `Ctrl` + `D`      |     选中当前词     |      `Ctrl` + `L`      |     选中当前句/行      |
|      `Ctrl` + `E`      |    选中当前区块    |      `Ctrl` + `F`      |      搜索当前选中      |
|      `Ctrl` + `B`      |    加粗当前选中    |      `Ctrl` + `H`      |      替换当前选中      |
|      `Ctrl` + `I`      |    倾斜当前选中    |      `Ctrl` + `U`      |      下划当前选中      |
|      `Ctrl` + `K`      | 将当前选中生成链接 |      `Ctrl` + `J`      | 滚动屏幕将选中滚至顶部 |
|      `Ctrl` + `W`      |    关闭当前窗口    |      `Ctrl` + `N`      |       打开新窗口       |
|      `Ctrl` + `O`      |      打开文件      |      `Ctrl` + `P`      |     搜索文件并打开     |
|    `Ctrl` + `回车`     |   表格下方插入行   |      `Ctrl` + `,`      |      打开偏好设置      |
|      `Ctrl` + `.`      | 切换全角/半角标点  |      `Ctrl` + `/`      |  切换正常/源代码视图   |
| `Ctrl` + `Shift` + `-` |    缩小视图缩放    | `Ctrl` + `Shift` + `+` |      放大视图缩放      |

还有一些不常用的/三键的快捷键不在此列出.

### 6. *Typora 的主题样式与检查元素

Markdown 在编译后约等于 HTML. 而 Typora 的正常视图就是编译后的 Markdown, 故Typora的主题样式本质就是 CSS 文件.

可以下载各种好看的主题给 Typora换上, 同时也可以自己调整对应的 CSS 文件, 或者自己手搓. 

在 Typora 设置中开启 `调试模式` 后即可在正常视图右击打开 `检查元素`, 在其中就可以完全将 Markdown 文件当成 HTML 来编辑.
