# Week 6 Lab Report

## 1. Streamlining ssh Configuration

![Image](Report3/sshConfig1.png)

In this part of the lab, I accessed the `.ssh/config` file on my own computer to change the username I need to input to log onto my given remote server. The phrase after **Host** represents the username, *yesoryes*, I would have to input after the `ssh` command. The fourth line of the file explicitly refers to my public key, so that I would not need to enter a password to log onto the remote server. In the terminal, I ran the command `ssh yesoryes` which used my previously generated public key to log me onto the **cs15lsp22ajk** remote server.

![Image](Report3/sshConfig2.png)

In this next screenshot, I used the `scp` command to copy over the *DELETEAFTER.txt* file over to the **cs15lsp22ajk** server. After logging onto the server using `ssh` and checking the files on the server with the `ls` commands, we can see that *DELETEAFTER.txt* was indeed copied over.

## 2. Setup Github Access from ieng6

![Image](Report3/SS2.png)

On VS Code, I opened up a new terminal by navigating through *terminal --> new terminal* at the top of the window. Before remotely connecting, I made sure to have installed [OpenSSH](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse) for Windows, as well as to make sure I know my [remote account](https://sdacs.ucsd.edu/~icc/index.php). The last step would be to run `ssh cs15lsp22ajk@ieng6.ucsd.edu` where the **ajk** specifies my given account.

## 3. Copy whole directories with `scp -r`

![Image](Report3/SS3.png)

Now that I am remotely connected to this account, I can run several commands to look at what files the account currently has. Some of the ones I have tried in my screenshot are: `cd`, `ls -l`, `ls -a`, `ls -lat`. I also learned that `l` prints out the files in **long format**, `a` prints out **all** files, `t` prints out the files in order **by time**, and that any combination of those key letters after `ls` outputs all of their information.
