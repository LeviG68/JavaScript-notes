a# Beginner JavaScript notes

## Table of Content
[Introduction] (#introduction)
6. [Lession 6 Types - Introduction ] (#Lession 6)
12. [Lession 12 Functions Built in ]  (#Lession 12)
13. [Lession 13 Functions Custom]  (#Lession 13)
    
# 6 Types - Introduction <a name="Lession 6"> Lession 6</a>
* So we have thins such as number, text, true or false. 
* All those this are called types, and what are all the of the different possible options are call JavaScript types.
* The 7 different types in JavaScript are:
  1 String - a string is anytime that you have some text (you will often see that in a single, double or backtick).
  2 Number - a number (regardless of whether it has decimal place in it. Some languages have multiple types to deal with numbers, but JavaScript only has the one).
  3 Object - this is a special one, Everything in JavaScript is an object, and we will understand what that is when doing methods. Everything that we use functions, dates and arrays are just objects at the end of the day. All other types except for objects are referred to as the "primitive types".
  4 Boolean - true or false.
  5 Null - can be used to set a variable to nothing (we will talk more about undefined and null shortly).
  6 undefined - can be used to set a variable to nothing ( we will discuss difference between undefined and null).
  7 Symbol - this is a new one to JavaScript, and it will always give us a guaranteed unique identifier. This is useful for when you are trying to come with a unique identifier inside of an object and you want to make sure are not overwriting something that already exists with that ID.
  
# 7 Types - Strings <a name = "Lession 7"> Lession 7 </a>
* Strings are used for holding text. There are 3 different ways  to create string texts in JavaScript:
  1 - Single quote 'text'.
  2 - Double quote "text".
  3 - Back-ticks `text`.

* A /* comment will open up what is called a block comment. You can close the block comment anywhere you wish to close it ( it can be a multiple line or only a single line).
*  A // can be used as a single line comment or used to comment a code block as well when debugging.
*  What are the difference between the single and double quotes ?, nothing both do the same thing.
*  The only reason why we have them is for sentence structure where you might need to use and apostrophe s (she's).
*  Before backticks where introduced, they only thing you could use to achieve that is concatenation.
   *  Another benefit of backticks is interpolation and concatenation.
   *  Concatenation - is when two or more strings are combined into one.
   *  Interpolation is when you put a variable inside of a string.

* Backticks
  * with backticks you can interpolate the sting like this.
      * const name = "Levi"
      * const hello = `Hello my name is ${name}. Nice to meet you`;
      * The ${} syntax can only ever be used in backticks. It is the easiest way to pop a variable into a string.
      * Almost anything can go between the curly brackets {} in that syntax. For example you can do math.
          - const hello = `Hello my name is ${name}. Nice to meet you. I am ${1 + 100} years old`;
      * JavaScript will run whatever is inside of the curly brackets in that syntax (weather it is a variable or an actual statement) and it will return the value that's inside of it.
      * To reiterate: 
        * you can do multiple lines with backticks, variable interpolation, and there is something a little more advanced that is called a tagged template literal, but that is more for when you get into functions.

# 8 Types - Numbers <a name="Lession 8"> Lession 8 </a>


# 12 Functions Built In <a name="Lession 12"> Lession 12 </a>
* allow us to group a set of statements 
* general related to one another 
* When you pass in data it is called an Argument in a function.
* example --Math.max (10, 12) -- this line is called a statement. Math.max is looking at the two numbers in the parenthesis and evaluated with is the max number.
*  In Math.max(10, 12) the data in the parenthesis are called arguments. Sometimes it will return you data that is the answer.
*  Built in things in JavaScript like console.log, Math.max() and Math.floor(), parseFloat(), Date.now() etc...

  
