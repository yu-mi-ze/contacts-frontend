# 前端代码规范

## 说明
本代码规范基于以下主流标准：
- HTML: [HTML5 Best Practices](https://developer.mozilla.org/zh-CN/docs/Web/Guide/HTML/HTML5)
- CSS: [Airbnb CSS / Sass Styleguide](https://github.com/airbnb/css)
- JavaScript: [Google JavaScript Style Guide](https://google.github.io/styleguide/jsguide.html)

## HTML 规范

### 1. 文档结构
- 始终使用 DOCTYPE 声明
- 使用标准的 HTML5 文档结构
- 每个页面只包含一个 `<h1>` 标签

### 2. 命名规范
- 类名和ID使用小写字母和连字符（kebab-case）
- 避免使用无意义的命名（如 `temp`, `test`）
- ID应具有唯一性，类名可重用

### 3. 代码风格
- 缩进使用2个空格
- 标签名使用小写
- 属性值使用双引号
- 自闭合标签不需要额外的斜杠（如 `<input type="text">`）

### 4. 最佳实践
- 使用语义化标签（`<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`）
- 避免内联样式和脚本
- 添加适当的 `alt` 属性给图片
- 设置合适的 `title` 属性

## CSS 规范

### 1. 命名规范
- 类名使用小写字母和连字符（kebab-case）
- ID使用小写字母和连字符
- 避免使用ID作为选择器，优先使用类

### 2. 代码风格
- 缩进使用2个空格
- 每个属性单独占一行
- 冒号后添加一个空格
- 右大括号与规则同一行
- 颜色值使用十六进制表示（如 `#3498db`）
- 避免使用 `!important`

### 3. 组织方式
- 按功能模块组织CSS代码
- 使用注释标记不同的功能区块
- 全局样式在前，组件样式在后
- 响应式设计相关样式放在最后

### 4. 最佳实践
- 避免过度使用简写属性
- 优先使用 Flexbox 和 Grid 布局
- 使用相对单位（如 `rem`, `%`）而非固定像素
- 为动画使用 `transform` 和 `opacity` 以获得更好的性能

## JavaScript 规范

### 1. 命名规范
- 变量和函数使用小驼峰命名法（camelCase）
- 常量使用全大写和下划线（UPPER_SNAKE_CASE）
- 类名使用大驼峰命名法（PascalCase）
- 避免使用单字符变量名（循环变量除外）

### 2. 代码风格
- 缩进使用2个空格
- 每行最多80个字符
- 大括号放在同一行
- 语句末尾使用分号
- 字符串使用单引号

### 3. 变量声明
- 使用 `const` 声明不可变变量
- 使用 `let` 声明可变变量
- 避免使用 `var`
- 变量声明放在作用域顶部

### 4. 函数
- 优先使用箭头函数（对于简短的函数）
- 函数参数不超过3个
- 每个函数只做一件事
- 函数长度不超过50行

### 5. 错误处理
- 使用 `try-catch` 捕获可能的异常
- 提供有意义的错误消息
- 记录错误日志

### 6. 异步代码
- 使用 `async/await` 编写异步代码
- 避免深层嵌套的回调
- 正确处理 Promise 的拒绝

## 项目特定规范

### 1. 注释
- 为复杂逻辑添加注释说明
- 为函数和类添加文档注释
- 避免冗余注释

### 2. 文件组织
- 相关功能的代码放在一起
- 文件名使用小写字母和连字符
- 按功能模块划分目录

### 3. 性能优化
- 减少DOM操作
- 使用事件委托
- 避免在循环中创建函数
- 适当使用缓存

### 4. 可访问性
- 确保所有交互元素可通过键盘访问
- 使用适当的ARIA属性
- 确保文本和背景有足够的对比度

## 检查工具
- HTML: 使用 [HTMLHint](https://htmlhint.com/)
- CSS: 使用 [Stylelint](https://stylelint.io/)
- JavaScript: 使用 [ESLint](https://eslint.org/) 并配置为 Google 风格