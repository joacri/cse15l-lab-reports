# Lab Report 5
> For this last lab report I chose to explore several options for a different command because I learned a lot of interesting things by researching commands for lab report 3.

## The command I chose to research this time is `find`
> The current working directory in which I will run the grep commands that I found is:
>
>   `/home/linux/ieng6/cs15lwi23/cs15wi23acn/docsearch/written_2/non-fiction/OUP/`
---
## 1.) `find . -size (+/-)(num)(unit) `
> Ex. 1 - Input:
```
find . -size +80k
```
> Output: 
![Image](L5-P1.1.png)
> Explanation: This command recursively searches the directory tree, for each specified Path, for files bigger than 80 kilobytes.The '+' means that it is looking for files that are greater in size than the given measure. No '+' means that it searches for fils exactly that size. An example of how this command can be useful is when you want to see what files have a greater size, so you can check if they are still usefull or they are just wasting space.
> 
> Source: [https://linuxhandbook.com/find-command-examples/](https://linuxhandbook.com/find-command-examples/)

> Ex. 2 - Input:
```
find . -size -2k
```
> Output: 
![Image](L5-P1.2.png)
> Explanation: This command recursively searches the directory tree, for each specified Path, for files smaller than 2 kilobytes. The '-' means that it is looking for files that are smaller in size than the given measure. The unit in this example and the last was 'k', which stands for kilobytes, but you can also use 'c' for bytes, 'M' for Megabytes, and 'G' for Gigabytes. An example of how this command can be useful is when you want to see what files might hold too little information that maybe they are useless and could just be deleted.
> 
> Source: [https://linuxhandbook.com/find-command-examples/](https://linuxhandbook.com/find-command-examples/)
---
## 2.) ` find -type f -mmin (+/-) (num of minutes)`
> Ex. 3 - Input:
```
find -type f -mmin -15
```
> Output: 
![Image](L5-P2.1.png)
> Explanation: This command recursively searches the directory tree, for each specified Path, for files that were modified in the last 15 minutes. In this example I created a new file in this repository and it was the only one to show up becuase the rest of the files have not been as recently modified. An example of how this command can be useful is when you forgot what files you just edited or are working with others and you want to check on the latest changes.
> 
> Source: [https://linuxhandbook.com/find-command-examples/](https://linuxhandbook.com/find-command-examples/)

> Ex. 4  - Input:
```
find -type f -cmin +24
```
> Output: 
![Image](L5-P2.2.png)
> Explanation: This command recursively searches the directory tree, for each specified Path, to find all files created more than 24 minutes ago. In this example all files that correspond with the current directory were returned except for the one I had recently created for the purpose of these tests. An example of how this command can be useful is when you want to check which files are the oldest in your directory because they may no longer be useful. For this you can also use `-ctime` instead of `-cmin` if you want to calculate based on days and not minutes.
> 
> Source: [https://linuxhandbook.com/find-command-examples/](https://linuxhandbook.com/find-command-examples/)

---
## 3.) `find . -maxdepth (num of depth)`
> Ex. 5 - Input:
```
find . -maxdepth 2 -type f -name "*ch1.txt"
```
> Output: 
![Image](L5-P3.1.png)
> Explanation: This command is used to search only in the current directory and its next subdirectory, because nuber used is 2. In this example we are searching for files within that range that end with "ch1.txt".This can be useful for when you are trying to find a specific chapter in the current directory, but you know that other directories might also have that same chapter number. 
> 
> Source: [https://linuxhandbook.com/find-command-examples/](https://linuxhandbook.com/find-command-examples/)

> Ex. 6 - Input:
```
find . -maxdepth 1 -type f -empty
```
> Output: 
![Image](L5-P3.2.png)
> Explanation: This command is used to search only in the current directory, because nuber used is 1. In this example we are searching for files in the current directory that are empty. This can be useful for when you are trying to find files that can be useless because they don't have anything in them.
> 
> Source: [https://linuxhandbook.com/find-command-examples/](https://linuxhandbook.com/find-command-examples/)

---
## 4.) `find . -type f -name "*.txt" -exec grep "string" {} +`
> Ex. 7 - Input:
```
find . -type f -name "*.txt" -exec grep -i abuelo {} +
```
> Output: 
![Image](L5-P4.1.png)

> Explanation: This command recursively searches the directory tree, for each specified Path, and is combined with the grep command to find all .txt files that contain the word abuelo. This can be helpful if you are looking for a specific topic across the directory and subdirectories because it gives you better chances of finding more information.
> 
> Source: [https://linuxhandbook.com/find-command-examples/](https://linuxhandbook.com/find-command-examples/)


> Ex. 8 - Input:
```
find . -type f -name "*.txt" -exec grep "jazz culture" {} +
```
> Output: 
![Image](L5-P4.2.png)
> Explanation: This command recursively searches the directory tree, for each specified Path, and is combined with the grep command to find all .txt files that contain the string "jazz culture". This can be helpful if you are looking for a specific topic across the directory and subdirectories because it gives you better chances of finding more information based on that specific string.
> 
> Source: [https://linuxhandbook.com/find-command-examples/](https://linuxhandbook.com/find-command-examples/)
