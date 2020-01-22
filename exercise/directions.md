

# Exercises: JavaScript loops

Paste your answers into this file.

<br>

## Print every number from 0 to 10

```
for(let i =0; i  <= 10; i++){
    console.log(i);
}
```

<br>

## Print every number from 10 to 0

```
for(let i = 10; i  >= 0; i--){
    console.log(i);
}
```

<br>

## Print every number from 4 to -16

```
for(let i = 4; i  >= -16; i--){
    console.log(i);
}
```

<br>

## Print every fifth number from 8 to 41

```
for(let i = 8; i  <= 41; i += 5){
    console.log(i);
}
```

<br>

# Exercises: JavaScript loops with array:

Paste your answers into this file.



1. Change all **odd** numbers to be those numbers multiplied by two:
```js
const numbers = [4, 9, 7, 2, 1, 8];

  // your code here

  for(let i =0; i<numbers.length; i++){
    if(numbers[i] % 2 !== 0){
      numbers[i] *= 2;
    }
  }

numbers; // => [4, 18, 14, 2, 2, 8]
```

2.  Create an array to hold your favorite colors.  For each choice, log to the screen a string like: `My #1 choice is blue.`

let colors = colors = ['yellow', 'blue', 'green', 'red'];

for(let i = 0; i < colors.length; i++){
    console.log("my #" + (i+1) + " choice is " + colors[i]);
}


3.  Create an array of ages.  Loop through and log only the ages that are over 21.

let ages = [15, 24, 23, 12, 33, 20, 50, 28, 14];

for(let i =0; i<ages.length; i++){
    if(ages[i] > 21){
        console.log(ages[i]);
    }
}

1. Create an array to hold your top five choices of something (music, books, movies, whatever).

    - For each choice, log to the screen a string like: "My #1 choice is blue."
    - **Bonus:** Change it to log "My 1st choice, "My 2nd choice", "My 3rd choice", picking the right suffix for the number based on what it is.

    let foods = ['pizza', 'fried chicken', 'cheese burger'];  

    for(let i = 0; i < foods.length; i++){
    console.log("my #" + (i+1) + " choice is " + foods[i]);
    }


## The classic Fizzbuzz Program

For every `number` between 1 and 100...

If the `number` is evenly divisible by 3, print "Fizz"

If the `number` is evenly divisible by 5, print "Buzz"

If the `number` is evenly divisible by 3 AND evenly divisible by 5, print "Fizzbuzz"


```
let answer = "";

for(let number =0; number <=100; number++){
   if(number % 3 === 0){
       answer += "Fizz";
    }
    if(number % 5 === 0){
        answer += "Buzz";
    }
    
    console.log(answer);
    answer = "";
}
```

<br>


## The even/odd reporter

Write a for loop that will iterate from 0 to 20. For each iteration, it will check if the current number is even or odd, and report that to the screen (e.g. "2 is even").

```
for(let number = 0; number <= 20; number++){
    if(number % 2 === 0){
        console.log(number + " is even.");
    }
    else{
        console.log(number + " is odd.");
    }
}
```

<br>

## Multiplication Tables

Write a for loop that will iterate from 0 to 10. For each iteration of the for loop, it will multiply the number by 9 and log the result (e.g. "2 * 9 = 18").

Bonus: Use a nested for loop to show the tables for every multiplier from 1 to 10 (100 results total).


```
for(let number = 0; number <= 10; number++){
    for(let table = 1; table <= 10; table++){
        console.log(number + " * " + table  + " = " + number * table);
    }
}
```

<br>

## The Grade Assigner

Check the results for every value from 60 to 100 - so your log should show "For 89, you got a B. For 90, you got an A.", etc.

```
for(let mark = 60; mark <= 100; mark++){
    if(mark >= 90 ){
        console.log("You got an A.");
    }
    else if(mark >= 80 ){
        console.log("You got a B.");
    }
    else if(mark >= 70 ){
        console.log("You got a C.");
    }
    else{
        console.log("You got a D.");
    }
}
```
