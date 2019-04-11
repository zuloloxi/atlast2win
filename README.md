
# ATLast 2.0 - https://www.fourmilab.ch/atlast/

Atlast is based upon the FORTH-83 language, but has been extended in many ways and modified to better serve its mission as an embedded toolkit for open, programmable applications. Atlast is implemented in a single file, written in portable C; it has been ported to many different machines and operating systems, including MS-DOS, OS/2, the Macintosh, and a wide variety of Unix machines. Atlast includes native support for floating point, C-like strings, Unix-compatible file access, and a wide variety of facilities for embedding within applications. Integers are 32 bits (64 bits in the 64-bit version of Atlast) and identifiers can be up to 127 characters; extensive stack and heap pointer checking is available to aid in debugging. Atlast may be configured at compilation time to include only the facilities needed by a given application, thus saving memory and increasing execution speed (when error checking is disabled).

Atlast was developed at Autodesk, Inc. Autodesk returned the rights to John Walker in 1991, and, subsequently placed the program in the public domain. Autodesk's connection with this program is purely historical: it is neither endorsed, used, nor supported by Autodesk, Inc.

Atlast was developed at Autodesk, Inc. Autodesk, returned the rights in 1991, to John Walker and subsequently placed the program in the public domain.

In this version there is a bug - access violation at address XXXX:XXXX - when compiling with: Microsoft (R) 32-bit C/C++ Optimizing Compiler Version 16.00.40219.01 for 80x86

   cl /FAcs /DMEMSTAT /DEXPORT /DOS2 /F 8000 atlast.c atlmain.c /link /subsystem:console  /DYNAMICBASE:NO /FIXED /NXCOMPAT /MACHINE:X86 /DEBUG /MAP /MAPINFO:EXPORTS


