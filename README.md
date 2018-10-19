# Unix 101.

We'll be covering these topics:
 - Why people use the shell 🤔
 - Basics of shell interaction 
   - `echo`, `Less`, basic editing like `nano` maybe?, `cd`, file system, running programs
 - Some fun commands
   - How to install new programs (Mac / Linux) :hammer_and_wrench:
 - Writing a simple script :writ
 - Background tasks (?)
 - `ssh`
 - Further learning! Ssh, git, scp, tmux
 

## Why people use the shell
The shell (also called terminal, or command line, I'll be using these interchangeably) is really powerful, a lot more powerful that programs with GUI's (Graphical User Interfaces).
Lots of programs only really work for the command line, and almost every software professional (💰) knows their way around it.

## Basics of shell interaction


### Opening the terminal
Linux :penguin:: On Ubuntu, Ctrl+Alt+T will open a Terminal. Otherwise, this might depend on your Linux distribution.

MacOS :apple:: Open up the application called Terminal. In the future, if you start to use the terminal more, you may want to install [iTerm2](https://www.iterm2.com/), as it's much more powerful and nicer.

### The terminal prompt
When you open the terminal, you will see something like this (The screenshot was taken on Ubuntu 17.04):

![Terminal Screenshot](https://raw.githubusercontent.com/zvory/Unix-101/master/TerminalScreenshot.png)

This is the terminal prompt. This is where you enter commands. You can see there's some text there already, the terminal will print this out when it's ready to accept commands from you, the default text it prints out is:

`username@machine-name:your-working-directory`

### Hello world (echo)

Let's try to print "Hello world!". The terminal command to display a line of text is `echo`. So lets put this command into the terminal:

`echo "Hello world!"`

And press enter. You should see the text "Hello world!" printed back at you.

Congrats, you've made a Hello world! program in the terminal.

### Creating a file (touch)
Let's make a file. In a GUI program with a nice user interface, we might right click in the program, and click 'New File', but we can't do that in the terminal.

Instead we will use a command called `touch`. This will create an empty file for us. Let's type `touch myFile.txt` into the terminal.

Once you've done that, you might notice you don't get any feedback, there's nothing that says "File created succesfully" or anything, you just see a new prompt to enter a new command. This is normal, in Unix there is a convention that if a program doesn't output anything, it executed succesfuly.

### Finding the file we just created (ls)
Remember the `your-working-directory` part of the terminal prompt we talked about earlier? That is where your terminal is currently open to. When we used `touch`, the file we created was created in the `your-working-directory`.

Lets list the files in our current directory. To do this, we use the command called `ls` (Sounds kinda like "list". Often times unix commands will be really short, like `rm` instead of "remove", this is so you have to type less).

