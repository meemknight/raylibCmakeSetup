# RaylibCmakeSetup 

---

## What is it?

I already set up a Raylib project for you! Take it and enjoy! You don't need to know CMake!

![image](https://github.com/meemknight/raylibCmakeSetup/assets/36445656/c50ab777-0cde-4d80-8df6-a0fd483f169d)


<p>Opening the Solution:</p> 

<img src="https://raw.githubusercontent.com/meemknight/photos/master/llge1.gif" width="350">

Or

<img src="https://raw.githubusercontent.com/meemknight/photos/master/llge2.gif" width="500">

Running the setup

Go to CMakeLists.txt, <kbd>CTRL + S</kbd> to make sure the solution was built.

Then, from this dropdown select mygame.exe

<img src="https://raw.githubusercontent.com/meemknight/photos/master/llge3.gif" width="200">

<kbd>Ctrl + F5</kbd> to build (<kbd>F5</kbd> oppens the debugger, you usually want to press <kbd>Ctrl + F5</kbd> because it oppens faster like this.

<p>Adding files:<br>
You should add .cpp in src/ and .h in include/ Whenever you add a new file CMake will ask you if you want to add that thing, say NO every time! I am already adding all of the things automatically!
If you accidentally say YES, just remove that file from the CMake.lists
</p>

<p>Refreshing your changes:<br>
After you add a file, the changes should be automatically added but if you want to be sure, you can refresh changes by saving the CMake file. If you want to make a hard refresh (you might have to do that sometimes) close Visual Studio, delete the out folder, reopen VS, <kbd>CTRL + S</kbd> on CMakeLists.txt</p>


# IMPORTANT!
  To ship the game: 
  In Cmakelists.txt, set the PRODUCTION_BUILD flag to ON to build a shippable version of your game. This will change the file paths to be relative to your exe (RESOURCES_PATH macro), will remove the console, and also will change the asserts to not allow people to debug them. To make sure the changes take effect I recommend deleting the out folder to make a new clean build!


  Also, if you read the CMAKE, even if you don't know CMAKE you should understand what happens with the comments there and you can add libraries and also remove the console from there if you need to! (there is a commented line for that!)
