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

