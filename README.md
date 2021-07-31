# ForGIT
GIT home works
-----------------------------------------------------
PART1:
Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (main)
$ git checkout -b feature2
Switched to a new branch 'feature2'

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (feature2)
$ git add .

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (feature2)
$ git commit -m "1 line"
[feature2 4ef4ae4] 1 line
 1 file changed, 1 insertion(+)
 create mode 100644 home-work-02.txt

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (feature2)
$ git add .

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (feature2)
$ git commit -m "2 line"
[feature2 c178f50] 2 line
 1 file changed, 2 insertions(+), 1 deletion(-)

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (feature2)
$ git add .

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (feature2)
$ git commit -m "3 line"
[feature2 1757878] 3 line
 1 file changed, 2 insertions(+), 1 deletion(-)

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (feature2)
$ git push --set-upstream origin feature2

Enumerating objects: 10, done.
Counting objects: 100% (10/10), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (9/9), 734 bytes | 244.00 KiB/s, done.
Total 9 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), done.
remote:
remote: Create a pull request for 'feature2' on GitHub by visiting:
remote:      https://github.com/AlexShten/ForGIT/pull/new/feature2
remote:
To https://github.com/AlexShten/ForGIT.git
 * [new branch]      feature2 -> feature2
Branch 'feature2' set up to track remote branch 'feature2' from 'origin'.

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (feature2)
$ git log --oneline --decorate --graph --all
* 1757878 (HEAD -> feature2, origin/feature2) 3 line
* c178f50 2 line
* 4ef4ae4 1 line
*   a61edeb (origin/main, origin/HEAD, main) merge with fix
|\
| * fc82864 (origin/feature1, feature1) feature1
* | 393eae1 Update home-work-01.txt
|/
* 462148e add new file
* b7618ec Initial commit

-----------------------------------------------------
PART2:
Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (feature2)
$ git reset 4ef4ae4
Unstaged changes after reset:
M       home-work-02.txt

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (feature2)
$ git log --oneline --decorate --graph --all
* 1757878 (origin/feature2) 3 line
* c178f50 2 line
* 4ef4ae4 (HEAD -> feature2) 1 line
*   a61edeb (origin/main, origin/HEAD, main) merge with fix
|\
| * fc82864 (origin/feature1, feature1) feature1
* | 393eae1 Update home-work-01.txt
|/
* 462148e add new file
* b7618ec Initial commit

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (feature2)
$ git add .

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (feature2)
$ git commit --amend
Error in /etc/nanorc on line 237: Error expanding /usr/share/nano/*.nanorc: No such file or directory
[feature2 f509500] (amend)1 line
 Date: Sat Jul 31 15:33:49 2021 +0300
 1 file changed, 3 insertions(+)
 create mode 100644 home-work-02.txt

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (feature2)
$ git log --oneline --decorate --graph --all
* f509500 (HEAD -> feature2) (amend)1 line
| * 1757878 (origin/feature2) 3 line
| * c178f50 2 line
| * 4ef4ae4 1 line
|/
*   a61edeb (origin/main, origin/HEAD, main) merge with fix
|\
| * fc82864 (origin/feature1, feature1) feature1
* | 393eae1 Update home-work-01.txt
|/
* 462148e add new file
* b7618ec Initial commit


Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (feature2)
$ git push --force
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 335 bytes | 167.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/AlexShten/ForGIT.git
 + 1757878...f509500 feature2 -> feature2 (forced update)

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (feature2)
$ git log --oneline --decorate --graph --all
* f509500 (HEAD -> feature2, origin/feature2) (amend)1 line
*   a61edeb (origin/main, origin/HEAD, main) merge with fix
|\
| * fc82864 (origin/feature1, feature1) feature1
* | 393eae1 Update home-work-01.txt
|/
* 462148e add new file
* b7618ec Initial commit

-----------------------------------------------------
PART3:
Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (feature2)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (main)
$ git add .

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (main)
$ git commit -m "changes in main"
[main e9c6483] changes in main
 1 file changed, 1 insertion(+), 1 deletion(-)

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 331 bytes | 165.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/AlexShten/ForGIT.git
   a61edeb..e9c6483  main -> main

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (main)
$ git checkout feature2
Switched to branch 'feature2'
Your branch is up to date with 'origin/feature2'.

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (feature2)
$ git add .

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (feature2)
$ git commit -m "changes in feature"
[feature2 6cf1eaf] changes in feature
 1 file changed, 1 insertion(+), 1 deletion(-)

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (feature2)
$ git  push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 302 bytes | 302.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/AlexShten/ForGIT.git
   f509500..6cf1eaf  feature2 -> feature2

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (feature2)
$ git log --oneline --decorate --graph --all
* 6cf1eaf (HEAD -> feature2, origin/feature2) changes in feature
* f509500 (amend)1 line
| * e9c6483 (origin/main, origin/HEAD, main) changes in main
|/
*   a61edeb merge with fix
|\
| * fc82864 (origin/feature1, feature1) feature1
* | 393eae1 Update home-work-01.txt
|/
* 462148e add new file
* b7618ec Initial commit

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (feature2)
$ git rebase main
error: could not apply 6cf1eaf... changes in feature
Resolve all conflicts manually, mark them as resolved with
"git add/rm <conflicted_files>", then run "git rebase --continue".
You can instead skip this commit: run "git rebase --skip".
To abort and get back to the state before "git rebase", run "git rebase --abort".
Could not apply 6cf1eaf... changes in feature
Auto-merging home-work-01.txt
CONFLICT (content): Merge conflict in home-work-01.txt

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (feature2|REBASE 2/2)
$ git add .

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (feature2|REBASE 2/2)
$ git commit -m "after fix"
[detached HEAD 6b489ba] after fix
 1 file changed, 3 insertions(+), 1 deletion(-)

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (feature2|REBASE 2/2)
$ git rebase --continue
Successfully rebased and updated refs/heads/feature2.

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (feature2)
$ git push --force
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (6/6), 584 bytes | 194.00 KiB/s, done.
Total 6 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/AlexShten/ForGIT.git
 + 6cf1eaf...6b489ba feature2 -> feature2 (forced update)

Alex@AlexPC MINGW64 ~/Desktop/HWGIT/ForGIT (feature2)
$ git log --oneline --decorate --graph --all
* 6b489ba (HEAD -> feature2, origin/feature2) after fix
* 89c4bc5 (amend)1 line
* e9c6483 (origin/main, origin/HEAD, main) changes in main
*   a61edeb merge with fix
|\
| * fc82864 (origin/feature1, feature1) feature1
* | 393eae1 Update home-work-01.txt
|/
* 462148e add new file
* b7618ec Initial commit


