1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

let percentage= function percentage(marks, total) {
  return (marks * 100) / total;
}

let percentage = function (marks, total) {
  return (marks * 100) / total;
};

let percentage=(marks,total){((marks * 100) / total)});
```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
//Function Declaration
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
//Function Expression
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
//Function Expression
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
//Function Expression
```

```js
let percentage = (marks, total) => (marks * 100) / total;
//Function Expression
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.
   A function is a special type of object in Javascript, hence it can be assigned to the right side of an assignment operator, which makes function a form of expression.

   e.g. let square= (x)=>{x*x};

4. Why is a function call an expression in JavaScript?
A function call executes the code inside a function and returns a value either implicitly as undefined or through a return statement , hence it is an expression. 

5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // Valid
five = add; // 
five = five(10, 11); //Valid
five = function () {
  return 'Hello';
}; // Valid
```

6. What is the difference between function definition and function call? Explain with an example.
A function definition is a declared collection of steps that needs to be performed. Whereas a fucntion call is the execution of those steps using the () after function name. 
E.g. funtion add(a,b){return a+b}; // is a function definition to add two numbers
      function(1+5); // It is a function call whihc will return a value of 6;

7. What is the similarities between function definition and function call?
A function definition and a function call both are values in Javascript. The definition when assigned to a variable is stored as a String , whereas a function call when assigned to variable gets executed and returns a value.

8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // Valid as functions are special type of objects, so they can have properties like objects too.
```

9. What is higher order function explain with an example.
A higher order function is a function that has another function as its argument or its return value is a function. 
E.g. addEventListener("click", handleClick); 

10. Explain what is callback function. Why you can pass a function inside a function?
     A callback function is a function definition, which is passed into another function as an arguemt to get executed later.
     In javascript a function is just like any other value, and more specifically it is a special type of object, and since an object is a value, it can be passed as arguments or as return values. 
