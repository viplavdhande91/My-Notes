

## Git Commands 

-   GIT Version

```bash
 git version
```

-   GIT config editing ***( global config file is present in user folder of windows)***

```bash
 git config --global --edit

 git config --global user.name "VP"

 git config --global user.email "viplav@example.com"


```

-   GIT config check ***(To check config of user)***

```bash
 git config --list
```

-   GIT status ***(Gives status and tracking of files)***

```bash
 git status
```


-   GIT init ***(Initialize blank repo folder)***

```bash
 git init
```


-   GIT merge ***(Merging of both branch will happen .Each changes will be reflected in developement)***

```bash
 git checkout developement

 git merge feature/22541


```

-   ***GIT remote origin check***

```bash
 git remote - version

 git remote add origin url
```

-   Compares staging area files VS working file Directory

```bash
 git diff
```


- ***Compares Staging area Files Vs Previous Commited Files***
``` bash
 git diff --staged
 ```

-  **DIRECT COMMIT-> No need to perform git add --all. It Automatically stages all tracked files and make commit [Ignores Untracked Files]**
```bash
git commit -a -m "Direct Commit"
 ```
-  ***REMOVE FILE*** -> Removes files and adds automatically to staging area
```bash
git rm "file.txt"
 ```

 -  ***RENAME FILE***-> Renames file name and adds automatically to staging area.
```bash
git rm "file.txt" "filename1.txt"
 ```


-  ***HOW TO UNTRACK FILES***-> Changing state from  tracked to untracked doesnt deletes file.After this command  do ADD THIS TO gitignore.
```bash
git rm --cached "file.txt" 
 ```


-  ***Clone repo with Customized name*** -> git repo will be cloned to myname folder  
```bash
git clone url "myname" 
 ```


- ***Detailed log*** 
```bash
git log -p 
 ```

-  ***Detailed log*** for 3 commits  
```bash
git log -p -3
 ```

-  ***short summary of logs***  
```bash
git log --stat
 ```

-  ***oneline for each git log [oneline / short/ full]***  
```bash
git log --pretty = oneline
 ```
 
 -  check recent 2 days git logs [2.weeks / 2.months / 2.years]  
```bash
git log --since=2.days
 ```
 

 -  Git Formatting ->Displays git log [format of hash <--> Author name]
```bash
git log --pretty=format:"%h -- %an"
 ```

 
 -  ***Amending the most recent commit message***->
    -  Edit = will open your editor, allowing you to change the commit message of the most recent commit. 
    -  new commit add =Additionally, you can set the commit message directly in the command line with:

```bash
git commit --amend
 ```

```bash
git commit --amend -m "New commit message"
 ```

 -  ***To unstage a file***
```bash
git restore --staged file.txt
 ```
 

 -  ***Prevent Accidently Modification*** : To get data back of file.txt as per previous commit if got accidently modified.
```bash
git checkout --file.txt
 ```

 -  ***To see Already merged branches*** 
```bash
git branch --merged
 ```

 -  ***To see Already not merged branches***
```bash
git branch --no-merged
 ```

 
 -  ***Deleting Branches:*** Gives error if branch develop is not merged
```bash
git branch -d develop
 ```

  -  ***Deleting Branches:*** Forcefully branch develop gets deleted
```bash
git branch -D develop
 ```

 
  -  **On remote deletes branch develop**
```bash
git push origin :develop
 ```

 
  -  ***Deleting branch on remote***
```bash
git push -d origin bugfix
 ```
