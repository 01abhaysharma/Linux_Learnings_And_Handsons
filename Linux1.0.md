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


# Options

Command sysntax: Command [options…] [arguments…]
Options can be used to alter the behavior of a command. 
In previous example, the ls command was used to list the contents of a directory. 
In the following example, the -l option is provided to the ls command, which results in a "long display" output, meaning the output gives more information about each of the files listed:

<img width="419" alt="image" src="https://user-images.githubusercontent.com/85710889/212566452-2fb03a6d-a8d0-4a20-b3f1-adaf4fcce956.png">

Note: in the command above, -l is a lowercase letter "L".
choosing the letter l for long or r for reverse. 
By default, the ls command prints the results in alphabetical order, so adding the -r option will print the results in reverse alphabetical order.

<img width="464" alt="image" src="https://user-images.githubusercontent.com/85710889/212566493-4600f33e-ac73-45ba-ac18-eaa1da0e6ac0.png">

Multiple options can be used at once, either given as separate options as in -l -r or combined like -lr. The output of all of these examples would be the same:
ls -l -r
ls -rl
ls -lr

As explained above, -l gives a long listing format while -r reverses the listing. The result of using both options is a long listing given in reverse order:

<img width="437" alt="image" src="https://user-images.githubusercontent.com/85710889/212566572-b0eb3ac3-43f9-45ad-8c32-7666bb0a76be.png">

<img width="427" alt="image" src="https://user-images.githubusercontent.com/85710889/212566581-bd128eee-ce71-41d6-92e7-dd2e54f7aef6.png">

Ultimately, commands can use many combinations of options and arguments. The possibilities for each command will be unique. Remember the aptitude easter egg?

<img width="315" alt="image" src="https://user-images.githubusercontent.com/85710889/212566608-f92e9ab2-160f-4415-b60d-c8fc606588d8.png">

It is possible to alter the behavior of this command using options. See what happens when the -v (verbose) option is added:

<img width="424" alt="image" src="https://user-images.githubusercontent.com/85710889/212566642-95331199-c3f2-4ad8-af5b-ab2a7318e7e6.png">

By combining multiple -v options, we can get a variety of responses:

<img width="446" alt="image" src="https://user-images.githubusercontent.com/85710889/212566682-adc3b2e2-6941-4f1e-9d5f-2d6d8f9752cb.png">

Remember multiple options can be denoted separately or combined:
aptitude -v -v moo
aptitude -vv moo
Keep adding -v options to see how many unique responses you can get!


# Printing Working Directory

In order to discover where you are currently located within the filesystem, the pwd command can be used. 

The pwd command prints the working directory, your current location within the filesystem:
Command syntax: pwd [OPTIONS]

<img width="415" alt="image" src="https://user-images.githubusercontent.com/85710889/212566741-093efae2-d8bf-4c3d-9eaa-572c38b1b34e.png">

The output of the above command indicates that the user is currently in their home folder, shown in the filesystem below.

![image](https://user-images.githubusercontent.com/85710889/212566770-227afdc5-0e5e-4f2b-b750-24125a2bf120.png)

Note: ~ is equivalent to /home/sysadmin, representing the user's home directory.

<img width="322" alt="image" src="https://user-images.githubusercontent.com/85710889/212566826-9f19daba-6f15-479b-aa22-e6b985935d65.png">

After changing directories (we will learn how to do this in the next section), the new location can also be confirmed in the new prompt, again shown in blue.

<img width="295" alt="image" src="https://user-images.githubusercontent.com/85710889/212566845-62620f6e-0d62-4e6f-b007-ab3515a81e95.png">








