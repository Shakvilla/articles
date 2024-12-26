---
title: "5. Fundamentals of JavaScript."
datePublished: Sat Dec 10 2022 12:48:31 GMT+0000 (Coordinated Universal Time)
cuid: clbhxnqbu000708mi69i42sps
slug: 5-fundamentals-of-javascript
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1670673096064/k20NpMhZy.jpeg
tags: javascript, frontend, web-development, frontend-development

---

## Lexical Structure of JavaScript.

Every language has a set of rules that govern how to speak it fluently. How to pronounce specific words, how to spell, and so on. Let's extend this analogy to programming languages as well. Every programming language has a set of rules that govern how we write and run code in the language. This set of rules specifies how we declare variables, write comments, separate two lines of code, use reserved words, and so on. This chapter will go over the low-level Javascript syntax. We will become better JavaScript developers if we understand the lexical structure of JavaScript. We will discuss;

*   Statements,
    
*   Case sensitivity,
    
*   Comments,
    
*   Whitespaces,
    
*   Identifiers,
    
*   Reserved Words,
    
*   Semicolons.
    

> Javascript borrows a lot of low-level syntaxes from other languages like Java, C++, C, Awk, Perl, and Python but still differs in some other ways from these languages.

A statement is a piece of code that instructs the JavaScript engine to perform a specific task. In JavaScript, statements are separated by a semicolon `;`

```javascript
let firstName = "John"; let lastName = "Doe";
console.log(firstName, lastName);
```

### Semicolons.

Even though a semicolon is optional, we must use one to separate multiple statements written on the same line. Furthermore, it is considered best practice to always include a semicolon in our Javascript code. The following code declares two variables, `firstName` and `lastName`, with the values `"John"` and `"Doe"` respectively.

```javascript
let firstName = "John"; let lastName = "Doe";
console.log(firstName, lastName);
```

### Case Sensitivity.

Because Javascript is case-sensitive, variables, function names, identifiers, and reserved words must be declared and called with consistent letter capitalization. Example;

```javascript
let firstName = "John"
```

`FirstName`, `FIRSTNAME`, and `firstname` are not the same variables, and a violation of this syntax rule will result in an error. As a result, we must always be on the lookout for such errors.

### Comments.

Comments allow us to include hints in our code for future reference or for any developer who is reading our code. The Javascript engine will ignore and not execute this section of code. Adding comments to your code is critical and considered best practice for code readability and comprehension.

When developing a real-world application, we often lose track of what each line of code is doing, so commenting our code will help us or any developer understand what the code is doing. There are two common methods for adding comments in Javascript;

*   **Single-Line Comments**
    
    We use two forward slashes `//` to implement a single-line comment in Javascript. Any texts that follow the two forward slashes will be commented out and ignored by the Javascript engine. Example;
    
    ```javascript
    // this is a single-line comment. this will be ignored by the engine
    // you can write multiple comments like this.
    ```
    
    **Note**: single-line comments always work in one line of code, if you have multiple comments, consider using multi-line and just bring the two forward-slashes in the next line.
    
*   **Multi-Line Comments**
    
    We use multi-line comments for long comments and comments that may require multiple lines to implement. To add multi-line comments, we use a forward slash followed by asterisks `/*` and ending with the opposite `*/`. Example;
    
    ```javascript
    /*
    * This is a multi-line comment. Use this to add multiple lines of comments in * your code.
    */
    ```
    
    **Note**: You might also see a third type of comment syntax at the start of some JavaScript files, which looks something like this: `#!/usr/bin/env node`.This is called **hashbang** comment syntax and is a special comment used to specify the path to a particular JavaScript engine that should execute the script. See [Hashbang's comments](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Lexical_grammar#hashbang_comments) for more details.
    

### Whitespaces:

Whitespaces in Javascript allow us to add spaces between characters. To add whitespaces to our code, we use tab, new line, carriage return, and space. Whitespaces are ignored by the JS engine. Whitespaces are frequently used to format our code in order to make it more readable. A code example without whitespaces;

```javascript
function fullName(firstName, lastName){console.log(firstName, lastName)}; fullName("John", "Doe")
```

The code above contains no whitespaces, and we can see that writing thousands of lines of code in this format will make it difficult to read. Consider the same example but with whitespaces below.

```javascript
function fullName(firstName, lastName){

	console.log(firstName, lastName);
};

fullName("John", "Doe");
```

### Identifiers

An identifier simply refers to a name of a constant, variable, function, classes, properties and labels for certain loops. An identifier can begin with an underscore`(_)`*, a dollar sign* `$` *a letter from* `a-z` *or* `A-Z` *and the following character can be any letter, a-z or A-Z, numbers* `(0-9)`*, underscore*`(_)` and dollar sign `($)`.

**Note**: Digits are not allowed to begin an identifier, this is for the JS engine to distinguish identifiers from numbers. Examples of acceptable identifiers in Javascript may include; `a`, `country`, `_code`, `$country`, `m23` etc.

### Reserved Words

Javascript has some keywords that are reserved for specific usages in the language. These reserved words cannot be used as identifiers for constants, variables, function names, or classes.

The table below contains reserved keywords in Javascript based on `ecma262`

| `let` | `as` | `const` | `if` | `export` | `break` |
| --- | --- | --- | --- | --- | --- |
| `null` | `void` | `function` | `class` | `async` | `await` |
| `continue` | `extends` | `import` | `false` | `in` | `set` |
| `catch` | `delete` | `for` | `while` | `do` | `else` |
| `from` | `debugger` | `return` | `throw` | `target` | `yield` |
| `case` | `new` | `switch` | `typeof` | `try` | `var` |
| `this` | `with` | `instanceof` | `static` | `default` | `true` |
| `finally` | `of` | `super` | `char` | `synchronized` | `volatile` |
| `protected` | `private` | `short` | `long` | `native` | `float` |
| `final` | `interface` | `eval` | `boolean` | `arguments` | `byte` |
| `enum` | `int` | `float` | `package` | `public` | `double` |