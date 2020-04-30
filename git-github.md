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

