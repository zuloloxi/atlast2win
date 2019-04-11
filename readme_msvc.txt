<<<<<<< HEAD
#added debug option
# compiler code C with msvc VS2010
# cl -c  atlmain.c
# cl -c  atlast.c
# generate .exe binary 
# cl -o atlast  atlmain.obj atlast.obj

#: fact dup 0= if drop 1 else dup 1- fact * then ;

CFLAGS = -c /W3 /nologo $(CVARS) -I. -Iproto -DHAVE_PATHDEF -DWIN32 \
		$(CSCOPE_DEFS) $(TERM_DEFS) $(NETBEANS_DEFS) $(CHANNEL_DEFS) \
		$(NBDEBUG_DEFS) $(XPM_DEFS) \
		$(DEFINES) -DWINVER=$(WINVER) -D_WIN32_WINNT=$(WINVER) \
		/FAcs 


cl -c /FAcs atlmain.c 
cl -c /FAcs atlast.c
cl -o atlast atlmain.obj atlast.obj /link /subsystem:console  /DYNAMICBASE:NO /FIXED /NXCOMPAT /MACHINE:X86 /DEBUG /MAP /MAPINFO:EXPORTS
=======
rem compiler code C with msvc VS2010
cl -c  atlmain.c
cl -c  atlast.c
rem gen .exe binary 
cl -o atlast  atlmain.obj atlast.obj

2019/04/01
access violation bug in lookup detected
>>>>>>> 9dddeb13438ae0340acffbabe7082865733ab64d
