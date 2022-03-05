# Type script  
- prerequisities: Javascript

Chapters:

1. Introduction
2. Environment setup
3. First Typescript program
4. Data Types - built-in

   - number, string, boolean, void, undefined, null

5. Data Types - user-defined

   - union type
   - Array type
   - tuple type
   - enum type
   - any type
   - object type
   - custom type

6. class

   - class basic, object
   - inheritance
   - abstract class
   - Encapsulation and access modifiers

7. interface
8. Generic
9. Module- export, import
10. typescript configuration
11. Build tools
12. convert js project to ts

### 1. Introduction

#### 1.1 What is TypeScript?

- In a simple words, Types + JavaScript = TypeScript
- It is a superset of JS
- developed and maintained by Microsoft  

#### 1.2 Why TypeScript?

- JS Check types in run time while typescript add static typing to JS so we can handle errors before running the program.
- increase readability and code quality
- popular JS libraray Angular use TypeScript.
- It can be used in both: client and server side.
- Intellisense IDE Support while coding: code completion, content assist and code hinting  

#### 1.3 Example:

```js
// index.js
// without typescript
function addNumbers(num1, num2) {
  console.log(num1 + num2);
}

addNumbers(20, 30);
addNumbers(20, "30");

// with typescript
// without typescript
function addNumbers(num1: number, num2: number) {
  console.log(num1 + num2);
}

addNumbers(20, 30); // no error
addNumbers(20, "30"); // error

// without typescript
let x;
x = 20; // correct
x = "anisul"; // correct
x = true; // correct
x = [10, 20]; // correct

// with typescript
let x: number;
x = 20; // correct
x = "20"; // Not correct
x = true; // Not correct
x = [10, 20]; // Not correct
```
