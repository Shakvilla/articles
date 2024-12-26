---
title: "6. Understand Variables (let, const and var) in JavaScript"
datePublished: Mon Dec 12 2022 06:02:42 GMT+0000 (Coordinated Universal Time)
cuid: clbke1jul0go2mlnv8vx146ds
slug: 6-understand-variables-let-const-and-var-in-javascript
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1670806083663/cazCThbIG.jpeg
tags: variables, javascript, web-development, frontend-development

---

Are you new to JavaScript, and looking to learn more about variables? Look no further! In this beginner's guide, we'll explain what variables are and how they are used in JavaScript. We'll also cover the different ways to declare variables in JavaScript, and provide some tips and best practices for working with variables in your code. By the end of this guide, you will have a strong foundation in the basics of variables in JavaScript, and be well on your way to becoming a proficient JavaScript developer. Let's get started!

The concept of variables in programming is an important part of the language. Computers are machines we use to process data and output information. Before a computer can process any data, it has to be saved to memory, before the computer can process that data, this is where variables come in.

### **The** `let` **keyword.**

The `let` keyword is used in JavaScript to declare a variable. This keyword was introduced in ECMAScript 6 (ES6) as a new way to declare variables, along with the `const` keyword.

The `let` keyword allows you to create variables that are limited in scope to the block, statement, or expression in which they are used. This means that a `let` the variable is only accessible within the context in which it was declared and is not visible outside of that context. This is different from the `var` keyword, which declares a variable with global or function scope.

Here's an example of using the `let` keyword to declare a variable in JavaScript:

```javascript
//Example 1:
let variableData; // undefined
	variableData = "Javascript is awesome"
	alert(variableData)
	
//Example 2:
let variableData = "Javascript is awesome"
	alert(variableData)
	variableData = "We can mutate this variable"

//Example 3:

let firstName = "John", secondName = "Doe", childName = "John Doe Jr"


// Example 4:
let variable_data = "Javascript is awesome" // camel_casing
	alert(variable_data)

//Example 5:  
let $function = "reserved word prevented" // reserved word prevented

//Example 6;
let function = "a reserved keyword used " //Uncaught SyntaxError: Unexpected token 'function’ 


//Example 7:
let _currency = "dollar"

//Example 8;
let 7days_of_the_week = "seven days make up a week" // Uncaught SyntaxError: Invalid or unexpected token
```

**In example 1**, we declared the variable `variableData` and assigned no value to it, so by default, `undefined` will be assigned to it, we then call `variableData` and assign “Javascript is awesome” to it, so now the container holding the value for the variable will be updated with the new value assigned.

**In example 2**, we declared the variable and assigned the value to it right away, this will work like the first one, just that, the engine’s work has been made easier. Observe how we changed(mutated) the value of the variable. So with `let` we can reassign a different value to a variable already declared and assigned to a previous value.

**In example 3,** observe how we have declared multiple variables in a single line by using just a single `let` keyword. This is acceptable in Javascript, but this way of declaring multiple variables is not recommended. Declare each variable in a single line for the sake of readability. For example, let us rewrite example 3.

```javascript
let firstName = "John";
let secondName = "Doe";
let childName = "John Doe Jr";
```

**Example 4**, we show how we can declare a variable using the [camelCasing](https://en.wikipedia.org/wiki/Camel_case) technique. When a variable name contains more than 2 words, it is recommended to use this casing technique.

**In example 5**, we intentionally used a reserved keyword but the JS engine won’t complain because we added the `$` before the `function` which tells the engine to accept the variable name.

**In example 7**, observe how the variable name starts with the underscore character. This is another way of declaring variables’ names in Javascript.

### **The** `var` **keyword.**

In this code, we declare a `var` variable called `myVariable` and assign it the string value `'Hello, world!'`. This variable can be accessed and used within the current global scope or within the current function.

In general, it is considered best practice to use the `let` or `const` keywords instead of the `var` keyword when declaring variables in JavaScript. This helps to avoid the potential issues mentioned above, and can make your code more readable and maintainable in the long run. Example;

```javascript
var firstName = "John";
var secondName = "Doe";
var childName = "John Doe Jr";
```

### **The** `const` **keyword**

In JavaScript, the `const` keyword is used to declare a constant variable. This means that the value of a `const` variable cannot be reassigned after it is declared.

The `const` keyword was introduced in ECMAScript 6 (ES6) as a new way to declare variables, along with the `let` keyword. It is considered best practice to use `const` whenever possible, because it helps to prevent accidental or intentional reassignment of variable values. This can make your code more predictable and easier to maintain in the long run.

Here's an example of using the `const` keyword to declare a constant variable in JavaScript:

```javascript
const constantVariable = "this is a constant variable and will not change" // constantVariable will always never change

const PI = 3.14159 // The PI Variable is immutable
```

As developers we strive to make our processed much easier and smooth, based on that, developers often use uppercase constants and underscores for difficult-to-remember values like colours, mathematical formulae etc and then assign the constants to variables.

```javascript
const COLOR_BLUE = "#00F";
let primary_color = COLOR_BLUE;

const PI = 3.14159 
const radius = 4
let circumference = 2 * PI * radius
alert(circumference) // 25.13272
```

In the example above, we create a constant(immutable) colour `COLOR_BLUE` and assign that `primary_color` which is mutable. Basically, we can reassign a different constant to `primary_color` because we use `let` keyword there.

In the second example, we create a constant variable, the value for `PI` which never changes, we create a `radius` constant which doesn’t change as well, then calculate for the circumference of our imaginary circle.

In general, it is best practice to use the `const` keyword to declare constant variables in JavaScript. This helps to prevent accidental or intentional reassignment of variable values, which can make your code more predictable and easier to maintain.

### **Naming Variables**

In JavaScript, variables can be named using any combination of letters, digits, underscores, and dollar signs. However, there are some rules and conventions that should be followed when choosing variable names:

1.  Variable names must not begin with a digit. For example, `1variable` is not a valid variable name in JavaScript.
    
2.  Variable names are case-sensitive. For example, `myVariable` and `myvariable` are two different variables in JavaScript.
    
3.  Variable names cannot be the same as reserved keywords in JavaScript. For example, you cannot use `var` or `let` as variable names because they are reserved keywords in JavaScript.
    
4.  Variable names should be descriptive and meaningful. It is generally best practice to use variable names that accurately reflect the purpose or value of the variable. For example, a variable that holds a user's first name might be named `firstName`, while a variable that holds an array of numbers might be named `numbersArray`.
    
5.  Variable names should use camelCase or snake\_case formatting. In JavaScript, it is common to use either camelCase (e.g. `myVariable`) or snake\_case (e.g. `my_variable`) for variable names. This helps to improve the readability and maintainability of your code.
    

By following these rules and conventions, you can choose variable names that are clear, descriptive, and easy to work with in your JavaScript code.

### Conclusion

variables are an essential part of any JavaScript program. They allow us to store and manipulate data, making our code more dynamic and flexible. By assigning unique names to our variables, we can easily reference and update their values as needed. By understanding the different data types and how to declare and initialize variables, we can effectively use them in our code to achieve our desired outcome.