# Hello! I'm known as RealToughCandy online, but you can call me Candy. 

#### Today, you're going to learn the basics of JavaScript. Even if you've never seen or used JavaScript before, that's OK! We're going to go through this together slowly and methodically so you can start using the language's building blocks to program your own JavaScript programs by the end of this lesson. If you have any questions, please feel free to join my [Gitter chatroom](https://gitter.im/realtoughcandy-community/Lobby) where welcoming developers will be happy to help you! 

##### Prerequisites: Basic knowledge of your browser's JavaScript console to run programs.
---
---
                                  		  Let's Get started!
----
---

# JavaScript is the language of the web. 

### In this lesson, I’m going to show you a few building blocks of the JavaScript language, including variables, arrays, conditional statements, and loops.  

A primary building block - one that you’ll work a lot with - is called a **_variable_**. Think of a variable simply as a container.  You can store all kinds of things in this container, like numbers, strings (which store a series of characters like ‘John Doe’), repetitive bits of code called _functions_, and lots of other things we’ll dive into later. 

# First, let’s build a _variable_ using a two-step process. 

To use a variable, we need to **_declare_** it. And to declare a variable, we'll simply type the keyword _var_ and name it something unique, followed by semi-colon:

``` javascript 
var thisLadyIsCool;
```
We've decalred our variable as _thisLadyIsCool_. . .Cool! 

Second, let’s initialize the variable. This is the part that gives it a value.
```javascript
thisLadyIsCool= "Linda"
```

Because Linda is a **string**, we put her name in double quotes. (We could also use single quotes if we wanted, but those can be tricky for new learners. More on that in a future lesson). 

We can actually combine this two-step process into a one-step process to make it more efficient: 
``` javascript
var thisLadyIsCool = "Linda" 
```
Now, our variable _thisLadyIsCool_ contains the value "Linda". 

Cool, right? Understanding the basics of variables means we can start building bigger things with them, like **_arrays_**.  

P.S. Using _var_ to declare a variable is the main way of doing things, but an update in the JavaScript language has made it so we can get even more specific. The keywords _let_ and _const_ are part of the ES6 JavaScript syntax and allow for greater specificity when declaring variables. We’ll discuss their nuances and when to use each as you get more comfortable with JavaScript basics. 

# Let’s talk about **_arrays_**. 

In JavaScript, an **_array_** is a special type of variable that can hold a list of values. If you have a list of grocery items, you could store those items in the array like this: 

```javascript
var item1 = 'olives';
var item2 = 'fresh mozzarella';
var item3 = 'organic tomatoes';
```

But this technique is very limiting. What if you wanted to loop through the grocery items to find something specific? Further, what if your grocery list was 40 - or even 400 - items? That could get ugly, quickly. The solution is to use an array.  Once again, we’ll use a two-step process to create an array. 

First, let’s declare an empty array: 
```javascript 
var groceryItems = [];
```
In order for JavaScript to understand our list, our grocery items need to go inside the brackets, separated by commas. Let's get to it! 
```javascript
var groceryItems = ["olives", "fresh mozzarella", "organic tomatoes"];
```
This works, but it's a little hard to read. Let’s make it easier to read by spacing the values out: 
``` javascript
var groceryItems = [
  "olives”", 
  "fresh mozzarella", 
  "organic tomatoes"
];
```
Note that the last value in an array is not followed by a comma. 

### OK, so this array exists — now what? Now we are able to access individual items in the array by referring to its index number. The first element’s index number in an array is [0]. 
Following that logic, [1] is the second element, [2] is the third… and so on. If we wanted to access the 300th item in our theoretical array, its index number would be [299]. To access an item, type the variable given to the array, followed by the index number of the item you want to access. For example, in the above example, if I wanted to access the item "olives" I would type _groceryItems[0]_.

### If we wanted to access "organic tomatoes" in our array, how would we do that?

Answer: We would type groceryItems[2]. 

We will take a closer look at arrays, including how to add and delete items of an array, in an upcoming lesson. Let's explore another building block of JavaScript, _conditional statements_. 
# _Conditional Statements_
### “Hey, buddy. If you are going to arrive after 6 pm, give me a phone call.” 

##### The above  is an example of a conditional statement we might use in every day conversation. 

Similarly, JavaScript has **_conditionals_** that determine how programs are executed. In this lesson, we’ll learn about JavaScript conditionals and how to use them. 

Just like in real life, conditional statements are used to perform different actions based on different conditions.

In JavaScript, you will use these conditional statements : 
###### if — Use if to specify a block of code to be executed, if a certain condition is true.
###### else — Use else to specify a block of code to be executed, if the same condition is false.
###### else if — Use else if to specify a new condition to test, if the first condition is false.
###### switch — Use switch to specify numerous alternative blocks of code to be executed.

## If
Let’s go back to our real-life conditional and turn it into something JavaScript can understand, using an _if_ conditional statement. 

**In English**: “If you’re going to arrive after noon, give me a phone call.”

**In JavaScript**: 
First, we’ll convert "noon" into something JavaScript can interpret: 12. So "noon" is now 12. 
#### Now, code the conditional: 

``` javascript
if (arrivalHour > 12) {
	message = "Hey, I am calling to say I am going to be arriving after noon!";
}
```
## Else
Let’s add another conditional to our English statement:
##### “If you are going to arrive after noon, give me a phone call. Otherwise, send me a text.”

It's the equivalent of a JavaScript if/else statement. 

**Now in JavaScript:**
```javascript 
if (arrivalHour > 12) {
	message= “Hey, I am calling to say I am going to be arriving after noon!”;
} else {
	message = “Hey, here is my text; I am not going to be arriving after noon!”;
}
 ```
Let’s keep pushing forward with more conditionals. This time, we’ll add _else if_.
## Else...if
##### “Hey, buddy. If you’re going to arrive after noon, give me a phone call. But if you arrive before noon, I’ll be in a meeting, so send me an email. Otherwise, send me a text.” 

The above was an example of an English _else if_ conditional. A phone call will be made after noon, an email will be sent before noon, and a text will shoot off for any other circumstance (which, in this case, is _exactly_ at noon). 
Notice how we’re just adding on to our original _if_ statement? It comes back to that building block concept I told you about at the very beginning of this lesson. We’re just going to keep on building! 
``` javascript
if (arrivalHour > 12) {
	message = "Hey, I am calling to say I am going to be arriving after noon!";
} else if (arrivalHour < 12) {
	message = "Hey, here is my email; I am not going to be arriving after noon!";
} else {
 message = "Hey, here is my text!;"
}
 ```
 ## Switch
Lastly, we have the _switch_ conditional statement. We use this when multiple blocks of code need to be executed. The switch statement helps us avoid using an overwhelming number of if/else if statements. Here's how it works:
* The switch expression is evaluated once.
* The value of the expression is compared with the values of each case.
* If there is a match, the associated block of code is executed.

With a switch statement, there’ll be some code concepts we haven’t covered yet, but it’s more important to  pay attention of the syntax right now. 

Here is an example of a switch statement with two case statements, and a fallback known as _default_.
```javascript
switch (arrivalHour) {
    case "After noon":
        console.log("Hey, I am calling to say I am going to be arriving after noon!")
        break;
    case "Before noon":
        console.log("Hey, here is my email; I am not going to be arriving before noon!”")
        break;
    default: console.log("Hey, here is my text; I am not going to be arriving after noon!")
}
```
Fittingly, the _break_ keyword breaks out of the switch block if the condition is met. This will stop the execution of code. If _break_ is omitted, the next code block in the switch statement is executed.



##### Once we get some more practice with _if/else if/else conditionals_, we will explore the switch statement more. Again, the most important thing as a beginner is to focus on the syntax above, since we’ll be covering in depth switch statements in a later lesson. 

# Loops
Loops do things on repeat… Over. And over. . .And _over_ again, however many times you specify. In JavaScript, the various loop mechanisms let you choose the start and end point of the loop. 
#### JavaScript has two main methods for running the same code repeatedly.

```
while - loops through a block of code while a specified condition is true
for - for loops are like an extended while loop. 
      They loop through a block of code a number of times, and include additional components, 
      such as initializers, for constructing them.
```
### I want JavaScript to count up to the number 2. What should I use? 

I should use a _for_ loop, like this: 
```js
var i;
for (i = 0; i < 3; i = i + 1)
{
    console.log(i);
}
 ```
This will print out the following:
```
0
1
2
 ```
The _for_ statement has three parts:

**Initialization** - Initializes the iterator variable i. In this example, we initialize i to 0.

**Condition** - As long as the condition is met, the loop continues to execute. In this example, we check that i is less than 3.

**Increment** - A directive which increments the iterator. In our case, we increment it by 1 on every loop.
We can also write a shorter notation for the statement by inserting the variable definition inside the for loop and incrementing using the ++ operator, like this:
```javascript
for (var i = 0; i < 3; i++)
{
    console.log(i);
}
 ```
 ### Remember our lesson on arrays earlier on? What loop method would we use to loop through our grocery items?
To iterate over our array and print out all of its items, we'll again use the _for_ loop. 
```javascript
var groceryItems = ["olives", "fresh mozzarella", "organic tomatoes"];
for (var i = 0; i < groceryItems.length; i++)
{
    console.log("The type of groceryItems in index " + i + " is " + groceryItems[i]);
}
 ```
This prints out the contents of the array:

```
The type of groceryItems in index 0 is olives
The type of groceryItems in index 1 is fresh mozzarella
The type of groceryItems in index 2 is organic tomatoes
 ```
Notice that we used the _length_ property of our array, which returns the number of items in the array, so we know when to stop iterating.

# The while statement

The _while_ statement is a simplified version of the _for_ statement. It checks if an expression evaluates to true, and continues to run so long as it stays true.

Let's take the classic _99 Bottles of Beer on the Wall_ folk song. 

In English, it goes: "Ninety-nine bottles of beer on the wall, ninety-nine bottles of beer. You take one down, pass it around...ninety-eight bottles of beer on the wall." And so on, until there no more bottles of beer.
The JavaScript version of the classic "99 Bottles of Beer on the Wall" looks like this:
```javascript
var i = 99;
while (i > 0)
{
    console.log(i + " bottles of beer on the wall");
    i -= 1;
}
```
 ## Beyond the two basic loops
 
 There are two other kinds of loops in JavaScript that extend the _for_ loop and the _while_ loop. 
 ```
for/in - loops through the properties of an object
do/while - This loop will execute the code block once, before checking if the condition is true, 
            then it will repeat the loop as long as the condition is true.
```
### For now, practice the two basic _for_ and _while_ loops in your browser's JavaScript console. We will have lots of time later to investigate the _for/in_ and _do/while_ loops while experimenting with their uses. 

# Congratulations! You made it to the end of Lesson 1! 
