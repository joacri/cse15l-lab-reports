# Lab Report 3
> Researching Commands

## The command I chose to research is `grep`
> The current working directory in which I will run the grep commands that I found is:
>
>   `/home/linux/ieng6/cs15lwi23/cs15wi23acn/skill-demo1-data/written_2/travel_guides/berlitz2/`
---
## 1.) `grep "[^(character)](string)" (filename)`
> Ex. 1 - Input:
```
grep "[^t]he " California-History.txt
```
> Output: 
```
![Image](L3-P1.png)
```
> Explanation: This command is looking for anywhere in the file that has the string "he ", but any characters before that string can't be "t". It can be a "T", which shows an example of how this command can be useful because if you are looking for when a sentence begins with the word "The" then your options to look through are significantly narrowed down.
> 
> Source: [https://www.digitalocean.com/community/tutorials/using-grep-regular-expressions-to-search-for-text-patterns-in-linux](https://www.digitalocean.com/community/tutorials/using-grep-regular-expressions-to-search-for-text-patterns-in-linux)

> Ex. 2 - Input:
```
grep "[^m]exico " Cancun-WhatToDo.txt
```
> Output: 
```
![Image](L3-P2.png)
```
> Explanation: This command is looking for anywhere in the file that has the string "exico", but any characters before that string can't be "m", so in this case it is showing us all the places where Mexico is writtena and properly capitalized. However, this command can be useful because if you are looking for when a proper noun like Mexico isn't properly capitalized in your text then you can simply edit the letter in the bracket of your command to be the capital starting letter.
> 
> Source: [[www.digitalocean.com](https://www.digitalocean.com/community/tutorials/using-grep-regular-expressions-to-search-for-text-patterns-in-linux)](https://www.digitalocean.com/community/tutorials/using-grep-regular-expressions-to-search-for-text-patterns-in-linux)
---
## 2.) `grep "..(string)" (filename)`
> Ex. 3 - Input:
```
```
> Output: 
```
```
> Explanation: What its doing, Why its useful
> 
> Source: [[www.digitalocean.com](https://www.digitalocean.com/community/tutorials/using-grep-regular-expressions-to-search-for-text-patterns-in-linux)](https://www.digitalocean.com/community/tutorials/using-grep-regular-expressions-to-search-for-text-patterns-in-linux)

> Ex. 4  - Input:
```
```
> Output: 
```
```
> Explanation: What its doing, Why its useful
> 
> Source: [https://www.digitalocean.com/community/tutorials/using-grep-regular-expressions-to-search-for-text-patterns-in-linux](https://www.digitalocean.com/community/tutorials/using-grep-regular-expressions-to-search-for-text-patterns-in-linux)

---
## 3.) `grep -E "(string)?(string)" (filename)`
> Ex. 5 - Input:
```
```
> Output: 
```
```
> Explanation: What its doing, Why its useful
> 
> Source: [[www.digitalocean.com](https://www.digitalocean.com/community/tutorials/using-grep-regular-expressions-to-search-for-text-patterns-in-linux)](https://www.digitalocean.com/community/tutorials/using-grep-regular-expressions-to-search-for-text-patterns-in-linux)

> Ex. 6 - Input:
```
```
> Output: 
```
```
> Explanation: What its doing, Why its useful
> 
> Source: [[www.digitalocean.com](https://www.digitalocean.com/community/tutorials/using-grep-regular-expressions-to-search-for-text-patterns-in-linux)](https://www.digitalocean.com/community/tutorials/using-grep-regular-expressions-to-search-for-text-patterns-in-linux)

---
## 4.) `grep "^[A-Z]" (filename) `
> Ex. 7 - Input:
```
```
> Output: 
```
```
> Explanation: What its doing, Why its useful
> 
> Source: [[www.digitalocean.com](https://www.digitalocean.com/community/tutorials/using-grep-regular-expressions-to-search-for-text-patterns-in-linux)](https://www.digitalocean.com/community/tutorials/using-grep-regular-expressions-to-search-for-text-patterns-in-linux)


> Ex. 8 - Input:
```
```
> Output: 
```
```
> Explanation: What its doing, Why its useful
> 
> Source: [[www.digitalocean.com](https://www.digitalocean.com/community/tutorials/using-grep-regular-expressions-to-search-for-text-patterns-in-linux)](https://www.digitalocean.com/community/tutorials/using-grep-regular-expressions-to-search-for-text-patterns-in-linux)
