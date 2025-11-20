### web 开发人员必须学习的 3 门语言区别
1.页的内容HTML 定义了网

2.CSS 描述了网页的布局

3.JavaScript 控制了网页的行为,使网页不再是静态的，而是可以根据用户的操作动态变化的。

### JavaScript 用法
#### JavaScript 用法

- <script> 和 </script> 会告诉 JavaScript 在何处开始和结束。

- Javascript 脚本代码可被放置在 HTML 页面的 <body> 和 <head> 部分中。

- 脚本可位于 HTML 的 <body> 或 <head> 部分中，或者同时存在于两个部分中。

**提示**：通常的做法是把函数放入 <head> 部分中，或者放在页面底部。这样就可以把它们安置到同一处位置，不会干扰页面的内容。

#### JavaScript 导入方式
与css导入方式相同。

### JavaScript 输出
JavaScript 没有任何打印或者输出的函数。

#### JavaScript 显示数据
JavaScript 可以通过不同的方式来输出数据：

- 使用 window.alert() 弹出警告框。

- 使用 document.write() 方法将内容写到 HTML 文档中。

- 使用 innerHTML 写入到 HTML 元素。

- 使用 console.log() 写入到浏览器的控制台。
#### JavaScript 语法
- JavaScript 是一个程序语言。语法规则定义了语言结构。

- JavaScript 是一个脚本语言。它是一个轻量级，但功能强大的编程语言。

- JavaScript 代码：JavaScript 代码是 JavaScript 语句的序列。浏览器按照编写顺序依次执行每条语句。

- JavaScript 代码块：代码块以左花括号开始，以右花括号结束。代码块的作用是一并地执行语句序列。

- 空格：JavaScript 会忽略多余的空格。您可以向脚本添加空格，来提高其可读性

- 折行：在文本字符串中使用反斜杠对代码行进行换行。但表达出来的内容不会折行。

- 注释：JavaScript 不会执行注释。
  单行注释以 // 开头。多行注释以 /* 开始，以 */ 结尾。

**提示**：注释用于阻止其中一条代码行的执行（可用于调试）。

- 字母大小写：JavaScript 对大小写是敏感的。
### JavaScript 作用
1.客户端脚本：用于在用户浏览器中执行，实现动态效果和用户交互。

2.网页开发：与HTML和CSS协同工作，使得网页具有更强的交互性和动态性。

3.后端开发：使用Node.js,JavaScript也可以在服务器端运行，实现服务器端应用开发。
### JavaScript 变量
变量是用于存储信息的"容器"。

在 JavaScript 中，变量用于存储数据，并可以在程序执行过程中动态更改。

在 JavaScript 中，变量可以存储各种类型的数据，如数字、字符串、对象、函数等。

变量名是标识符，用于引用存储在变量中的数据。

在 JavaScript 中，可以使用 var、let 和 const 关键字来声明变量。

- var：ES5 引入的变量声明方式，具有函数作用域。

  var 声明特点：

  1.变量可以重复声明（覆盖原变量）。
  
  2.变量未赋值时，默认值为 undefined。
  
  3.var 声明的变量会提升（Hoisting），但不会初始化。
  
  4.可以在一条语句中声明很多变量。该语句以 var 开头，并使用逗号分隔变量即可。
  
- let：ES6 引入的变量声明方式，具有块级作用域。

- const：ES6 引入的常量声明方式，具有块级作用域，且值不可变。

**提示**：您可以把变量看做存储数据的容器。

### JavaScript 数据类型
- **值类型(基本类型)**：字符串（String）、数字(Number)、布尔(Boolean)、空（Null）、未定义（Undefined）、Symbol。

- **引用数据类型（对象类型）**：对象(Object)、数组(Array)、函数(Function)，还有两个特殊的对象：正则（RegExp）和日期（Date）。
![图像理解](https://www.runoob.com/wp-content/uploads/2013/08/Javascript-DataType.png)

**注**：Symbol 是 ES6 引入了一种新的原始数据类型，表示独一无二的值。

**JavaScript 拥有动态类型**这意味着相同的变量可用作不同的类型。变量的数据类型可以使用 typeof 操作符来查看：

















