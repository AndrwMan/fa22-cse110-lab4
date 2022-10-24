1. 'values added: 20'. As expected since 10 + 10 = 20 and `var result` is 
declared within the `if` block so it can be printed
2. 'final result: 20'. Still 20 since `var` is function scope and though we are
attempting to print outside the `if` block the `var result` is still within function
3. 'values added: 20'. As expected since 10 + 10 = 20 and `let result` is 
declared within the `if` block so it can be printed
4.  ReferenceError: result is not defined. Not 20 since `let` is block scope and we are attempting to print outside the `if` block the `let result` is not defined
5. Throws error. Since `const result` does not allow reassignment of the variable which is attempted at line 7.
6.  Technically there is no print or error since the error crashes execution before program control can reach line 13. But if you comment out lines 7 then you get ReferenceError since `const result` has block scope and line 13 is not in the block it is declared.
7. 3 . As expected `var i` is function scope and it follows the loop so the console.log prints the last value the loop incremented (the length of the prices array) had after it terminated
8. 150 . As expected `var discounted` is function scope and console.log follows the loop so it prints the last value the loop assigned to `var discounted` (the result of the last price 300 * 1 - 0.5 = 150).
9.