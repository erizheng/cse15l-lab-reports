# Lab Report 4: Vim
## **Part 1**: Changing the name of the start parameter and its uses to base using vim

<br>**Vim Key Strokes**
<br>After entering vim with `vim DocSerachServer.java`
<br>I press the following keys `/start<enter>cgnbase<esc>n.n.<shift>;wq<enter>`
<br>resulting in > 24 keystrokes

<br>The first part after getting in vim, the cursor will highlight the very first character in the file, then you can type `/start<enter>` to find the word "start" in the file which the third image show it highlighting the first charcter of "start".
<br><img src="images5/vim1.png" alt="drawing" width="300"/>
<br><img src="images5/vim2.png" alt="drawing" width="300"/>
<br><img src="images5/vim3.png" alt="drawing" width="300"/>

<br>After you can type `cgn` to replace the word which you then type the word you want in this case being "base" and click `<esc>` to exit the editing.
<br><img src="images5/vim4.png" alt="drawing" width="300"/>
<br><img src="images5/vim5.png" alt="drawing" width="300"/>

<br>The next step, you can press `n` to find the next instance of the word you searched for and press `.` to repeat your previous action which was deleteing and replacing "start" with "base" using `cgn`.
<br><img src="images5/vim6.png" alt="drawing" width="300"/>
<br><img src="images5/vim7.png" alt="drawing" width="300"/>

<br>Then you repeat `n.`
<br><img src="images5/vim8.png" alt="drawing" width="300"/>

<br>Lastly to save and exit you use ":wq<enter>` or `<shift>;wq<enter>`.
<br><img src="images5/vim9.png" alt="drawing" width="300"/>

## **Part 2**: Comparing Vim and Scp
<br>**SCP Method**
<br>Use pastable scp to upload file to remote server, then use bash test.sh to run test file
<br>Time took: 46.52 seconds
<br>The most difficult part of scp is the scp and ssh process which I have to type in or copy a long user name.

<br>**Vim Method**
<br>Do part 1 on remote server
<br>Time took: 30.41 seconds
<br>The most difficult part of vim is to get use to the the way vim operates and how each key works

<br>I think I still would prefer the general scp method because I get to see the file more clearly with its color code. It is just easier for me to read and I am too use to using the mouse to navigate through the code. However, if it is for smaller changes I think I would like vim more because of its efficiency. I can't deny how mich faster vim can be, for this comparison, I fumbled on typing while working with vim but somehow I was still 10 seconds quicker than scp. 
