# Array
+ An array in JavaScript is a data structure used to store multiple values in a single variable. Arrays can hold various data types, such as numbers, strings, objects, and even other arrays. They are particularly useful for managing lists of items and performing operations on collections of data.
## JavaScript Array Methods

JavaScript arrays are versatile and come with a variety of built-in methods to manipulate and interact with array elements. Below are some commonly used array methods:

## What is method
In JavaScript, a method is a function that is a property of an object. Methods are used to perform actions on the data stored in objects or to manipulate the object itself.


![method](https://www.shutterstock.com/image-photo/word-method-made-wood-building-260nw-1770808247.jpg)

## Basic Array Methods


### `length`
Returns the number of elements in an array.
```javascript
let fruits = ["Banana", "Orange", "Apple", "Mango"];
console.log(fruits.length); // Outputs: 4
```

# Method of array in Javascript
![](https://media.dev.to/cdn-cgi/image/width=1280,height=720,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2Fxi0sv200ldxhex3rs2be.png)

## toString()
+ Converts an array to a string of (comma-separated) array values.
```javascript
const fruits = ["Banana", "Orange", "Apple", "Mango"];
console.log(fruits.toString()); // Outputs: Banana,Orange,Apple,Mango
```
## pop()
+ Removes the last element from an array and returns that element.
```javascript
const fruits = ["Banana", "Orange", "Apple", "Mango"];
const lastFruit = fruits.pop();
console.log(lastFruit); // Outputs: Mango
console.log(fruits);    // Outputs: ["Banana", "Orange", "Apple"]
```
## push()
+ Adds one or more elements to the end of an array and returns the new length of the array.
```javascript
const fruits = ["Banana", "Orange", "Apple"];
const newLength = fruits.push("Mango");
console.log(newLength); // Outputs: 4
console.log(fruits);    // Outputs: ["Banana", "Orange", "Apple", "Mango"]
```
## shift()
+ Removes the first element from an array and returns that element.
```javascript
const fruits = ["Banana", "Orange", "Apple", "Mango"];
const firstFruit = fruits.shift();
console.log(firstFruit); // Outputs: Banana
console.log(fruits);     // Outputs: ["Orange", "Apple", "Mango"]
```
## unshift()
+ Adds one or more elements to the beginning of an array and returns the new length of the array.
```javascript
const fruits = ["Orange", "Apple", "Mango"];
const newLength = fruits.unshift("Banana");
console.log(newLength); // Outputs: 4
console.log(fruits);    // Outputs: ["Banana", "Orange", "Apple", "Mango"]
```
## slice()
+ Returns a shallow copy of a portion of an array into a new array object.
```javascript
const fruits = ["Banana", "Orange", "Apple", "Mango"];
const citrus = fruits.slice(1, 3);
console.log(citrus); // Outputs: ["Orange", "Apple"]
```
## splice()
+ Changes the contents of an array by removing or replacing existing elements and/or adding new elements.
```javascript
const fruits = ["Banana", "Orange", "Apple", "Mango"];
const citrus = fruits.slice(1, 3);
console.log(citrus); // Outputs: ["Orange", "Apple"]
```
## concat()
+ The concat method in JavaScript is used to merge two or more arrays. 
```javascript
const letters = ["a", "b", "c"];
const numbers = [1, 2, 3];
const alphaNumeric = letters.concat(numbers);
console.log(alphaNumeric); // Outputs: ["a", "b", "c", 1, 2, 3]
```
## concat()
+ The concat method in JavaScript is used to merge two or more arrays. 
```javascript
const letters = ["a", "b", "c"];
const numbers = [1, 2, 3];
const alphaNumeric = letters.concat(numbers);
console.log(alphaNumeric); // Outputs: ["a", "b", "c", 1, 2, 3]
```
## join()
+ The join method in JavaScript is used to concatenate all the elements of an array into a single string.
```javascript
const fruits = ["Apple", "Banana", "Cherry"];
const result = fruits.join();
console.log(result); // Outputs: "Apple,Banana,Cherry"
```
## indexOf()
+ The indexOf method searches the array for the specified element, starting at the given index (or at the beginning if no index is specified).
```javascript
const fruits = ["Apple", "Banana", "Cherry", "Banana"];
console.log(fruits.indexOf("Banana")); // Outputs: 3
```
## toReversed()
+ The toReversed method in JavaScript is a new addition that allows you to reverse the order of elements in an array without modifying the original array. 
```javascript
const fruits = ["Apple", "Banana", "Cherry"];
const reversedFruits = fruits.toReversed();
console.log(reversedFruits); // Outputs: ["Cherry", "Banana", "Apple"]
console.log(fruits);         // Outputs: ["Apple", "Banana", "Cherry"]
```



## Callback method
![](https://miro.medium.com/v2/resize:fit:809/1*vBp7f-zK1UeO18OHyYt11w.jpeg)

### What is callback?
+ A callback in JavaScript is a function that is passed as an argument to another function and is executed after the completion of certain operations. It often helps create asynchronous code and handle the results of functions at a specific point in time

### map()
+ In JavaScript, map() is a method of the Array object. It creates a new array by calling a function on every element of the original array and storing the results in a new array.

```javascript
const numbers = [1, 2, 3, 4, 5];
const doubledNumbers = numbers.map(function(number) {
  return number * 2;
});
console.log(doubledNumbers); // [2, 4, 6, 8, 10]
```


### forEach()
+ Sure! The forEach() method in JavaScript is used to execute a provided function once for each array element. Here’s a simple example:

```javascript
const fruits = ['apple', 'banana', 'cherry'];

fruits.forEach(function(fruit) {
  console.log(fruit);
});

// Output:
// apple
// banana
// cherry
```



### filter()
+ The filter() method in JavaScript is used to create a new array with all elements that pass a test implemented by a provided function. Here’s a simple example:

```javascript
const numbers = [1, 2, 3, 4, 5, 6];

const evenNumbers = numbers.filter(function(number) {
  return number % 2 === 0;
});
console.log(evenNumbers); // [2, 4, 6]
```



### reduce()
+ The reduce() method in JavaScript is used to execute a reducer function on each element of the array, resulting in a single output value. Here’s a simple example:

```javascript
const numbers = [1, 2, 3, 4, 5];

const sum = numbers.reduce(function(accumulator, currentValue) {
  return accumulator + currentValue;
}, 0);

console.log(sum); // 15
```



### find()
+ The find() method in JavaScript is used to search an array and return the value of the first element that satisfies a provided testing function. Here’s a simple example:

```javascript
const numbers = [1, 2, 3, 4, 5];

const firstNumberGreaterThanThree = numbers.find(function(number) {
  return number > 3;
});

console.log(firstNumberGreaterThanThree); // 4
```




### toSorted()
+ The toSorted() method in JavaScript is a new addition that creates a sorted copy of an array without modifying the original array. Here’s a simple example:

```javascript
const fruits = ['banana', 'apple', 'mango', 'kiwi'];

const sortedFruits = fruits.toSorted();

console.log(sortedFruits); // ['apple', 'banana', 'kiwi', 'mango']
console.log(fruits); // ['banana', 'apple', 'mango', 'kiwi']
```



## What is mechanism injavascript?
+ Unlike most programming languages, JavaScript language has no concept of input or output. It is designed to run as a scripting language in a host environment, and it is up to the host environment to provide mechanisms for communicating with the outside world.

### Destructuring
+ Unlike most programming languages, JavaScript language has no concept of input or output. It is designed to run as a scripting language in a host environment, and it is up to the host environment to provide mechanisms for communicating with the outside world.

```javascript
let a, b, rest;
[a, b] = [10, 20];

console.log(a);
// Expected output: 10

console.log(b);
// Expected output: 20

[a, b, ...rest] = [10, 20, 30, 40, 50];

console.log(rest);
// Expected output: Array [30, 40, 50]
```


### Spread
+ The spread (…) syntax allows an iterable, such as an array or string, to be expanded in places where zero or more arguments (for function calls) or elements (for array literals) are expected. In an object literal, the spread syntax enumerates the properties of an object and adds the key-value pairs to the object being created.

```javascript
function sum(x, y, z) {
  return x + y + z;
}

const numbers = [1, 2, 3];

console.log(sum(...numbers));
// Expected output: 6
```



### Rest
+ The rest parameter syntax allows a function to accept an indefinite number of arguments as an array, providing a way to represent variadic functions in JavaScript. A function definition can only have one rest parameter, and the rest parameter must be the last parameter in the function definition.

```javascript
function myFun(a, b, ...manyMoreArgs) {
  console.log("a", a);
  console.log("b", b);
  console.log("manyMoreArgs", manyMoreArgs);
}

myFun("one", "two", "three", "four", "five", "six");

// a, "one"
// b, "two"
// manyMoreArgs, ["three", "four", "five", "six"] — an array
```
