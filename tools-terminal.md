# Classifications of Text Editors

There are many types of text editors to house coding projects. The type of text editor to use varies by the coder and their preferences. There are four important features to look for:

1. Code completion
1. Syntax completion
1. Variety of themes
1. Variety of extensions

Coders have to consider these four features becaue they will be spending most of their time on these text editors. The completion features are **essential** for a coder because even a few seconds saved add up over a long epriod. This feature also helps coders *avoid* coding mistakes or missing closing code. Viewing a screen for long periods of times can take a toll on coders eyes. It is suggested to use darker background white bright text rather than the normal white background and dark font. The extensions are like web page extensions allowing the text editor outside/extra features which may help their page or code. 

## Additional Readings
As with other code, these too follow certain formulas. When you have a prompt, yo umust enter a command a space and command line arguments. If there is an option before the line argument (they are used to modify behavior of the command) you must put a **space** between as well. In other words:

```DISPLAY.NAME: COMMAND OPTION ARGUMENT```

Once enter is hit it should spit out your command. Which the text editor will always spit out a display name showing it is ready for a new command. 

>*The Shell, Bash* \:
> it is part of the operating system that defines how the terminal will behave and looks after running the commands for you.

There are various shells available but **bash** is more common and it stands for *Bourne again shell* 

> *echo* \:
> used to display a system variable stating your current shell. 
\*Note: if it prints something ending in bash then you're all set. 

As with other code languages, shortcuts will make life easier and will help avoid code typos. 

Here are some shorcuts throughtout the reading:


Shortcut|Description
---------|------------
prefill|the program stores previous commands and offers them as suggestions
\~ | home directory. rather than ```/home/NAME/DOCUMENTS``` can use ```~/DOCUMENTS```
\. | reference current directory, as ```./DOCUMENTS```
\.\. | reference to the *parent directory*. This allows you to go higher up in the hierarchy. 
cd | ```cd LOCATION``` specifies the location you want to change into.
Tab Completion | when you start typing a path the program with suggest an auto complete command. Hit the tab key to view the possibilities. 


## Moving Around the System

To be able to work effectively in Terminal we must be able to know where we are in the system. To help us we can use **pwd**, *Print Working Directory*, it tells us our current working directory. Use this often to remind where we are at. 

The command **ls**, or *list*, is used to show what is in the current location. Its general formula is 
```ls OPTIONS LOCATIONS```

\* Though the bolded phrases are optional

The command ```-l``` represents a long listing, and they have:
+ first charachter determines normal file ```-``` vs directory ```d```
+ next 9 characters are permissions 
+ followed by number of blocks
+ followed by group file or directory it belongs to
+ followed by file size
+ followed by modification time
+ Lastly by the actual name 

The argument ```/etc``` is used to specify to list the **contents** of the directory.

## Paths

Referring to a file or directory uses either relative or absolute paths, which we can use either one. There is a heirarchy in the file system with **root directory** at the very top which is denoted by ```/```. As a root in real life may have roots from roots, root directory too has subdirectories which have subdirectories and so on which may house various files. 

Absolute | Relative
---------|----------
Specifies location in relation to the root directory. Can be spotted because they begin with ```/``` | Specifies location in relation to where we are currently in the system, and they do not have a slash. 
More precise | A little more vague

\* Some new codes I have questions as of so far into the reading ```bin boot dev lib var```

### Moving Around Locations

To move around the system we use ``cd LOCATION``. Running it without a LOCATION will take us back to the home directory. 

## More on Files

*Everything is a file!*

As noticed in file folders, ```.wxyz``` characters after the file name describe the type of file. 

The formula ```file PATH``` helps us confirm the type of file of the item. 

**BE CAREFUL WITH CASE SENSATIVITY!**

**Spaces** in this program are used to separate commands so when referencing a file with a space in its file name we can use 

+ Quotes, either single or double
+ Escape Characters, ```\``` which nullifies the next character

Distinguishing hidden files is done by a ```.``` as its first character of the File Name. This is the way to create a hidden file too. 

The ```-a``` command option after ```ls``` will list hidden files. 

The ```-A``` command option after ```ls``` will not list implied ```.``` and ```..```

## Manual Pages

> **Manual pages** are a set of pages that explain (*synopsis*) every command in the system and description of what they do. It will also list the command line options available for the COMMAND YOU WANT. 

To bring up the manual pages use ```man COMMAND YOU WANT```, and to exit it press ```q```.

### Search Keywords
To search keywords in manual pages use ```man -k SEARCH TERM```. If you are already in a manual page simply press ```/ SEARCH TERM``` and hit enter, pressing ```n``` to go through each item.

long hand | short hand 
----------|-----------
easier to remember commands | easier to chain multiple commands
line options begin with ```--``` | line options begin with ```-``` and can group them like ```-pv```

## Manipulating Files

### Making directories

 *Be organized with YOUR FILES* 
 
 Use ```mkdir OPTIONS DIRECTORY``` to create a directory. Using the option ```-p``` with it tells it to make parent directories as needed. The option ```-v``` tells it to tell us what it is doing. 

### Removing directories

Use ```rmdir OPTIONS DIRECTORY``` to remove a directory. It supports both ```-v``` and ```-p```, but the directory must be empty to be removed. 

### Making blank files

Use ```touch OPTOINS FILENAME``` to create blank files. This command is useful to modify the access and modification times on a file. Apparently students try to use this feature to change the time last modified on an assignment :joy:

### Copying files or directories

Use ```cp OPTIONS SOURCE DESTINATION``` to copy a file with DESTINATION as its name. \* Should use ```man``` to see other options for this command!

> Question I have so far on the reading, how do we properly use the cp command?

The option ```-r``` stands for recursive and it copies directoreies. It looks at all files and directories and subdirectories within it, go into them and do this over and over again. 

### Moving files or directories

Use ```mv OPTIONS SOURCE DESTINATION``` to move file, similar to the **cp** command but doesn't use the **-r** option. 

### Renamining files or directories

Use the **mv** command along with options as ```mv FILE NEWNAMEOFFILE```. Can think of it as it is moving the file named FILE into a new file named NEWNAMEOFFILE. 

### Removing files or non empty directories

Use ```rm OPTIONS FILE``` to remove or delete a file. For directories it brings up ```-r``` again, which I need more clarification on. 
> Ask about ```-i``` which stands for interactive.
