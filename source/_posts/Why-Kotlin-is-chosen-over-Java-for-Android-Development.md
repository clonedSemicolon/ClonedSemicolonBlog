---
title: "Why Kotlin is better than Java in Android Development perspective?"
catalog: true
toc_nav_num: true
date: 2023-1-5 22:26:24
subtitle: "Avishak Chakroborty"
header-img: "/img/article_header/article_header.png"
tags:
- Android
- Kotlin
catagories:
- Android
updateDate: 2023-1-5 22:26:24
author: Avishak Chakroborty
top: 1

---


![](https://i.ibb.co/nkSwKX8/Untitled-design-8.png)

Kotlin is a programming language that was developed by JetBrains. It was first released in 2011 and since then has become one of the most popular languages for Android development. For a very long time, Java has existed. Although it had a few minor limitations, millions of programmers around the world nevertheless used it. Then Google unveils a brand-new language designed particularly for Android that is allegedly superior to Java.

Along with the already-existing support for Java and C++, Kotlin was designated by Google as a "first-class" language for Android development last year. The results of GitHub's analysis show the effects of Google's choice to adopt Kotlin. In this article, we will discuss why Kotlin is chosen over Java and when you should use it instead of Java. 

### Why Kotlin?

> Less code to write
> More readable code
> Fewer bugs
> More maintainable code


### Kotlin is simpler than Java

Kotlin is a statically typed language, which means that you don't have to worry about the type of variable you're using. This means that your code is more concise and safer because it's easier to write down what type each variable has and what each operator does.

Because Kotlin is less verbose than Java, we can also use fewer characters in our program. When writing a piece of code in Kotlin:

> You'll only need two spaces instead of four!
> There will be no curly braces or semicolons required for every line!

### Support for nullability

In Kotlin, nullability is represented using nullable types and non-null types. A nullable type is a type that can hold a null value, while a non-null type is a type that cannot hold a null value.

To declare a nullable type in Kotlin, you can use the '?' operator after the type name. 

```
val str: String? = null
```
In this example, str is a nullable String, which means it can hold a null value.

Kotlin provides several features to help you safely work with nullable types. For example, you can use the `?.` operator to safely access a member of a nullable type, like this:

```
val str: String? = "Hello, World!"
val length = str?.length
```

In this example, length will be assigned the value of str.length if str is not null, and null if str is null.

### Better Supports for Funcitonal Programming

Kotlin supports functional programming constructs, including higher-order functions, lambda expressions, and function types.

Higher-order functions are functions that take other functions as parameters or return them as a result. Kotlin allows you to pass a function as an argument to another function using the :: operator. For example:

```
fun process(str: String, process: (String) -> Unit) {
    process(str)
}

fun main() {
    process("Hello, World!", ::println)
}

```

In this example, the process function takes a String and a function as arguments, and invokes the function with the String as an argument. The main function calls the process function with the println function as the second argument.

Lambda expressions are anonymous functions that can be passed as arguments to higher-order functions. Kotlin allows you to write lambda expressions using the `{}` syntax. For example:

```
fun process(str: String, process: (String) -> Unit) {
    process(str)
}

fun main() {
    process("Hello, World!", { str -> println(str) })
}
```

In this example, the main function calls the process function with a lambda expression as the second argument. The lambda expression takes a String as an argument and prints it to the console.

Function types are a way of referring to functions in Kotlin. You can declare a variable of a function type using the (args) -> returnType syntax. For example:
```
val process: (String) -> Unit = ::println
```

In this example, the process variable is of type (String) -> Unit, which means it refers to a function that takes a String as an argument and returns Unit. The value of the process variable is the println function.


### Highly Compatible with Java

Kotlin is designed to be fully interoperable with Java, so you can use Kotlin and Java code together in the same project. This means you can take advantage of the features of Kotlin without having to rewrite your existing Java code.

Kotlin is also highly compatible with Java 6, which means you can use Kotlin in projects that are using an older version of Java. This can be particularly useful if you are working on a large project that has a lot of legacy code written in Java 6, or if you are working on a project that has strict version requirements.


### No raw types or checked Exception

Java's raw types feature enables you to utilize a generic class's or interface's type without supplying any type parameters. Raw types are not supported in Kotlin since all generic types need to have their type parameters defined.

Java has a feature called checked exceptions that mandates that you manage or disclose any exceptions that a function might throw. Kotlin uses exceptions only when they are absolutely necessary; you are not obligated to handle or declare them. Kotlin, on the other hand, comes with a built-in method for handling exceptions known as "try/catch" blocks.


```
try {
    // code that might throw an exception
} catch (e: Exception) {
    // code to handle the exception
}
```

In this sample, the code in the try block is run, and any thrown exceptions are captured and dealt with in the catch block.

Overall, Kotlin's lack of checked exceptions and raw types can help your code be shorter and simpler because you won't have to bother about handling or declaring exceptions or specifying type parameters.


The modern, concise, and potent language Kotlin has numerous advantages over Java. Compared to Java, it is simpler to learn, has a more natural syntax, and performs better overall. Because the Kotlin compiler is open-source software and supports JVM virtual machines on Linux and Windows, you can use it for desktop and server-side development projects alike.


# Happy Dev ^_^ 
---
<!-- Place this tag in your head or just before your close body tag. -->
<script async defer src="https://buttons.github.io/buttons.js"></script>
<!-- Place this tag where you want the button to render. -->

Please <a class="github-button" href="https://github.com/clonedSemicolon/clonedSemicolon.github.io" data-icon="octicon-star" aria-label="Star huweihuang/hexo-theme-huweihuang on GitHub">Star</a> this Project if you like it! <a class="github-button" href="https://github.com/clonedSemicolon" aria-label="Follow @ClonedSemicolon on GitHub">Follow</a> would also be appreciated!

Peace!
