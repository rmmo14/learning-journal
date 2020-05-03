javascript notes go here 

# Javascript
It is an **integrated programming language**.

A browser uses an interpreter or a scripting engine to translate your instructions to the page. 

Its process is:
1. browser receives an html page
1. creates a model of the page and stores it in memory
1. shows the page using the engine

The saying, calling a method of an object refers to ```OBJECT.METHOD()```

# Basics of JS

> A script is a series of instructions that a coputer can follow one-by-one. Each individual instruction or step is konown as a statement. Statements should end with semicolons!

Single-line comments|Multi-line comments
---------------------|-------------------
use ```//TEXT ```|use ```/* TEXT */```

A **variable**, in my words, similar to mathematics definition it is a placeholder for a number, name, data type, etc. As in math, you must always introduce (declare) the variable before assigning (=) it a value aka ```var X;```.

A few data types are: 
+ **Numeric**: for numbers, can be any rational number
+ **String**: for text and other characters (always in matching quotes)
+ **Boolean**: true or false 

\*You can always change the value of your variable simply by declaring it a new value. 

Rules for naming variables:
1. must begin with a letter, dollar sign, or underscore, **NOT** a number 
1. **DO NOT** use dash or period 
1. cannot use keywords specific to code like "var" and reserved words
1. Though it **IS** case-sensitive, it is not good practice to give files the same name
1. feel free to use camel case or snake case

### Live notes from class
```new Date()``` gets the current date.

``` today.getHours()``` gets todays hours.

```document.write(<h3> VAR or TEXT </h3>)``` spits out the text or string stored in the variable. 