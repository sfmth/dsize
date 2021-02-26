# dsize
### dsize - Directory size monitoring command
This simmple bash command outputs a list of all directoris present in the curent directory sorted by their size. It also generates a "size" file in that directory with the output of the command written inside of the file.
The generated file is useful in large directories where running the command takes some time.
There is known issues for mac users as they don't have the -h option for the sort command.

To install you just run this command:

`echo "alias dsize='du -h -d 1 | sort -r -h > size && cat size'" >> ~/.bashrc`

To use it you can just type "dsize" into your command line. :)
