# HW_9_Loop_Game 
# Command Prompt


E:\>Dir
 Volume in drive E is PRASUN
 Volume Serial Number is B0CF-9DF4

 Directory of E:\

10/09/2015  10:22 AM    <DIR>          .metadata
10/09/2015  10:22 AM    <DIR>          Prasun
10/26/2015  10:05 AM        12,563,873 introduction-to-java-programming-comprehe
nsive-version-10th-edition.zip
10/26/2015  10:13 AM    <DIR>          Fun_With_Functions
10/26/2015  10:42 AM             2,706 Comment_Line_md.txt
11/02/2015  10:30 AM    <DIR>          Listing_Project
11/03/2015  10:07 PM             3,394 Command.txt
02/11/2015  11:05 PM    <DIR>          workspace
11/04/2015  04:27 PM             9,982 README.md
11/11/2015  10:38 AM    <DIR>          Methods_Loops_Addition_Game
               4 File(s)     12,579,955 bytes
               6 Dir(s)  15,405,072,384 bytes free

E:\>cd Methods_Loops_Addition_Game

E:\Methods_Loops_Addition_Game>echo # HW_9_Loop_Game >> README.md

E:\Methods_Loops_Addition_Game>git init
Initialized empty Git repository in E:/Methods_Loops_Addition_Game/.git/

E:\Methods_Loops_Addition_Game>git add README.md

E:\Methods_Loops_Addition_Game>git config user.name "Prasun Thapa"

E:\Methods_Loops_Addition_Game>git config user.email thapap@student.swosu.edu

E:\Methods_Loops_Addition_Game>git commit -m "First commit"
[master (root-commit) 6f92b53] First commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md

E:\Methods_Loops_Addition_Game>git remote add origin https://github.com/prasunth
apa10/HW_9_Loop_Game.git

E:\Methods_Loops_Addition_Game>git push -u origin master
Username for 'https://github.com': prasunthapa10
Password for 'https://prasunthapa10@github.com':
Counting objects: 3, done.
Writing objects: 100% (3/3), 238 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/prasunthapa10/HW_9_Loop_Game.git
 * [new branch]      master -> master
Branch master set up to track remote branch master from origin.

E:\Methods_Loops_Addition_Game>git add .

E:\Methods_Loops_Addition_Game>git commit -m "Some codes"
[master 5f8e2d3] Some codes
 4 files changed, 96 insertions(+)
 create mode 100644 .classpath
 create mode 100644 .project
 create mode 100644 bin/Loop_Game.class
 create mode 100644 src/Loop_Game.java

E:\Methods_Loops_Addition_Game>git push
warning: push.default is unset; its implicit value has changed in
Git 2.0 from 'matching' to 'simple'. To squelch this message
and maintain the traditional behavior, use:

  git config --global push.default matching

To squelch this message and adopt the new behavior now, use:

  git config --global push.default simple

When push.default is set to 'matching', git will push local branches
to the remote branches that already exist with the same name.

Since Git 2.0, Git defaults to the more conservative 'simple'
behavior, which only pushes the current branch to the corresponding
remote branch that 'git pull' uses to update the current branch.

See 'git help config' and search for 'push.default' for further information.
(the 'simple' mode was introduced in Git 1.7.11. Use the similar mode
'current' instead of 'simple' if you sometimes use older versions of Git)

Username for 'https://github.com': prasunthapa10
Password for 'https://prasunthapa10@github.com':
Counting objects: 8, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (6/6), done.
Writing objects: 100% (8/8), 2.83 KiB | 0 bytes/s, done.
Total 8 (delta 0), reused 0 (delta 0)
To https://github.com/prasunthapa10/HW_9_Loop_Game.git
   6f92b53..5f8e2d3  master -> master

E:\Methods_Loops_Addition_Game>
