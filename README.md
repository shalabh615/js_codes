 // que 1 -Fibonacci Series
 
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

console.log("---next que----");

// que 2- Sum of Digits
function sumOfDigits(num) {
    let sum = 0;
    while (num > 0) {
        sum += num % 10;
        num = Math.floor(num / 10);
    }
    return sum;
}

console.log("Sum of digits:", sumOfDigits(1234));

console.log("---next que----");

//que 3- Palindrome Check
function isPalindrome(str) {
    let reversed = str.split('').reverse().join('');
    return str === reversed;
}

console.log("Is Palindrome:", isPalindrome("madam"));

console.log("---next que-----");

// que 4--Triangle Pattern
function printTriangle(n) {
    console.log("Triangle Pattern:");
    for (let i = 1; i <= n; i++) {
        console.log("*".repeat(i));
    }
}

printTriangle(5);

console.log("-----next que-----");

// que 5- Factorial
function factorial(n) {
    let result = 1;
    for (let i = 1; i <= n; i++) {
        result *= i;
    }
    return result;
}

console.log("Factorial:", factorial(5));
