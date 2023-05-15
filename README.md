# SDL2madeeasy
A respositry for new explorers to ease their work with SDL2.

# ---------------GUIDELINES TO FOLLOW BEFORE USING SDL2 (for new users, for sure)---------------------

1. SUGGESTED TO FOLLOW THIS POST (https://www.matsson.com/prog/sdl2-mingw-w64-tutorial.php).

2. Download SDL2-mingw.tar.gz from  offcial github(https://github.com/libsdl-org/SDL.git).

3. Download mingw from offcial source x86_64(for 64 bit windows) and x86(for 32 windos).

4. For 64 bit you can download mingw.

5. An error() often comes while downloading mingw_x64 from sourceforgenet to prevent it just follow below steps.

6. Follow the steps in this stackoverflow (https://stackoverflow.com/questions/46455927/mingw-w64-installer-the-file-has-been-downloaded-incorrectly).

7. repositr.txt link (https://sourceforge.net/projects/mingw-w64/files/Toolchains%20targetting%20Win32/Personal%20Builds/mingw-builds/installer/)

8. Get repositry.txt and find 8.1.0|x86_64|posix|seh|rev0 in it (for 64 bit windows only).

9. I suggest you to follow second post because it solved my issue.

10. Also if you have successfully followed STEP 1 , just run the sample program of creating a windows.

11. Don't forget to add #include<SDL2/SDL.h> in header file.

12. Add a Makefile in your project (for peace of mind) and put the configuration same as the post in STEP1.

13. In my case -
all:
	g++  main.cpp -IC:\Tutorial\SDL2\include -LC:\Tutorial\SDL2\lib -Wall -lmingw32 -lSDL2main -lSDL2 -o main

11. Compile it using terminal using this command -> mingw32-make -f Makefile . 

12. If everything works properly you should get a main.exe .

13. AND IF YOU ARE LAZY THEN JUST CLONE THIS REPO SIMPLE :) 
