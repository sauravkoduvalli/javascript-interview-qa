# 🚀 JavaScript & TypeScript Interview Questions and Answers

Welcome to the **JavaScript Interview Questions and Answers** repository! This collection is designed to help developers prepare for technical interviews by covering essential concepts, tricky questions, and expert answers. 🌟

---

## 📌 JavaScript Questions

| #   | Question                                                                                                                           |
| --- | ---------------------------------------------------------------------------------------------------------------------------------- |
| 1   | [What is JavaScript?](#what-is-javascript)                                                                                         |
| 2   | [Is JavaScript a compiled or interpreted language or both?](#is-javascript-a-compiled-or-interpreted-language-or-both)             |
| 3   | [What is the difference between `let`, `const`, and `var` keywords?](#what-is-the-difference-between-let-const-and-var-keywords)   |
| 4   | [Explain the concept of Hoisting?](#explain-the-concept-of-hoisting)                                                               |
| 5   | [What is Temporal Dead Zone (TDZ)?](#what-is-temporal-dead-zone-tdz)                                                               |
| 6   | [How does hoisting affect function declarations and expressions?](#how-does-hoisting-affect-function-declarations-and-expressions) |
| 7   | [What are the different data types in JavaScript?](#what-are-the-different-data-types-in-javascript)                               |
| 8   | [Different types of scopes in JavaScript?](#different-types-of-scopes-in-javascript)                                               |

---

### What is JavaScript?

JavaScript is a versatile, high-level, interpreted programming language created by **Brendan Eich** in 1995.

- It’s primarily used for building dynamic and interactive web applications.
- JavaScript is multi-paradigm—it supports object-oriented (prototype-based), functional, and imperative programming.
- Although single-threaded by design, it handles asynchronous operations efficiently through the event loop, callbacks, and Promises.
- Modern engines like V8 also JIT-compile JavaScript for performance.
- Beyond the browser, it’s widely used on the server-side with Node.js.

[🔼 Back to top](#-javascript-questions)

### Is JavaScript a compiled or interpreted language or both?

JavaScript is both compiled and interpreted. While JavaScript is fundamentally an interpreted language, JavaScript engines uses **Just-In-Time (JIT)** compilation in modern browsers. This means, the JavaScript code is compiled into machine code at runtime, just before it's executed. This makes JavaScript a compiled and interpreted programming language.

[🔼 Back to top](#-javascript-questions)

### What is the difference between `let`, `const`, and `var` keywords?

In JavaScript, variables are declared using the keywords `var`, `let` and `const`. They are differ in terms of scope, initialization, whether they can be redeclared or reassigned, and the behavior when they are accessed before declaration.

| Feature                   | `var`              | `let`            | `const`          |
| ------------------------- | ------------------ | ---------------- | ---------------- |
| Scope                     | Function or Global | Block            | Block            |
| Initialization            | optional           | optional         | required         |
| Re-declaration            | Allowed            | Not allowed      | Not allowed      |
| Re-assignment             | Allowed            | Allowed          | Not allowed      |
| Access before declaration | `undefined`        | `ReferenceError` | `ReferenceError` |

[🔼 Back to top](#-javascript-questions)

### Explain the concept of Hoisting?

Hoisting is a JavaScript mechanism of moving (hoisting) the declaration of variables, functions and classses to the top of their containing scope during the compilation phase.

- **Variable declaretion** (`var`): Declarations are hoisted but not initialisation. Accessing before initialisation return `undefined`.
- **Variable declaration** (`let` and `const`): Declarations are hoisted but not initialied. Accessing the variable before initialization throw `ReferenceError`.
- **Function expression** (`var`): Declarations are hoisted but not initialisation. the value of the variable is `undefined` if accessed before initialization.
- **Function declaration** (`function`): Both declaration and deefinition are fully hoiseted.
- **Class declaration** (`class`): Declarations are hoisted, but not initialized. Accessing them results in `ReferenceError` until the actual declaration is encoutered.
- **Import declaration**: (`import`): Declarations are hoisted, and side effects of importing the module are executed before the rest of the code.

| Declaration             | Accessing before initializing |
| ----------------------- | ----------------------------- |
| `var foo`               | `undefined`                   |
| `let foo`               | `ReferenceError`              |
| `const foo`             | `ReferenceError`              |
| `var foo = () => {...}` | `undefined`                   |
| `fucntion() {...}`      | Normal                        |
| `class foo`             | `ReferenceError`              |
| `import {} from ...`    | Normal                        |

[🔼 Back to top](#-javascript-questions)

### What is Temporal Dead Zone (TDZ)?

Temporal Dead Zone (TDZ) refers to the period between the entering of a scope (such as a function or block) and the actual initialization of a variable declared with `let` or `const`. During this time, any reference to the variable before its initialization will throw a `ReferenceError`.

[🔼 Back to top](#-javascript-questions)

### How does hoisting affect function declarations and expressions?

```javascript
// Function declaration
console.log(foo()); // Works fine
function foo() {
  return 'Hello';
}

// Function expression
console.log(bar()); // Throws TypeError: bar is not a function
var bar = function () {
  return 'Hello';
};

```

### What are the different data types in JavaScript?

Data Types in JavaScript can be categorized into primitive and non-primitive based on how they are stored, handled in memory, and how they behave during assignments and comparisons.

1. **Primitive Data Type** - values are immutable and are stored by value.

   - **Number**: Represents numeric values (integers and decimals).
   - **BigInt**: Represents integers larger than Number.MAX_SAFE_INTEGER.
   - **String**: Represents text enclosed in single or double quotes.
   - **Boolean**: Represents a logical value (`true` or `false`).
   - **Undefined**: A variable that has been declared but not assigned a value.
   - **Null**: Represents an intentional absence of any value.
   - **Symbol**: Represents unique and immutable values, often used as object keys.

2. **Non-Primitive Data Type** - values are mutable and stored by their reference in the memory

   - **Object**: Represents key-value pairs.
   - **Array**: An ordered collection of elements.
   - **Function**: Represents reusable blocks of code.
   - **Map**: An ordered collection of key-value pairs.
   - **Set**: An unordered collection of unique values.

[🔼 Back to top](#-javascript-questions)

### Different types of scopes in JavaScript?

###
