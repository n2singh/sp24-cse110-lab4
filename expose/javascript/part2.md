# Part 2. A Little More of a Challenge...
---
1. The code prints `3`. At line 12, the code will print the value of `i`, which will be equal to the length of `prices` array because `i` is defined using the `var` keyword inside the `for` loop. Therefore, `i` will still be accessible outside of the loop and its value will be the length of the `prices` array. 

2. The code prints `150`. At line 13, the code will print the value of `discountedPrice` for each iteration of the loop. This variable is declared using the `var` keyword inside the loop, which means it has function scope, allowing it to be accessed anywhere within the `discountPrices` function. Therefore, `discountedPrice` will be accessible and will hold the value calculated in each iteration of the loop.

3. The code prints `150`. At line 14, the code will print the value of `finalPrice`. Since `finalPrice` is declared using the `var` keyword inside the function scope, it's accessible anywhere within the `discountPrices` function. Therefore, when `console.log(finalPrice)` is executed, it will print the last calculated value of `finalPrice`, which is the final discounted price after all iterations of the loop.

4. This function will return an array: `[50, 100, 150]`. It calculates the discounted price for each item in the `prices` array by applying the provided discount percentage. The discounted prices are then rounded to two decimal places using `Math.round` and pushed into the `discounted array`. Finally, the function returns the array of discounted prices.

5. At line 12, a ReferenceError will occur because `i` is declared using the `let` keyword inside the `for` loop. Variables declared with `let` have block scope, and are only accessible within the block in which they are declared. Therefore, when trying to access `i` outside of the loop, it's out of scope, resulting in a ReferenceError.

6. At line 13, a ReferenceError will occur because `discountedPrice` is declared using the `let` keyword inside the `for` loop. Variables declared with `let` have block scope, and are only accessible within the block in which they are declared. Therefore, when trying to access `discountedPrice` outside of the loop, it's out of scope, resulting in a ReferenceError.

7. The code prints `150`. At line 14, the code will print the value of `finalPrice`. Since `finalPrice` is declared using the `let` keyword inside the function scope, it's accessible anywhere within the `discountPrices` function. Therefore, when `console.log(finalPrice)` is executed, it will print the last calculated value of `finalPrice`, which is the final discounted price after all iterations of the loop.

8. This function will return an array: `[50, 100, 150]`. It calculates the discounted price for each item in the `prices` array by applying the provided discount percentage. The discounted prices are then rounded to two decimal places using `Math.round` and pushed into the `discounted` array. Finally, the function returns the array of discounted prices.

9.  At line 11, a ReferenceError will occur because `i` is declared using the `let` keyword inside the `for` loop. Variables declared with `let` have block scope, meaning they are only accessible within the block in which they are declared. Therefore, when trying to access `i` outside of the loop, it's out of scope, resulting in a ReferenceError.

10. The code prints `3`. At line 12, the code will print the value of `length`, which is the length of the prices array. The length variable is declared using the `const` keyword, indicating that its value remains constant and cannot be reassigned. Therefore, when `console.log(length)` is executed, it will print the length of the `prices` array as it was assigned initially.

11. This function will return an array: `[50, 100, 150]`. It calculates the discounted price for each item in the `prices` array by applying the provided discount percentage. The discounted prices are then pushed into the `discounted` array, and the array is returned at the end of the function. The use of `const` for `discounted` and `length` ensures that their values remain constant throughout the execution of the function.

### Data Types

12. Given the above Object, write the notation for: 
- A. `student.name;`
- B. `student['Grad Year'];`
- C. `student.greeting();`
- D. `student['Favorite teacher'].name;`
- E. `student.courseLoad[0];`

### Basic Operators & Type Conversion

13. Arithmetic
- A. Output: `32`. When the addition operator (+) is used with a string and a number, JavaScript performs concatenation. Therefore, the string 3 is concatenated with the number 2, resulting in the string '32'
- B. Output: `1`. When the subtraction operator (-) is used with a string and a number, JavaScript attempts to convert the string into a number. Therefore, the string '3' is converted to the number 3, and then subtraction is performed, resulting in the number 1.
- C. Output: `3`. Null is converted to 0 in numeric contexts. Therefore, when adding 3 and null, the result is 3.
- D. Output: `3null`. Similar to question A, the addition operator (+) concatenates strings. Therefore, the string '3' is concatenated with the string representation of null, resulting in '3null'.
- E. Output: `4`. True is converted to 1 in numeric contexts. Therefore, when adding true and 3, the result is 4.
- F. Output: `0`. False is converted to 0 in numeric contexts, and null is also converted to 0. Therefore, when adding false and null, the result is 0.
- G. Output: `3undefined`. Similar to question D, the addition operator (+) concatenates strings. Therefore, the string '3' is concatenated with the string representation of undefined, resulting in '3undefined'.
- H. Output: `NaN`. Undefined is converted to NaN (Not a Number) in numeric contexts. Therefore, when trying to subtract undefined from the string '3', the result is NaN.
    
14.  Comparison
- A. `true`. When comparing a string to a number, JavaScript converts the string to a number. Therefore, '2' is converted to the number 2, which is indeed greater than 1.
- B. `false`. When comparing strings, JavaScript compares character by character. '2' is not less than '12' because the comparison is based on the characters '2' and '1', where '2' comes after '1', making '2' greater than '12'.
- C. `true`. The == operator performs type coercion if the operands are of different types. Therefore, the number 2 is converted to the string '2', and then they are compared as strings, resulting in true.
- D. `false`. The === operator does not perform type coercion. Therefore, since 2 and '2' are of different types (number and string), they are not considered equal.
- E. `false`. The == operator performs type coercion if the operands are of different types. True is converted to the number 1, but 1 is not equal to 2, so the result is false.
- F. `true`. Both operands are of the same type (boolean) and have the same value (true). The === operator checks for strict equality without performing type coercion, so true is strictly equal to true.

15. The main difference between the == and === operators lies in how they handle equality comparisons. The == operator (loose equality) performs type coercion, meaning it converts the operands to the same type before making the comparison. This can lead to unexpected results as different data types may be considered equal after conversion. On the other hand, the === operator (strict equality) does not perform type coercion. It checks if the operands are of the same type and have the same value. This results in a more precise and predictable comparison, ensuring that the types of the operands are identical for them to be considered equal.

### Loops

16. The code is in `part2-question16.js`. This loop iterates through each property in the `statistics` object using the `for...in` syntax. Inside the loop, it checks if the property name starts with the letter 'r' using `startsWith('r')`, or if the value of that property is an odd number using `% 2 !== 0`. If either condition is true, it prints out the value of that property.

### Functions

17. The result is `[2, 4, 6]`. When the `modifyArray` function is called with the parameters `modifyArray([1,2,3], doSomething)`, the result will be `[2, 4, 6]`. The `modifyArray` function takes an array and a callback function as parameters. It iterates through each element of the array. For each element, it calls the callback function (`doSomething`) with the element as an argument.The callback function (`doSomething`) multiplies the given number by 2. The result of the callback function is then pushed into a new array (`newArr`). Finally, the `modifyArray` function returns the new array containing the modified elements.

### setInterval(), setTimeout(), clearTimeout()

18. The code is in `part2-question18.js`. We define a function called `printTime` that logs the current time using `toLocaleTimeString()` method of the `Date` object. We use `setInterval()` function to repeatedly call the `printTime` function every 1000 milliseconds (1 second).
This change ensures that the program prints out the current time every second.

19. The output of the code will be: `1`, `4`, `3`, `2`. Initially, `1` is logged when `printNums()` is called. Then, `4` is logged. After that, `3` is logged. Even though it has a timeout of 0 milliseconds, it's scheduled in the event loop to execute after other synchronous code. Finally, `2` is logged after 1 second because of the timeout of 1000 milliseconds
    
