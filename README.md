# test4
第一次上传仓库
# 视频最后我所说的遇到的问题解决
1.git报错：'fatal:remote origin already exists'怎么处理？附上git常用操作以及说明。
https://www.cnblogs.com/leaf930814/p/6664706.html

2.git错误 error: failed to push some refs to 'https://github.com/...
https://blog.csdn.net/qq_30152625/article/details/90404727

********************************************************************************************************************************
运行的一些过程，可以忽略，具体应该很快就学会了，遇到错误调错百度就好

























24302@DESKTOP-8DP6U4C MINGW64 /d/C++_learning/test4 (master)
$ git add 20200705github.docx

24302@DESKTOP-8DP6U4C MINGW64 /d/C++_learning/test4 (master)
$ git commit -m "如何上传本地文件到git-hub上"
On branch master
Untracked files:
        few_shot_classification_on_graphs_with_structural_regularized_
        learn1.txt

nothing added to commit but untracked files present

24302@DESKTOP-8DP6U4C MINGW64 /d/C++_learning/test4 (master)
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        few_shot_classification_on_graphs_with_structural_regularized_
        learn1.txt

nothing added to commit but untracked files present (use "git add" to

24302@DESKTOP-8DP6U4C MINGW64 /d/C++_learning/test4 (master)
$ git remote add origin https://github.com/zhang-wei-wei/test4.git
fatal: remote origin already exists.

24302@DESKTOP-8DP6U4C MINGW64 /d/C++_learning/test4 (master)
$ git push -u origin master
To github.com:zhang-wei-wei/test4.git
 ! [rejected]        master -> master (fetch first)
error: failed to push some refs to 'git@github.com:zhang-wei-wei/test4
hint: Updates were rejected because the remote contains work that you
hint: not have locally. This is usually caused by another repository p
hint: to the same ref. You may want to first integrate the remote chan
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for deta

24302@DESKTOP-8DP6U4C MINGW64 /d/C++_learning/test4 (master)
$ git push --help

24302@DESKTOP-8DP6U4C MINGW64 /d/C++_learning/test4 (master)
$ git remote rm origin

24302@DESKTOP-8DP6U4C MINGW64 /d/C++_learning/test4 (master)
$ git push -u origin master
fatal: 'origin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

24302@DESKTOP-8DP6U4C MINGW64 /d/C++_learning/test4 (master)
$ git remote rm origin
fatal: No such remote: 'origin'

24302@DESKTOP-8DP6U4C MINGW64 /d/C++_learning/test4 (master)
$ git remote add origin https://github.com/zhang-wei-wei/test4.git

24302@DESKTOP-8DP6U4C MINGW64 /d/C++_learning/test4 (master)
$ git push -u origin master
fatal: TaskCanceledException encountered.
   ▒▒ȡ▒▒һ▒▒▒▒▒▒
To https://github.com/zhang-wei-wei/test4.git
 ! [rejected]        master -> master (fetch first)
error: failed to push some refs to 'https://github.com/zhang-wei-wei/test4.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

24302@DESKTOP-8DP6U4C MINGW64 /d/C++_learning/test4 (master)
$ git pull --rebase origin master
warning: no common commits
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.
From https://github.com/zhang-wei-wei/test4
 * branch            master     -> FETCH_HEAD
 * [new branch]      master     -> origin/master
First, rewinding head to replay your work on top of it...
Applying: “如何将文件上传到github

24302@DESKTOP-8DP6U4C MINGW64 /d/C++_learning/test4 (master)
$ git push -u origin master
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 188.65 KiB | 6.74 MiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/zhang-wei-wei/test4.git
   730aa92..f2d6fa5  master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.

24302@DESKTOP-8DP6U4C MINGW64 /d/C++_learning/test4 (master)
$
