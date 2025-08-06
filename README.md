# git-quick-start

Follow these steps to create a private repo and allow password-less access to it.

1. Create private Git repo on https://github.com/

2. Create a Git fine-grained token. It must have repository permissions for Read and Write access to code under Content.
   Copy the token to your clipboard.

3. Enable Git credential storage.
```
git config --global credential.helper store
```

4. Store token.
```
$ echo "https://user:token@github.com" >> ~/.git-credentials 
```

5. Clone repo. 
```
$ git clone https://github.com/user/repo
```

6. Finish git configuration.
```
git config --global user.name "Claudio Fahey"
git config --global user.email "claudiofahey@gmail.com"
```
