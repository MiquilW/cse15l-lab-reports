# Lab Report 3

For this lab report, I chose the `find` command to research and experiment on. Here are four different ways I found to use it:

## 1. `find -iname`
### Example 1:

Input:
```
find -iname pArIs*
```
Output:
```
./travel_guides/berlitz2/Paris-WhatToDo.txt
./travel_guides/berlitz2/Paris-WhereToGo.txt
```
This command is searching case insensitively for paris. This is useful because you may forget how exactly a file is written case-wise.

### Example 2:

Input:
```
find -iname Berlitz*
```
Output:
```
./travel_guides/berlitz1
./travel_guides/berlitz2
```
This command is searching case insensitively for berlitz (the one we want is uncapitilized, but we entered is capitilized). 
This is useful because we may forget whether we capitilized the name of a file or directory.

**Source: https://adamtheautomator.com/bash-find/**

## 2. `find -type f/d`
### Example 1:

Input:
```
find */*/Berk/* -type f
```
Output:
```
non-fiction/OUP/Berk/ch1.txt
non-fiction/OUP/Berk/ch2.txt
non-fiction/OUP/Berk/CH4.txt
non-fiction/OUP/Berk/ch7.txt
```
This command is searching in a specific directory for anything that is a file. This could be useful if you need to find files specifically in a 
directory cluttered environment.

### Example 2:

Input:
```
find * -type d
```
Output:
```
non-fiction
non-fiction/OUP
non-fiction/OUP/Abernathy
non-fiction/OUP/Berk
non-fiction/OUP/Castro
non-fiction/OUP/Fletcher
non-fiction/OUP/Kauffman
non-fiction/OUP/Rybczynski
travel_guides
travel_guides/berlitz1
travel_guides/berlitz2
```
This command is searching in every directory within `written_2` for anything that is a directory. This could be useful if you need to know what directories 
exist in a cluttered space.

**Source: https://adamtheautomator.com/bash-find/**

## 3. `find -not -name`
### Example 1:

Input:
```
find -not -name *.txt
```
Output:
```
.
./non-fiction
./non-fiction/OUP
./non-fiction/OUP/Abernathy
./non-fiction/OUP/Berk
./non-fiction/OUP/Castro
./non-fiction/OUP/Fletcher
./non-fiction/OUP/Kauffman
./non-fiction/OUP/Rybczynski
./travel_guides
./travel_guides/berlitz1
./travel_guides/berlitz2
```
The `-not` command allows you to search in files and directories for everything except what you write after the `-not` operator. It will filter out everything you don't want to see, and show everything else in the file/directory. This command is searching for anything that is **not** a `.txt` file. This could be useful if you need to avoid `.txt` files if they are cluttering a space where you need to find something else.

### Example 2:

Input:
```
find -not -name c*
```
Output:
```
.
./non-fiction
./non-fiction/OUP
./non-fiction/OUP/Abernathy
./non-fiction/OUP/Berk
./non-fiction/OUP/Berk/CH4.txt
./non-fiction/OUP/Castro
./non-fiction/OUP/Fletcher
./non-fiction/OUP/Kauffman
./non-fiction/OUP/Rybczynski
./travel_guides
./travel_guides/berlitz1
./travel_guides/berlitz1/HandRHawaii.txt
./travel_guides/berlitz1/HandRHongKong.txt
...
```
This command is searching in for anything that does **not** start with a lower-case c. This could be useful if you need to filter out a mass amount of files that
all start with the same letter.

**Source: https://adamtheautomator.com/bash-find/**

## 4. `find -prune`
### Example 1:

Input:
```
find */* -prune
```
Output:
```
non-fiction/OUP
travel_guides/berlitz1
travel_guides/berlitz2
```
This command is searching for anything in a specific directory and ONLY that directory (or directories if you use a pattern). This could be useful if you need 
to restrict your search to a specific directory because otherwise there would be too much clutter.

### Example 2:

Input:
```
find non-fiction/OUP/* -prune
```
Output:
```
non-fiction/OUP/Abernathy
non-fiction/OUP/Berk
non-fiction/OUP/Castro
non-fiction/OUP/Fletcher
non-fiction/OUP/Kauffman
non-fiction/OUP/Rybczynski
```
This command is searching for anything in a specific directory and ONLY that directory. This could be useful if a lot of files are similarly named and you are
searching for just the parent directories to reduce the clutter.

**Source: https://adamtheautomator.com/bash-find/**
