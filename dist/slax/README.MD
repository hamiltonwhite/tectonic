# Academic Writing Platform (2/1/19)
Version: 0.0.1:02-01-2019

## Introduction
The purpose of this folder and these files are to release a distribution of tectonic that can be used portably using the Slax linux distribution.  Over the past week I've been developing these files since I desired a portable implementation of the Tectonic Project that could be easily dropped onto any flashdrive and allow me to do academic writing while traveling.  I based this work off of Slax because it is a simple and highly extensible framework to which all sorts of "portable" packages could be added on the fly to extend the use of operating system while running everything more or less out of ram (or in a virtual machine).  

## Included Packages:
The core package is 06-academicwriting.sb, and incorporates the following packages into it (based on apt and other package managers, including their dependencies):
* build-essential
* Miniconda3
* Tectonic
* Atom Editor (as an appimage)

I've also compiled the system into a full iso of Slax 9.7.0, which is the basis for the system usage description below.

## System Usage:
* Boot as normal
* Add Miniconda and Tectonic to PATH: export=~/miniconda/bin:$PATH
* ^ Leave this terminal window open
* Test to ensure the following packages load in the CLI:
 - conda
 - tectonic
* Change to the Documents/Apps directory and open in CLI
* Run: chmod a+x Atom-1.10.2-x86_64.AppImage
* Open the text editor and start working
* You can run and compile software using make
* Run savechanges [filename] when you're finished working to save state (to another .sb file that you should copy to a flashdrive) before shutdown

## Notes:
* I have not edited the writing template I've included yet, so bare with me.
* I will be making further changes to this distribution soon, and will include a set of working modules when that happens.
