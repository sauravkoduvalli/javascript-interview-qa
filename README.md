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
| 1  | [What is the difference between `null` and `undefined`?](#q1) |
| 2  | [Explain event delegation in JavaScript.](#q2) |
| 3  | [What is a closure in JavaScript?](#q3) |
| 4  | [How does prototypal inheritance work?](#q4) |
| 5  | [What is the difference between `let`, `const`, and `var`?](#q5) |

---

## 📌 TypeScript Questions

| #  | Question |
|----|----------|
| 1  | [What are TypeScript interfaces?](#tq1) |
| 2  | [Explain TypeScript generics with an example.](#tq2) |
| 3  | [What is the `readonly` modifier in TypeScript?](#tq3) |

---

### Q1: What is the difference between `null` and `undefined`? {#q1}

**Answer:**
- `null` is an assigned value that represents "no value".
- `undefined` means a variable has been declared but has not been assigned a value.

```js
let a = null;
let b;
console.log(a); // null
console.log(b); // undefined
```

[🔼 Back to top](#-javascript-questions)

---

### Q2: Explain event delegation in JavaScript. {#q2}

**Answer:**
Event delegation is a technique that leverages event bubbling. Instead of adding event listeners to individual child elements, you can place a single event listener on a parent element and use `event.target` to determine which child was clicked.

```js
document.getElementById("parent").addEventListener("click", function (event) {
  if (event.target.matches("button")) {
    console.log("Button clicked!", event.target.textContent);
  }
});
```

[🔼 Back to top](#-javascript-questions)

---

### TQ1: What are TypeScript interfaces? {#tq1}

**Answer:**
Interfaces define the structure of an object and ensure type safety. Example:

```ts
interface Person {
  name: string;
  age: number;
}

const user: Person = { name: "John", age: 30 };
```

[🔼 Back to top](#-typescript-questions)
