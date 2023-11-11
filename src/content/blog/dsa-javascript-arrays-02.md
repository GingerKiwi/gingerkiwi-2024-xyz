---
title: "Data Structures and Algorithms: Javascript Arrays #02"
date: 2023-09-01
tags:
  - post
  - featured
  - code
  - dsa
  - javascript
  - technical
description: It's time to go down the data structures and algorithms (dsa) rabbit hole. But let's make things more fun - no "foo" and "bar" here! This is a series of pet and Alice in Wonderland themed DSA articles. We're starting with the basics of arrays in Javascript.
---
## About This Article Series

I've been preparing for technical interviews and DSA challenges lately. But it can be so dry! I mean I love a puzzle, but I've found that I prefer solving puzzles that result in an actual project people can use. To keep things interesting, I've been making my own notes with pet and Alice in Wonderland themes. So here's the first of (likely) many DSA articles in Javascript with no foo or bar. 

The focus is also on ES6 Javascript to keep things current and just easier to read. I'm assuming that readers will have the basics of programming in Javascript or another language, though I do give a quick overview and some definitions. This is intended as a reference for other devs who are practicing for technical interviews, or want a more fun reference for Javascript programming.

## Javascript Arrays Part 02
### Concat
Used to merge two or more arrays. It returns a new array. Concat doesn't mutate the original arrays.

```js
const shoppingList = ['earl grey tea', 'cream', 'whole milk']

const fruits = ['apples', 'oranges', 'peaches', 'pears']

const veggies = ['carrots', 'parships', 'potatoes']

shoppingList.concat(fruits)

// [ 'earl grey tea', 'cream', 'whole milk', 'apples', 'oranges', 'peaches', 'pears' ]

fruits.concat(shoppingList)

// [ 'apples', 'oranges', 'peaches', 'pears', 'earl grey tea', 'cream', 'whole milk' ]


const allFood = shoppingList.concat(fruits, veggies)

allFood
// [ 'earl grey tea', 'cream', 'whole milk', 'apples', 'oranges', 'peaches', 'pears', 'carrots', 'parships', 'potatoes' ]
```

### Includes (Boolean)

Determines whether an array includes a certain value among its entries, returning true or false as appropriate.

```js
const shoppingList = ['earl grey tea', 'cream', 'whole milk']

const playlist = ['Her Name Is Alice','Drink Me','Follow Me Down','Painting Flowers','Queen of Hearts'
];
 
shoppingList.includes('cream')

playlist.includes('Drink Me', 3)

'Play the list'
```

### IndexOf

Returns the first index at which a give element can be found in the array, or -1 if the element is not present.

```js
playlist.indexOf('Follow Me Down')

if (playlist.indexOf('Drink Me')) {
  console.log('Play the list')
}
```

### Reverse

Reverses an array *in place*. The first array element becomes the last, and the least array element becomes the first.

```js
topSongs.reverse()

// [ 'Queen of Hearts', 'Painting Flowers', 'Follow Me Down', 'Drink Me', 'Her Name Is Alice' ]

```

### Join

Join creates and returns a new string by concatenating all of the elements in an array (or an array-like object) separated by commas or a specified separator string. If an array has only one item, then that item will be returned without using the separator.

```js
topSongs.join((', '))

// 'Her Name Is Alice, Drink Me, Follow Me Down, Painting Flowers, Queen of Hearts'

yellBackwards.reverse().join(' ')
// 'off with their heads!'

numbers.join(('-'))
// '2-4-5-8-9-10-7'
```

### Slice

Slice returns a shallow copy of a portion of an array into a new array object selected from begin to end (end not included) where begin and end represent the index of items in that array. The original array will not be modified. 

```js
const games = ['crochet', 'chess', 'cards', 'painting the roses red']

const indoorGames.slice(1,3)

// indoorGames = [ 'chess', 'cards' ]

favouriteGames = games.slice(-2)

// [ 'cards', 'painting the roses red' ]

const myGames = games.slice()
// makes a ccomplete opy of the array - sometimes used to make a quick copy
// myGames = ['crochet', 'chess', 'cards', 'painting the roses red']
```

### Splice

Changes the contents of an array by removing or replacing existing elements and/or adding new elements *in place*.

To add an element without replacing any other element

```js 
arrayName.splice(index to add something in at, how many items to replace, what to splice in)

playlist.splice(4, 0, 'White Rabbit')

// [ 'Her Name Is Alice', 'Drink Me', 'Follow Me Down', 'Painting Flowers', 'White Rabbit', 'Queen of Hearts' ]
```

To replace element with another one

```js 
playlist.splice(4, 1, 'White Rabbit')

// [ 'Her Name Is Alice', 'Drink Me', 'Follow Me Down', 'Painting Flowers', 'White Rabbit', ]

```
Can be used to simply remove one or more elements in the middle of an array.


```js
topSongs.splice(2,2)
// removes: [ 'Follow Me Down', 'Painting Flowers' ]

// topSongs = [ 'Her Name Is Alice', 'Drink Me', 'Queen of Hearts' ]
```

### Sort

Sorts the elements of an array *in place* and returns the sorted array. The default sort order is built upon converting the elements into strings, then comparing their sequences of UTF-16 code unit values.

It is *NOT* a numerical sort!

```js
yell.sort()

// returns: [ 'heads!', 'off', 'their', 'with' ]

numbers.sort()
// returns: [ 10, 2, 4, 5, 7, 8, 9 ]
```

