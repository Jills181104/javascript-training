# JavaScript Fundamentals -- Part 1

## 1. What is JavaScript?

JavaScript is a high-level, object-oriented and multi-paradigm
programming language. It is mainly used to make websites interactive and
build web applications.

It is also dynamically typed, so JavaScript figures out a value's data
type automatically.

## 2. Role in Web Development

Web development mainly uses three technologies:

- **HTML -- Content:** Creates the structure of a webpage.
- **CSS -- Presentation:** Controls how the webpage looks.
- **JavaScript -- Behaviour:** Adds actions and interactivity.

For example, HTML creates a button, CSS styles it, and JavaScript makes
it respond when clicked.

## 3. What Can JavaScript Be Used For?

JavaScript can: - Add dynamic effects to webpages. - Show or update
content without reloading the page. - Display loading indicators while
data is being fetched. - Build front-end applications using tools such
as React, Angular and Vue. - Build back-end applications with Node.js. -
Create mobile and desktop applications using tools such as React Native
and Electron.

## 4. JavaScript Versions

JavaScript follows the **ECMAScript (ES)** standard.

Some important versions are:

Version Year

---

ES5 2009
ES6 / ES2015 2015
ES7 / ES2016 2016
ES8 / ES2017 2017
ES9 / ES2018 2018
ES10 / ES2019 2019
ES11 / ES2020 2020

ES6 was a major update. The term **Modern JavaScript** generally refers
to the newer features introduced from ES6 onwards.

## 5. Objects and Primitive Values

JavaScript values are either objects or primitives.

**Object:** Stores related information using properties.

```javascript
let person = {
  name: "Jonas",
};
```

**Primitive:** A basic value that is not an object.

```javascript
let firstName = "Jonas";
let age = 30;
```

## 6. The 7 Primitive Data Types

Type Meaning Example

---

Number Integers and decimal numbers `let age = 23;`
String Text `let name = "Jonas";`
Boolean `true` or `false` `let isStudent = true;`
Undefined Declared but not assigned a value `let children;`
Null Intentionally empty value `let result = null;`
Symbol A unique value `let id = Symbol("id");`
BigInt Very large integers `let big = 12345678901234567890n;`

Symbol was introduced in ES2015, while BigInt was introduced in ES2020.

## 7. Dynamic Typing

JavaScript is dynamically typed. We do not need to specify a variable's
type when declaring it. The type depends on the value currently stored
in the variable.

```javascript
let age = 23; // Number
age = "Twenty-three"; // String
```

The same variable can hold values of different types.

## 8. Boolean Logic

Boolean logic works with two values: `true` and `false`. JavaScript has
three basic logical operators.

### AND (`&&`)

Returns `true` only when **both conditions are true**.

A B A && B

---

true true true
true false false
false true false
false false false

```javascript
let hasLicense = true;
let hasGoodVision = true;

console.log(hasLicense && hasGoodVision); // true
```

### OR (`||`)

Returns `true` if **at least one condition is true**. It returns false
only when both are false.

A B A \|\| B

---

true true true
true false true
false true true
false false false

```javascript
let hasLicense = true;
let hasGoodVision = false;

console.log(hasLicense || hasGoodVision); // true
```

### NOT (`!`)

Reverses a Boolean value: true becomes false, and false becomes true.

```javascript
let isTired = true;

console.log(!isTired); // false
```

## 9. Boolean Logic Example

```javascript
let age = 16;

let isAdult = age >= 20; // false
let isUnder30 = age < 30; // true

console.log(!isAdult); // true
console.log(isAdult && isUnder30); // false
console.log(isAdult || isUnder30); // true
console.log(!isAdult && isUnder30); // true
```

The result depends on whether each condition evaluates to true or false.
