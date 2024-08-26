1. What is the difference between the two `sum` function given below?

```js
// first
function sum(a, b) {
  return a + b;
}

// second
function sum(a, b) {
  console.log(a + b);
}
```

// both are a function names that receive 2 arguments a and b; the first sum will return the result of addition back to where
// the function was called from and the same sum will display the result of addition of a and b

2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.

// firstsecond

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?
   // 36
4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?

// yes you can store a function in a variable and that will be called 'function expression'

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.

function sayHello(name){

return "Hello "+name;
}
sayHello('Arya');

6. What will be the output of the function below and why?

```js
let userName = "John";

function showMessage() {
  let message = "Hello, " + userName;
  return message;
}

showMessage();
```

// ReferenceError: userName is not defined

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = "John";

function showMessage() {
  let message = "Hello, " + userName;
  return message;
}

alert(userName); // Output 1 = John

showMessage(); // Output 2 = John

alert(userName); // Output 3 = John
```

8. What is a Anonymous Function give example of three functions.

'''An anonymous function is a function that is defined without a name. In many programming languages, these are also known as lambda functions or lambda expressions.
They are typically used for short, simple operations where defining a full function with a name would be unnecessarily verbose.

// Using function keyword
const multiply = function(x, y) {
return x \* y;
};
console.log(multiply(4, 7)); // Output: 28

// Using arrow function
const subtract = (x, y) => x - y;
console.log(subtract(10, 3)); // Output: 7

''' 9. Can function declaration be a Anonymous Function? Explain
'''
No, a function declaration cannot be an anonymous function. The key difference between a function declaration and an anonymous function lies in how they are defined and named.

'''

10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.

```md
Functions are actions. So their name is usually a verb. It should be brief, as accurate as possible and describe what the function does, so that someone reading the code gets an indication of what the function does.

It is a widespread practice to start a function with a verbal prefix which vaguely describes the action. There must be an agreement within the team on the meaning of the prefixes.

For instance, functions that start with "show" usually show something.

Function starting with…

"get…" – return a value,
"calc…" – calculate something,
"create…" – create something,
"check…" – check something and return a boolean, etc.
```

## getUserProfile:

Purpose: This function retrieves the profile data of a user.
Explanation: The get prefix indicates that the function will return a value, in this case, the user's profile information.

## calcTotalPrice:

Purpose: This function calculates the total price of items in a shopping cart.
Explanation: The calc prefix suggests that the function performs a calculation, specifically the total price in this case.

## createNewOrder:

Purpose: This function creates a new order in the system.
Explanation: The create prefix indicates that the function is responsible for creating something, which in this case is a new order.

## checkUserPermission:

Purpose: This function checks if a user has the required permissions for a certain action.
Explanation: The check prefix suggests that the function performs a check and likely returns a boolean value indicating whether the user has the necessary permissions.

## showErrorMessage:

Purpose: This function displays an error message to the user.
Explanation: The show prefix indicates that the function will present or display something, which in this case is an error message.
