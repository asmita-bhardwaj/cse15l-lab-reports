# Lab Report 1

## Step 1: Install VS Code

- Visit the [Visual Studio Code website](https://code.visualstudio.com)
- Follow downloading and set up instructions for particular operating system (OSX or Windows)
- To verify that VS Code has succesfully been installed, open a window on the app. Your screen should look similar to the image below. 

![Image](VSCodeInstall.jpg)

## Step 2: Remotely Connecting

- If you are working on a windows, install [git](https://gitforwindows.org) and with the help of this [post](https://stackoverflow.com/questions/42606837/how-do-i-use-bash-on-windows-from-the-visual-studio-code-integrated-terminal/50527994#50527994) set the default terminal to **git bash**.
- Next, Open a terminal on the VS Code App (access Terminal → New Terminal through menu). Your screen should now look like this:
![Image](VSCodeTerminal.jpg)
- In the first line, after the '$', feed in the command `ssh cs15lwi23zzz@ieng6.ucsd.edu`. Replace 'zzz' with letters from your specific account and press enter 
- The terminal should ask for the account's password. Fill in the password and press enter once again.
The terminal should look something like this now:
![Image](VSCodeAfterPass.jpg)

## Step 3: Trying Some Commands

- Explore running some of the following commands in the terminal:
  - cd ~ : useful for changing the current working directory to ~, the home directory. The home directory is where all of a user's paths are stored.
  - ls -lat : ls is useful for listing all the files and folders in the specified path. 
  - cat /home/linux/ieng6/cs15lwi23/public/hello.txt : this command is useful in printing the contents of the file hello.txt. after the command 'cat', a path must be specified to identify which file's contents should be printed.
 

Below is what such commands would run like:
![Image](TryingCommands.jpg) 
 
 
 
 Lastly, to exit the remote server in your terminal, run the command `exit`

