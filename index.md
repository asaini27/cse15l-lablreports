# WEEK 2 LAB REPORT 
# BY ADITYA SAINI

## INSTALLING AND DOWNLOADING VISUAL STUDIO CODE:

For downloading VS code, go to the Visual Studio Code website linked below:
[VS CODE LINK](<https://code.visualstudio.com/(http://a.com>) 
Then follow the instructions to download and install it on your computer. There are versions for all the
major operating systems, like OSX (for Macs) and Windows (for PCs).

When it is installed, you should be able to open a window that looks like this (it might
have different colors, or a different menu bar, depending on your system and settings):

<img width="1440" alt="Screenshot 2022-04-09 at 6 23 52 PM" src="https://user-images.githubusercontent.com/103229052/162649766-cfb51094-95a1-4d70-86d7-1bc12d6313f0.png">

![](https://drive.google.com/file/d/1Xi4kNqVkzcAoTD3Zntj1dRtR-GHj2SDh/view?usp=sharing)

## REMOTELY CONNECTING

If working on windows, then install open ssh.

We would need to find a our CSE 15L account name and password as well through the link attached below. 
[LINK](<https://sdacs.ucsd.edu/~icc/index.php(http://a.com>)

Now we follow the steps to connect to a remote host

* Open terminal in VS code and command will look like this, but with the zz replaced by the
  letters in your course-specific account.
  ```
  $ ssh cs15lsp22zz@ieng6.ucsd.edu
  ```

* After this you would see a message like this:
  Are you sure you want to continue connecting
  (yes/no/[fingerprint])?
  respond yes to this. 
  
* Then we give our password and once we give our password we would be logged in

Something similar to this screenshot should be there.
<img width="854" alt="Screenshot 2022-04-10 at 5 32 33 PM" src="https://user-images.githubusercontent.com/103229052/162649709-bc454148-3055-479e-91d8-881f5e2310c1.png">


![](<https://drive.google.com/file/d/1C12yGaRF-R52el4OjPxsIkXoTFttUbao/view?usp=sharing>)

After this our terminal is connected to the computer in the CSE basement.


## TRYING SOME COMMANDS

Here are some useful commands:

* cd ~
* cd
* ls -lat
* ls -a
* ls <directory> where <directory> is /home/linux/ieng6/cs15lsp22/cs15lsp22abc, where the abc is one
of the other group members’ username
* cp /home/linux/ieng6/cs15lsp22/public/hello.txt ~/
* cat /home/linux/ieng6/cs15lsp22/public/hello.txt
  
The following screenshot shows the command cd and ls -lat:
  <img width="959" alt="Screenshot 2022-03-31 at 7 22 00 PM" src="https://user-images.githubusercontent.com/103229052/162649607-022b25ee-bac3-431e-a08b-4a7f1fb69048.png">

![](<https://drive.google.com/file/d/1hWtDNb_u5-ieL2DxCM5hJpZijM7MeZkM/view?usp=sharing>)
  
## MOVING FILES WITH SCP
  
We’ll now see a way to copy a file (or many files!) from your computer to a remote
computer. The command is called scp, and we will always run it from the client (that
means from your computer, not logged into ieng6). First we create a file named WhereAmI.java with the follwoing code:
  
```
class WhereAmI {
  public static void main(String[] args) {
    System.out.println(System.getProperty("os.name"));
    System.out.println(System.getProperty("user.name"));
    System.out.println(System.getProperty("user.home"));
    System.out.println(System.getProperty("user.dir"));
  }
}
```
Now we run this file and we would see the following result : 

![](<https://drive.google.com/file/d/1eVb3b0tILvQiXNsm0owVwJBZRheIE3yK/view?usp=sharing>)
  
<img width="869" alt="Screenshot 2022-04-10 at 6 15 01 PM" src="https://user-images.githubusercontent.com/103229052/162649467-65d355bc-7a7b-4f94-b67e-7f96ce284cbc.png">
  
Then, in the terminal from the directory where you made this file, run this command (as
usually, using your username):
```
scp WhereAmI.java cs15lsp22zz@ieng6.ucsd.edu:~/
```

Then, log into ieng6 with ssh again, and use ls. You should see the file there in your
home directory! Now you can run it on the ieng6 computer using javac and java.

The following screenshot shows the whole method and the result: 
  <img width="961" alt="Screenshot 2022-03-31 at 7 23 10 PM" src="https://user-images.githubusercontent.com/103229052/162650360-604ca86f-75eb-45c6-80fe-6562e0b724ad.png">

![](<https://drive.google.com/file/d/1JrrYsTqF1L3FFEMfmIMprcN6a7IM_RO2/view?usp=sharing>)
  
## SETTING AN SSH KEY

Every time we log in or run scp, we have to type (or copy-paste) our
password. This is frustrating, time consuming, and interrupts whatever task we were
trying to do. there is a great solution – ssh keys. The idea behind ssh keys is that a
program, called ssh-keygen, creates a pair of files called the public key and private
key. You copy the public key to a particular location on the server, and the private key in
a particular location on the client. Then, the ssh command can use the pair of files in
place of your password.
  
Here’s what you should run to set this up:

```
# on client (your computer)
$ ssh-keygen
Generating public/private rsa key pair.
Enter file in which to save the key
(/Users/<user-name>/.ssh/id_rsa): /Users/<user-name>/.ssh/id_rsa
Enter passphrase (empty for no passphrase):
```
** Note: Make sure to not add a paraphrase

We will see a similar desktop:
  
![](<https://drive.google.com/file/d/13KHn8gIdWgYbOFvbQmZI7doRkeyNJKG2/view?usp=sharing>)
  
<img width="1074" alt="Screenshot 2022-03-31 at 7 36 18 PM" src="https://user-images.githubusercontent.com/103229052/162652893-74ad016e-1b37-495d-a42a-873d30dbb0e0.png">
  
## OPTIMIZING REMOTE RUNNING 

* Write a command in quotes at the end of an ssh command to directly
run it on the remote server, then exit. For example, this command will log in and
list the home directory on the remote server:
```
$ ssh cs15lsp22zz@ieng6.ucsd.edu "ls"      
```
* Using semi colon to run multiple commands on the same line in most terminals. Eg:
```
  $ cp WhereAmI.java OtherMain.java; javac OtherMain.java;
java WhereAmI
```
* Use the up arrow key to run the previous commands. 
  
  
