
# GIT [PART-2]

GIT Commands


## Commands 

#### 1. Compares staging area files VS working file Directory

```
 git diff
```


#### 2. Compares Staging area Files Vs Previous Commited Files
```
 git diff --staged
 ```

#### 3. DIRECT COMMIT-> No need to perform git add --all.It Automatically stages all tracked files and make commit [Ignores Untracked Files]
```
git commit -a -m "Direct Commit"
 ```
#### 4. REMOVE FILE -> Removes files and adds automatically to staging area
```
git rm "file.txt"
 ```

 #### 5. RENAME FILE-> Renames file name and adds automatically to staging area.
 ```
git rm "file.txt" "filename1.txt"
 ```


#### 6. HOW TO UNTRACK FILEs-> Changing state from  tracked to untracked doesnt deletes file.After this command  do ADD THIS TO gitignore.
 ```
git rm --cached "file.txt" 
 ```


#### 7. Clone repo with Customized name -> git repo will be cloned to myname folder  
 ```
git clone url "myname" 
 ```


#### 8. Detailed log  
 ```
git log -p 
 ```

#### 9. Detailed log for 3 commits  
 ```
git log -p -3
 ```

#### 10. short summary of logs  
 ```
git log --stat
 ```

#### 11. oneline for each git log [oneline / short/ full]  
 ```
git log --pretty = oneline
 ```
 
 #### 12. check recent 2 days git logs [2.weeks / 2.months / 2.years]  
 ```
git log --since=2.days
 ```
 

 #### 13. Git Formatting ->Displays git log [format of hash <--> Author name]
 ```
git log --pretty=format:"%h -- %an"
 ```

 
 #### 14. Amending the most recent commit message->1)Edit= will open your editor, allowing you to change the commit message of the most recent commit.  2)new commit add =Additionally, you can set the commit message directly in the command line with:

 ```
git commit --amend
 ```

```
git commit --amend -m "New commit message"
 ```

 #### 15. To unstage a file
 ```
git restore --staged file.txt
 ```
 

 #### 16. Prevent Accidently Modification ->To get data back of file.txt as per previous commit if got accidently modified.
 ```
git checkout --file.txt
 ```

 #### 17. To see Already merged branches 
 ```
git branch --merged
 ```

 #### 18. To see Already not merged branches
 ```
git branch --no-merged
 ```

 
 #### 19. Deleting Branches: Gives error if branch develop is not merged
 ```
git branch -d develop
 ```

  #### 20. Deleting Branches: Forcefully branch develop gets deleted
 ```
git branch -D develop
 ```

 
  #### 21. On remote pushes branch bugfix as mybugfix
 ```
git push origin bugfix:mybugfix
 ```

 
  #### 22. Deleting branch on remote
 ```
git push -d origin bugfix
 ```
