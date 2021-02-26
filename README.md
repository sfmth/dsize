# dsize
### dsize - Directory size monitoring command
This simmple bash command outputs a list of all directoris and files present in the curent directory sorted by their size. It also generates a "size" file in that directory with the output of the command written inside of the file. The generated file is useful in large directories where running the command takes some time.


There is known issues for mac users as they might not have the -h option for the sort or the ls command

To install you just run this command:

`echo "alias dsize='du -h -d 1 > size && ls -s -h | sed 1d >> size && cat size | sort -r -h -o size size && cat size'" >> ~/.bashrc`

To use it you can just type "dsize" into your command line. :)
