# JavaScript

>  不会 JavaScript 可以做好前端么？

这个问题可以这么来看，据说在腾讯等产业线巨长、部门众多的互联网公司里，前端是会划分成前端重构/前端开发/Node开发等不同岗位的，其中前端重构主要负责将设计图转化为页面及性能优化等，技能偏设计和 CSS + HTML，确实不太需要特别高深的 JavaScript 技能。但是在业界大多数的公司里是不会有这么详细的划分的，而且腾讯的这些前端重构岗的大牛们也必定都精通 JavaScript 的知识，所以大家还是老老实实把基础打牢吧～

下面我们看看在 JavaScript 部分，我们要掌握哪些基本技能：

## JavaScript 语言基础

- 语法
- JavaScript 中的面向对象编程、原型继承
- 作用域与闭包
- this 指向
- 事件处理模型
- BOM 与 DOM 操作
- 异步处理机制

以上大部分内容可以在 JavaScript 相关教程中学习到，关于事件处理和异步处理的章节我会稍后补充章节专门说明。

与很多后端语言不同，除了 JavaScript 的语法本身以外，对 DOM 及 BOM 操作的知识也很重要，请大家不要忽略。

在此推荐《JavaScript 语言精粹》一书：JavaScript 是一门出色的语言，如果你按照正确的方式去使用它的话！

在 ES6 章节我会简要提到这门语言存在的一些问题，新的语言标准和工具协助解决了一部分问题，但知道它在实现上有哪些坑确实可以有效提高我们的编程水平，毕竟那些工具也只是按照最佳实践自动化处理了那些坑而已。

《JavaScript高级程序设计》是 JavaScript 学习的“红宝书”，但是由于这本书内容太多，建议大家在阅读时尽量先一次速读本书，然后阅读《JavaScript 语言精粹》，在日后的工作和学习中可以不时回来针对性的阅读具体章节，以加深理解。

## ES6

> ECMAScript 6 （或 ECMAScript 2015+）

ES6 并不是一种语言，相反它是语言的标准和规范，包括现在 JavaScript、TypeScript 等都是这个标准一种实现。ES6 和 ES2015+ 说的都是同一个事儿，ES6 就是在 2015 年发布的，在那之后每年 6 月份滚动发布的版本名称确定为 ECMAScript + 当年月份，所以我们一般会用 ES6 代指 ES2015 及之后几年发布的标准，当然也有人用 ES7/8 特别指称近期发布的一些版本。

在 ES6 标准发布之前，我们使用的 JavaScript 多是 ECMAScript 4.0 - ECMAscript 5.1 标准的实现，因为各厂商的浏览器版本对标准的实现都有差异，在那时直接用 JavaScript 实现我们的前端逻辑面临着很严峻的兼容风险，jQuery 正是在这一时代快速流行起来：jQuery 屏蔽了部分浏览器兼容性问题，为我们操纵 DOM 等提供了同一的接口。但是由于 ECMAScript 本身也存在很多问题，导致在使用 JavaScript 时我们经常要用很多特殊的写法或工具来避免这些问题，比如 var 变量没有块级作用域等，更多可参见这里：[10个JavaScript常见BUG及修复方法](https://blog.fundebug.com/2017/11/15/top_10_bugs_and_fixing_method/) 。

ES6 延期了多次才正式发布，在这之间社区也提出了其他对下一代标准的实现，比如 Ruby 社区提出的 CoffeeScript 等，但现在来看 CoffeeScript 等已经用的不太多了，ES6 和 TypeScript 成为了业界主流。

在此推荐阮一峰老师的[《ECMAScript 6 入门》](http://es6.ruanyifeng.com/)，这也是我的 ES6 入门教材。

TypeScript 是微软贡献的 ECMAScript 实现语言，我们一般认为相比 ES6 它对大型前端项目能带来更好的可维护性[^1]，我现在还没有在大型项目中实践 TypeScript ，只有一些个人的实验性质的小项目中有使用，后续我会再增加 TypeScript 的相关章节。

[^1]: 众所周知，JavaScript 是一门动态类型语言，足够灵活，但这对于一个大型项目来说增加了运行时的不可预知性。TypeScript 提供的类型系统，可以在编译阶段就发现这些类型定义和使用的问题，同时语言层面增加的接口、泛型等特性，可以帮我们更好的以面向对象的编程范式完成代码的抽象和复用。
