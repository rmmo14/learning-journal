# Github vs Git

## Version Control
Version control is like a central location that holds files and modifications of files. **Centralized Version Control Systems** (CVCS) is a single server storing all changes and versions that can be accessed by various clients which streamlined the collaboration process for coders. The CVCS has a major vulnerability being that the server as a single point of failure. If it goes down than no one can work on it. 

**Distributed Version Control systems** prevents that failur in CVCS by allowing clients to create mirrored repos. Because so many file versions are created teams can collaborate in various combinations. 

## Que es GIT?

+ Snapshots: DVCS stores data in a file system made up of snapshots. It stores it for reference, if the file is not changed then a reference to the stored version is stored. 
+ Local Operations: Git works on local operations meaning you can work on a project even without internet!
+ Tracking Changes: Everything is tracked and noted.
+ Loss of Data: it is extremely difficult for a snapshot of a file to be lost.
+ States: Files in Git reside in either of the three states
    + Committed: Data stored locally
    + Modified: You can edit but not commit files to the database
    + Staged: Flagged a file's changed version to be committed next time

> *Commit*: a saved changed version of your project 
 
 \*Git is the recipe, Github is the kitchen.


A few things Git can do:

 + We can assign messages to commits, they are like writing a caption for your snapshot. 
 + Can save files

 >HEAD: the most recent file. \(You are here\)

A few things Github can do:

+ collab space
+ online cloud for code
+ uses Git to manage teamwork 
    + Version tracking
    + review changes

**Repositories**: it is a collection of files. Some large projects may have multiple repos. 

**Graphical User Interface** (GUI) tools are included in Git. 

There are three ways to get more info on a particular command by:

```git help command```

```git command --help```

```man git-command```

## The steps to import an existing file

**Get to the target project's directory**
- use: ```cd TARGET```

**Create a subdirectory called NAME.git**
- use: ```git init```

**Start tracking repos**
- use: ```git add *.c1```
- then: ```git add FILE```
- then: ```git commit -m "MESSAGE"```

## The steps for cloning/duplicating

**While on github**: Hit the ```+``` button at the top right by profile picture, and be sure to check the read me option. Once created, click the ```clone or download``` button. Copy the link. 

**Head to Terminal**
type in ```git clone LINK``` where LINK refers to the link copied in the step above. 

\*If you want to clone a file with a new name simply input ```git clone LINK NEWNAME```

## Workflow

The local Git has three components
1. *Working directory*, where the file resides
1. *Index*, area used for staging
1. *Head*, points to most recent commit

All files are either tracked or untracked.
Tracked|Untracked
--------|--------
can be modified, unmodified, or staged; part of most recent snapshot. |not in the last snapshot and not ureside in staging area

List of codes:
1. ```git status``` determines the state of files (modified or not).
1. ```git add FILE``` is used to track one file only 
1. ```git add *``` is used to track all files in a repo
1. ```git commit -m "CHANGE" ``` commits changes for file(s)
1. ```git commit -a``` commits a snapshot of all modifications to tracked files
1. ```git push origin master``` pushes changes from the local branch to the origin
1. ```git stash``` used when you don't want to lose modifications not ready to commit; storage
1. ```git stash apply``` used when you want to retrieve hiddenc changes from code above

**Remote repos**, versions of a project residing online or on a network (collab).

### How to save modifications
```git status``` | ```git add MODIFIEDFILE``` | ```git commit -m "NOTE"``` | ```git push origin master```

\*Feel free to use ```git status``` thru out 

