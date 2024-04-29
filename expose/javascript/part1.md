# Part 1. A Quick Introduction...
---
### var declaration 
1. Line 9 prints `values added: 20`.
2. Line 13 prints `final result: 20`.
### let declaration
3. Line 9 prints `values added: 20`.
4. Line 13 results in an error because the `result` variable is declared using the `let` keyword within the `if` statement. This keyword has a block scope, so when accessing `result` outside the `if` statement, it is out of scope and a ReferenceError occurs.
### const declaration
5. Line 9 results in an error because the `result` variable is declared using the `const` keyword within the `if` statement and assigned a value of `0`. This keyword has a TypeError because the code is trying to reassign a value to `result` but can not because it has been declared using `const`.
6. Line 13 results in an error because the `result` variable is declared using the `let` keyword which has a block scope and only acessible within the `if` statement it was declared in. When accessing `result` outside the `if` statement, it is out of scope and a ReferenceError occurs.
