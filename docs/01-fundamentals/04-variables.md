# Variables

**Variables are used to store data. Think of a variable as a named container that holds a value.**

### Creating Variables

You can create a variable using the `let` keyword:
```
let greeting
```

You can assign a value to it using the assignment operator `=`:
```
let greeting
greeting = "Good Morning!"
```

You can also declare and assign in one line:
```
let greeting = "Good Morning!"
```

To use the value stored in a variable:
```
let greeting = "Good Morning!"
console.log(greeting)
```

### Declaring Multiple Variables**

You can declare multiple variables:
```
let name = 'John Doe'
let age = 25
let greeting = 'Good Morning!'
```

Although JavaScript allows multiple variables in one line:
```
let name = 'John Doe', age = 25, greeting = 'Good Morning!'
```

**It’s better to use one variable per line for readability.**

### How Variables Work

A variable acts like a labeled box that stores a value.
```
let greeting = "Good Morning!"
```

You can change the value anytime:
```
let greeting = "Good Morning!"
greeting = "Good Night!"
```

You can also copy values between variables:
```
let greeting = "Good Morning!"
let message = greeting

console.log(message)
```

A variable should only be declared once:
```
let greeting = "Good Morning!"
let greeting = "Good Night!"
```

> ##### `let` vs `var`
> You may also see `var`:
> ```
> var greeting = "Good Morning!"
> ```
> * `var` is older and behaves differently in some cases.
> * `let` is modern and recommended for most use cases.

### Variable Naming Rules

A variable name must follow these rules:

1. Can contain letters, digits, $, and _
2. Cannot start with a digit
```
let userName
let $price
let _count
```

### Naming Conventions

Use **camelCase** for multi-word names:
```
let firstName
let totalPrice
```

JavaScript is case-sensitive:
```
let apple
let Apple // different variable
```

Avoid non-English names (even though allowed):
```
let имя = "...";
let 我 = "...";
```

Reserved words cannot be used:
```
let let = 5      // Error
let return = 10  // Error
```

### Strict Mode and Undeclared Variables

If you don’t declare a variable, JavaScript may create it automatically (not recommended):
```
num = 5
```
In strict mode, this throws an error:
```
"use strict"
num = 5 // Error
```

### Constants (`const`)

Use `const` for values that should not change:
```
const birthYear = 2000
```

Trying to change it will cause an error:
```
const birthYear = 2000
birthYear = 1999 // Error
```

### Naming Constants

Use uppercase for fixed values:
```
const PI = 3.14
const MAX_USERS = 100
```

Use normal naming if the value is assigned later:
```
const pageLoadTime = 200 // value determined at runtime
```

### Choosing Good Variable Names

Good variable names make code easier to understand.

**Best Practices**

Use clear and meaningful names:
```
let userName
let cartTotal
```

Avoid vague names:
```
let data  // bad
let value // unclear
```

Avoid unnecessary short names:
```
let a, b, c // only okay in small contexts
```

Be consistent:
```
let currentUser
let newUser
```

## Summary

* Use `let` to declare variables.
* Use `const` for values that should not change.
* Avoid using `var` in modern code.
* Always choose meaningful variable names.
