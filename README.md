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
| 5  | [What is the difference between `let`, `const`, and `var`?](#q5) |

---

## 📌 TypeScript Questions

| #  | Question |
|----|----------|
| 1  | [What are TypeScript interfaces?](#tq1) |
| 2  | [Explain TypeScript generics with an example.](#tq2) |
| 3  | [What is the `readonly` modifier in TypeScript?](#tq3) |

---

### Q1. What is JavaScript?

JavaScript is a versatile, dynamically typed programming language used for interactive web applications, supporting both client-side and server-side development.

- JavaScript is a single-threaded language that executes one task at a time.
- It is an Interpreted language which means it executes the code line by line.
- The data type of the variable is decided at run-time in JavaScript that’s why it is called dynamically typed.
- JavaScript is considered a lightweight language due to its low CPU usage, minimalist syntax, and ease of implementation.

[🔼 Back to top](#-javascript-questions)


### Q2. Applications of JavaScript?

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


### Q3. What are the limitations of JavaScript?

- **Weak Type Checking**: JavaScript is weakly typed, meaning variables don’t require explicit types. This can lead to runtime errors.
- **Security Risks**: JavaScript can be used for attacks like Cross-Site Scripting (XSS), where malicious scripts are injected into a website to steal data
- **Performance**:  JavaScript is slower than traditional languages for complex tasks, but for simple tasks in a browser, performance is usually not a major issue.
- **Complexity**: To write advanced JavaScript, programmers need to understand core programming concepts, objects, and both client- and server-side scripting, which can be challenging.

[🔼 Back to top](#-javascript-questions)


### Q4. Is JavaScript Compiled or Interpreted or both?

JavaScript is both compiled and interpreted. While JavaScript is fundamentally an interpreted language, JavaScript engines uses **Just-In-Time (JIT)** compilation in modern browsers. This means that the JavaScript code is compiled into machine code at runtime, just before it's executed. This makes JavaScript a compiled and interpreted programming language.

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
