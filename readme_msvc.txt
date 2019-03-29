rem compiler code C with msvc VS2010
cl -c  atlmain.c
cl -c  atlast.c
rem gen .exe binary 
cl -o atlast  atlmain.obj atlast.obj