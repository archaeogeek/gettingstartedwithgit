# Command-line Primer

## What's the Command-Line?

Aka, **Terminal** on the Mac or Linux, **cmd** or **Cygwin** on windows. Might also be called **Command Prompt**, **CLI**, **Bash**, **DOS**...

We will call it the Command Prompt throughout this workshop.


## Windows

Start -> Windows System -> Command Prompt

Looks like:

    somethingsomething >

## Mac

Applications -> Utilities -> Terminal

Looks like:

    somethingsomething $

## Linux (Ubuntu)

Accesssories -> Terminal

Looks like:

    somethingsomething $

## Basic Usage

To the left of the prompt symbol (indicated by ```somethingsomething``` above) will be helper info, which may differ from install to install. Generally it will tell you which directory you are in, possibly which user you are. It can even be configured to tell you which git branch you are in. 

The prompt symbol will not be included in the commands you follow in this workshop. When typing a command, assume you are starting to the right of the prompt above. 

All commands have the following format, where options and arguments are not always required. This is indicated by the square brackets around them- these are not part of the command:

    commandname [options] [arguments]

They are finished, or submitted, with the return or enter key on your keyboard.

For example, a command with no options or arguments is:

    whoami

Type this and press enter- it will respond with your username.

A command with an argument is:

    mkdir dirname

This will create a new folder with the name ```dirname``` in the current working directory.

## Directory Notation

This is done differently in Windows compared to Mac and Linux. Mac and Linux do not use drive letters, and use a **forward slash** to denote directories. Windows uses drive letters, and a **back slash**.

### Windows

    C:\Users\Jo\mydocs

### Mac and Linux

    /Users/Jo/mydocs


## Caution

Many commands are slightly different in Windows, compared to Mac and Linux. For example the following commands do the same thing, which is to print the contents (files and folders) in the current directory:

### Windows

    dir

### Mac or Linux

    ls

In some cases, the same command behaves differently in Windows compared to Mac and Linux. For example the following variation on the ```mkdir``` command above will create the following structure in all cases:

    dir1
    ....dir2
    ........dir3

### Windows

    mkdir dir1\dir2\dir3

### Mac and Linux

    mkdir -p dir1\dir2\dir3

## Navigation

**Backspace** clears text in an un-submitted command

**Tab** autocompletes a command or directory structure (where possible)

**Up and Down Arrows** cycle through the current command history

## Summary of Useful Commands

(Copied from [https://tutorial.djangogirls.org/en/intro_to_command_line/](https://tutorial.djangogirls.org/en/intro_to_command_line/))

|Command (Windows)|Command (Mac OS / Linux)|Description |Example|
|-----------------|------------------------|------------|-------|
|exit             |exit                    |close the window  |  exit
|cd|  cd | change directory  |  cd test
|cd | pwd |show the current directory  |cd (Windows) or pwd (Mac OS / Linux)
|dir |ls | list directories/files | dir
|copy |   cp |copy file  | copy c:\test\test.txt c:\windows\test.txt
|move |   mv | move file  | move c:\test\test.txt c:\windows\test.txt
|mkdir |  mkdir  | create a new directory  |mkdir testdirectory
|rmdir (or del)|  rm | delete a file |  del c:\test\test.txt
|rmdir /S |   rm -r  | delete a directory | rm -r testdirectory



