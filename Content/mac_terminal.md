<h1 align="center">Terminal on Mac</h1>

* https://www.makeuseof.com/tag/beginners-guide-mac-terminal/
* https://www.library.unlv.edu/sites/default/files/inline-images/wRkOVKa8PENf9196S4Q6Kpjbo7QwuzviXOI20clS9QHEPtJQY6.pdf
* https://www.techrepublic.com/article/16-terminal-commands-every-user-should-know/

A zsh (or Bash) command typically follows this pattern: 

```zsh
[Command] [Options] [Input or Path to File or Directory]
```

## Moving Around Using Terminal

### pwd
Prints the working (your current) directory.

```zsh
(base) caseydelaney@Caseys-MacBook-Pro ~ % pwd
/Users/caseydelaney
```

### ls
View the directories and files that are available in your location.

```zsh
(base) caseydelaney@Caseys-MacBook-Pro ~ % ls
Applications	Desktop		Documents	Downloads	Library		Movies		Music		Pictures	Public		anaconda3
```

### cd
Change the working directory.
* Use quotes for folders/files that have a space in them

```zsh
(base) caseydelaney@Caseys-MacBook-Pro ~ % cd /Users/caseydelaney/Documents/"CSE 6242"
(base) caseydelaney@Caseys-MacBook-Pro CSE 6242 % pwd
/Users/caseydelaney/Documents/CSE 6242
```

To get back to the initial working directory, simply use cd without a following file path.

```zsh
(base) caseydelaney@Caseys-MacBook-Pro CSE 6242 ~ % cd
(base) caseydelaney@Caseys-MacBook-Pro % pwd
/Users/caseydelaney
```

### open
Open a file.
* You can include the file path in the command or just choose the folder that contains the file as your pwd:

```zsh
(base) caseydelaney@Caseys-MacBook-Pro CSE 6242 % cd /Users/caseydelaney/Documents/"CSE 6242"/HW1/Q1
(base) caseydelaney@Caseys-MacBook-Pro Q1 % open edges.csv
```

### clear
Clear the Terminal screen of all previous commands.
* Can also press Command + K

```zsh
(base) caseydelaney@Caseys-MacBook-Pro Q1 % clear
```

### man
Displays a manual of a command to help you better understand the command. The following fields are displayed for each command:
* NAME
* SYNOPSIS
* DESCRIPTION
* EXAMPLES
* and more

To get out of a manual, simply press Q.

```zsh
(base) caseydelaney@Caseys-MacBook-Pro Q1 % man pwd
```

## Quick Tips

* Capitalization matters when calling folders/files
* You can drag and drop folders into Terminal instead of typing out the filepath
* Using the up arrow will recall commands. Press it once for the previous command, twice for the command before the previous, etc.
