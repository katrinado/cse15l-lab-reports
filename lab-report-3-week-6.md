# Lab Report 3, Week 6

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

---

## 3. Copy whole directories with `scp -r`
