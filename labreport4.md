# Lab Report 4

For this lab report, I'm going to show how I went about completing the competition as fast as possible. Before we begin, I had some tabs open to make it easier to paste things into the terminal. I already had the GitHub repo link on my clipboard.

![image](https://user-images.githubusercontent.com/100905820/221748588-9f700417-9226-490a-ad5c-3d4bbd8a6559.png)

_Keys pressed: `ssh<space>cs15lwi23asv@ieng6.ucsd.edu<enter>`_

I typed out the `ssh` command above to log onto ieng6. It may be faster for some if you copied and pasted it from somewhere, but I timed myself to be faster doing it this way. As with all the commands from here on out, I pressed `<enter>` to

![image](https://user-images.githubusercontent.com/100905820/221749396-8cfd22ff-2401-4498-819d-635180c846e1.png)

_Keys pressed: `git<space>clone<space><ctrl+v><enter>`, `cd<space>lab7<enter>`_

I typed out `git clone` then pasted the forked GitHub repo link in (as mentioned earlier, it was already on my clipboard). I did not want to bother writing the link out obviously, so I just had it ready to be copied. I then quickly typed `cd lab7` because it's short.

![image](https://user-images.githubusercontent.com/100905820/221752930-85503590-7b94-468a-b306-e7befba7aa59.png)

_Keys pressed: `<alt+tab><ctrl+c><alt+tab><ctrl+v><enter>`, `<alt+tab><ctrl+c><alt+tab><ctrl+v><space>L<tab>Tests<enter>`_

Using `<alt+tab>`, I switched to a different window to copy the `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` command to compile with JUnit, tabbed back to the terminal, and then pasted it. I again tabbed out, copied `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore` to run the JUnit tests, then pasted it. After that, I typed out a space and then `L` and a `tab` to finish it, but it only went to `ListExamples` so I finished it by manually typing `Tests`.

![image](https://user-images.githubusercontent.com/100905820/221758308-040b55e5-86b1-4e35-992c-20045ec33496.png)

_Keys pressed: `nano<space>L<tab>Tests.java<enter>`_

I typed `nano` because it's quick, did the same `tab` method as the command before this, but finished it by typing `.java` at the end.

![image](https://user-images.githubusercontent.com/100905820/221758480-3c40b6aa-ba68-4d10-966b-2239709173bf.png)

_Keys pressed: `<ctrl+w>while(index2<space><less-than(<)><enter><down><down><right><right><right><right><right><right><right><right><backspace>1<ctrl+o><enter><ctrl+x>`_

When I was in nano, I used `<ctrl+w>` to search for the string `while(index2 <` and it returns the first result which is close to where we need to be. Then I went down 2 times and right 8 times to change `index1` to `index2`. I then typed `<ctrl+o><enter>` to save the file and `<ctrl+x>` to quit nano and get back to the command line.

![image](https://user-images.githubusercontent.com/100905820/221760219-eba6de01-fa38-4235-960c-39877d390270.png)

_Keys pressed: `<up><up><up><enter>`, `<up><up><up><enter>`_

I pressed up 3 times in order to get back to the `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` command to compile, entered it, then pressed up 3 more times to get to the `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests` command and entered that to rerun the tests.

![image](https://user-images.githubusercontent.com/100905820/221760928-5dc706a5-3da8-40e9-9c36-f15426dc983d.png)

_Keys pressed: `git<space>add<space>L<tab>Tests.java<enter>`, `git<space>commit<space>-m<space>"g"<enter>`, `git<space>push<enter>`_

I added the changes to be committed and used the `tab` technique from earlier, then I committed them with a short message `"g"` to be quicker, and finally I pushed them using a simple `git push`.




