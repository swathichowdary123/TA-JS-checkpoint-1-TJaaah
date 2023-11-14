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
the first function returns the result of the addotion ,while the second function logs the result to the console but doesnot provide a return value .
2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.
in the first case the function returns the result of the addition ,so first will be assigned the value.in the second case the function logs the result to the console but doesnot explicitly returns a value. so second will be assigned the value undefined.
3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?
if we call it with three parameters the third parameter will be ignored because the function is not designed to handle it .
4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?
yes ,we ca store the first sum function in a variable named add.in javascript functions are first class citizens which means they can be assigned to variables.
5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.
function sayHello(name){
  return "hello" + name;
}
6. What will be the output of the function below and why?

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

showMessage();
```
hello, john
7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); // Output 1
john
showMessage(); // Output 2
hello,john
alert(userName); // Output 3
john
```

8. What is a Anonymous Function give example of three functions.
anonymous function is a function without a name.in javascript you can define anonymous function using function expression.
expression:
let add=function(a,b){
  return a+b;
}
console.log(add(2,3));
anonymous arrow function:
let multiply=(a,b)=>{
  return a*b;
}
console.log(multiply(4,5));
9. Can function declaration be a Anonymous Function? Explain
no,a function declaration cannot be a anonymous function .in javascript ,a function declaration always has a name.
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
function getUserDetails(userId){
  //function logic
}

function calcTotalPrice(quantity,price){
  //function logic
}

function createNewUser(username,email){
  //function logic
}

function checkUserExists(username){
  //function logic
}