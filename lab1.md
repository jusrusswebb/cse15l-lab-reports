# Installing VS Code

First, head to [Visual Studio Code](https://code.visualstudio.com/) and follow the system specific instructions for either masOS or Windows. If you are working with a PC you will need to scroll down to the bottom of the page to find the download instructions.  

![Image](vscodehome.png)

After VS code is downloaded, open your files and look for VS code Zip file. After you click on the zip file, a file named Visual Studio Code should be downloaded into your files. 

![Image](vscodefile.png)

Once you click on the Visual Studio Code file in your files you should reach a home page that looks similar to the one below. To get started, you can either open an existing file or create a new one by clicking New File. 

![Image](vscodeapp.png)

# Remotely Connecting

Open the terminal in VS code.(Ctrl or Command + `, or use the Terminal → New Terminal menu option), and type in ssh followed by your account name.

![Image](ssh1.png)

If this is your first time logging in to the server, you should be met with a repsponse saying "Are you sure you want to continue connecting (yes/no/[fingerprint])?". Type yes, press enter, and then you should be met with a request to input your password as below. 

![Image](password_req.png)

Once you have input your password, you should see a message similar to the one below. Notice how the server displays information like the different hosts and how many users are using those hosts. This can give you an idea of how fast or slow the server will be running.  

![Image](login_success.png)

# Trying Some Commands

There are many commands you can make to access and manipulate files in your directory. To check where you currently are in the directory, use command pwd as shown below. The pwd command outputs the entire path to the current directory. 

![Image](pwd_pic.png)

Other useful commands involve changing the current directory. To see which files your current working directory has access to, input ls. To update the directory further down the path, input cd [filename]. To return to your previous working directory, simply input cd -. Examples of all of these commands in action are shown below.

![Image](commands.png)

You are also able to read input and write output to files and directories. Two commands that can do this are cp and cat. While cp makes a copy of the file just like the original, cat creates a new file with the same content. As shown below, cat also outputs the contents of a file out to the console.

![Image](cp_cat.png)

