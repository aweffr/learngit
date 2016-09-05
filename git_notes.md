Git is a tool under Linux/Unix environment, so that it need simulation environment called Cygwin under Windows. Fortunatly there is a packed distribution 'msysgit' to install both Cygwin and git on Windows.

- To create a new repository: git init
- To add a file into stage: git add<file>
- To commit these file into repo: git commit

![working -> index(staged) -> repo](http://www.liaoxuefeng.com/files/attachments/001384907702917346729e9afbf4127b6dfbae9207af016000/0)
- to diff the working tree and staged area:	git diff
- to diff the staged area and HEAD(repo):	git diff --staged
- to diff the working tree and HEAD:		git diff HEAD