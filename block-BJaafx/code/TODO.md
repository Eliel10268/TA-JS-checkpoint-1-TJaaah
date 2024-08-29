1. Using loops take 10 inputs from user and find the average of all the numbers.

let sum = 0;

for (let i = 0; i < 10; i++){
let userInput = parseFloat(prompt("Enter a number: "));
sum += userInput;
}

let average = sum / 10;

console.log("The average of the numbers is : "+average);

2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println("hi");
  i++;
}
```

It is will output : ReferenceError: println is not defined

since println is not recognized in Javascript.

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.

function getEvenSum(max = 10){

let sum = 0;

for(let i = 0; i <= max; i++){

if (i % 2 == 0)
{
sum += i;
}

return sum
}

}

console.log(getEvenSum(20));

4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.

function getOddSum(max = 10){

let sum = 0;

for(let i = 0; i <= max; i++){

if (i % 2 != 0)
{
sum += i;
}

return sum
}

}

5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

function getProductOfDigits(num) {

// Check if the input is less than 0

if (num < 0) {
return 'not a valid input';
}

    // Convert the number to a string to iterate over each digit
    let numStr = num.toString();

    // Initialize the product to 1 (since multiplying by 0 would always result in 0)
    let product = 1;

    // Iterate over each character in the string
    for (let i = 0; i < numStr.length; i++) {
        // Convert each character back to a number and multiply to the product
        product *= parseInt(numStr[i], 10);
    }

    return product;

}

// Example usage
console.log(getProductOfDigits(123)); // Output: 6
console.log(getProductOfDigits(-456)); // Output: not a valid input

6. What will be the output of the following code below in multiple conditions? Explain with reason?

```js
function check(num) {
  if (num > 5) {
    return "Bigger than 5";
  }

  if (num < 5) {
    return "Smaller than 5";
  }

  return num;
}

check(10); // output 'Bigger than 5' because it  passes for the first condition
check(1); // output  'Smaller than 5' because the first condition does not pass but the 2nd does
check(5); // output   5  because all the contions fail then it will return the number
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === "Arya") return "You are arya";
  if (name === "John") return "You are john";
  return "Who are you";
}

getOutput("Arya"); // what will be the output = 'You are arya' because the argument passed correspond to the first condition
getOutput("John"); // what will be the output = 'You are john' because the argument passed correspond to the 2nd condition
getOutput(); // what will be the output = 'Who are you' because the argument passed does not correspond to any of the conditions above
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === "Arya") console.log("You are arya");
  if (name === "John") console.log("You are john");
  return "Who are you";
}

getOutput("Arya"); // what will be the output = 'You are arya' because the argument passed correspond to the first condition
getOutput("John"); // what will be the output = 'You are john' because the argument passed correspond to the 2nd condition
getOutput(); // what will be the output = 'Who are you' because the argument passed does not correspond to any of the conditions above
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.

Yes, a function in JavaScript can have multiple return statements. This is often used when you want to return different values based on certain conditions within the function. Once a return statement is executed, the function terminates, and the value specified in the return statement is returned to the caller.

Here's an example:

function checkNumber(num) {
if (num > 0) {
return "Positive";
} else if (num < 0) {
return "Negative";
} else {
return "Zero";
}
}

// Example usage:
console.log(checkNumber(5)); // Output: "Positive"
console.log(checkNumber(-3)); // Output: "Negative"
console.log(checkNumber(0)); // Output: "Zero"

10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.

for is used when the number of times to be looped is known beforehand but while is used when you don't know exact time it will loop before it starts.
