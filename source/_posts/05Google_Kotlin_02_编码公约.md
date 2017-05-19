---
title: 2017Android官方新编程语言Kotlin | Kotlin编码公约
date: 2017-5-19 13:27:12  #文章生成时间
categories: #法律法规 #文章分类目录 可以省略 # 加 <!--more-->以分割摘要与文章正文。
- Android官方新编程语言Kotlin
tags: #文章标签 可以省略 #设置为则当前页没有打赏按钮reward: false
- Android官方新编程语言Kotlin
- #YouTube
---
3该页面包含Kotlin语言的当前编码风格。
<!--more-->
# 命名风格 #
如果有疑问，请默认使用Java编码约定，例如：

1. 使用camelCase作为名称（并避免在名称中使用下划线）
2. 类型从大写开始
3. 方法和属性从小写开始
4. 使用4空格缩进
5. 公共职能应该有文件，使其出现在Kotlin Doc

# Colon  #

冒号之前有一个空格，冒号分隔了类型和超类型，并且没有空格，冒号分隔实例和类型：

	interface Foo<out T : Any> : Bar { fun foo(a: Int): T } 

# Lambda表达式 #

在lambda表达式中，大括号周围应该使用空格，以及将参数与正文分开的箭头。 只要有可能，一个lambda应该被传递到括号之外。

	list.filter { it > 10 }.map { element -> element * 2 }
 
在短而不嵌套的lambdas中，建议使用it惯例，而不是明确声明参数。 在具有参数的嵌套lambdas中，参数应始终声明明确。

# 类头格式化 #

有几个参数的类可以写成一行：

	class Person(id: Int, name: String) 

具有较长标题的类应格式化，以使每个主构造函数参数与单独的行缩进。 此外，右括号应该在新的一行。 如果我们使用继承，则超类构造函数调用或实现接口列表应位于与括号相同的行上：

	class Person( id: Int, name: String, surname: String ) : Human(id, name) { // ... } 

对于多个接口，超类构造函数调用应首先定位，然后每个接口应位于不同的行：

	class Person( id: Int, name: String, surname: String ) : Human(id, name), KotlinMaker { // ... } 
构造函数参数可以使用常规缩进或连续缩进（双倍的常规缩进）。

# 单元 #

如果函数返回Unit，则返回类型应该省略：

	 fun foo() { // ": Unit" is omitted here } 

# 功能与属性 #

在某些情况下，没有参数的函数可能与只读属性可互换。 虽然语义是相似的，但是有一些风格约定是什么时候喜欢一个。
当基础算法时，优先于一个函数的属性：

1. 不抛出
2. 具有O(1)复杂性
3. 算是便宜的（或者在第一次跑步）
4. 通过调用返回相同的结果


来源： https://translate.googleusercontent.com/translate_c?depth=1&hl=en&rurl=translate.google.com&sl=en&sp=nmt4&tl=zh-CN&u=https://kotlinlang.org/docs/reference/coding-conventions.html&usg=ALkJrhjCIElDFOeme3dv9P9gdU8oXATYGQ
