# Typescript Interview Questions and Answers of 2025

Welcome to the **Typescript Interview Questions and Answers of 2025** repository! This collection is designed to help developers preparing for technical interviews by covering essential concepts, tricky questions, and expert answers from beginner to advance level.

## Table of Contents

| #   | Question                                                                       |
| --- | ------------------------------------------------------------------------------ |
| 1   | [What is Typescript?](#what-is-typescript)                                     |
| 2   | [Explain the data types of Typescript?](#explain-the-data-types-of-typescript) |

---

### What is Typescript?

Typescript is an oper-source, statically typed programming language developed and maintained by Microsoft. It act as a superset of JavaScript by adding optional type-checking and the features of object-oriented programming such as class, interface, modules etc.. into JavaScript.

- **Static type-check**: Allows developers to explicitly define types for variables, function parameters and return values, enabling type-checking during the development (compile-time) rather than solely at runtime, helping to catch errors earlier.
- **Compilation to JavaScript**: TypeScript code is not directly executed by browsers or Node.js. Instead, it needs to be compiled (or "transpiled") into plain JavaScript using the TypeScript Compiler (tsc). This generated JavaScript can then run on any platform that supports JavaScript.

[🔼 Back to top](#table-of-contents)

### Explain the data types of Typescript?

The data types of Typescript can been categrorised into three: Primitive, Non-Primitive (Object), and user defined data types.

_Primitive Types_: These are the simplest data types, copied by value.

1. **number**: represents numeric values (integers, floats, hex, binary, etc...).
2. **string**: represents text enclosed in single, double, or backticks.
3. **boolean**: represents either `true` or `false`.
4. **null**: represents an intentional absence of a value.
5. **undefined**: depresents a variable that has been declared but not assigned a value.
6. **any**: disables type checking, allows any type of value.
7. **unknown**: similar to `any` but requires type-checking before use.
8. **void**: used for functions that return any value.
9. **never**: represents values that never occur (e.g., a function that always throws an `error`).
10. **symbol**: represents a unique and immutable identifier.
11. **bigint**: represents large integers beyond `Number.MAX_SAFE_INTEGER`.

_Non-primitive_: These include collections and reference types, meaning they store memory reference rather than actual value.

1. **object**: general object.
2. **array**: represents a list of values of the same type (`string[]`, `number[]`).
3. **tuple**: represents a fixed-length array with specific types (`[string, number]`).
4. **function**: callable object with parameters + return type
5. **class**: blueprint for objects.

_User defined_: These are for creating your own types, helps builing strongly-typed, reusable structures.

1. **enum**: defines a set of named constants (numeric or string values).
2. **interface**: defines the shape of an object.
3. **type alias**: custom type definitions.
4. **union** (|): variable can hold multiple types (`string | number`)
5. **intersection** (&): combine multiple types (`A & B`)

[🔼 Back to top](#table-of-contents)
