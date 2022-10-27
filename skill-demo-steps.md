<br>1. Clone this repository (we recommend using the command line in VScode!): https://github.com/ucsd-cse15l-f22/skill-demo1

<br>`git clone https://github.com/ucsd-cse15l-f22/skill-demo1`

<br>2. Build and run the tests locally, using javac and java (note that bash will not work locally on the Windows machines)

<br>`javac -cp ".;lib/hamcrest-core-1.3.jar;lib/junit-4.13.2.jar" *.java`
<br>`java -cp ".;lib/junit-4.13.2.jar;lib/hamcrest-core-1.3.jar" org.junit.runner.JUnitCore TestDocSearch`

<br>3. Fix the broken test (the test is wrong, not the implementation) and rerun locally

<br>change 10 to 1391
<br>`javac -cp ".;lib/hamcrest-core-1.3.jar;lib/junit-4.13.2.jar" *.java`
<br>`java -cp ".;lib/junit-4.13.2.jar;lib/hamcrest-core-1.3.jar" org.junit.runner.JUnitCore TestDocSearch`

<br>4. Build and run the server locally, using javac and java (note that bash will not work locally on the Windows machines)

<br>`javac Server.java DocSearchServer.java`
<br>`java DocSearchServer 4444`

<br>5. In a browser, visit the paths / and /search?q=... where ... is a search term of your choice that finds at least 2 files on localhost to demonstrate that it works

<br>/search?q=chapter


<br>6. Get the code for the server onto ieng6 and build and run it there (your choice of how) as the provided account. A ssh key will be configured for the account you are provided for the exam.

<br>`ssh provided-server`
<br>`git clone https://github.com/ucsd-cse15l-f22/skill-demo1`

<br>7. Open the path / and /search?q=... where ... is a search term of your choice that finds at least 2 files on the ieng6 server to demonstrate that it works

<br>`javac Server.java DocSearchServer.java`
<br>`java DocSearchServer 4444`
<br>visit `http://ieng6-202.ucsd.edu:4444/`

<br>exit

<br>8. Change the program so that it searches for substrings within the path based on the query, rather than within the file’s contents. For example, a query like /search?q=rr74 would find the file technical/biomed/rr74.txt

<br>change line 47 to f.toString()

<br>9. Build and run the server locally and demonstrate the new behavior

<br>`javac Server.java DocSearchServer.java`
<br>`java DocSearchServer 4444`
<br>visit local

<br>10. Copy the change to the remote ieng6, then build and demonstrate the new behavior there

<br>`scp DocSearchServer.java cs15lfa22mr@ieng6.ucsd.edu:skill-demo1`
<br>`ssh provided-server`
<br>`cd skill-demo1`
<br>`javac Server.java DocSearchServer.java`
<br>`java DocSearchServer 4444`
<br>visit `http://ieng6-202.ucsd.edu:4444/`
<br>/search?q=chapter
