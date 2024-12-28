# Essential commands for daily terminal navigation

### cd
This is very important in navigating directories. 
Use `pwd` to know the current directory you're in.

### ls
View the contents of a directory. While `cd` moves you to a directory, `ls` only lists the contents of a directory.

### rm
Delete files. One can delete several files by enumerating the files after rm, e.g. `rm this_file also_this_file another_file`

To delete a folder, use `rm -r`.

### cp
Copy files. To copy a folder, use `cp -r`. The `-r` flag stands for recursive.

### mv
Move file or folder. This can also be used for renaming, e.g. `mv old_file_name new_file_name`.

### mkdir
Create directory.

### utilizing *
This is not a command but rather an important hack, something for pattern recognition. For instance, to delete all image files with png extension, one can simply use `rm *.png` instead of manually deleting each file.

### grep
Find text.
`grep -A#`: display # lines after
`grep -B#`: display # lines before

### chmod +x
Make a file executable. This also changes the color of the file which makes it easier to spot the executable file.

### for f in old*; do mv "$f" "$(echo "$f" | sed s/old/new/)"; done
Rename multiple files at once. I got this syntax from [here](https://stackoverflow.com/questions/6840332/rename-multiple-files-by-replacing-a-particular-pattern-in-the-filenames-using-a).

### vi
Text editor. Use `vi -b`  to open as binary file.
