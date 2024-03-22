# RemoteConnect

**1.Create a project locally**

**2.Open gitbash and go to the path of the project**

**Git commands to procure :**

1.git -init

2.git status

3.git add .

4.git commit -m "commit_message"

**Now, we have to connect this local to some remote repo for which we will go with below set of commands :**

1.git remote add origin ssh_repo_url [Ex. git@github.com:rohit-sinha-lab49/PlaywrightAPIWithJava.git]

2.git push -u -f origin main

**In case if any issue occurs then have to go with below set of commands :**

1.git remote -v

2.git remote set-url origin ssh_repo_url [Ex. git@github.com:rohit-sinha-lab49/PlaywrightAPIWithJava.git]

2.git push --set-upstream origin main [Might not need this but can be used]

**If issue comes such as 'Please make sure you have the correct acceess rights and the repository exists.', 
the go with below set of commands :**

1.ssh-add -l -E md5

2.ssh-add ~/.ssh/git_rsa

3.cat ~/.ssh/id_rsa.pub

**After all the above steps its recommended to remote the remote branch with below set of commands :**

1.git remote rm origin

2.git remote add origin ssh_repo_url [Ex. git@github.com:rohit-sinha-lab49/PlaywrightAPIWithJava.git]



3.git fetch

4.git push -u -f origin main
