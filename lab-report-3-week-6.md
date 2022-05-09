# Lab Report 3, Week 6

## 1. Streamlining ssh Configuration

![Image](/labpics3/labrep3_1.png)

The first step a user must take is to change their directory so that they are on the *.ssh* directory. The the user can use the *touch* command followed by the *open .* command in their terminal to access their config file in their local server. Once they have accessed the file they can input the following.
```
Host ieng6
HostName ieng6.ucsd.edu
User cs15lsp22zzz (use your username)
```

![Image](/labpics3/labrep3_2.png)

Once everything has been setup, the user can now use `ssh ieng6` to access their remote, course-specific account. The user no longer no longer needs to type out their whole account address, saving the user time.



---

## 2. Setup Github Access from ieng6

---

## 3. Copy whole directories with `scp -r`
