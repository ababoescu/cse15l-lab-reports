# Researching the Command: find
Source: Man find (using the built manual in the VS Code Terminal)

## Find -empty
-empty: returns whether or not the file is empty (if return nothing = no empty files in directory)

### Example 1:
```
#finding if there are any empty files in the subdirectory written_2/travel_guides
$ find written_2/travel_guides -empty
(nothing is returned)
```

The example above shows the searching for empty files in the subdirectory travel_guides, in the case of this example there are no empty files. This command is helpful to find if there are any empty files in your directory/subdirectory without having to search each file independently.

### Example 2:
```
#finding if there are any empty files in the directory written_2/
$ find written_2/ -empty
(nothing is returned)
```

Much like the example before, however this example is searching for an empty file in the written_2 directory.

## Find -ls
-ls: list current file in ls


## Find -name
-name: find the path based off of the file name

### Example 1:
```
#finding files that start with "Cuba"
$ find written_2/ -name "Cuba*"
written_2/travel_guides/berlitz2/Cuba-History.txt
written_2/travel_guides/berlitz2/Cuba-WhatToDo.txt
written_2/travel_guides/berlitz2/Cuba-WhereToGo.txt
```

The above example is searching for files with the name Cuba in them and the path to that file containing the string "Cuba" in the written_2/ directory. This command is helpful for searching the subdirectories to find a specific file with the name matching the imputed string and include their path so that the user can easily find which directories and subdirectories the file is located.

### Example 2:
```
#finding files that contain the text file name "ch1.txt"
$ find written_2/ -name "ch1.txt"
written_2/non-fiction/OUP/Abernathy/ch1.txt
written_2/non-fiction/OUP/Berk/ch1.txt
written_2/non-fiction/OUP/Fletcher/ch1.txt
written_2/non-fiction/OUP/Kauffman/ch1.txt
written_2/non-fiction/OUP/Rybczynski/ch1.txt
```

Much like the example before, however this example is searching for the file with the name "ch1.txt" in the written_2 directory.

## Find -type d -name
-name: find the path based off of the file name
-type d: searches for directories only

### Example 1:
```
#finding directories that contain the name berlitz
$ find -type d -name "berlitz*"
./written_2/travel_guides/berlitz1
./written_2/travel_guides/berlitz2
```

The above example is much like the previous examples searching for the name of files in a directory, however, this specific command allows you to specifically search for directories in the written_2/ directory that contain the string **berlitz**. This command is helpful for a user to simplify their search if they wish to search up specific directories rather than every possible file, directory, subdirectory, etc. that contain the string **berlitz**.

### Example 2:
```
#finding the directory OUP
$ find -type d -name "OUP"
./written_2/non-fiction/OUP
```

Much like the example before, however this example is searching for the directory with the name "OUP" in the written_2 directory.
