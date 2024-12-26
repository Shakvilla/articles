---
title: "1. Getting started with JavaScript"
datePublished: Wed Dec 07 2022 12:16:01 GMT+0000 (Coordinated Universal Time)
cuid: clbdm6e4k000a08kz9kyd9ehr
slug: 1-getting-started-with-javascript
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1670416795803/XRT-uM0uT.png
tags: programming-blogs, javascript, beginners, frontend-development

---

**JavaScript** was created to add interactivity to web browsers. Before deciding to study Javascript, I recommend that you study HTML and CSS, which serve as the foundations of the web. If you don’t have any prior experience with HTML or CSS, visit the [MDN Docs](https://developer.mozilla.org/en-US/docs/) link to get a basic understanding of these technologies. This definition of Javascript is targeted at people who have no prior knowledge of any programming language. But if you have experience with another programming language, then I believe the definition below will make a lot of sense to you.

**JavaScript** is a high-level, prototype-based, object-oriented, multi-paradigm, interpreted or just-in-Time compiled, dynamic, single-threaded, garbage-collected programming language with first-class functions and a non-blocking event loop concurrency model. 😀. If you don’t know what some of these terms mean, don’t worry, I will briefly explain them in a jiffy.

The majority of the websites and web applications that exist on the World Wide Web are powered by Javascript. With the creation of Javascript libraries and frameworks like [React](https://reactjs.org/), [React Native](https://reactnative.dev/), [ElectronJS](https://www.electronjs.org/), [ThreeJS](https://threejs.org/), [TensorflowJS](https://www.tensorflow.org/js/), [Web3Js](https://web3js.readthedocs.io/en/v1.5.2/index.html) etc., we can now build single-page web apps, mobile apps, desktop apps, browser-based games, machine learning modules, and blockchain applications, respectively.

## Definition of Keywords:

### **1\. What Does High-Level Language (HLL) Mean?**

**Yes**, JavaScript is considered a high-level programming language. In general, high-level languages are easier for humans to read, write, and understand than low-level languages, which are closer to the machine code that is executed by a computer's processor.

Some characteristics of high-level languages that make them easier to use than low-level languages include the use of natural language elements, the use of higher-level abstractions for representing data and operations, and the use of a more flexible syntax that allows for more concise and expressive code.

In contrast to low-level languages, which are designed to be executed directly by a computer's processor, high-level languages are typically translated into machine code by another program, called a compiler or interpreter, before they can be executed. This intermediate step makes it easier for developers to write and debug their code, and it also makes it possible to write code that can be executed on a variety of different platforms without having to be rewritten for each specific platform.

Overall, the use of high-level languages like JavaScript allows developers to write more powerful and flexible programs in less time, and with fewer errors, than they could, using low-level languages.

## **2\. What Does Garbage-Collection mean:**

In the context of programming, garbage collection refers to a system for automatically freeing up memory that is no longer being used by a program. In JavaScript, the garbage-collection system is responsible for automatically releasing memory that is no longer needed by an application. This is important because, in JavaScript, memory is allocated for objects when they are created, but it is not automatically freed up when those objects are no longer needed. This means that, if a JavaScript program creates a large number of objects and then discards them, it can quickly use up all of the available memory, which can cause the program to crash. By using a garbage-collection system, JavaScript can automatically free up the memory used by objects that are no longer needed, which helps prevent these types of crashes and improves the overall performance of the program.

### **3\. Interpreted or Just-In-Time compiled:**

JavaScript is an interpreted language, which means that it is not compiled into machine code before it is executed. Instead, the code is interpreted and executed directly by a JavaScript engine, such as the one built into web browsers.

One advantage of using an interpreted language like JavaScript is that it is generally easier to write and debug code, because there is no need to compile the code before it can be executed. This also means that JavaScript code can be executed on any platform that has a JavaScript engine, without the need to compile the code specifically for that platform.

However, there are also some disadvantages to using an interpreted language. Because the code is not compiled before it is executed, interpreted languages like JavaScript can be slower to run than compiled languages, which have been optimized for performance. Additionally, because the code is not checked for errors before it is executed, it is possible for runtime errors to occur that would not have been detected by a compiler.

To address these issues, some JavaScript engines, such as Google's V8 engine, use a technique called just-in-time (JIT) compilation, which compiles JavaScript code into machine code at runtime, just before it is executed. This can improve the performance of JavaScript code by allowing it to run faster, while still maintaining the flexibility and ease of use of an interpreted language.

### **4\. Multi-Paradigm:**

JavaScript is a multi-paradigm language, which means that it supports multiple programming paradigms, or ways of organizing and structuring code.

Some of the paradigms that JavaScript supports include object-oriented programming, functional programming, and event-driven programming. This means that JavaScript code can be written using techniques from any of these paradigms, or even using a combination of techniques from multiple paradigms.

Being a multi-paradigm language allows JavaScript to be used for a wide variety of programming tasks and enables developers to choose the programming approach that is best suited to their specific needs. This makes JavaScript a highly versatile language that can be used to build a wide range of applications, from simple websites to complex back-end systems.

### 5\. Prototype Based Object-Oriented:

In JavaScript, objects can be created using the prototype-based object-oriented programming paradigm. This means that, rather than using a class to define the properties and behaviors of an object, a prototype is used to specify the characteristics of a new object.

In prototype-based object-oriented programming, an object’s properties and methods are defined by its prototype, which is an object that serves as a template for creating new objects. When a new object is created, it inherits the properties and methods of its prototype, which can be modified or extended to provide the specific behavior that is needed for the new object.

This approach to object-oriented programming is different from the class-based approach used by languages like Java and C++, where objects are created by instantiating a class, which defines the properties and methods of the object.

Prototype-based object-oriented programming can be a powerful way to create flexible and reusable code, because it allows for the dynamic creation of objects and the easy extension of existing objects to add new functionality. It is also a key feature of JavaScript, which does not have a built-in support for classes.

### **6\. First-Class Functions:**

In JavaScript, functions are first-class objects, which means that they can be treated like any other value in the language. This means that they can be assigned to variables, passed as arguments to functions, and returned as values from functions.

Having first-class functions is a key feature of JavaScript, which allows for the use of powerful programming techniques, such as higher-order functions and closures. Higher-order functions are functions that operate on other functions, either by taking a function as an argument or by returning a function as a result. Closures are a special type of function that can reference variables from their containing scope, even after that scope has been exited.

Together, these features enable the creation of sophisticated, flexible, and reusable code in JavaScript. They also make it possible to use functional programming techniques in JavaScript, which can help improve the readability and maintainability of the code.

### **7\. Dynamic:**

Yes, JavaScript is a dynamic language, which means that it can modify its behaviour at runtime. This is in contrast to static languages, which have a fixed set of rules and behaviours that are determined at compile time and cannot be changed at runtime.

One of the key characteristics of dynamic languages is that they support reflection, which is the ability of a program to examine and modify itself at runtime. In JavaScript, reflection is possible through the use of the `typeof` operator, which can be used to determine the type of a value at runtime, and through the `eval` function, which allows JavaScript code to be executed at runtime.

Being a dynamic language allows JavaScript to be highly flexible and adaptable, which makes it well-suited to a variety of programming tasks. It also enables the use of advanced programming techniques, such as metaprogramming and runtime code generation, which can help improve the expressiveness and power of the language. However, it can also make it more difficult to predict the behaviour of JavaScript code, which can make it harder to debug and maintain.

### **8\. Single-threaded:**

In JavaScript, single-threaded refers to the fact that the language has a single execution thread, or a single sequence of instructions that can be executed at a time. This means that, in JavaScript, only one piece of code can be executed at a time, and any other code must wait until the current code has finished executing before it can be run.

Having a single execution thread can be a limitation of JavaScript, because it means that the language is not well suited to handling multiple concurrent tasks. This can make it difficult to write programs that need to perform multiple complex operations at the same time, such as a web application that needs to handle multiple user interactions and data updates simultaneously.

To address this issue, some JavaScript engines, such as the ones used in web browsers, use a technique called concurrency, which allows multiple pieces of code to be executed in parallel. However, this is not a native feature of JavaScript, and it requires the use of special APIs and techniques to implement. Overall, the single-threaded nature of JavaScript is an important aspect of the language that can affect its performance and scalability.

### **9\. Non-blocking:**

In JavaScript, non-blocking refers to the ability of the language to execute code without stopping, or blocking, the execution of other code. This means that, in JavaScript, multiple pieces of code can be executed concurrently, without one piece of code needing to wait for the other to finish before it can be run.

Having non-blocking behaviour is an important feature of JavaScript because it allows the language to handle multiple tasks concurrently. This is particularly important in the context of web development, where a single web page can have many different components, such as user input fields, buttons, and animations, that all need to be handled simultaneously.

To achieve non-blocking behaviour in JavaScript, the language uses an event-driven programming model, where different pieces of code are executed in response to events, such as user actions or data updates. This allows the JavaScript engine to execute multiple pieces of code concurrently, without blocking the execution of other code.

Overall, the non-blocking nature of JavaScript is a key feature of the language that enables it to handle complex, interactive applications, and it is an important aspect of the language that developers need to understand to write effective and efficient code.

### **Conclusion:**

This section is just to introduce, in detail without code, what JavaScript is. I have provided theoretical definitions of most of the keywords in the definition of the JavaScript language. We will revisit all of the in this series with code examples in subsequent series.