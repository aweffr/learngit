Git is a tool under Linux/Unix environment, so that it need simulation environment called Cygwin under Windows. Fortunatly there is a packed distribution 'msysgit' to install both Cygwin and git on Windows.

- To create a new repository: git init
- To add a file into stage: git add<file>
- To commit these file into repo: git commit

![working -> index(staged) -> repo](http://www.liaoxuefeng.com/files/attachments/001384907702917346729e9afbf4127b6dfbae9207af016000/0)
- to diff the working tree and staged area:	git diff
- to diff the staged area and HEAD(repo):	git diff --staged
- to diff the working tree and HEAD:		git diff HEAD

- git log: if the output message is to much, add: --pretty=oneline
- git uses "362...e101" as the version id computed by SHA1 (radix==16), because it is a distributed version control tool. Using SHA1 will avoid the id conflicts.

- To go to the old version:
- HEAD represents for the current version.
- HEAD^ represents for the last old version.
- HEAD^^ 2nd; HEAD~100,go 100 times back.
- Sample code: git reset --hard HEAD^

- To go back to the current version: find the commit_id.
- how: git reflog
- tips: we can just type >=6 digits of commit_id and it will search and find the exact commit_id.

- How it work:
- HEAD is just a pointer which points to different commits. When we use reset, the HEAD points to the certain commit version.

- A **key difference** between git and other version control system is that what git tracks is **diff** rather than **file**.

- **How to draw back the change text in the working area**
- git checkout -- (file)
- this command will make this file back to last version of (git add / git commit).
- **Draw back the change text already staged**
- git reset HEAD (file)
- e.g: git reset HEAD readme.txt
- this command called "unstage"

- *To be contine...*

---
[NextChapter](http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/0013758392816224cafd33c44b4451887cc941e6716805c000)