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

  What if you aren't satisfied with the directories that are available to you? (Long-term, this is inevitable, right? You probably won't want to store all of your files in one place.) No problem!

  Type **mkdir [your name]** &mdash; but don't literally type that; replace "[your name]" with your actual first name :) 

  Now change directory into the directory with your name. Scroll up for a reminder about changing directories, if you need it. Remember to use **pwd** to make sure you're in the right place.
	
* nano

  It's time to make a text file! There are lots of text editors available&mdash;and lots of strong opinions about which is the best one&mdash;but for today, we're going to use a simple one. It'll work great for anything you want to do, from writing to-do lists to writing code. 

  Type **nano myfile**
  And then *don't panic* when the screen changes entirely! 

  You're inside an application, inside the command line. (How cool is that?) As you can see, there are commands along the bottom. Where you see a caret (^), it means you hold down the ctrl key along with that letter to execute that command. But first let's enter some text, before we worry about any of the commands.

  Type **whatever you like**. I typed "Hi, my name is Coral. I like birds and chinchillas and coffee." Pretty much anything will do. 

  Once you've entered some text, hold down the *ctrl key* and hit *X* (shortened from now on to *ctrl-x*)

  A prompt appears at the bottom of the screen: *Save modified buffer (ANSWERING "No" WILL DESTROY CHANGES)?*

  Type *y* 

  The prompt now asks if this is the filename you want to write. It is, so

  Hit *enter*

  Congratulations! You just made a text file!

## Look at stuff

* ls

  How do you *know* you made a file, though? Not a problem. Let's have a look! 

  Type **ls**

  The output should be 
  *myfile*

  For fun, let's change directory up one level and look at what's inside that directory:

  **cd ..**
  **ls**

  The output should be 
  *[your name] README.md workspace* &mdash; the order might vary, based on where your name falls in the alphabet; that's fine

  Now, change directory back into [your name], and make sure you're in the right place with **pwd**

* more / less

  Let's say you want to know what's in *myfile* without opening it up in *nano*. That's totally doable.

  Type **more myfile**

  And, just to compare,

  Type **less myfile** &mdash; you can escape the screen that comes up by typing **q**

  It turns out, *less* is a bit more complex. For big files, *more* will let you go through it all in order, where *less* will let you scroll through it, both forward and backward. 

* file ?

## Move stuff

* cp

  Oh, but we forgot to add an extension, showing that it's a text file, didn't we? Not a problem. We can copy this file and give it a new name in the process.

* rm
* mv

## Find stuff
* grep
* man
* find

## Just a couple more things....
* python
* ctrl-c