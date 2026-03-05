# JavaScript Programming Questions

Author: Shalabh Malik

---

## 1. Fibonacci Series

**Approach:**  
Start with two numbers, 0 and 1, and print them.  
Use a loop to generate the next number by adding the previous two numbers until N terms are printed.

```javascript
function fibonacci(n) {
    let a = 0, b = 1;
    console.log("Fibonacci Series:");

    for (let i = 0; i < n; i++) {
        console.log(a);
        let next = a + b;
        a = b;
        b = next;
    }
}

fibonacci(10);
```

---

## 2. Sum of Digits

**Approach:**  
Extract the last digit of the number using modulus and add it to a sum variable.  
Repeat the process after removing the last digit until the number becomes zero.

```javascript
function sumOfDigits(num) {
    let sum = 0;

    while (num > 0) {
        sum += num % 10;
        num = Math.floor(num / 10);
    }

    return sum;
}

console.log("Sum of digits:", sumOfDigits(1234));
```

---

## 3. Palindrome Check

**Approach:**  
Compare the reversed string with the original to check if both are equal.

```javascript
function isPalindrome(str) {
    let reversed = str.split('').reverse().join('');
    return str === reversed;
}

console.log("Is Palindrome:", isPalindrome("madam"));
```

---

## 4. Triangle Pattern

**Approach:**  
Run a loop from 1 to N. In each iteration, print the star symbol equal to the current loop number to form a triangle.

```javascript
function printTriangle(n) {
    console.log("Triangle Pattern:");
    for (let i = 1; i <= n; i++) {
        console.log("*".repeat(i));
    }
}

printTriangle(5);
```

---

## 5. Factorial

**Approach:**  
Initialize a variable with 1 and multiply it by each number from 1 to N. After the loop finishes, the variable stores the factorial of the number.

```javascript
function factorial(n) {
    let result = 1;

    for (let i = 1; i <= n; i++) {
        result *= i;
    }

    return result;
}

console.log("Factorial:", factorial(5));
```

---
