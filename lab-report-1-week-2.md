
# Lab Report 1

**Installing VScode**
![Screenshot1](https://media.discordapp.net/attachments/763128098999894087/962608452713193492/vsc.png)
To install VScode, go [here](https://code.visualstudio.com/) and follow the directions depending on whichever operating system you have. It supports mac, Windows, and Linux operating systems. 

**Remotely Connecting**
![Screenshot2](https://cdn.discordapp.com/attachments/763128098999894087/962609708592668732/sshss.png)
To connect to the remote server, install OpenSSH if you're using Windows, and make sure to have your class account, which can be found [here](https://sdacs.ucsd.edu/~icc/index.php), and password ready. In VScode, open a new terminal and enter $ ssh cs15lwi22zz@ieng6.ucsd.edu where zz is your class account. Finally, enter your password when prompted.

**Trying Some Commands**
![pwdScreenshot](https://media.discordapp.net/attachments/763128098999894087/962773496277127208/pwdss.png?width=1393&height=663)
- pwd: prints out the path of your current directory
![lsScreenshot](https://cdn.discordapp.com/attachments/763128098999894087/962774682124308560/lsss.png)
- ls: lists out the files in your current directory
![cdScreenshot](https://media.discordapp.net/attachments/763128098999894087/962775211273515089/cdss.png?width=1367&height=663)
- cd: changes your current directory 
![mkdirScreenshot](https://cdn.discordapp.com/attachments/763128098999894087/962775996992462858/mkdirss.png)
- mkdir: creates a new directory of the specified name
![cpScreenshot](https://media.discordapp.net/attachments/763128098999894087/962779409427865631/cpss.png?width=1343&height=662)
- cp: makes a copy of a file or directory with a different name 

**Moving Files with scp**
![Screenshot4](https://media.discordapp.net/attachments/763128098999894087/962610342540771348/scpss.png)
In a terminal on your client, run `scp yourFileName cs15lwi22zz@ieng6.ucsd.edu:~/` where zz is replaced with your account and yourFileName is the name of your file. When you log into the remote server and run the ls command, the file from your local computer should appear. The file can be ran on the server using javac and java. 

**Setting an SSH Key**
![Screenshot5](https://cdn.discordapp.com/attachments/763128098999894087/962924951961227304/step5ss.png)
- To generate the keys, run `ssh-keygen -t ed25519` and enter the name of the file you'd like to save your key in and then enter in a passphrase. 
- If you're on Windows, follow these additional [directions](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_keymanagement#user-key-generation) to store your private key. 
- Copy the public key that ends in .pub to .ssh in your remote server by running mkdir .ssh on the server and scp /Users/joe/.ssh/id_rsa.pub cs15lwi22@ieng6.ucsd.edu:~/ .ssh/authorized on your local computer with your account name and the path your key was saved in. 
  
  
**Optimizing Remote Running**
![Screenshot6](https://cdn.discordapp.com/attachments/763128098999894087/962802179637395528/speedyss.png)
- Use SSH keys to avoid entering long password.
- Put command in quotes after command to log in to remote server to run both together. (E.g. ssh cs15lsp22zz@ieng6.ucsd.edu "ls")
- Run multiple commands together by separating them with a semicolon. (E.g. javac WhereAmI.java; java WhereAmI)

