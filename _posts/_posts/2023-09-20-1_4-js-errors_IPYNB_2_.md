---
layout: post
title: 1.4 Correcting errors
description: Practice with identifying and correcting code blocks
type: ccc
author: Safin Singh and Rohan Juneja
permalink: /basics/js-debug
hide: True
---

{% include nav_basics.html %}

[College Board Big Idea 1](https://apclassroom.collegeboard.org/103/home?unit=1)

## Identifying and Correcting Errors (Unit 1.4)

> Become familiar with types of errors and strategies for fixing them

- Review CollegeBoard videos and take notes on blog
- Complete assigned MCQ questions if applicable

# Code Segments

Practice fixing the following code segments!

## Segment 1: Alphabet List

Intended behavior: create a list of characters from the string contained in the variable `alphabet`

### Code:


```python
%%js

var alphabet = "abcdefghijklmnopqrstuvwxyz";
var alphabetList = ["a", "b", "c", "d", "e",""];

for (var i = 0; i < 0; i++) {
	alphabetList.push(i);
}

console.log(alphabetList);
```

### What I Changed

I changed the array list for "var alphabetList" to include all of the alphabet listed. I also change the " i < 10" in the 6th line to be "i < 0" since it otherwise starts to repeat itself. My end result is a array list of the alphabet with the number it is.

## Segment 2: Numbered Alphabet

Intended behavior: print the number of a given alphabet letter within the alphabet. For example:
```
"_" is letter number _ in the alphabet
```

Where the underscores (_) are replaced with the letter and the position of that letter within the alphabet (e.g. a=1, b=2, etc.)

### Code:


```python
%%js
var alphabet = "abcdefghijklmnopqrstuvwxyz";
var alphabetList = ["abcdefghijklmnopqrstuvwxyz"];
for (var i = 0; i < 0; i++) {
    alphabetList.push(alphabet[i]);
}
console.log(alphabetList);
let letterNumber = "e"
for (var i = 0; i < alphabetList; i++) {
    if (i === letterNumber) {
    }
}
console.log(letterNumber + " is letter number 5 in the alphabet")
// Should output:
// "e" is letter number 5 in the alphabet
```

### What I Changed

I changed the letterNumber varrible to represent E instead of the number 5 since the "console.log(letterNumber...)" already had a command to say "e is letter number 5 in the alphabet." I then moved that piece of code outside of the "if (i === letterNumber)..." to the very end of the sequence.

## Segment 3: Odd Numbers

Intended behavior: print a list of all the odd numbers below 10

### Code:


```python
%%js
let evens = [];
let i = 1;
while (i <= 10) {
  evens.push(i);
  i += 2;
}
console.log(evens);
// Should output:
// "e" is letter number 5 in the alphabet
```

### What I Changed

I changed I changed the letterNumber varrible to represent E instead of the number 5 since the "console.log(letterNumber...)" already had a command to say "e is letter number 5 in the alphabet." I then moved that piece of code outside of the "if (i === letterNumber)..." to the very end of the sequence.

# BELOW NOT EDITED

The intended outcome is printing a number between 1 and 100 once, if it is a multiple of 2 or 5 
- What values are outputted incorrectly. Why?
- Make changes to get the intended outcome.


```python
%%js
var numbers = []
var newNumbers = []
var i = 0
while (i <= 100) {
    numbers.push(i)
    i += 1
}
for (var i of numbers) {
    if (numbers[i] % 5 === 0)
        newNumbers.push(numbers[i])
    if (numbers[i] % 2 === 0)
        newNumbers.push(numbers[i])
}
console.log(newNumbers)
```

# Challenge

This code segment is at a very early stage of implementation.
- What are some ways to (user) error proof this code?
- The code should be able to calculate the cost of the meal of the user

Hint:
- write a “single” test describing an expectation of the program of the program
- test - input burger, expect output of burger price
- run the test, which should fail because the program lacks that feature
- write “just enough” code, the simplest possible, to make the test pass

Then repeat this process until you get program working like you want it to work.


```python
%%js

var menu =  {"burger": 3.99,
         "fries": 1.99,
         "drink": 0.99}
var total = 0

//shows the user the menu and prompts them to select an item
console.log("Menu")
for (var item in menu) {
    console.log(item + "  $" + menu[item].toFixed(2)) //why is toFixed used?
}
//ideally the code should support mutliple items
var item = "burger"

//code should add the price of the menu items selected by the user 
console.log(total)
```

## Hacks
- Fix the errors in the first three segments in this notebook and say what you changed in the code cell under "What I Changed" (Challenge is optional)
