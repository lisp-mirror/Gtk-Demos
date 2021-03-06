See "Introduction" below.

The most recent version of Gtk-Demos is an update of the January 17 version.  The following changes have been made since January 17:

1. It's no longer necessary to install sbcl to run the scripts.  They're invoked by a new script named demos.  A file named sanssbcl has to be with the scripts.  See "Info about sanssbcl" below.

2. The demo scripts have minor changes whose purpose is for them to be invoked differently than before.  To invoke them now, run the demos script, with the command: ./demos

3. Some of the object names in the demos have been changed to make them unique, because all the demos now get loaded into one name space.

4. The menu was demo4, but is now named menu.  All the demos have been combined into one Gtk application, which is established by the gapp in menu.

5. Six de minimis demos have been added, so you can easily make your own demos by editing de minimis demos.  The de minimis demos are demo4 through demo9.  You should also edit the menu to give your demos appropriate names.  The button name doesn't matter, and only has to be unique.  The label text is what will show as the button label.  Also change the window title in your demo, to no longer indicate it's a de minimis demo.

6. The syntax of the Gtk function prototypes has been changed again, to make them shorter and neater.  If you need more Gtk functions than are presently in the list, simply add them to the list, using the same syntax.


The demos are here:   https://github.com/mifpasoti/Gtk-Demos


Info about sanssbcl

With the sanssbcl file, the demo scripts can be run with or without sbcl being installed.  If sbcl is installed, you can make sanssbcl by running the makesans script.  The makesans script is short and easy to understand.  And sanssbcl is easy to understand, by understanding makesans.  To make sanssbcl, replacing any existing sanssbcl, use the command:  ./makesans


The January 17 version of the demos had the following changes from the original version:

1. Added a menu of the other demos.  It was demo4 in the January 17 version, but is now named menu.

2. The syntax for the list of Gtk function prototypes in demostuff was changed, but has been changed again.

3. Loading the Gtk shared object file by name only, without specifying the path, but using SBCL's built-in path logic, to be compatible with more Linux distros.


Introduction

To run the demos, use the command:  ./demos

To make changes to the demos, use any text editor, then run the demos again.

These demos demonstrate using Gtk directly from a higher level language.  None of the demos have any low level code in them.  There is no need for any makefiles, C compilers, or any other low level stuff.  There is probably no need to install Gtk, because it's probably already used by your Linux.

You don't need to install sbcl if you have the sanssbcl file.  But, if you want to install sbcl, you can usually install it via the Linux distro.  In the rare circumstance that a particular Linux distro doesn't have sbcl, you could install, via sbcl.org, either a binary version, or the sources to compile.

To use a different high level language for these demos, it is of course necessary to edit them to change the language.  But they aren't very long and that might not take very long.  It's strongly advised to run the present demos first, and make some minor changes to them, to see the differences, to make sure to understand how they work, before starting to change them to a different language.
