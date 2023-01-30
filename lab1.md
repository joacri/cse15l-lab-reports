# Lab Report 1

> In this week's lab we learned about setting up remote access.
> This is a tutorial on how to log into a course-specific account on ieng6.

## Installing VScode
>  - On the personal laptop that you plan to use open up the following website: [code.visualstudio.com](https://code.visualstudio.com/)
>  - The website has several download options, so you should choose the right one that matches your device. 
>  ![Image](Vscode_web2.png)
>  - You should open your download and follow the instructions to finish installing VScode on your device. When the installation process is done, VScode should look similar to the picture below when opened:
>  ![Image](Vscode_installed.png)

## Remotely Connecting
> Windows 
> - If you are on Windows (like me), then a very important step is to install git for Windows on your device. Use the following link for download: [gitforwindows.org](https://gitforwindows.org/) 
> - The next step for Window users is to follow the steps in this new [link](https://stackoverflow.com/questions/42606837/how-do-i-use-bash-on-windows-from-the-visual-studio-code-integrated-terminal/50527994#50527994) in order to open the Git Bash terminal in VScode. After that you can continue with the rest of the instructions. 

> CSE15L Account & Password
> - In order to access your account information you have to use the following link : [sdacs.ucsd.edu](https://sdacs.ucsd.edu/~icc/index.php)
> - That is where you need to input your school username and student ID.
> - The course specific account you found should begin with 'cs15lwi23' and be followed by some letters.
> - Also visible on that page should be the link that takes you to change your password for that account.
> - Make sure to change your password and for a more in depth explanation go to this [Tutorial](https://docs.google.com/document/d/1hs7CyQeh-MdUfM9uv99i8tqfneos6Y8bDU0uhn1wqho/edit).
> - Once you successfully reset your password you can continue with the steps that follow!!!

> - Open a new terminal by using the menu option or Ctrl + ` . It should look like this: 
> ![Image](rc_open.png)
> - Type in the following command but the letters between the 23 and the @ should be the ones that correspond to your own course-specific account.
> ![Image](rc_login.png)
> - When it is your first time connecting to a server it will give you basic messages that you can just type `yes` in order to continue.
> - It should then ask for your password. (When it asked for my password it wouldn't let me see what I was typing, but I just typed in my password and pressed enter at the end and it worked fine). Should look like this when you have connected successfully.
> ![Image](rc_in.png)

## Trying Some Commands
> The following commands can produce different results based on the input that follows them and the order that they are called.
> - `cd`    - change directory 
> - `pwd`   - print working directory 
> - `ls`    - lists the the files and directories
> ![Image](tsc1.png)
> - `cp`    - copies files or group to specific destination
> - `cat`   - prints the the contents of one or more files 
> ![Image](tsc2.png)
> - `mkdir` - creates directories
> - `rmdir` - removes the directory
> - `exit`  - logs you out of the remote server in your terminal
> ![Image](tsc3.png)
