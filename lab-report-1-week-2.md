
# Lab Report 1

**Installing VScode**
![Screenshot1](https://media.discordapp.net/attachments/763128098999894087/961692270829142076/labreport1.png?width=1179&height=663)
To install VScode, go [here](https://code.visualstudio.com/) and follow the directions depending on whichever operating system you have. It supports mac, Windows, and Linux operating systems. 

**Remotely Connecting**
![Screenshot2](https://media.discordapp.net/attachments/763128098999894087/961692270829142076/labreport1.png?width=1179&height=663)
To connect to the remote server, install OpenSSH if you're using Windows, and make sure to have your class account, which can be found [here](https://sdacs.ucsd.edu/~icc/index.php), and password ready. In VScode, open a new terminal and enter $ ssh cs15lwi22zz@ieng6.ucsd.edu where zz is your class account. Finally, enter your password when prompted.

**Trying Some Commands**
![Screenshot3](https://media.discordapp.net/attachments/763128098999894087/961692270829142076/labreport1.png?width=1179&height=663)
Run some commands such as cd ~, cd, ls -lat, ls -a, cp, pwd, and cat. Test these commands for a terminal on your local computer and a terminal where you're connected to the server and note any differences. 

**Moving Files with scp**
![Screenshot4](https://media.discordapp.net/attachments/763128098999894087/961692270829142076/labreport1.png?width=1179&height=663)
In a terminal on your client, run scp <your file name> cs15lwi22zz@ieng6.ucsd.edu:~/ where zz is replaced with your account. When you log into the remote server and run the ls command, the file from your local computer should appear. The file can be ran on the server using javac and java. 

**Setting an SSH Key**
![Screenshot5](https://media.discordapp.net/attachments/763128098999894087/961692270829142076/labreport1.png?width=1179&height=663)
  

**Optimizing Remote Running**
![Screenshot6](https://media.discordapp.net/attachments/763128098999894087/961692270829142076/labreport1.png?width=1179&height=663)
