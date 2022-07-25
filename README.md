# Fizz Buzz Challenge

## Table of Contents

- [Description](#description)
- [Deployed Page](#deployed-page)
- [Screenshot](#screenshot)
- [Contact Me](#contact-me)
- [JavaScript Code](#javascript-code)

## Description

Write a program that prints the numbers from 1 to 100. However, for any number that is a multiple of 3, print 'Fizz' and for any number that is a multiple of 5, print 'Buzz'. For numbers that are multiples of both 3 and 5, print 'FizzBuzz'.

## Deployed Page

View the Fizz Buzz Project here: https://sophia4422.github.io/fizz-buzz/

## Screenshot

![](./assets/images/fizz-buzz-2.png)

## Contact Me

If you have any questions, please contact me via email: sophiapwall@yahoo.co.uk

-My Github profile is [here](https://github.com/sophia4422)

-My LinkedIn profile is [here](https://www.linkedin.com/in/sophia-wall/)

-My Portfolio is [here](https://sophia4422.github.io/my-portfolio/)

## JavaScript Code

<details>
<summary>See the JavaScript code here</summary>
<br/>

```
    //declare a function that takes in two parameters

    const fizzBuzzAnswer = (value1, value2) => {

    //this variable is set to an empty string
    let returnValue = "";

    //print out the numbers between 1 and 100 using a loop

    //start at 1, whilst i is less than 100, add one each time

    for (let i = 1; i <= 100; i++) {

    //how to know if the number is divisible by 3 or 5 using the modulus operator

    //if both values are divisible by value1 (3) and value2 (5) return fizzbuzz

    if (i % value1 == 0 && i % value2 == 0) {
      returnValue += "FizzBuzz, ";

      //if it is only divisible by value1 (3) return fizz
    } else if (i % value1 == 0) {

      returnValue += "Fizz, ";

      //if it is only divisible by value2 (5) return buzz
    } else if (i % value2 == 0) {

      returnValue += "Buzz, ";

    } else {

      //otherwise just return the number it is
      returnValue += i + ", ";
    }

    }
    return returnValue;
    };

    //display the fizzbuzz function in the html

    const buzzIt = () => {
    let output = "";

    const val1 = document.getElementById("fizzValue").value;
    const val2 = document.getElementById("buzzValue").value;

    output = fizzBuzzAnswer(val1, val2);

    document.getElementById("results").innerHTML = output;
    };

```
