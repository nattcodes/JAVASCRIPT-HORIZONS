### **JavaScript (Problem 3)**

### 1 **Comprehensive JavaScript Guide Outline**

1. **What is JavaScript?**
2. **Install a JavaScript Source Code Editor**
3. **Use the Console Tab of Web Development Tools**
4. **Writing Your First JavaScript Code (External Script)**

---

### 2 **Core JavaScript Concepts**

1. **Variable and Scope**

   - Global Scope
   - Local Scope
   - Block Scope (Let and Const)

2. **Operators and Statements**

   - Operators (e.g., Arithmetic, Logical, Assignment)
   - Statements (e.g., Expression Statements, Control Statements)

3. **Keywords and Reserved Words**

   - Examples of Reserved Words
   - Usage Restrictions

4. **Expressions**

   - Arithmetic Expressions
   - Logical Expressions
   - String Expressions

5. **Data Types**

   - Primitive Types:
     - String
     - Number
     - Boolean
     - Null
     - Undefined
   - Reference Types:
     - Object
     - Array

6. **Primitive vs. Reference Values**
   - Differences
   - Memory Allocation
   - Examples with Arrays and Objects

---

### 4 **Operators in Detail**

1. **Arithmetic Operators**

   - Addition (`+`)
   - Subtraction (`-`)
   - Multiplication (`*`)
   - Division (`/`)
   - Modulus (`%`)
   - Exponentiation (`**`)

2. **Assignment Operators**

   - Simple Assignment (`=`)
   - Compound Assignments (e.g., `+=`, `-=`, `*=`, `/=`)

3. **Logical Operators**

   - AND (`&&`)
   - OR (`||`)
   - NOT (`!`)

4. **Equality Operators**

   - Strict Equality (`===`)
   - Loose Equality (`==`)
   - Not Equal (`!=`, `!==`)

5. **Relational/Comparison Operators**

   - Greater Than (`>`)
   - Less Than (`<`)
   - Greater Than or Equal To (`>=`)
   - Less Than or Equal To (`<=`)

6. **Increment/Decrement Operators**

   - Postfix (`x++`, `x--`)
   - Prefix (`++x`, `--x`)

7. **Type Conversion Operators**

   - Implicit Conversion
   - Explicit Conversion (e.g., `Number()`, `String()`)

8. **Operator Precedence and Associativity**
   - Precedence Rules
   - Associativity Examples

---

### 5 **Control Flow Statements**

- **If-Else Statements**
- **Switch Statements**
- **Ternary Operator**

---

### 6 **Loops**

- **For Loop**
- **While Loop**
- **Do-While Loop**
- **forEach Loop**
- **for...in Loop**
- **Break and Continue**

---

### 7 **Functions**

- **Function Declaration**
- **Arrow Functions**
- **Default Parameters**
- **Recursive Functions**

---

### 8 **Objects and Prototypes**

- **Objects (Key-Value Pairs)**
- **Methods**
- **Constructor Functions**
- **Prototypes**
- **Object Destructuring**
- **Object Literal Syntax Extensions**

---

### 9 **DOM (Document Object Model)**

1. **Core Concepts**
   - Text Node
   - Element Node
   - Child Node
   - Parent Node
   - Descendant Node
   - Sibling Node
2. **Query/Get Elements**
3. **Create and Clone Elements**
4. **Add Nodes to the Document**
5. **Modify Element Content and Attributes**
6. **Get and Modify Element Class**
7. **Remove Node**
8. **Event Listeners**
   - Add Event Listener
   - Remove Event Listener
9. **Event Flow**
   - Capturing Phase
   - Target Phase
   - Bubbling Phase

## **What is JavaScript?**

JavaScript is a high-level, interpreted programming language primarily used to add interactivity, control multimedia, and dynamically update content on web pages. Unlike HTML and CSS, which structure and style a webpage, JavaScript enables dynamic functionalities such as animations, form validations, and API integration.

### Key Features:

- **Lightweight:** Designed to run in browsers without consuming much memory.
- **Interpreted:** Does not require compilation; executed directly in browsers.
- **Versatile:** Can be used for front-end (browser), back-end (Node.js), and even mobile development.
- **Object-Oriented:** Allows the use of objects for structuring data and behavior.

---

## **Install a JavaScript Source Code Editor**

A source code editor simplifies writing and debugging JavaScript code.

### Recommended Editors:

1. **Visual Studio Code (VS Code):**

   - Lightweight and fast.
   - Features intelligent code completion, debugging, and extensions.
   - Download: [https://code.visualstudio.com/](https://code.visualstudio.com/)

2. **Sublime Text:**

   - Known for speed and simplicity.
   - Offers features like syntax highlighting and multi-selection editing.
   - Download: [https://www.sublimetext.com/](https://www.sublimetext.com/)

3. **Atom:**
   - Open-source and customizable.
   - Perfect for collaborative projects.
   - Download: [https://atom.io/](https://atom.io/)

---

## **Use the Console Tab of Web Development Tools**

### What is the Console?

The **console** is part of a browser's developer tools, allowing developers to:

- Test and debug JavaScript code.
- Log outputs for troubleshooting.
- Interact with the DOM dynamically.

### How to Open the Console:

1. Open any modern browser (e.g., Chrome, Firefox).
2. Press `Ctrl + Shift + I` (Windows/Linux) or `Cmd + Option + I` (Mac) to open Developer Tools.
3. Navigate to the **Console** tab.

### Example:

Type the following in the console and press Enter:

```javascript
console.log("Hello, Console!");
```

The console will display:

```
Hello, Console!
```

---

## **Writing Your First JavaScript Code (External Script)**

### Why Use External Scripts?

- **Separation of Concerns:** Keeps HTML clean and modular.
- **Reusability:** The same script file can be used across multiple pages.
- **Easier Maintenance:** Modifications in the external file automatically apply to all linked pages.

### Example:

1. **HTML File (`index.html`):**

   ```html
   <!DOCTYPE html>
   <html lang="en">
     <head>
       <meta charset="UTF-8" />
       <meta name="viewport" content="width=device-width, initial-scale=1.0" />
       <title>JavaScript Demo</title>
     </head>
     <body>
       <h1>Welcome to JavaScript</h1>
       <p>Check the console for output.</p>
       <!-- Link to External JavaScript -->
       <script src="script.js"></script>
     </body>
   </html>
   ```

2. **JavaScript File (`script.js`):**

   ```javascript
   console.log("Hello, World!");
   ```

3. Open the `index.html` file in a browser and view the console to see:
   ```
   Hello, World!
   ```

---

---

## **Variable and Scope of Variable**

### Variables:

Variables store data that can be used or manipulated in a program. In JavaScript, variables can be declared using `var`, `let`, or `const`.
var and let create variables that can be reassigned another value.
const creates "constant" variables that cannot be reassigned another value.

Variable names must start with a letter, an underscore ( \_ ) or a dollar sign ( $ ). Variable names cannot contain spaces. Variables cannot be the same as reserved keywords such as if or const . By convention, JavaScript variable names are written in camelCase.

- **`var`:** Global or function-scoped (not block-scoped).
- **`let`:** Block-scoped.
- **`const`:** Block-scoped, immutable (value cannot be reassigned).

```javascript
var globalVar = "I am global"; // Can be accessed anywhere
let blockVar = "I am block-scoped"; // Limited to block
const constantVar = "I am constant"; // Cannot be reassigned
```

### Scope:

Scope in Javascript refers to the visibility of variables and functions within a program.

- **Global Scope:** Variables accessible anywhere in the code.
- **function Scope:** Variables declared inside functions or blocks.
- **Block Scope:** Variables declared using `let` or `const` within curly braces `{}`.

```javascript
function localScopeExample() {
  let localVar = "I'm local!";
  console.log(localVar);
}
localScopeExample();
// console.log(localVar); // Error: localVar is not defined
```

---

## **Operators and Statements**

### Operators:

Operators are symbols or keywords that perform operations on operands.

- **Arithmetic Operators:** Perform mathematical calculations (`+`, `-`, `*`, `/`, `%`, `**`).
- **Assignment Operators:** Assign values (`=`, `+=`, `-=`).
- **Logical Operators:** Perform logical operations (`&&`, `||`, `!`).

```javascript
let a = 10;
let b = 5;
console.log(a + b); // Arithmetic: 15
console.log(a > b && b > 0); // Logical: true
a += b; // Assignment
console.log(a); // 15
```

### Statements:

Statements execute instructions, such as conditionals (`if`), loops (`for`), and declarations.

---

## **Keywords and Reserved Words**

Keywords are predefined words in JavaScript with special meanings. Reserved words cannot be used as variable or function names.

### Examples:

- **Keywords:** `let`, `const`, `function`, `return`, `if`, `else`, etc.
- **Reserved Words:** `class`, `enum`, `extends`, `interface`, etc.

```javascript
let returnValue = "Valid";
const enum = "Invalid"; // Error: 'enum' is a reserved word
```

---

## **Expressions**

Expressions produce values. Examples include:

1. **Arithmetic Expressions:**
   ```javascript
   let result = 10 + 5; // 15
   ```
2. **Logical Expressions:**
   ```javascript
   let isTrue = 5 > 3 && 2 < 4; // true
   ```
3. **String Expressions:**
   ```javascript
   let greeting = "Hello" + " " + "World!"; // "Hello World!"
   ```

---

## **Data Types**

### **What is a Data Type?**

A **data type** defines the kind of value a variable can hold in a programming language. It determines how the data is stored in memory, how it can be manipulated, and what operations are permitted. JavaScript is a dynamically typed language, meaning variables do not need to be explicitly assigned a type when declared; their type is inferred based on the value they hold.

### **Primitive Data Types in JavaScript**

Primitive data types are the most basic building blocks of data in JavaScript. They are immutable, meaning their values cannot be changed once created. JavaScript has **7 primitive data types**:

---

1. **String**  
   Represents a sequence of characters. Strings are used for text.

   **Examples:**

   ```javascript
   let singleQuote = "Hello!";
   let doubleQuote = "World!";
   let templateLiteral = `Hello, ${singleQuote}`;
   console.log(typeof singleQuote); // "string"
   ```

---

2. **Number**  
   Represents numeric values, including integers and floating-point numbers. JavaScript uses a single `Number` type to represent all numbers.

   **Examples:**

   ```javascript
   let integer = 42;
   let float = 3.14;
   let negative = -7;
   let infinityValue = Infinity; // Represented by `Infinity`
   let notANumber = NaN; // Result of invalid numeric operations
   console.log(typeof integer); // "number"
   ```

---

3. **BigInt**  
   Represents numbers larger than the safe integer limit for the `Number` type (`2^53 - 1`). It is used for extremely large integers.

   **Examples:**

   ```javascript
   let bigIntValue = 1234567890123456789012345678901234567890n;
   console.log(typeof bigIntValue); // "bigint"
   ```

---

4. **Boolean**  
   Represents logical values: `true` or `false`. Booleans are often used in conditional statements and logical operations.

   **Examples:**

   ```javascript
   let isJavaScriptFun = true;
   let isJavaScriptDifficult = false;
   console.log(typeof isJavaScriptFun); // "boolean"
   ```

---

5. **Undefined**  
   Represents a variable that has been declared but not yet assigned a value. It is the default value for uninitialized variables.

   **Examples:**

   ```javascript
   let uninitialized;
   console.log(uninitialized); // undefined
   console.log(typeof uninitialized); // "undefined"
   ```

---

6. **Null**  
   Represents an intentional absence of any object value. It is used when a variable is explicitly set to have no value.

   **Examples:**

   ```javascript
   let empty = null;
   console.log(empty); // null
   console.log(typeof empty); // "object" (this is a known quirk in JavaScript)
   ```

---

7. **Symbol**  
   Represents a unique and immutable identifier, often used as object property keys to avoid name clashes.

   **Examples:**

   ```javascript
   let symbol1 = Symbol("id");
   let symbol2 = Symbol("id");
   console.log(symbol1 === symbol2); // false (each Symbol is unique)
   console.log(typeof symbol1); // "symbol"
   ```

---

### **Key Characteristics of Primitive Data Types**

- **Immutability:** The actual value of a primitive type cannot be changed; operations create new values.
- **Stored by Value:** Primitive types are stored directly in the variable's memory location, not as references.
- **Fixed Behavior:** Their operations and limits are predefined.

## **Operators**

Operators are symbols or keywords used to perform operations on values (operands) in JavaScript. They allow you to manipulate data, perform calculations, compare values, and control the flow of a program.

### 1. Arithmetic Operators:

Used for mathematical calculations.

```javascript
let x = 10,
  y = 2;
console.log(x + y); // 12
console.log(x ** y); // 100 (Exponentiation)
```

### 2. Assignment Operators:

```javascript
let a = 5;
a += 2; // a = a + 2
console.log(a); // 7
```

### 3. Logical Operators:

Used to combine or invert conditions.

```javascript
let isTrue = true && false; // false
```

### 4. Equality Operators:

```javascript
console.log(5 == "5"); // true (loose equality)
console.log(5 === "5"); // false (strict equality)
```

### 5. Relational Operators:

```javascript
console.log(10 > 5); // true
```

### 6. Increment/Decrement:

```javascript
let count = 0;
console.log(++count); // 1 (prefix)
console.log(count++); // 1 (postfix)
```

### 7. Operator Precedence:

```javascript
console.log(3 + 5 * 2); // 13 (* has higher precedence than +)
```

### 8. Operator Associativity:

```javascript
console.log(10 - 5 - 2); // 3 (evaluates left-to-right)
```

---

## **Control Flow Statements**

Control flow statements allow you to manage the execution path of your code.

### **If-Else Statements**

Used to execute code based on conditions.

```javascript
let score = 80;

if (score >= 90) {
  console.log("Grade: A");
} else if (score >= 75) {
  console.log("Grade: B");
} else {
  console.log("Grade: C");
}
```

### **Switch Statements**

Ideal for multiple conditions.

```javascript
let day = "Monday";

switch (day) {
  case "Monday":
    console.log("Start of the week!");
    break;
  case "Friday":
    console.log("Almost weekend!");
    break;
  default:
    console.log("Midweek vibes!");
}
```

### **Ternary Operator**

A concise way to write conditional expressions.

```javascript
let age = 18;
let message = age >= 18 ? "You are an adult." : "You are a minor.";
console.log(message);
```

---

## **Loops**

Loops allow repetitive execution of code.

### **For Loop**

Executes a block of code a fixed number of times.

```javascript
for (let i = 0; i < 5; i++) {
  console.log(i); // Output: 0, 1, 2, 3, 4
}
```

### **While Loop**

Executes while the condition is true.

```javascript
let i = 0;
while (i < 5) {
  console.log(i);
  i++;
}
```

### **Do-While Loop**

Executes at least once before checking the condition.

```javascript
let i = 0;
do {
  console.log(i);
  i++;
} while (i < 5);
```

### **forEach Loop**

Iterates over each element in an array.

```javascript
const fruits = ["Apple", "Banana", "Cherry"];
fruits.forEach((fruit, index) => {
  console.log(`${index}: ${fruit}`);
});
// Output:
// 0: Apple
// 1: Banana
// 2: Cherry
```

### **for...in Loop**

Iterates over the keys of an object.

```javascript
const person = {
  name: "Alice",
  age: 25,
  job: "Engineer",
};
for (let key in person) {
  console.log(`${key}: ${person[key]}`);
}
// Output:
// name: Alice
// age: 25
// job: Engineer
```

### **Break and Continue**

- **Break:** Terminates the loop.
- **Continue:** Skips the current iteration.

```javascript
for (let i = 0; i < 10; i++) {
  if (i === 5) break;
  if (i % 2 === 0) continue;
  console.log(i); // Output: 1, 3
}
```

---

## **Functions**

Functions are reusable blocks of code that performs a specific task. You define it once.

### Function Declaration

```javascript
function greet(name) {
  return `Hello, ${name}!`;
}
console.log(greet("Alice")); // Output: Hello, Alice!
```

### Arrow Functions

A shorter syntax for functions.

```javascript
const add = (a, b) => a + b;
console.log(add(5, 3)); // Output: 8
```

### Default Parameters

Set default values for parameters.

```javascript
function greet(name = "Guest") {
  return `Hello, ${name}!`;
}
console.log(greet()); // Output: Hello, Guest!
```

### Recursive Function

A function that calls itself.

```javascript
function factorial(n) {
  return n === 1 ? 1 : n * factorial(n - 1);
}
console.log(factorial(5)); // Output: 120
```

---

## **Objects and Prototypes**

Objects are collections of key-value pairs.

### Example Object:

```javascript
const person = {
  name: "Alice",
  age: 25,
  greet() {
    console.log(`Hi, I'm ${this.name}`);
  },
};
person.greet(); // Output: Hi, I'm Alice
```

### Prototypes

Allow inheritance of methods.

```javascript
function Person(name, age) {
  this.name = name;
  this.age = age;
}
Person.prototype.sayHello = function () {
  console.log(`Hello, I'm ${this.name}`);
};
const john = new Person("John", 30);
john.sayHello(); // Output: Hello, I'm John
```

---

## **What is the DOM (Document Object Model)?**

The DOM is a programming interface for web documents. It represents the structure of an HTML or XML document as a tree-like structure where each node is an object representing a part of the document (e.g., elements, attributes, text).

### Why is the DOM Important?

- **Dynamic Interaction:** JavaScript uses the DOM to dynamically update, add, or remove elements and content.
- **Event Handling:** It enables interaction between users and web applications through event listeners.
- **Traversal and Manipulation:** Allows navigation through parent, child, and sibling nodes and manipulation of their content or attributes.

### Core DOM Concepts

1. **Text Node:** Represents the text content of an element or attribute.

   ```html
   <p>Hello, World!</p>
   ```

   The text "Hello, World!" is a text node.

2. **Element Node:** Represents an HTML or XML element.

   ```html
   <p>Hello, World!</p>
   ```

   The `<p>` tag is an element node.

3. **Child Node:** Any node that is a direct descendant of another node.

   ```html
   <div>
     <p>This is a child node.</p>
   </div>
   ```

4. **Parent Node:** The node that contains a child node.

   ```html
   <div>
     <!-- Parent node -->
     <p>Child node</p>
   </div>
   ```

5. **Descendant Node:** Any node nested within another node (not limited to direct children).
6. **Sibling Node:** Nodes that share the same parent.

---

## **DOM Manipulation and Examples**

### **Query/Get Elements**

Retrieve elements from the DOM using different methods.

- By **ID**:
  ```javascript
  let element = document.getElementById("title");
  console.log(element.textContent);
  ```
- By **Class Name**:
  ```javascript
  let elements = document.getElementsByClassName("items");
  console.log(elements[0]);
  ```
- By **Tag Name**:
  ```javascript
  let paragraphs = document.getElementsByTagName("p");
  console.log(paragraphs);
  ```
- By **CSS Selector**:
  ```javascript
  let button = document.querySelector(".btn");
  console.log(button);
  ```

---

### **Create and Clone Elements**

- **Create an Element**:

  ```javascript
  let newElement = document.createElement("div");
  newElement.textContent = "This is a new div!";
  document.body.appendChild(newElement);
  ```

- **Clone an Element**:
  ```javascript
  let clonedElement = newElement.cloneNode(true);
  document.body.appendChild(clonedElement);
  ```

---

### **Add Nodes to the Document**

- **Append Child**:

  ```javascript
  let parent = document.getElementById("container");
  let child = document.createElement("span");
  child.textContent = "I'm a child!";
  parent.appendChild(child);
  ```

- **Insert Before**:
  ```javascript
  let reference = document.getElementById("reference");
  parent.insertBefore(child, reference);
  ```

---

### **Modify Element Content and Attributes**

- **Text Content**:

  ```javascript
  let title = document.getElementById("title");
  title.textContent = "New Title";
  ```

- **HTML Content**:

  ```javascript
  let container = document.getElementById("container");
  container.innerHTML = "<p>New Content</p>";
  ```

- **Attributes**:
  ```javascript
  let link = document.querySelector("a");
  link.setAttribute("href", "https://example.com");
  console.log(link.getAttribute("href"));
  ```

---

### **Get and Modify Element Class**

- **Add Class**:

  ```javascript
  let element = document.getElementById("box");
  element.classList.add("highlight");
  ```

- **Remove Class**:

  ```javascript
  element.classList.remove("highlight");
  ```

- **Toggle Class**:
  ```javascript
  element.classList.toggle("highlight");
  ```

---

### **Remove Node**

```javascript
let element = document.getElementById("box");
element.remove();
```

---

### **Event Listeners**

Event listeners let you run JavaScript when a specific event occurs.

- **Add an Event Listener**:

  ```javascript
  let button = document.querySelector("button");
  button.addEventListener("click", () => {
    console.log("Button was clicked!");
  });
  ```

- **Remove an Event Listener**:
  ```javascript
  const handleClick = () => console.log("Button was clicked!");
  button.addEventListener("click", handleClick);
  button.removeEventListener("click", handleClick);
  ```

---

## **JavaScript Event Flow**

Events in JavaScript follow a specific flow:

1. **Capturing Phase:** Event moves from the root to the target element.
2. **Target Phase:** Event reaches the target element.
3. **Bubbling Phase:** Event propagates back to the root.

### Example of Event Bubbling:

```javascript
document.querySelector("div").addEventListener("click", () => {
  console.log("Div clicked!");
});

document.querySelector("button").addEventListener("click", () => {
  console.log("Button clicked!");
});
```

Clicking the button will log:

```
Button clicked!
Div clicked!
```

---

## **Summary of the DOM**

The DOM enables dynamic, interactive web applications by providing methods to query, traverse, and manipulate the document structure. Mastering the DOM unlocks the full potential of JavaScript in web development. Use the methods and concepts outlined here to build user-driven, responsive web applications.
