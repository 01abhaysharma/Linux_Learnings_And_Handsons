# What is Linux?

Linux is operating system software that runs on a hardware computer system. 
An operating system is software that allows other programs like word processors and web browsers to be installed and run on a computer.
Your cell phone, tablet, laptop and desktop all need an operating system to run the software (often called applications) you want to use. 


To understand why Linux skills are unique, let’s examine the graphical user interface (GUI). This is the interface that you are probably using on your smartphone, tablet or computer today. 
A GUI displays icons and images that you can select to tell your device what you want to do or use. 
Behind the GUI, is a code that a programmer developed. When you click on an icon or folder in a GUI, it sends a command to the code telling the system what to do

Linux desktops use a GUI but it also has a more efficient tool for carrying out the same actions as a GUI, the command-line interface (CLI).
The Linux command-line is a text-based interface that accepts commands that you type into it. 
These commands cause an action to be executed onto the computer system’s operating system. Of course, windows and icons are easy to use, however, the command-line is often the hero when it comes to system administration and troubleshooting as it gives a clear picture of what the system is doing at any given moment.


# Basic Command Syntax

What is a command? 

A command is a software program that when executed on the CLI (command line interface), performs an action on the computer. 
When you type in a command, a process is run by the operating system that can read input, manipulate data and produce output. 
A command runs a process on the operating system, which then causes the computer to perform a job.

To execute a command, the first step is to type the name of the command. Click in the terminal on the right. Type ls (lowercase letters L and S) and hit Enter. The result should resemble the example below:

<img width="473" alt="image" src="https://user-images.githubusercontent.com/85710889/212458782-0ee5b8a1-36f4-45c3-aaf9-2ea181f86ce7.png">

the ls command displays a listing of information about files. 

Note: Every part of the command is normally case-sensitive, so LS is incorrect and will fail, but ls is correct and will execute.

<img width="461" alt="image" src="https://user-images.githubusercontent.com/85710889/212458832-305f2988-dd27-464e-a9bd-3ecbfacb9b20.png">

Most commands follow a simple pattern of syntax:
command [options…] [arguments…]

In other words, you type a command, followed by any options and/or arguments before pressing the Enter key. 
Typically options alter the behavior of the command and arguments are items or values for the command to act upon. 

Although there are some commands in Linux that aren’t entirely consistent with this syntax, most commands use this syntax or something similar.
In the example above, the ls command was executed without any options or arguments. When this is the case, it’s default behavior is to return a list of files contained within the current directory.

<img width="458" alt="image" src="https://user-images.githubusercontent.com/85710889/212458872-bf0559ae-9a95-4953-8261-74e99b042611.png">

# Arguments

Command syntax: command [options…] [arguments…]

An argument can be used to specify something for the command to act upon. 
The ls command can be given the name of a directory as an argument, and it will list the contents of that directory. 
In the next example, the Documents directory will be used as an argument:

<img width="463" alt="image" src="https://user-images.githubusercontent.com/85710889/212458984-e85014aa-dadf-4b47-97ef-9c38d58e490b.png">

The resulting output is a list of files contained with the Documents directory.

(Because Linux is open source, there are some interesting secrets that have been added by developers. For example, the aptitude command is a package management tool available on some Linux distributions. This command will accept moo as an argument:

<img width="448" alt="image" src="https://user-images.githubusercontent.com/85710889/212459051-ea3ed469-4c9c-4500-bd3d-c1dac7281870.png">

