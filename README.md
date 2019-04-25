# OS_Project4 - File System Implementation
Contributors: Octavio Avila-Cardet  5699410
              Kent Miguel           4804988

This project aims to show students how a file system works. It focuses on the directory hierarchy and storage management in particular. In addition, to have a better understanding of some of the performance issues file systems encounter.

In this project, we worked on a user-level library, libFS, which implements a file system. Our file system will be built inside of a library that applications can link with to access files and directories. The library links with a layer that implements a "disk"; the library is provided, LibDisk. The only modified file in this project is LibFS.c.

RUN THE TEST

The commands on this project do the following:
a. Create a file
b. Remove a file
c. Create a directory
d. Remove a directoy
e. List all the items in the disk, or given path

TO COMPILE:

make

TO CLEAN: make reset

- creates the necessary executables for all the required tests

TO RUN THE TESTS:

Perform simple test: ./simple-test.exe example

List the file system: ./slow-ls.exe example / 

Touch a file to the file system: ./slow-touch.exe example

Check if the new created file is showing: ./slow-ls.exe example / 

Remove file: ./slow-rm.exe test /examplefile

Check the remove result: ./slow-ls.exe example /

Create directory: ./slow-mkdir.exe example /exampledir
                  ./slow-ls.exe example / 

Remove directory: ./slow-rmdir.exe example exampledir
                  ./slow-ls.exe test / 


