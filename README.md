Introduction to the Command Line
=====================

> “Then the interface-makers went to work on their GUIs, and introduced a new semiotic layer between people and machines. People who use such systems have abdicated the responsibility, and surrendered the power, of sending bits directly to the chip that’s doing the arithmetic, and handed that responsibility and power over to the OS.”
>	—Neal Stephenson, In the Beginning was the Command Line

## What is the command line?

The Command Line Interface (CLI) is a text-only interface to your computer. You can use it to access folders, files, settings&mdash;pretty much anything you would want to do on a computer. 

## Why is it awesome?

* **Control!** You can type commands out and control _exactly_ what your computer is doing, unlike on a Graphical User Interface (GUI), where your options are limited by the icons/menus some programmer has chosen to offer (and where what they do might not be what you intend).
* **Scripting!** You can use the command line to automate lots of things, like backing up files, editing text... the possibilities are endless!
* **Programming!** Most programming languages can be run from a CLI. When we do Python (yes, we'll _eventually_ do Python), that's how we'll do it. So getting comfortable on the command line will make learning programming easier.
* And really? It just feels pretty cool to use it. :)

## Set up your environment

We'll be using [Nitrous.IO](https://www.nitrous.io). This is a really powerful tool, and we're only using a small part of it for this workshop. Definitely feel free to play with some of its functionality on your own! 

You can set up your account before the workshop, if you want! [Here are directions](https://github.com/anchorageprogramming/intro-to-command-line/blob/master/APW-NitrousIO.pdf?raw=true).

When you have the Nitrous console taking up the full screen, continue to the commands below

## Navigate

* pwd

  Type **pwd** into the terminal.

  You should see output that looks something like
  */home/action*

  This tells you where you are in the file structure. Linux, like Windows, organizes files into folders (also called *directories*) and subfolders (*subdirectories*). So if **pwd** returns */home/action*, you're in a directory called *action*, which is in a directory called *home*

* cd
  
  Let's say you don't want to be in the */action* directory anymore. You want to go up a level and be in */home*. 

  Type **cd ..**
  Now type **pwd**

  The output should be 
  */home*

  You've changed directories ("cd" - get it?), up a level (that's what ".." means). But what if you didn't really want to do that? What if you think, "No, I want to be in */home/action* now"? No problem!

  Type **cd action**
  Type **pwd**

  Now, as you can see, you're back where you started, in */home/action*.

## Make stuff
* mkdir
* nano
* cp
* rm
* mv
	
## Look at stuff
* ls
* more / less
* file ?

## Find stuff
* grep
* man
* find

## Just a couple more things....
* python
* ctrl-c