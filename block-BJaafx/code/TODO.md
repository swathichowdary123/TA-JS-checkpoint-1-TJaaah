1. Using loops take 10 inputs from user and find the average of all the numbers.
let sum=0;
for (let i=1;i<=10;i++){
  let userInput= Number(prompt(`enter number ${i}`));
  if(isNaN(userInput)){
    console,log(`enter valid input`);
    i--;
    continue;
  }
  sum+=userInput;
}
const average=sum/10;
console.log(`the average of 10 numbers is :${average}`);
2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
hi
hi
hi
```

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.
function getEvenSum(max=10){
  let sum=0;
  for(let i=0;i<=max;i+=2){
    sum+=i;
  }
  return sum;
}
4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.
function getOddSum(max=10){
  let sum=0;
  for(let i=1;i<=max;i+=2){
    sum+=i;
  }
  return sum;
}
5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.
function gerProductDigits(number){
  if(number<0>){
    return "not a valid input";
  }
  let digitString=Math.abs(number).toString();
  let product=1;
  for(let i=0; i<digitString.length; i++){
    product*=Number(digitString[i],10);
  }
  return product;
}
6. What will be the output of the following code below in multiple conditions? Explain with reason?

```js
function check(num) {
  if (num > 5) {
    return 'Bigger than 5';
  }

  if (num < 5) {
    return 'Smaller than 5';
  }

  return num;
}

check(10);  bigger than 5
check(1);  smaller than 5
check(5);  num
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); you are arya
getOutput('John'); you are john
getOutput();  who are you
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya');  you are arya
getOutput('John'); you are john
getOutput(); who are you
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.
yes,a function can have a multiple return statements .
function checkNumber(number){
  if(number>0){
    return "positive";
  }else if(number<0){
    return "negative";
  }else{
    return "zero";
  }
}
10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.
while loop when the number of iterations is not known beforehand,and the loop continues as long as specified condition is true.
let i=0;
while(i<5){
  console.log(i);
  i++;
}
for loop when the number of iterations is known beforehand or when theres clear structure for initialization ,condition and iteation.
for(let i=0;i<5;i++){
  console.log(i);
}