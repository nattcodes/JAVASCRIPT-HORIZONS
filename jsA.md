### **1. Variable and Scope**

#### Task: Variable Declaration and Scope Understanding

**Solution:**

```javascript
// Global Scope
var globalVar = "I am global"; // Accessible anywhere
let globalLet = "I am also global";
const globalConst = "I never change globally";

function testScope() {
  // Function Scope
  var functionVar = "I exist only in this function";
  if (true) {
    // Block Scope
    let blockLet = "I exist only in this block";
    const blockConst = "I am also block-scoped";
    console.log(blockLet); // Accessible here
    console.log(blockConst); // Accessible here
  }
  // console.log(blockLet); // Error: blockLet is not defined
}

testScope();
// console.log(functionVar); // Error: functionVar is not defined
```

---

### **2. Operators**

#### Task: Arithmetic Operations

**Solution:**

```javascript
let num1 = 10,
  num2 = 5;
console.log("Addition:", num1 + num2); // 15
console.log("Subtraction:", num1 - num2); // 5
console.log("Multiplication:", num1 * num2); // 50
console.log("Division:", num1 / num2); // 2
console.log("Modulus:", num1 % num2); // 0
```

#### Task: Type Conversion

**Solution:**

```javascript
let userInput = "42"; // String input
let converted = Number(userInput);
console.log(typeof converted, converted); // number 42
```

#### Task: Associativity Challenge

**Solution:**

```javascript
let a = 10,
  b = 20,
  c = 30;
console.log(a - b - c); // -40 (Left-to-right for subtraction)
console.log((a = b = c)); // 30 (Right-to-left for assignment)
```

---

### **3. Control Flow Statements**

#### Task: Grading System

**Solution:**

```javascript
let score = 85;
if (score >= 90) {
  console.log("Grade: A");
} else if (score >= 80) {
  console.log("Grade: B");
} else if (score >= 70) {
  console.log("Grade: C");
} else if (score >= 60) {
  console.log("Grade: D");
} else {
  console.log("Grade: F");
}
```

```javascript
let dayNumber = 3; // Example input; you can change this to test different values.

switch (dayNumber) {
  case 1:
    console.log("Monday");
    break;
  case 2:
    console.log("Tuesday");
    break;
  case 3:
    console.log("Wednesday");
    break;
  case 4:
    console.log("Thursday");
    break;
  case 5:
    console.log("Friday");
    break;
  case 6:
    console.log("Saturday");
    break;
  case 7:
    console.log("Sunday");
    break;
  default:
    console.log("Invalid input! Please enter a number between 1 and 7.");
}
```

```javascript
let age = 18; // Example input; change this to test different values.

let message =
  age >= 18 ? "You are old enough to vote!" : "You are not old enough to vote.";

console.log(message);
```

#### Task: Fibonacci Sequence

**Solution:**
Using `for`:

```javascript
let n1 = 0,
  n2 = 1,
  nextTerm;
for (let i = 1; i <= 10; i++) {
  console.log(n1);
  nextTerm = n1 + n2;
  n1 = n2;
  n2 = nextTerm;
}
```

Using `while`:

```javascript
let count = 1,
  first = 0,
  second = 1,
  next;
while (count <= 10) {
  console.log(first);
  next = first + second;
  first = second;
  second = next;
  count++;
}
```

#### Task: Array and Object Traversal

**Solution:**
Using `forEach` for an array:

```javascript
let array = [10, 20, 30];
array.forEach((value, index) => {
  console.log(`Index ${index}: Value ${value}`);
});
```

Using `for...in` for an object:

```javascript
let obj = { name: "John", age: 25, city: "New York" };
for (let key in obj) {
  console.log(`${key}: ${obj[key]}`);
}
```

---

### **4. Functions**

#### Task: Sum Function

**Solution:**

```javascript
function sum(a, b) {
  return a + b;
}
console.log(sum(5, 7)); // 12
```

#### Task: Factorial Calculation (Recursive Function)

**Solution:**

```javascript
function factorial(n) {
  if (n === 0 || n === 1) {
    return 1;
  }
  return n * factorial(n - 1);
}
console.log(factorial(5)); // 120
```

#### Task: Default Parameters

**Solution:**

```javascript
function greet(name = "Guest") {
  console.log(`Hello, ${name}!`);
}
greet(); // Hello, Guest!
greet("Alice"); // Hello, Alice!
```

---

Let me know if you'd like me to proceed with answers for the remaining sections! 😊
