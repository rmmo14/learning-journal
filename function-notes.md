## Script
- Naming convention: name implies functionality or use one word
- declaration: when the function is defined / when the logic is created
- parameters: a special type of variable created and used in a specific function
- arguments: when you call on your function you pass values as arguments, and they take the place of your parameters
- return statement: manages output
- local variables: variable declared **inside** a function
- global variables: variables created in a GLOBAL namespace

Computers need step-by-step instructions to run its commands, in other words, a script. 

Scripts are created by first having already defined the goal of the page, and then with the script with commands to lead you to the goal. They are often shown as flowcharts showing each step that the computer will follow. 

## Arrays
It is a special type of variable that stores a list of values. They are helpful when you do not know how many items a list will containg. Values in an array are separated by commas. The values in an array can be different data types! 
**Array literal** is the techinque when creating an array. 

ex:
>```var colors;```
```colors = ['color1', 'color2','color3']```

or 

You can use an **Array constructor**
>```var colors = new Array('color1', 'color2','color3');```

To retrieve an item in the array list, the array name is specified along with the index number in square brackets:
>```var itemThree; itemThree = colors[2]```

### To change a value in an array
After the array has already been made, you can change a value by specify the index number and asigning it the new value
>```colors[2]='beige';```

\*This changes "color3" in my array to "beige".

# Functions

Functions let you group a series of statements together to perform a specific task. When declaring a function:
>`function sayHello(){ document.write('Hello');}` 

Calling a function is when you execute all of the statements between the curly braces. When you declare a function you give it parameters (interchangable with arguments), where they act like variables. 
>`function getArea(width, height){ return width*height;}`
**Argument** is the specific detail used on the parameters. 




