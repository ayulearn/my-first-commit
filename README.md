# my-first-commit

**demonstrate- how to make first commit on git**
---

Hope you configure your [user.name and use.email](https://github.com/ayulearn/git-begining). Now its time to make first commit 

**GOOD TO KNOW**
+ Always check `git status` before do anything.
+ Before `commit` work is `add` to staging area 
+ `commit` message is always written in Imperetive tens (present tens)
+ Before `add` work to staging area if you check `git status` file name have "red" in color
+ After `add` work to staging area if you check `git status` file name have "green" in color


## STEPS

This steps are also valid for window machine (use git bash) 
---
### 1. First of all check `git status` weather git is initialise in folder or not 

```git
git status
```

##### OUTPUT
![git status](https://github.com/ayulearn/git-practice/blob/main/3.png)

*(NOTE- if output not look like this👆 or show warning "fatal: not a git repository (or any of the parent directories): .git" then first [initialise-git](https://github.com/ayulearn/git-begining))*

---


### 2. Make file 

+ create file using `touch` command in linux 
 ```bash
  touch my_first_commit.txt
 ```
+ check file is created or not using `ls` command in linux
```bash
ls -l
```
##### OUTPUT
![output](https://github.com/ayulearn/git-practice/blob/main/6.png)

+ Check `git status` 
``` git 
git status
```
#### OUTPUT

![output](https://github.com/ayulearn/git-practice/blob/git-first-commit-ss/7.png)

output look like this 👆, it means a file is created which is untracked by git, so tu track it now we have to `add` this file to staging area 

### 3. `add` file to staging area
+ use `git add` command 

```git 
git add my_first_commit.txt
```
+ Again, Check `git status`

#### OUTPUT TEXT
``` bash
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
	new file:   my_first_commit.txt
```
*NOTE- Now color of `my_first_commit.txt` changed from "red" to "green" it means file add to staging areaa and now it's time to commit*
*OPTIONAL- You can check `git log` by using  command as below you will get no output*
```
git log
```

### 4. `commit` the changes 
+ use `git commit` command 
```
git commit -m "my first commit"
````
#### OUTPUT TEXT 
```bash
[master (root-commit) 8870f44] my first commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 my_first_commit.txt
```
+ Again, check `git status`
```
git status
```
#### OUTPUT TEXT 
```
On branch master
nothing to commit, working tree clean
```
**👆 it means you sucessfully commit on git to confirm it check the `log` this time you get the output**

```
git log 
```
#### OUTPUT

![output](https://github.com/ayulearn/git-practice/blob/git-first-commit-ss/log.png)

*Arrow mark text is the message you written during the commit command inside double quote you can change the message to during commit*

To get all the commands used [click here](https://github.com/ayulearn/my-first-commit/blob/main/linux-command.txt)
 





