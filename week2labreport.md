# Week 1 Lab Report
---
# Part 1
Here is the code for `StringServer.java`:

![StringServer.java](StringServer.png)

Here is me using `/add-message` to display "joe politz" on the website:

![First Line](firstline.png)

For this output, we call the `handleRequest` method in the `StringServer.java` file. After it sees that the path contains `add-message?s=` then it adds the query (everything after the `=`) and a new line to the `displayString` (which was empty before this) and displays it on the page. Because of this, the `displayString` is concatenated with the query and a new line. 

**Note: the `%20` between "joe" and "politz" is there because URLs can't have spaces. The `%20` represents a space.**

Here is me using `/add-message` to display "is the greatest of all time" on the website:

![SecondLine](secondline.png)
