# GuidedHacking Injector
Fully Featured DLL Injector made by [Broihon](https://guidedhacking.com/members/broihon.49430/) for Guided Hacking
Release Downloads: [Register & Download DLL Injector Here ](https://guidedhacking.com/resources/guided-hacking-dll-injector.4/)

![](https://i.gyazo.com/23b497942ade7bc6a13b2d7029567c6b.png)

**This repo doesn't contain the compiled binaries, just the source code for the library. If you want the compiled program, you must be a paying customer on our website where you can download it. You do not have permission/license to distribute the compiled binaries or any of our other content from our website.**

**Injection Methods:**
* LoadLibrary
* LdrLoadDll Stub
* Manual Mapping

**Launch Methods:**
* NtCreateThreadEx
* Thread Hijacking
* SetWindowsHookEx
* QueueUserAPC

**Requirements**

Windows 10 1809 or above

**Description**

* Compatible with both 32-bit and 64-bit programs
* Settings of the GUI are saved to a local ini file
* Processes can be selected by name or process ID and by the fancy process picker.

# GH Injector Library

Since GH Injector V3.0 the actual injector has been converted in to a library

To use it in your applications you can either use InjectA (ansi) or 
InjectW (unicode) which are the two functions exported by the "GH 
Injector - x86.dll" and "GH Injector - x64.dll".

These functions take a pointer to a INJECTIONDATAA/INJECTIONDATAW structure. For more the 
struct definition / enums / flags check "Injection.h".

How To Use GH Injector & Source Code Review: https://youtu.be/zhA9kSCY3Ec

# FAQ
* It's not a virus, it is packed with UPX and uses Autoit, according to most antivirus software that means it's a virus.
* It connects to the internet to check for updates


# How to Build from Source

Compile "GH Injector Library\GH Injector Library.sln" with these steps:
1. Open the project
2. Click "Build" in the menubar
3. Click "Batch Build"
4. Tick all 4 release builds (Configuration = Release)
5. Click "Build"
6. Done

Install AutoIt - It is Required to compile GUI - https://www.autoitscript.com/site/autoit/downloads/


Run CompileAndMerge.bat

It will compile the AutoIt files and merge all the required files into "GH Injector\".

To run the GH Injector simply open "GH Injector\GH Injector.exe".

# Credits

For the Manual Mapping a lot of credits go to [Joachim Bauch](https://www.joachim-bauch.de/tutorials/loading-a-dll-from-memory/).  I highly recommend you to go there and take a look if you're interested in Manual Mapping and the PE format itself.

The windows structures I use for the unlinking process are mostly inspired by [this site](https://sandsprite.com/CodeStuff/Understanding_the_Peb_Loader_Data_List.html) which is also a very interesting read.

I also want to credit Anton Bruckner and Dmitri Shostakovich because most of the time coding this I listened to their fantastic music which is probably one of the reasons why this took me way too long.

<h3>Official GH Courses</h3>
<ul>
	<li><a href="https://guidedhacking.com/ghb" target="_blank">The Game Hacking Bible</a>&nbsp;- a massive 70 chapter Game Hacking Course</li>
	<li><a href="https://guidedhacking.com/threads/squally-cs420-game-hacking-course.14191/" target="_blank">Computer Science 420</a>&nbsp;- an eight chapter lecture on CS, Data Types &amp; Assembly</li>
	<li><a href="https://guidedhacking.com/forums/binary-exploit-development-course.551/" target="_blank">Binary Exploit Development</a>&nbsp;- a 9 chapter series on exploit dev&nbsp;from a certified OSED</li>
	<li><a href="https://guidedhacking.com/forums/game-hacking-shenanigans/" target="_blank">Game Hacking Shenanigans</a>&nbsp;- a twenty lesson Cheat Engine hacking course</li>
	<li><a href="https://guidedhacking.com/threads/python-game-hacking-tutorial-1-1-introduction.18695/" target="_blank">Python Game Hacking Course</a>&nbsp;- 7 chapter external &amp; internal python hack lesson</li>
	<li><a href="https://guidedhacking.com/threads/python-game-hacking-tutorial-2-1-introduction.19199/" target="_blank">Python App Reverse Engineering</a>&nbsp;- Learn to reverse python apps in 5 lessons</li>
	<li><a href="https://guidedhacking.com/threads/web-browser-game-hacking-intro-part-1.17726/" target="_blank">Web Browser Game Hacking</a>&nbsp;- Hack javascript games with this 4 chapter course</li>
	<li><a href="https://guidedhacking.com/forums/roblox-exploit-scripting-course-res100.521/" target="_blank">Roblox Exploiting Course</a>&nbsp;- 7 Premium Lessons on Hacking Roblox</li>
	<li><a href="https://guidedhacking.com/forums/java-reverse-engineering-course-jre100.538/" target="_blank">Java Reverse Engineering Course</a>&nbsp;- 5 chapter beginner guide</li>
	<li><a href="https://guidedhacking.com/forums/java-game-hacking-course-jgh100.553/" target="_blank">Java Game Hacking Course</a>&nbsp;- 6 Chapter Beginner Guide</li>
</ul>
