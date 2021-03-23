Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = 'Arya';
}
console.log(useranme); // output
```

In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = 'Arya';
}
console.log(useranme); // output
```
In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside the block and has scope of const i.e. block- scope
The above code will throw an error `Reference Error username is not defined`.

3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = 'Arya';
}
console.log(username); // output
```
In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside the block and has scope of let i.e. block- scope
The above code will throw an error `Reference Error username is not defined`.

4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = 'Arya';
}
console.log(username); // output
```
In above code we are looking for the variable named `username`. There is a variable named `username` in the global scope. The variable is inside the block and has scope of var . output will be "Arya" in console

5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(username); // output
```
In above code we are looking for the variable named `username`. The variavle named username has already been defined in global scope. So we will get Syntax Error.

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(username); // output
```
In above code we are looking for the variable named `username`. Here username will be "John" as it is defined in global scope. The username variable inside block will have no effect on the global variable.

7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(username); // output
```
In above code we are looking for the variable named `username`. Here username will be "John" as it is defined in global scope. The username variable inside block will have no effect on the global variable.

8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, 'First'); // output
}
console.log(i, 'Second'); // output
```
In above code we are running for loop 10 times from i=0 to i=9. And then i is declared using var, which gives it global scope here. After loop i will get updated to 10.  So we will get following output: 
 0 "First"
 1 "First"
 2 "First"
 3 "First"
 4 "First"
 5 "First"
 6 "First"
 7 "First"
 8 "First"
 9 "First"
 10 "Second"

9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, 'First'); // output
}
console.log(i, 'Second'); // output
```
In above code we are running for loop 10 times from i=0 to i=9. And then i is declared using let, which gives it local scope here. After loop i will get updated to 10, but it is not accesible outside the for loop.  So we will get Reference Error: i is not defined. 