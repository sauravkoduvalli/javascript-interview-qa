# 🚀 JavaScript & TypeScript Interview Questions and Answers

Welcome to the **JavaScript & TypeScript Interview Questions and Answers** repository! This collection is designed to help developers prepare for technical interviews by covering essential concepts, tricky questions, and expert answers. 🌟

## 📜 Table of Contents

- [📌 JavaScript Questions](#-javascript-questions)
- [📌 TypeScript Questions](#-typescript-questions)

## 🤝 Contributing

We welcome contributions! 🚀 If you have an interesting JavaScript/TypeScript interview question, feel free to:

1. Fork this repository
2. Add your question and answer in the respective section
3. Create a pull request

## ⭐ Support

If you found this repository helpful, please give it a **star** ⭐ and share it with others! Good Luck, Aliens👽🚀

---

## 📌 JavaScript Questions

| #  | Question |
|----|----------|
| 1  | [What is JavaScript?](#jq1-what-is-javascript) |
| 2  | [Applications of JavaScript?](#jq2-applications-of-javascript) |
| 3  | [What are the limitations of JavaScript?](#jq3-what-are-the-limitations-of-javascript) |
| 4  | [Is JavaScript Compiled or Interpreted or both?](#jq4-is-javascript-compiled-or-interpreted-or-both) |
| 5  | [What is the difference between `let`, `const`, and `var`?](#jq5-what-is-the-difference-between-let-const-and-var) |
| 6  | [What are the different data types in JavaScript?](#jq6-what-are-the-different-data-types-in-javascript) |
| 6  | [Explain the concepts Hoisting and Temporal Dead Zone?](#jq7-explain-the-concepts-hoisting-and-temporal-dead-zone) |

---

## 📌 TypeScript Questions

| #  | Question |
|----|----------|
| 1  | [What are TypeScript interfaces?](#tq1) |
| 2  | [Explain TypeScript generics with an example.](#tq2) |
| 3  | [What is the `readonly` modifier in TypeScript?](#tq3) |

---

### JQ1. What is JavaScript?

JavaScript is a versatile, dynamically typed programming language used for interactive web applications, supporting both client-side and server-side development.

- JavaScript is a single-threaded language that executes one task at a time.
- It is an Interpreted language which means it executes the code line by line.
- The data type of the variable is decided at run-time in JavaScript that’s why it is called dynamically typed.
- JavaScript is considered a lightweight language due to its low CPU usage, minimalist syntax, and ease of implementation.

[🔼 Back to top](#-javascript-questions)


### JQ2. Applications of JavaScript?

1) **Front-end development**: Works with HTML and CSS to build interactive and dynamic web pages. (React, Angular, Vue.js)
2) **Backend Development**: Node.js enables JavaScript to run on the server side. Used to build RESTful APIs, real-time applications, and microservices. (Express.js, NestJS)
3) **Desktop Application**: Electron.js allows JavaScript to build cross-platform desktop apps (e.g., VS Code, Slack).
4) **Mobile Application**: Cross-platform mobile apps using frameworks like React Native, Ionic, and NativeScript.
5) **Game Development**: Used to create browser-based games with libraries like Phaser.js and Three.js for 3D graphics.
6) **Internet of Things (IoT)**: JavaScript (with Node.js) is used in IoT applications to control hardware devices.
7) **Machine Learning & AI**: Libraries like TensorFlow.js enable machine learning models to run in the browser.
8) **Data Visualization**: Libraries like D3.js and Chart.js help create interactive charts and graphs.
9) **Automation & Scripting**: JavaScript (via Node.js) can be used for automating tasks, web scraping (Puppeteer), and browser automation.
10) **Blockchain & Web3 Development**: JavaScript is used in smart contract development and blockchain applications with libraries like Web3.js and Ethers.js.

[🔼 Back to top](#-javascript-questions)


### JQ3. What are the limitations of JavaScript?

- **Weak Type Checking**: JavaScript is weakly typed, meaning variables don’t require explicit types. This can lead to runtime errors.
- **Security Risks**: JavaScript can be used for attacks like Cross-Site Scripting (XSS), where malicious scripts are injected into a website to steal data
- **Performance**:  JavaScript is slower than traditional languages for complex tasks, but for simple tasks in a browser, performance is usually not a major issue.
- **Complexity**: To write advanced JavaScript, programmers need to understand core programming concepts, objects, and both client- and server-side scripting, which can be challenging.

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
-   

**Temporal Dead Zone (TDZ)** refers to the period between the entering of a scope (such as a function or block) and the actual initialization of a variable declared with `let` or `const`. During this time, any reference to the variable before its initialization will throw a ReferenceError.
     


[🔼 Back to top](#-javascript-questions)

---

### TQ1. What are TypeScript interfaces?

Interfaces define the structure of an object and ensure type safety. Example:

```ts
interface Person {
  name: string;
  age: number;
}

const user: Person = { name: "John", age: 30 };
```

[🔼 Back to top](#-typescript-questions)
