# 🚀 JavaScript & TypeScript Interview Questions and Answers

Welcome to the **JavaScript Interview Questions and Answers** repository! This collection is designed to help developers prepare for technical interviews by covering essential concepts, tricky questions, and expert answers. 🌟

---

## 📌 JavaScript Questions

| #  | Question |
|----|----------|
| 1  | [What is JavaScript?](#what-is-javascript) |
| 4  | [Is JavaScript Compiled or Interpreted or both?](#jq4-is-javascript-compiled-or-interpreted-or-both) |
| 5  | [Difference between `let`, `const`, and `var`?](#jq5-what-is-the-difference-between-let-const-and-var) |
| 6  | [Different data types in JavaScript?](#jq6-what-are-the-different-data-types-in-javascript) |
| 6  | [Explain the concepts Hoisting and Temporal Dead Zone?](#jq7-explain-the-concepts-hoisting-and-temporal-dead-zone) |

---

### What is JavaScript?

JavaScript is a versatile, high-level, interpreted programming language created by **Brendan Eich** in 1995.

- It’s primarily used for building dynamic and interactive web applications.
- JavaScript is multi-paradigm—it supports object-oriented (prototype-based), functional, and imperative programming.
- Although single-threaded by design, it handles asynchronous operations efficiently through the event loop, callbacks, and Promises.
- Modern engines like V8 also JIT-compile JavaScript for performance.
- Beyond the browser, it’s widely used on the server-side with Node.js.

[🔼 Back to top](#-javascript-questions)



### JQ4. Is JavaScript Compiled or Interpreted or both?

JavaScript is both compiled and interpreted. While JavaScript is fundamentally an interpreted language, JavaScript engines uses **Just-In-Time (JIT)** compilation in modern browsers. This means that the JavaScript code is compiled into machine code at runtime, just before it's executed. This makes JavaScript a compiled and interpreted programming language.

[🔼 Back to top](#-javascript-questions)


### JQ5. What is the difference between `let`, `const`, and `var`?

In JavaScript, variables are declared using the keywords `let`, `const` or `var`.

-  **Scope**: `var` is function-scoped, while both `let` and `const` are block-scoped (Introduced in JavaScript ES6 version).
-  **Re-declaration**: `var` redeclared within its scope. While `let` and `const` cannot be redeclared. 
-  **Re-assignment**: `var` and `let` variables can be reassigned within the same scope. But `const` variables cannot be re-assigned after initialization.
-  **Modification**: `var` and `let` variables can be modified but `const` variable cannot. However, if a `const` variable holds an object or an array, the contents of that object or array can be modified.
-  **Hoisting**: variables declared with `var` is hoisted to the top of its scope (function or global). Both `let` and `const` are also hoisted, but they are not initialized.

| Feature       | `var`                          | `let`                           | `const`                          |
|--------------|--------------------------------|---------------------------------|----------------------------------|
| Scope        | Function-scoped               | Block-scoped                    | Block-scoped                     |
| Hoisting     | Hoisted with `undefined`      | Hoisted but not initialized     | Hoisted but not initialized      |
| Re-declaration | Allowed                      | Not allowed                     | Not allowed                      |
| Re-assignment | Allowed                      | Allowed                         | Not allowed                      |
| Mutable      | Yes                            | Yes                             | No (must be initialized)         |
| Use Case     | Legacy code, avoid using      | Recommended for variables       | Use for constants                |
   

[🔼 Back to top](#-javascript-questions)


### JQ6. What are the different data types in JavaScript?

Data Types in JavaScript can be broadly categorized into primitive and non-primitive types.

1) **Primitive Data Type** - Primitive datatypes represent single values and are immutable.

   - Number: Represents numeric values (integers and decimals).
       
     ```ts
     let n = 42;
     let pi = 3.14;
     ```
     
   - String: Represents text enclosed in single or double quotes.
       
     ```ts
     let s = "Hello, World!";
     ```
     
   - Boolean: Represents a logical value (true or false).
     
     ```ts
     let bool= true;
     ```
     
   - Undefined: A variable that has been declared but not assigned a value.
    
     ```ts
     let notAssigned;
     console.log(notAssigned);
     ```
     
   - Null: Represents an intentional absence of any value.
    
     ```ts
     let empty = null;
     ```
     
   - Symbol: Represents unique and immutable values, often used as object keys.
  
     ```ts
     let sym = Symbol('unique');
     ```
     
   - BigInt: Represents integers larger than Number.MAX_SAFE_INTEGER.
  
     ```ts
     let bigNumber = 123456789012345678901234567890n;
     ```
   
3) **Non-Primitive Data Type** - Non-primitive types are objects and can store collections of data or more complex entities.

   - Object: Represents key-value pairs.
       
     ```ts
     let obj = {
       name: "Amit",
       age: 25
     };
     ```
     
   - Array: An indexed collection which represents ordered list of values.
       
     ```ts
     let a = ["red", "green", "blue"];
     ```
     
   - Function: Represents reusable blocks of code.
       
     ```ts
     function fun() {
        console.log("GeeksforGeeks");
     }
     ```

### JQ7. Explain the concepts Hoisting and Temporal Dead Zone?

**Hoisting** refers to the behaviour where JavaScript moves the declarations of variables, functions, and classes to the top of their scope during the compilation phase. This can sometimes lead to surprising results, especially when using var, let, const, or function expressions.

-   Hoisting applies to variable and function declarations.
-   Initializations are not hoisted, they are only declarations.
-   `var` is hoisted to the top of its scope (function or global) and initialized with undefined until assiging a value.
-   `let` and `const` are also hoisted, but they are not initialized. accessing these varaible will throw `ReferenceError`.

**Temporal Dead Zone (TDZ)** refers to the period between the entering of a scope (such as a function or block) and the actual initialization of a variable declared with `let` or `const`. During this time, any reference to the variable before its initialization will throw a ReferenceError.
     
[🔼 Back to top](#-javascript-questions)
