---
title: Lab Report 3, Week 6
---

# Report 3


## 1. Streamlining ssh Configuration

![Image](/labpics3/labrep3_1.png)

The first step a user must take is to change their directory so that they are on the *.ssh* directory. The the user can use the *touch* command followed by the *open .* command in their terminal to access their config file in their client computer. Once they have accessed the file they can input the following.
```
Host ieng6
HostName ieng6.ucsd.edu
User cs15lsp22zzz (use your username)
```

![Image](/labpics3/labrep3_2.png)

Once everything has been setup, the user can now use `ssh ieng6` to access their remote, course-specific account. The user no longer no longer needs to type out their whole account address, saving the user time.

![Image](/labpics3/labrep3_3.png)
![Image](/labpics3/labrep3_4.png)

Now that the account is easier to access, the user can even use the `scp` command quicker. For my example I removed the *WhereAmI.java* file from my remote computer and used `scp WhereAmI.java ieng6:~/` , while in the local server, to copy the file from the client computer to the remote computer. A lot of time is saved now that it no longer requires the whole account address.

---

## 2. Setup Github Access from ieng6

![Image](/labpics3/pt2_1.png)
When trying to push, it initially fails and can be explained by the following link, [This Link!](https://github.blog/2020-12-15-token-authentication-requirements-for-git-operations/) , but for short, you are no longer able to access github operations with password alone. We can use an alternative to access github actions following steps specified in [this link](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent).

![Image](/labpics3/pt2_2.png)
By following the given steps from the website and using the `ssh-keygen` command, I am able to make a key.

![Image](/labpics3/pt2_3.png)
Once the key is created, I then made sure that it was added.

![Image](/labpics3/pt2_4.png)
![Image](/labpics3/pt2_5.png)
![Image](/labpics3/pt2_6.png)
I copied the public key and added it through the github website.


![Image](/labpics3/pt2_7.png)
While I was trying to do this from my remote computer I still had to create a personal account token to be able to access github actions, specifically pushing to main. So I went into settings and created one.


![Image](/labpics3/pt2_9.png)
I used the PAT to be able to push from my remote server.

![Image](/labpics3/pt2_10.png)
I was able to push without a PAT from my local computer.

Attached is the [Link to the Commit](https://github.com/katrinado/skill-demo/blob/main/SkillDemo.java)

---

## 3. Copy whole directories with `scp -r`
![Image](/labpics3/scp1.png)
In this example I'm copying my `markdown-parser` repository to my course specific account. In the above image, it can be seen that `markdown-parser` isn't currently in my course specific server.

![Image](/labpics3/scp2.png)
In order to copy a whole directory, use `scp -r . ieng6:~/markdown-parser` command. Before using the command in the terminal, ensure that you are currently in your local `markdown-parser` directory. The files from the repository should then be listed as they are being copied into your ieng6 server.

![Image](/labpics3/scp3.png)
Above shows that the repository was successfully copied into the ieng6 server.

![Image](/labpics3/scp4.png)
To check that its corresponding files have also been copied, you can change your directory while in your ieng6 server and use the `ls` command to ensure everything was copied.