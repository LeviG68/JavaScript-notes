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
* Typeof is a keyword in JavaScript that allows you to check the type of a value.
* You can use Typeof in the console by writing typeof followed by a space and a variable or value. That will tell you whether its a number, a sting , or any of the other types.
* Numbers in JavaScript are pretty simple.
  * You can create an integer, which is a whole number like 100 or you can create a float which is a number that has a decimal like 100.5.
  * You need to beware of is mixing types.
    * If you try and do math with a string type for example you start to get into concatenation.
    *  like const math = "1" + "1" will output "11" because of the concatenation of the two string compared to "2" if you where just doing math.
    *  That is refer to in JavaScript as "the plus sign is loaded" meaning the plus sign can be used with numbers to add, with stings to concatenate, and then there is a lot of room to run into bugs.
    *  If you try to do math with strings, it will convert them for you if you are doing subtraction, division or multiplication, but not for addition.
    *  When doing math, we need to make sure that we are dealing with true numbers and not mixing types.
 * Along with number we also have what we call helper methods.
   * If you go into the browser console and type "Math." you will see a lot of built in helper methods.
  ### Helper Methods
  *There are four you are most likely to use.
    1. Math.round()
    2. Math.floor()
    3. Math.ceil()
    4. Math.random()
 1. to use Math.round(), you pass a value in between the parenthesis () (that is referred to as passing a value). It will return to you number that was passed in, round up or down depending on the number. Math.round(20.5) -> 21 or Math.round(20.2) -> 20.
 2. Math.floor() which will give you the lower end of that number. -> like Math.floor(20.2) -> 20 or Math.floor(20.9999) -> 20
 3. You have Math.ceil() and that will give you the upper number. -> like Math.ceil(20.99) -> 21 
 4. There is Math.round() which will give you a random number every time between 0 and 1. -> Math.round() -> output some long decimal number like 0.014844055
   
### Modulo and Power operators
* Along with multiplication, division, subtraction and addition, we have two more operators which are called the modulo and the power.
  * example, in the console that evaluates to:
    const smarties = 20;
    const kids = 3;
    const eachKidGets = smarties / kids;
    console.log(`Each kid gets ${eachKidGets}`);
    output --> Each kid gets 6.66666666667
    That number is not going to work since we are not going to split the candy.
    So instead, what we can do is specify that it is a whole number of smarties that we need and can't round up so we can use Math.floor().
    Modify the code to --> const eachKidGets = Math.floor(smarties / kids);
    output --> Each kid gets 6.

# 9 Types Objects <a name="Lession 9"> Lession 9 </a>
* Objects in JavaScript are the biggest building block and almost everything in JavaScript is an object.
* Object are used for collections of data or collections of functionality.
* You need to know that when something is an object in JavaScript, it's because we want to group things together.
* If you have been using random variable like const name = 'Levi' or const age = 100;. That is not the best way of doing things, because the values are not associated.
* What you can do instead is create an object called person.
  * We will create it using two curly brackets and a semi colon. That is the most common way to make an object, but there are other ways that we will go over.
    const person = {};
  * Inside of the person object, you have what are called properties and values. 
      const person = {
        first: 'levi',
        last: 'Toddy',
        age: 55,
      };
  * What we have done here is created an object that allows us to group together variables. In the example above we have first , last  and age variables all contained within an object for a collection that is "person".
  * In the console, if you type person it will return the value, which is the object.
  * If you check the typeof the person variable, it will return the object type.
* You might have noticed that the object properties are in a different order than what we typed, the short and skinny of that is the order doesn't matter in an object. If you need order to matter, then use array or Map data structure.
* To access the properties, there are different ways to do that.
  * There is dot notation 
      person.first --> "Levi"
      person.last --> "Toddy"
* When we get deeper into objects in the future, we will go over the other ways to do that as well, like nesting objects and objects vs reference and copying objects.

# 10 Types - Null and undefined <a name="Lession 10"> Lession 10 </a>
* Two ways to express nothing in JavaScript, that is with Null and undefined.
* Undefined - if you create a variable and set it to nothing, then it will be undefined.
  * Undefined is something that has been  created ( a variable ) but has not yet been defined.
    * The same thing goes for properties of objects, why ? because there is nothing there.
  
* Null - is a value of nothing, whereas undefined is a variable that has not yet had a value assigned to it.
  * NOTE - you can not use the const variable without setting a value.
  


# 12 Functions Built In <a name="Lession 12"> Lession 12 </a>
* allow us to group a set of statements 
* general related to one another 
* When you pass in data it is called an Argument in a function.
* example --Math.max (10, 12) -- this line is called a statement. Math.max is looking at the two numbers in the parenthesis and evaluated with is the max number.
*  In Math.max(10, 12) the data in the parenthesis are called arguments. Sometimes it will return you data that is the answer.
*  Built in things in JavaScript like console.log, Math.max() and Math.floor(), parseFloat(), Date.now() etc...

  
