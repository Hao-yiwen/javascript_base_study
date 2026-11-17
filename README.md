# JavaScript 基础学习笔记

![HTML](https://img.shields.io/badge/HTML-静态页面-E34F26?logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-浏览器内联脚本-F7DF1E?logo=javascript&logoColor=black)
![示例](https://img.shields.io/badge/示例页面-149-2F6F4E)

按章节整理的浏览器端 JavaScript 学习记录。每个知识点是一个独立 HTML 文件，脚本写在页面里，用浏览器打开即可看效果。仓库里没有应用入口、包管理文件或构建脚本。

目录名与 Nicholas C. Zakas《JavaScript 高级程序设计》（第 3 版）的章节对应，目前收录第 3–16 章和第 20–22 章的练习。第 1、2、17、18、19 章以及第 23 章之后没有对应目录。这些页面是单独写的练习片段，不是该书的配套工程。

## 仓库里有什么

一共 148 个 `.html`、1 个 `.xhtml`、1 个文本夹具 `example.txt`。没有图片、样式表文件、JavaScript 模块或第三方库；页面也不引用外部脚本。

多数示例把结果打到控制台（`console.log`），少数使用 `alert`，Canvas 和表单类页面则直接画在页面上。不少页面的 `<title>` 仍是 `Title` 或 `Document`，主题以目录名和文件名为准。

| 章节目录 | 子目录与示例 |
| --- | --- |
| `第三章基本概念` | **变量**：`var` 作用域。**操作符**：按位取反、正负号、相等 / 不相等、逻辑非。**数据类型**：`typeof`、`Object`、字符串字面量、`String` / `toString`、`Number` 转换、`parseInt`、`parseFloat`、`hasOwnProperty`。**语句**：`for`、`switch`、`arguments`（文件名为 `argumnets.html`） |
| `第四章变量作用域和内存问题` | **基本类型和引用类型**：动态属性、复制变量值、传递参数、检测类型。**执行环境及作用域**：作用域链、延长作用域链、查询标识符、没有块级作用域 |
| `第五章引用类型` | **Object**：对象创建。**Array**：创建、`concat`、`slice`、`splice`、归并、迭代、重排序、检测数组。**Date**：创建日期 |
| `第六章面向对象的程序设计` | `创建对象/`：构造函数模式、原型模式、组合继承、构造函数里 `this` 的指向 |
| `第七章函数表达式` | **闭包**：闭包与变量、立即执行函数。**模仿块级作用域**：私有作用域。**私有方法** |
| `第八章BOM` | **window**：`frameset`、`iframe`、`screenLeft`、`setTimeout`、`alert` / `prompt` / `confirm`，以及配套页 `a.html`、`b.html`。**location**：查询串封装、跳转、`reload`。**navigator**：属性查看、`registerContentHandler`。**screen**、**history** |
| `第九章客户端检测` | `window` / `document` 查看、宿主方法检测（`isHostMethod`）、`document.all`。`4.检测浏览器 .html` 的脚本是空的 |
| `第十章DOM` | **Node** 关系。**Document**：文档信息、查找元素、`getElementsByName`、文档写入。**Element**：标签名、属性、创建元素。**Text**：`nodeValue`（文件名为 `1.nideValue.html`）、`createTextNode`、`normalize`、`splitText`。**DOM 操作**：动态插入脚本、动态插入样式（文件名为 `2.动态央视.html`） |
| `第十一章Dom扩展` | **选择符**：`querySelector`。**HTML5**：`getElementsByClassName`、焦点管理、`readyState`、插入标记。**专有扩展**：`children`、插入文本、滚动 |
| `第十二章DOM2和DOM3` | **DOM 变化**：特性检测、XHTML 中的 SVG（`2.xhtml实例.xhtml`）、`DocumentType`、节点比较、`isSameNode`（文件名为 `5.isSanmeNode.html`）、框架。**样式**：行内样式、`@import`、计算样式、样式表、元素尺寸、滚动尺寸。**遍历**：`NodeIterator` |
| `第十三章事件` | **事件流**：HTML 事件处理函数、作用域、`addEventListener` / `removeEventListener`、`this` 与 `event`、`preventDefault`、`stopPropagation`、`eventPhase`。**事件类型**：`load`、`resize`（文件名为 `2.reseze事件.html`）、`scroll`、鼠标、鼠标按钮、滚轮、键盘、`contextmenu`。**设备事件**：触摸 |
| `第十四章表单脚本` | **表单**：`submit`。**文本框**：取值、`change` / `focus`、`select`、过滤输入、自动切换焦点、约束验证、`checkValidity`。**选择框**：读取选项、在两个 `<select>` 之间移动选项。**富文本**：`iframe` 与 `contenteditable` |
| `第十五章使用canvas绘图` | **基本用法**：获取 2D 上下文、导出图像。**2D 上下文**：填充与描边、矩形。`3.画五角星.html` 里实际画的是圆、两根指针和文字「12」，没有五角星路径 |
| `第十六章脚本编程` | **跨文档消息**：`postMessage`（父页面 `1.postmessage.html`，子页面 `a.html`）。**拖放**：给放置目标监听 `dragover` / `dragenter` 并 `preventDefault`，没有 `drop` 处理 |
| `第二十章JSON` | `JSON.stringify` 与 `JSON.parse`（文件名为 `1.JSON.strafity.html`） |
| `第二十一章ajax` | `XMLHttpRequest`：`readyState`、GET、`FormData`、超时、`application/x-www-form-urlencoded`。同目录有响应夹具 `example.txt`，内容为 `adsadd`。后三个 POST 示例指向仓库里不存在的 PHP 地址，见下方说明 |
| `第二十二章高级技巧` | **高级函数**：`bind` 固定 `this`，以及用 `bind` 预置参数（文件名为柯里化）。**防篡改对象**：`Object.preventExtensions`、`Object.seal`；同目录的 `3.高级定时器.html` 演示的是 `setTimeout` 显示元素。**函数节流**：点击后用 `setTimeout` 延迟打印 |

## 技术栈

- HTML 页面，JavaScript 全部内联。脚本混用 `var` 与 `let`，没有 `type="module"`，也没有打包工具。
- 浏览器 API：DOM、BOM、事件、表单约束校验、Canvas 2D、`JSON`、`XMLHttpRequest`、`postMessage`。
- 无 npm / pnpm / yarn 依赖，仓库中没有 `package.json`。

## 目录结构

```text
.
├── 第三章基本概念/
├── 第四章变量作用域和内存问题/
├── 第五章引用类型/
├── 第六章面向对象的程序设计/
├── 第七章函数表达式/
├── 第八章BOM/
├── 第九章客户端检测/
├── 第十章DOM/
├── 第十一章Dom扩展/
├── 第十二章DOM2和DOM3/
├── 第十三章事件/
├── 第十四章表单脚本/
├── 第十五章使用canvas绘图/
├── 第十六章脚本编程/
├── 第二十章JSON/
├── 第二十一章ajax/
│   └── 1.ajax/
│       └── example.txt
└── 第二十二章高级技巧/
```

## 环境要求

- 一个支持 `let` 的现代桌面浏览器。打开开发者工具才能看到 `console.log` 的结果。
- 建议用本地静态服务器打开。直接双击 HTML（`file://`）可以看大部分控制台示例；`XMLHttpRequest` 在 `file://` 下会被浏览器拦截。
- 不需要安装 Node.js，也不需要执行安装依赖的命令。下面的静态服务使用 Python 3 标准库。

## 运行

在仓库根目录执行：

```bash
python3 -m http.server 8080
```

浏览器打开 <http://127.0.0.1:8080/>。页面是目录列表，点进章节文件夹，再打开具体的 HTML。目录名是中文，用列表里的链接即可，不必手写编码后的地址。

看控制台示例时，打开开发者工具的 Console。例如：

- `第三章基本概念/数据类型/typeof.html`：依次打印 `undefined`、`boolean`、`string`、`number`、`object`、`function`，以及 `typeof null` 的 `object`、`typeof NaN` 的 `number`。
- `第七章函数表达式/闭包/立即执行函数.html`：打印 `1`。
- `第二十章JSON/1.JSON.strafity.html`：打印 JSON 字符串，再打印 `JSON.parse` 得到的对象。
- `第二十一章ajax/1.ajax/1.readyState.html`：请求同目录的 `example.txt`，成功时打印 `adsadd`。
- `第十五章使用canvas绘图/2.2D上下文/3.画五角星.html`：图形画在 `<canvas>` 上，控制台没有输出。

本仓库在 Python 3.12.3 上用 `python3 -m http.server` 核对过：站点根路径、上述 HTML、`example.txt` 以及 XHTML 示例均返回 HTTP 200。又用 Chrome 无头模式打开了这几个页面，控制台输出与脚本一致，Canvas 页没有脚本异常。

## 阅读时注意

这些是学习过程中的草稿，文件名里的笔误保持原样。下面几处脚本不完整，打开后不能得到文件名所写的结果：

- `第九章客户端检测/4.检测浏览器 .html`：`<script>` 为空。
- `第九章客户端检测/2.属性检测.html`：调用 `isHostMethod(xhr, "open")`，但页面没有声明 `xhr`。
- `第九章客户端检测/3.用户代理字符串.html`：打印未声明的 `clientInformation`。
- `第二十一章ajax/1.ajax/2.get请求.html`：同步 GET `example.txt`，只把拼接后的 URL 打到控制台，没有读取响应。
- `第二十一章ajax/1.ajax/4.formDate.html`：向不存在的 `pdsadsad.php` 发送 `FormData`，页面上也没有 `id="user-info"` 的表单；`readyState` 的判断写成了赋值。
- `第二十一章ajax/1.ajax/5.超时限定.html`：设置了 `timeout`，但 `open()` 没有参数。
- `第二十一章ajax/1.ajax/x-www-form-erlencoded.html`：向不存在的 `postdasda.php` 发 POST，并调用了未定义的 `serialize`。
- `第十六章脚本编程/1.跨文档消息传递/a.html`：收到消息后调用了未定义的 `processMessage`。
- `第二十二章高级技巧/2.防篡改对象/2.密封的对象.html`：`Object.seal` 之后打印了未声明的 `per`。

`第八章BOM` 里的 `<frameset>`、`document.all`、`registerContentHandler` 属于旧接口，当前浏览器可能忽略或不再提供。

仓库中没有截图。

## 参考

- 章节划分对应《JavaScript 高级程序设计》（Professional JavaScript for Web Developers）第 3 版。
- 各浏览器 API 的现行行为以 [MDN Web Docs](https://developer.mozilla.org/) 为准。
