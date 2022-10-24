### part 1
1. 'values added: 20'. As expected since 10 + 10 = 20 and `var result` is 
declared within the `if` block so it can be printed
2. 'final result: 20'. Still 20 since `var` is function scope and though we are
attempting to print outside the `if` block the `var result` is still within function
3. 'values added: 20'. As expected since 10 + 10 = 20 and `let result` is 
declared within the `if` block so it can be printed
4.  ReferenceError: result is not defined. Not 20 since `let` is block scope and we are attempting to print outside the `if` block the `let result` is not defined
5. Throws error. Since `const result` does not allow reassignment of the variable which is attempted at line 7.
6.  Technically there is no print or error since the error crashes execution before program control can reach line 13. But if you comment out lines 7 then you get ReferenceError since `const result` has block scope and line 13 is not in the block it is declared.
### part 2
1. 3 . As expected `var i` is function scope and it follows the loop so the console.log prints the last value the loop incremented (the length of the prices array) had after it terminated
2. 150 . As expected `var discountedPrice` is function scope and console.log follows the loop so it prints the last value the loop assigned to `var discounted` (the result of the last price 300 * 1 - 0.5 = 150).
3. 150 . As expected `var finalPrice` is function scope and console.log follows the loop so it prints the last value the loop assigned to `var finalPrice` (the result of the last price 150*100/100 = 150).
4. [50, 100, 150] an array of size 3 with discount applied to intially passed prices. With 0.5 passed as the discount, the values of the orignal array 
[100, 200, 300] is just halfed in the loop and pushed to discounted array.
5. ReferenceError: i is not defined. Not 3 since `let` is block scope and we are attempting to print outside the `for` loop `let i` is not defined
6. ReferenceError: discountedPrice is not defined.  Not 150 since `let discountedPrice` is block scope and we are attempting to print outside the `for` loop `let discountedPrice` is not defined
7. 150 . As expected `let finalPrice` is block scope (the key here is that it is declared outside of for loop) and console.log follows the loop so it prints the last value the loop assigned to `let finalPrice` (the result of the last price 150*100/100 = 150).
8. [50, 100, 150] an array of size 3 with discount applied to intially passed prices. With 0.5 passed as the discount, the values of the orignal array 
[100, 200, 300] is just halfed in the loop and pushed to discounted array. Still the same as `var` since `let discounted` block is the entire function.
9. ReferenceError: i is not defined. Not 3 since `let` is still block scope and we are attempting to print outside the `for` loop so `let i` is not defined
10. 3 . As expected `const i` is block scope but the same as the entire function here. Console.log follows the loop so the console.log prints the constant value of the length of the array (3) which does not change.
11. [50, 100, 150] an array of size 3 with discount applied to intially passed prices. With 0.5 passed as the discount, the values of the orignal array 
[100, 200, 300] is just halfed in the loop and pushed to discounted array. Even though the `discounted` array is `const` that means the reference to tthe array is constant and adding values (ie: pushing discountedPrice) to the empty array is still allowed.