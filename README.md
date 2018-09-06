# git-quick-start

1. Create private Git repo on https://github.com/

2. Create a Git personal access tokens with **repo** permissions.

3. Enable Git credential storage.
```
git config --global credential.helper store
```

4. Clone repo and enter the token. 
```
$ git clone https://github.com/user/repo
Username for 'https://github.com': user
Password for 'https://user@github.com': personal access token
```

5. Note that the password will be automatically stored.
```
$ cat ~/.git-credentials 
https://user:token@github.com
```
