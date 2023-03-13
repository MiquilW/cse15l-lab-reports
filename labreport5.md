# Lab Report 5 (CLDQ)

When I had initially done the CSE Labs Done Quick challenge, I was writing commands line-by-line using simple techniques like using `tab` or copying and pasting.

When I lost in a mere 10 seconds to who would end up winning the competition, I was intrigued by how exactly he did it so fast. 

And that was when I learned about the most powerful tool for this challenge: **the semi-colon**.

Using semi-colons allows you to write multiple commands one after another that will be sequentially executed.

With this in mind, you can do the entire challenge with a **single** line of code 

And the best part is that it is completely legal under the competition's rules.

Here is a recreation of the command that the winner of my lab used: 

```
ssh -t cs15lwi23asv@ieng6.ucsd.edu 'git clone git@github.com:MiquilW/lab7.git ; cd lab7 ; javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java ; java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests ; nano ListExamples.java ; javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java ; java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests ; git add ListExamples.java ; git commit -m "g" ; git push'
```

Here is how it looks in the terminal (extremely messy):

![image](https://user-images.githubusercontent.com/100905820/224841514-8bfbe161-98cc-48c1-8ff0-143f9de238fa.png)

The `-t` is placed in the `ssh` command which opens up a terminal on the remote host and executes the commands inside the quotations. After finishing the commands, it autoamtically exits out of the remote host.

You may notice, though, that we have to change the `ListExamples.java` file to fix a bug. This is something that can't be automated on the command line (as far as I know).

In my case, I use nano, so I have to manually go through the file and fix the bug. If you memorize a few key presses to get there though, it can be fast.

![image](https://user-images.githubusercontent.com/100905820/224841433-718a7409-a0bb-42c2-a0be-98cb0ed0a47d.png)

My key presses were: `<ctrl+w>while(index2<space><less-than(<)><enter><down><down><right><right><right><right><right><right><right><right><backspace>1<ctrl+o><enter><ctrl+x>`

It's a bit inefficient. A better way (and the way the winner used) was Vim. I believe Vim can get the job done in three to four key presses, but I'll save learning Vim for another day.

![image](https://user-images.githubusercontent.com/100905820/224842919-0fa973e2-0f52-4f11-a098-b744f6c1042a.png)

As you can see in this very long image, I successfully completed the tasks with a single command.

Thank you to the winner of the 12:00 pm Thursday section winner of CLDQ. He is the one who wrote the command that this one is based on.
