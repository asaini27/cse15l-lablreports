# WEEK 2 LAB REPORT 
# BY ADITYA SAINI

## INSTALLING AND DOWNLOADING VISUAL STUDIO CODE:

For downloading VS code, go to the Visual Studio Code website linked below:
https://code.visualstudio.com/(http://a.com) 
Then follow the instructions to download and install it on your computer. There are versions for all the
major operating systems, like OSX (for Macs) and Windows (for PCs).

When it is installed, you should be able to open a window that looks like this (it might
have different colors, or a different menu bar, depending on your system and settings):

!https://drive.google.com/file/d/1Xi4kNqVkzcAoTD3Zntj1dRtR-GHj2SDh/view?usp=sharing(http://url/a.png)

## REMOTELY CONNECTING

If working on windows, then install open ssh.

We would need to find a our CSE 15L account name and password as well through the link attached below. 
https://sdacs.ucsd.edu/~icc/index.php(http://a.com)

Now we follow the steps to connect to a remote host

* Open terminal in VS code and command will look like this, but with the zz replaced by the
  letters in your course-specific account.
  $ ssh cs15lsp22zz@ieng6.ucsd.edu

* After this you would see a message like this:
  Are you sure you want to continue connecting
  (yes/no/[fingerprint])?
  respond yes to this. 
  
* Then we give our password and once we give our password we would be logged in

Something similar to this screenshot should be there.
![https://drive.google.com/file/d/1C12yGaRF-R52el4OjPxsIkXoTFttUbao/view?usp=sharing](http://url/a.png)

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
![https://drive.google.com/file/d/1hWtDNb_u5-ieL2DxCM5hJpZijM7MeZkM/view?usp=sharing](http://url/a.png)

  
  
