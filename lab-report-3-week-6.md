# Lab Report 3

**Streamlining ssh Configuration**

![configFile](https://user-images.githubusercontent.com/103210217/167228163-81be92f5-8463-444c-8a81-37383e4a187d.png)
- This is the config file in .ssh and how I edited it in VSCode.

![sshCommand](https://user-images.githubusercontent.com/103210217/167228267-72435a0f-8119-4cbf-9413-6bd5a18698d8.png)
- This is the `ssh` command I used to log in with just my alias.

![scpWAlias](https://user-images.githubusercontent.com/103210217/167229068-2da06dd7-8fca-47ae-8394-1778bd0f737b.png)
- This is the `scp` command I used to copy a file into my ieng account using just my alias.

```
To streamline ssh configuration, create a configuration file within the ssh directory that tells SSH your host name alias, server username, and path to your ssh key file. Then you can `ssh` and `scp` with just your alias so you no longer have to type out your username and password. 
```

**Setup Github Access from ieng6**

![pubKey](https://user-images.githubusercontent.com/103210217/167229259-6c95754c-33c8-4bbf-bd66-cbfe26989869.png)
- This is a screenshot showing where my public key is stored on GitHub.

![pubKeyLocal](https://user-images.githubusercontent.com/103210217/167229342-bc550b5e-e9c9-4e21-98b0-7045e014d55e.png)
- This is where my public key is stored on my user account.

![privKey](https://user-images.githubusercontent.com/103210217/167229348-452438d2-9334-4eb4-880f-0fbd1c5b44a5.png)
- This is where my private key is stored on my user account.

![image](https://user-images.githubusercontent.com/103210217/167230249-773b4bf6-d87d-4163-b5a7-e4577cd09f75.png)
![image](https://user-images.githubusercontent.com/103210217/167230447-2c649d86-3df8-48be-91fc-f4653ca5664f.png)
![image](https://user-images.githubusercontent.com/103210217/167230462-2aa626ea-cb6f-41f4-8a52-5e6d0ac7bfd6.png)
![image](https://user-images.githubusercontent.com/103210217/167230477-366098c1-ba20-4736-b3ed-98290e9b1726.png)
- These are images of the `git add`, `git pull', and `git push` commands that I ran when logged into my ieng6 account.

- [This](https://github.com/aejiang/markdown-parser/blob/main/testFileeee.txt) is the link to the resulting commit.

```
To set up Github access from ieng6, you first generate a key by entering `ssh-keygen` in the terminal. Then you copy the public key generated from this to your Github ssh keys. Once you have set up Github access, you can use git commands in your remote server to directly update your repository. 
```

**Copy whole directories with `scp -r`**

![copydir1](https://user-images.githubusercontent.com/103210217/167238395-c48bb22c-9746-4234-b40a-2cf3c3e88d35.png)
![copydir2](https://user-images.githubusercontent.com/103210217/167238407-a0563b39-c429-4ff0-bfc3-731c87f6a903.png)
![copydir3](https://user-images.githubusercontent.com/103210217/167238415-858c4b8f-bd09-402b-b905-a0d420566b3c.png)
![copydir4](https://user-images.githubusercontent.com/103210217/167238424-8c525e97-96fe-4cc9-90c4-7afb26cfd565.png)
- This is what I did to copy my entire markdown-parse directory to my ieng6 account.

![iengtest](https://user-images.githubusercontent.com/103210217/167238643-7fbfad0a-5631-47f1-937b-93da3583302e.png)
- This is me logging into my ieng6 account and compiling and running the tests.


![all1](https://user-images.githubusercontent.com/103210217/168527682-b3e398cc-81fe-4c50-8ed6-7b1a7a17fbe5.png)
![tests](https://user-images.githubusercontent.com/103210217/168527942-5dfd60bf-69f5-42ec-9182-06d1178b626e.png)

- This is my `scp`, `;`,`ssh`, and JUnit test commands being run on one line. 

```
You can run `scp -r . cs15lsp22aoi@ieng6.ucsd.edu:~\markdown-parser` to copy your current directory into your remote server by creating a new directory in the remote server. Then you can check if the directory was successfully copied over by running `ssh ieng6` to log in. After changing into the correct directory, you can run `javac -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar MarkdownParseTest.java` and `java -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar org.junit.runner.JUnitCore MarkdownParseTest` to run the JUnit tests. All of these commands can be combined into one line with semicolons to separate each command.
```






