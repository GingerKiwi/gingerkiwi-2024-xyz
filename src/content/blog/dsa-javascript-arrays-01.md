---
title: "Data Structures and Algorithms: Javascript Arrays #01"
date: 2023-09-10
tags:
  - post
  - featured
  - code
  - dsa
  - javascript
  - technical
imageCaption: ADD CAPTION
description: It's time to go down the data structures and algorithms (dsa) rabbit hole. But let's make things more fun - no "foo" and "bar" here! This is a series of pet and Alice in Wonderland themed DSA articles. We're starting with the basics of arrays in Javascript.
---
## About This Article Series

I've been preparing for technical interviews and DSA challenges lately. But it can be so dry! I mean I love a puzzle, but I've found that I prefer solving puzzles that result in an actual project people can use. To keep things interesting, I've been making my own notes with pet and Alice in Wonderland themes. So here's the first of (likely) many DSA articles in Javascript with no foo or bar. 

The focus is also on ES6 Javascript to keep things current and just easier to read. I'm assuming that readers will have the basics of programming in Javascript or another language, though I do give a quick overview and some definitions. This is intended as a reference for other devs who are practicing for technical interviews, or want a more fun reference for Javascript programming.

## Javascript Arrays 101

An array is a collection of items with a single name.

For example a list of songs could have the name "playlist". In this array, all the names of songs are strings.

```js
const playlist = ['Her Name Is Alice','Drink Me','Follow Me Down','Painting Flowers','Queen of Hearts'
];
```
Alternatively, we could have an array of numbers. The following is taken from Alice in Wonderland when Alice says *"Let me see: four times five is twelve, and four times six is thirteen, and four times seven is-oh dear! I shall never get to twenty at that rate!"* 

```js
const aliceNumbers = [4, 5, 12, 4, 6, 13, 4, 7, 0, 20]
```

Arrays are "zero indexed", meaning the first element has an index of 0, the second element has an index of 1, and so on.

```js
playlist[2] = 'Follow Me Down'
aliceNumbers[5] = 13
```

To get the number or items/elements in an  array we use array.length

```js
playlist.length = 5
aliceNumbers.length = 10
```

## 5 Basic Javascript Array Methods 

Here are five basic Javascript array methods that let you add or delete items from arrays.

### 1) Inserting an Element at an Index Value

If we want to insert a value at a particular point in an array we can use the following:


```js
const shoppingList = ['earl grey tea', 'cream', '2% milk']
// Add a value
shoppingList[3] = 'scones'
//Now shoppingList is
shoppingList = ['earl grey tea', 'cream', '2% milk', 'scones']
```

To replace a value we use the same syntax, but use the index number of the item we want to overwrite/replace:

```js
const shoppingList = ['earl grey tea', 'cream', '2% milk', 'scones']

//update a value
shoppingList[2] = 'whole milk'

//Now shoppingList is
shoppingList = ['earl grey tea', 'cream', 'whole milk']
```
### 2) Push

Push adds an element to the end of an array.

```js
playlist.push('White Rabbit');

// Now playlist is:
playlist = ['Her Name Is Alice','Drink Me','Follow Me Down','Painting Flowers','Queen of Hearts', 'White Rabbit'];

// If we push another song onto 'playlist' 
playlist.push('Wonderland');

// Now playlist is:
playlist = ['Her Name Is Alice','Drink Me','Follow Me Down','Painting Flowers','Queen of Hearts', 'White Rabbit', 'Wonderland'];

```

You can also use push to push multiple items onto the end of an array.

```js
const playlist = ['Her Name Is Alice','Drink Me','Follow Me Down','Painting Flowers','Queen of Hearts', 'White Rabbit', 'Wonderland'];

playlist.push('Fell Down a Hole', 'Follow Me Down', 'Always Running Out of Time')

console.log(playlist)

['Her Name Is Alice','Drink Me','Follow Me Down','Painting Flowers','Queen of Hearts', 'White Rabbit', 'Wonderland', 'Fell Down a Hole', 'Follow Me Down', 'Always Running Out of Time'];
```

### 3) Pop

Pop is the opposite of push. It "pops off" the last item in an array.

```js
playlist = ['Her Name Is Alice','Drink Me','Follow Me Down','Painting Flowers','Queen of Hearts', 'White Rabbit', 'Wonderland'];
// To remove the last item
playlist.pop(); 

// Now playlist is:
playlist = ['Her Name Is Alice','Drink Me','Follow Me Down','Painting Flowers','Queen of Hearts', 'White Rabbit'];

console.log(playlist.pop());

// The expected output is 'White Rabbit'

```


### 4) Shift

Deletes the first item in an array, and returns that deleted item.

```js
const playlist = ['Her Name Is Alice','Drink Me','Follow Me Down','Painting Flowers','Queen of Hearts', 'White Rabbit', 'Wonderland'];

let mySong = playlist.shift()

console.log(mySong) // returns 'Her Name Is Alice'
// Our playlist array now contains:
playlist = ['Drink Me','Follow Me Down','Painting Flowers','Queen of Hearts', 'White Rabbit', 'Wonderland'];
```

### 5) Unshift

Unshift adds an item to the start of an array, and returns that new item.

```js
const playlist = ['Her Name Is Alice','Drink Me','Follow Me Down','Painting Flowers','Queen of Hearts', 'White Rabbit', 'Wonderland'];

let mySong = playlist.shift('Very Good Advice')
console.log(mySong) // returns 'Very Good Advice'

const playlist = ['Very Good Advice', 'Her Name Is Alice','Drink Me','Follow Me Down','Painting Flowers','Queen of Hearts', 'White Rabbit', 'Wonderland'];
```


That's it for now. The next few articles will cover more array methods and how to use arrays to solve string DSA challenges.
___
