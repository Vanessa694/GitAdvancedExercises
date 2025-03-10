# git exercises
## part1
### challenge1 
```bash
USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ touch test{1..4}.md

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git add test1.md

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git commit -m "chore: Create initial file"
[main 8b11782] chore: Create initial file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test1.md

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git add test2.md

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git commit -m "chore:  create another file"
[main 3b8821e] chore:  create another file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test2.md

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git add test3.md

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git commit -m "chore:  create third and fourth files"
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test4.md

nothing added to commit but untracked files present (use "git add" to track)

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test4.md

nothing added to commit but untracked files present (use "git add" to track)

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git log
commit 3b8821e84714f2cb08e162a6fa7b61b5ad855d27 (HEAD -> main)
Author: Vanessa Gatete <gatevanessa86@gmail.com>
Date:   Mon Mar 3 11:25:43 2025 +0200

    chore:  create another file

commit 8b11782a44d561b38610c90fd2b15c647601bb05
Author: Vanessa Gatete <gatevanessa86@gmail.com>
Date:   Mon Mar 3 11:25:30 2025 +0200

    chore: Create initial file

commit 3cc7dac7b1b25b514aafb1e84441b73a6bbbf846
Author: Vanessa Gatete <gatevanessa86@gmail.com>
Date:   Mon Mar 3 11:23:19 2025 +0200

    chore:  create another file

commit 59b135bcca77803fe0dad2b64a71cdf8b224ac41
Author: Vanessa Gatete <gatevanessa86@gmail.com>
Date:   Mon Mar 3 11:22:37 2025 +0200

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git add test4.md

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git commit -m "chore:  create fourth file"
[main 84f372a] chore:  create fourth file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test4.md
 ```
### Challeng2
```bash
USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git rebase -i HEAD~2
[detached HEAD 37f49ac] chore:  create second file
 Date: Mon Mar 3 11:25:43 2025 +0200
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test2.md
Successfully rebased and updated refs/heads/main.

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$
Display all 5098 possibilities? (y or n)
!
./
:
[
[.exe
[[
]]
___git_complete
__git
__git_aliased_command
__git_checkout_default_dwim_mode
__git_complete
__git_complete_command
__git_complete_common
__git_complete_config_variable_name
__git_complete_config_variable_name_and_value
__git_complete_config_variable_value
__git_complete_fetch_refspecs
__git_complete_file
__git_complete_force_with_lease
__git_complete_index_file
__git_complete_log_opts
__git_complete_refs
__git_complete_remote_or_refspec
__git_complete_revlist
__git_complete_revlist_file
__git_complete_strategy
__git_complete_symbol
__git_complete_worktree_paths
__git_compute_all_commands
__git_compute_config_sections
__git_compute_config_vars
__git_compute_config_vars_all
__git_compute_first_level_config_vars_for_section
__git_compute_merge_strategies
__git_compute_second_level_config_vars_for_section
__git_config_get_set_variables
__git_count_arguments
__git_dequote
__git_dwim_remote_heads
__git_eread
__git_find_last_on_cmdline
__git_find_on_cmdline
__git_find_repo_path
__git_find_subcommand
__git_func_wrap
__git_get_config_variables
__git_get_option_value
__git_has_doubledash
__git_have_func
__git_heads
__git_index_files
__git_is_configured_remote
__git_list_merge_strategies
__git_ls_files_helper
__git_main
__git_match_ctag
```
### challenge3
```bash
USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git rebase -i HEAD~3
[detached HEAD babfe62] chore: Create initial file
 Date: Mon Mar 3 11:25:30 2025 +0200
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test1.md
 create mode 100644 test2.md
Successfully rebased and updated refs/heads/main.
```
### challenge4
```bash
USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git log
commit 8e6d243edb42d3451ee8753d0a6bfbd54e6c6fa7 (HEAD -> main)
Author: Vanessa Gatete <gatevanessa86@gmail.com>
Date:   Mon Mar 3 11:30:59 2025 +0200

    chore:  create fourth file

commit babfe6293238d7fd5bc5cbe1137ad359de7c0fc6
Author: Vanessa Gatete <gatevanessa86@gmail.com>
Date:   Mon Mar 3 11:25:30 2025 +0200

    chore: Create initial file

    chore:  create second file

commit 3cc7dac7b1b25b514aafb1e84441b73a6bbbf846
Author: Vanessa Gatete <gatevanessa86@gmail.com>
Date:   Mon Mar 3 11:23:19 2025 +0200

    chore:  create another file

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git reset

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git reset HEAD^

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git add test3.md

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git commit -m "Create Third File"
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme.md
        test4.md

nothing added to commit but untracked files present (use "git add" to track)

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git add test4.md

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git commit -m "Create fourth File"
[main 57071f6] Create fourth File
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test4.md

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git log
commit 57071f6f5b5c05a0c720838f9dcc984cbcf8c3bd (HEAD -> main)
Author: Vanessa Gatete <gatevanessa86@gmail.com>
Date:   Mon Mar 3 14:14:37 2025 +0200

    Create fourth File

commit babfe6293238d7fd5bc5cbe1137ad359de7c0fc6
Author: Vanessa Gatete <gatevanessa86@gmail.com>
Date:   Mon Mar 3 11:25:30 2025 +0200

    chore: Create initial file

    chore:  create second file

commit 3cc7dac7b1b25b514aafb1e84441b73a6bbbf846
Author: Vanessa Gatete <gatevanessa86@gmail.com>
Date:   Mon Mar 3 11:23:19 2025 +0200

    chore:  create another file
:
```
### challenge5
```bash
USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git log --oneline
5ffcd14 (HEAD -> main) Unwanted commit
6c73f9f (origin/main) Add readme.md
b394919 Create fourth File
babfe62 chore: Create initial file
3cc7dac chore:  create another file
59b135b chore: Create initial file
c1fc39e chore: Create create another file
2940878 (master) chore: Create initial file
aac3fd8 chore: Create initial file
...skipping...
5ffcd14 (HEAD -> main) Unwanted commit
6c73f9f (origin/main) Add readme.md
b394919 Create fourth File
babfe62 chore: Create initial file
3cc7dac chore:  create another file
59b135b chore: Create initial file
c1fc39e chore: Create create another file
2940878 (master) chore: Create initial file
aac3fd8 chore: Create initial file

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git rebase -i HEAD~1
error: cannot rebase: You have unstaged changes.
error: Please commit or stash them.

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git add unwanted.txt

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git commit -m "Unwanted commit"
[main 65f8830] Unwanted commit
 1 file changed, 1 insertion(+)

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git rebase -i HEAD~1
Successfully rebased and updated refs/heads/main.

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git log --oneline
5ffcd14 (HEAD -> main) Unwanted commit
6c73f9f (origin/main) Add readme.md
b394919 Create fourth File
babfe62 chore: Create initial file
3cc7dac chore:  create another file
59b135b chore: Create initial file
c1fc39e chore: Create create another file
2940878 (master) chore: Create initial file
aac3fd8 chore: Create initial file

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git rebase -i HEAD~3
Successfully rebased and updated refs/heads/main.
```
### Challenge 6
```bash
USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git add unwanted.txt

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git commit -m "Unwanted commit"
[main 65f8830] Unwanted commit
 1 file changed, 1 insertion(+)
```
### challenge 7
```bash
USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git log --oneline
5ffcd14 (HEAD -> main) Unwanted commit
6c73f9f (origin/main) Add readme.md
b394919 Create fourth File
babfe62 chore: Create initial file
3cc7dac chore:  create another file
59b135b chore: Create initial file
c1fc39e chore: Create create another file
2940878 (master) chore: Create initial file
aac3fd8 chore: Create initial file

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git rebase -i HEAD~3
Successfully rebased and updated refs/heads/main.
```
### challenge 8
```bash
USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git checkout -b ft/branch
Switched to a new branch 'ft/branch'

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (ft/branch)
$ touch test5.md

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (ft/branch)
$ echo "Test file 5 content" > test5.md

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (ft/branch)
$ git add test5.m
fatal: pathspec 'test5.m' did not match any files

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (ft/branch)
$ git add test5.md

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (ft/branch)
$ git commit -m "Implemented test 5"
[ft/branch c139841] Implemented test 5
 1 file changed, 1 insertion(+)
 create mode 100644 test5.md

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (ft/branch)
$ git checkout main
Switched to branch 'main'

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git log --oneline
0fd9a1f (HEAD -> main) Add readme.md
d65d834 Create fourth File
159727b Unwanted commit
babfe62 chore: Create initial file
3cc7dac chore:  create another file
59b135b chore: Create initial file
c1fc39e chore: Create create another file
2940878 (master) chore: Create initial file
aac3fd8 chore: Create initial file

USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git cherry-pick a1b2c3
fatal: bad revision 'a1b2c3'

```
### challenge 9
```bash
USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git log --graph
* commit 19ddd0ff61e7bcefb3082ee40b0924223451190e (HEAD -> main)
| Author: Vanessa Gatete <gatevanessa86@gmail.com>
| Date:   Thu Mar 6 15:44:11 2025 +0200
|
|     Implemented test 5
|
* commit 0fd9a1f4d893e47bebba9b408e1827435c02e556
| Author: Vanessa Gatete <gatevanessa86@gmail.com>
| Date:   Mon Mar 3 15:25:10 2025 +0200

```
### challenge 10
```bash
USER@DESKTOP-LNUFN1R MINGW64 ~/Documents/GitAdvancedExercises (main)
$ git reflog
19ddd0f (HEAD -> main) HEAD@{0}: cherry-pick: Implemented test 5
0fd9a1f HEAD@{1}: checkout: moving from ft/branch to main
c139841 (ft/branch) HEAD@{2}: checkout: moving from main to ft/branch
0fd9a1f HEAD@{3}: checkout: moving from ft/branch to main
c139841 (ft/branch) HEAD@{4}: commit: Implemented test 5
0fd9a1f HEAD@{5}: checkout: moving from main to ft/branch
0fd9a1f HEAD@{6}: rebase (finish): returning to refs/heads/main
0fd9a1f HEAD@{7}: rebase (pick): Add readme.md
d65d834 HEAD@{8}: rebase (pick): Create fourth File
:...skipping...
159727b HEAD@{9}: rebase (pick): Unwanted commit
babfe62 HEAD@{10}: rebase (start): checkout HEAD~3
:...skipping...
19ddd0f (HEAD -> main) HEAD@{0}: cherry-pick: Implemented test 5
0fd9a1f HEAD@{1}: checkout: moving from ft/branch to main
c139841 (ft/branch) HEAD@{2}: checkout: moving from main to ft/branch
0fd9a1f HEAD@{3}: checkout: moving from ft/branch to main
c139841 (ft/branch) HEAD@{4}: commit: Implemented test 5
0fd9a1f HEAD@{5}: checkout: moving from main to ft/branch
0fd9a1f HEAD@{6}: rebase (finish): returning to refs/heads/main
d65d834 HEAD@{8}: rebase (pick): Create fourth File
159727b HEAD@{9}: rebase (pick): Unwanted commit
babfe62 HEAD@{10}: rebase (start): checkout HEAD~3
5ffcd14 HEAD@{11}: rebase (finish): returning to refs/heads/main
5ffcd14 HEAD@{12}: rebase (start): checkout HEAD~1
65f8830 HEAD@{13}: commit: Unwanted commit
5ffcd14 HEAD@{14}: commit: Unwanted commit
6c73f9f (origin/main) HEAD@{15}: rebase (finish): returning to refs/heads/main
6c73f9f (origin/main) HEAD@{16}: rebase (start): checkout HEAD~3
:...skipping...
19ddd0f (HEAD -> main) HEAD@{0}: cherry-pick: Implemented test 5
0fd9a1f HEAD@{1}: checkout: moving from ft/branch to main
c139841 (ft/branch) HEAD@{2}: checkout: moving from main to ft/branch
0fd9a1f HEAD@{3}: checkout: moving from ft/branch to main
c139841 (ft/branch) HEAD@{4}: commit: Implemented test 5
0fd9a1f HEAD@{5}: checkout: moving from main to ft/branch
0fd9a1f HEAD@{6}: rebase (finish): returning to refs/heads/main
0fd9a1f HEAD@{7}: rebase (pick): Add readme.md
159727b HEAD@{9}: rebase (pick): Unwanted commit
babfe62 HEAD@{10}: rebase (start): checkout HEAD~3
5ffcd14 HEAD@{11}: rebase (finish): returning to refs/heads/main
5ffcd14 HEAD@{12}: rebase (start): checkout HEAD~1
65f8830 HEAD@{13}: commit: Unwanted commit
5ffcd14 HEAD@{14}: commit: Unwanted commit
6c73f9f (origin/main) HEAD@{15}: rebase (finish): returning to refs/heads/main
6c73f9f (origin/main) HEAD@{16}: rebase (start): checkout HEAD~3
6c73f9f (origin/main) HEAD@{17}: rebase (finish): returning to refs/heads/main
6c73f9f (origin/main) HEAD@{18}: rebase (start): checkout HEAD~2
6c73f9f (origin/main) HEAD@{19}: commit: Add readme.md
b394919 HEAD@{20}: reset: moving to b394919
7c1921a HEAD@{21}: commit: Create fourth File
:...skipping...
19ddd0f (HEAD -> main) HEAD@{0}: cherry-pick: Implemented test 5
0fd9a1f HEAD@{1}: checkout: moving from ft/branch to main
c139841 (ft/branch) HEAD@{2}: checkout: moving from main to ft/branch
0fd9a1f HEAD@{3}: checkout: moving from ft/branch to main
c139841 (ft/branch) HEAD@{4}: commit: Implemented test 5
0fd9a1f HEAD@{5}: checkout: moving from main to ft/branch
0fd9a1f HEAD@{6}: rebase (finish): returning to refs/heads/main
0fd9a1f HEAD@{7}: rebase (pick): Add readme.md
d65d834 HEAD@{8}: rebase (pick): Create fourth File
159727b HEAD@{9}: rebase (pick): Unwanted commit
babfe62 HEAD@{10}: rebase (start): checkout HEAD~3
5ffcd14 HEAD@{11}: rebase (finish): returning to refs/heads/main
5ffcd14 HEAD@{12}: rebase (start): checkout HEAD~1
65f8830 HEAD@{13}: commit: Unwanted commit
5ffcd14 HEAD@{14}: commit: Unwanted commit
6c73f9f (origin/main) HEAD@{15}: rebase (finish): returning to refs/heads/main
6c73f9f (origin/main) HEAD@{16}: rebase (start): checkout HEAD~3
6c73f9f (origin/main) HEAD@{17}: rebase (finish): returning to refs/heads/main
6c73f9f (origin/main) HEAD@{18}: rebase (start): checkout HEAD~2
6c73f9f (origin/main) HEAD@{19}: commit: Add readme.md
b394919 HEAD@{20}: reset: moving to b394919
7c1921a HEAD@{21}: commit: Create fourth File
eec6e52 HEAD@{22}: commit: Create third File
:...skipping...
19ddd0f (HEAD -> main) HEAD@{0}: cherry-pick: Implemented test 5
0fd9a1f HEAD@{1}: checkout: moving from ft/branch to main
c139841 (ft/branch) HEAD@{2}: checkout: moving from main to ft/branch
0fd9a1f HEAD@{3}: checkout: moving from ft/branch to main
c139841 (ft/branch) HEAD@{4}: commit: Implemented test 5
0fd9a1f HEAD@{5}: checkout: moving from main to ft/branch
0fd9a1f HEAD@{6}: rebase (finish): returning to refs/heads/main
0fd9a1f HEAD@{7}: rebase (pick): Add readme.md
d65d834 HEAD@{8}: rebase (pick): Create fourth File
159727b HEAD@{9}: rebase (pick): Unwanted commit
babfe62 HEAD@{10}: rebase (start): checkout HEAD~3
5ffcd14 HEAD@{11}: rebase (finish): returning to refs/heads/main
5ffcd14 HEAD@{12}: rebase (start): checkout HEAD~1
65f8830 HEAD@{13}: commit: Unwanted commit
5ffcd14 HEAD@{14}: commit: Unwanted commit
6c73f9f (origin/main) HEAD@{15}: rebase (finish): returning to refs/heads/main
6c73f9f (origin/main) HEAD@{16}: rebase (start): checkout HEAD~3
6c73f9f (origin/main) HEAD@{17}: rebase (finish): returning to refs/heads/main
6c73f9f (origin/main) HEAD@{18}: rebase (start): checkout HEAD~2
6c73f9f (origin/main) HEAD@{19}: commit: Add readme.md
b394919 HEAD@{20}: reset: moving to b394919
7c1921a HEAD@{21}: commit: Create fourth File
eec6e52 HEAD@{22}: commit: Create third File
aac3fd8 HEAD@{23}: reset: moving to HEAD~1
```
## part2
### challenge1
```bash
PS C:\Users\USER\Documents\GitAdvancedExercises> git branch ft/new-feature
>>
PS C:\Users\USER\Documents\GitAdvancedExercises> git checkout ft/new-feature
>>
M       readme.md
Switched to branch 'ft/new-feature'
```
### challenge 2
```bash
PS C:\Users\USER\Documents\GitAdvancedExercises> echo "This is the core functionality for the new feature." > feature.txt
>>
PS C:\Users\USER\Documents\GitAdvancedExercises> git add feature.txt
>>
PS C:\Users\USER\Documents\GitAdvancedExercises> git commit -m "Implemented core functionality for new feature"
>>
[ft/new-feature 626e16e] Implemented core functionality for new feature
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 feature.txt
PS C:\Users\USER\Documents\GitAdvancedExercises> git log --oneline
>>
626e16e (HEAD -> ft/new-feature) Implemented core functionality for new feature
10d9056 (origin/main, main) Added some challenges
61d633f Implemented test 5
514f9a0 Unwanted commit
6c73f9f Add readme.md
b394919 Create fourth File
babfe62 chore: Create initial file
3cc7dac chore:  create another file
59b135b chore: Create initial file
c1fc39e chore: Create create another file
2940878 (master) chore: Create initial file
aac3fd8 chore: Create initial file
PS C:\Users\USER\Documents\GitAdvancedExercises> 
```
### challenge 3
```bash
PS C:\Users\USER\Documents\GitAdvancedExercises> git checkout main
>>
M       readme.md
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\USER\Documents\GitAdvancedExercises> echo "This project implements various features for better functionality." > readme.txt
>>
PS C:\Users\USER\Documents\GitAdvancedExercises> git add readme.txt
>>
PS C:\Users\USER\Documents\GitAdvancedExercises> git commit -m "Updated project readme"
>>
[main 74344f7] Updated project readme
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 readme.txt
PS C:\Users\USER\Documents\GitAdvancedExercises> 
```
### challenge 4
```bash
PS C:\Users\USER\Documents\GitAdvancedExercises> git merge ft/new-feature
>>
Merge made by the 'ort' strategy.
 feature.txt | Bin 0 -> 108 bytes
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 feature.txt
```
### challenge 5
```bash
PS C:\Users\USER\Documents\GitAdvancedExercises> git branch -d ft/new-feature
>> 
Deleted branch ft/new-feature (was 626e16e).
PS C:\Users\USER\Documents\GitAdvancedExercises> 
```
### challenge 6
```bash
PS C:\Users\USER\Documents\GitAdvancedExercises> git log --oneline
>>
b842b79 (HEAD -> main) Merge branch 'ft/new-feature'
74344f7 Updated project readme
626e16e Implemented core functionality for new feature
10d9056 (origin/main) Added some challenges
61d633f Implemented test 5
514f9a0 Unwanted commit
6c73f9f Add readme.md
b394919 Create fourth File
babfe62 chore: Create initial file
3cc7dac chore:  create another file
59b135b chore: Create initial file
c1fc39e chore: Create create another file
2940878 (master) chore: Create initial file
PS C:\Users\USER\Documents\GitAdvancedExercises> git checkout -b ft/new-branch-from-commit 626e16e
>>
M       readme.md
Switched to a new branch 'ft/new-branch-from-commit'
PS C:\Users\USER\Documents\GitAdvancedExercises> 
```
### challenge 7
```bash
PS C:\Users\USER\Documents\GitAdvancedExercises> git checkout main
>>
M       readme.md
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)
PS C:\Users\USER\Documents\GitAdvancedExercises> git merge ft/new-branch-from-commit
>>
Already up to date.
PS C:\Users\USER\Documents\GitAdvancedExercises> git status
>>
On branch main
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   readme.md

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\USER\Documents\GitAdvancedExercises> git add readme.md
>>
PS C:\Users\USER\Documents\GitAdvancedExercises> git merge ft/new-branch-from-commit
>> 
Already up to date.
PS C:\Users\USER\Documents\GitAdvancedExercises> git status       
>> 
On branch main
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   readme.md

PS C:\Users\USER\Documents\GitAdvancedExercises> git commit -m "Merged ft/new-branch-from-commit into main"
>> 
[main bcde941] Merged ft/new-branch-from-commit into main
 1 file changed, 107 insertions(+)
PS C:\Users\USER\Documents\GitAdvancedExercises>
```
### challenge 8
```bash
PS C:\Users\USER\Documents\GitAdvancedExercises> git checkout ft/new-branch-from-commit
>>
error: Your local changes to the following files would be overwritten by checkout:
        readme.md
Please commit your changes or stash them before you switch branches.
Aborting
PS C:\Users\USER\Documents\GitAdvancedExercises> git add readme.md
>>
PS C:\Users\USER\Documents\GitAdvancedExercises> git commit -m "Updated readme.md before rebasing"
>>
[main 04a4129] Updated readme.md before rebasing
 1 file changed, 41 insertions(+)
PS C:\Users\USER\Documents\GitAdvancedExercises> git checkout ft/new-branch-from-commit
>>
Switched to branch 'ft/new-branch-from-commit'
PS C:\Users\USER\Documents\GitAdvancedExercises> git rebase main
>>
Successfully rebased and updated refs/heads/ft/new-branch-from-commit.
```
### challenge 9
```bash
PS C:\Users\USER\Documents\GitAdvancedExercises> git checkout ft/new-branch-from-commit
>>
M       readme.md
Already on 'ft/new-branch-from-commit'
PS C:\Users\USER\Documents\GitAdvancedExercises> git branch -m ft/improved-branch-name
>>
PS C:\Users\USER\Documents\GitAdvancedExercises> git branch
>>
  ft/branch
* ft/improved-branch-name
  main
  master
```
### challenge 10
```bash
PS C:\Users\USER\Documents\GitAdvancedExercises> git checkout bcde941
>>
Note: switching to 'bcde941'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at bcde941 Merged ft/new-branch-from-commit into main
PS C:\Users\USER\Documents\GitAdvancedExercises> git checkout main
>>      
error: Your local changes to the following files would be overwritten by checkout:
        readme.md
Please commit your changes or stash them before you switch branches.
Aborting
PS C:\Users\USER\Documents\GitAdvancedExercises> git add readme.md
>>      
PS C:\Users\USER\Documents\GitAdvancedExercises> git commit -m "Updated readme.md before checking out a specific commit"
>>
[detached HEAD df73ca2] Updated readme.md before checking out a specific commit
 1 file changed, 54 insertions(+)
```
## part 3
### challenge 1
```bash
PS C:\Users\USER\Documents\GitAdvancedExercises> git stash
>>
No local changes to save
PS C:\Users\USER\Documents\GitAdvancedExercises> git status
>>
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
PS C:\Users\USER\Documents\GitAdvancedExercises> git stash list
>>
PS C:\Users\USER\Documents\GitAdvancedExercises> 
```
### challenge 2
```bash
PS C:\Users\USER\Documents\GitAdvancedExercises> git stash pop
>>
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   readme.md

no changes added to commit (use "git add" and/or "git commit -a")
Dropped refs/stash@{0} (7e4699ef54d37eb678024515c6159399ed068125)
PS C:\Users\USER\Documents\GitAdvancedExercises> 
```
### challenge 3

```bash
PS C:\Users\USER\Documents\GitAdvancedExercises> git checkout -b feature-branch
>>
Switched to a new branch 'feature-branch'
PS C:\Users\USER\Documents\GitAdvancedExercises> nano README.md
>>
nano : The term 'nano' is not recognized as the name of a cmdlet, function, script file, or operable program. 
Check the spelling of the name, or if a path was included, verify that the path is correct and try again.       
At line:1 char:1
+ nano README.md
+ ~~~~
    + CategoryInfo          : ObjectNotFound: (nano:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException

PS C:\Users\USER\Documents\GitAdvancedExercises> code README.md                          
>> 
PS C:\Users\USER\Documents\GitAdvancedExercises> git checkout feature-branch   
>> 
M       readme.md
Already on 'feature-branch'
PS C:\Users\USER\Documents\GitAdvancedExercises> code README.md
>> 
PS C:\Users\USER\Documents\GitAdvancedExercises> code readme.md
>> 
PS C:\Users\USER\Documents\GitAdvancedExercises> git checkout main          
M       readme.md
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\USER\Documents\GitAdvancedExercises> git checkout -b feature-branch
>> 
fatal: a branch named 'feature-branch' already exists
PS C:\Users\USER\Documents\GitAdvancedExercises> git add heyyyy.md 
PS C:\Users\USER\Documents\GitAdvancedExercises> git commit -m "Modified heyyyy.md in feature branch"
[main 338e214] Modified heyyyy.md in feature branch
 1 file changed, 1 insertion(+)
 create mode 100644 heyyyy.md
PS C:\Users\USER\Documents\GitAdvancedExercises> git checkout main
>>
M       readme.md
Already on 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)
PS C:\Users\USER\Documents\GitAdvancedExercises> git add heyyyy.md
PS C:\Users\USER\Documents\GitAdvancedExercises> git commit -m "Modified heyyyy.md in main branch"
[main f72a3c8] Modified heyyyy.md in main branch
 1 file changed, 1 insertion(+), 1 deletion(-)
PS C:\Users\USER\Documents\GitAdvancedExercises> git merge feature-branch
>>
Already up to date.
PS C:\Users\USER\Documents\GitAdvancedExercises> 
```
### challenge 4
```bash
PS C:\Users\USER\Documents\GitAdvancedExercises> git mergetool

This message is displayed because 'merge.tool' is not configured.
See 'git mergetool --tool-help' or 'git help config' for more details.
'git mergetool' will now attempt to use one of the following tools:
tortoisemerge emerge vimdiff nvimdiff
No files need merging
PS C:\Users\USER\Documents\GitAdvancedExercises> 
```
### challenge 5
```bash
PS C:\Users\USER\Documents\GitAdvancedExercises> git checkout f72a3c8      
M       readme.md
Note: switching to 'f72a3c8'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at f72a3c8 Modified heyyyy.md in main branch
PS C:\Users\USER\Documents\GitAdvancedExercises> 
```
### challenge 6
```bash
PS C:\Users\USER\Documents\GitAdvancedExercises> New-Item -ItemType File -Name .gitignore
>>


    Directory: C:\Users\USER\Documents\GitAdvancedExercises


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----         3/10/2025   7:20 PM              0 .gitignore


PS C:\Users\USER\Documents\GitAdvancedExercises> notepad .gitignore
>>
PS C:\Users\USER\Documents\GitAdvancedExercises> /tmp
>>
/tmp : The term '/tmp' is not recognized as the name of a cmdlet, function, script file, or operable program. 
Check the spelling of the name, or if a path was included, verify that the path is correct and try again.       
At line:1 char:1
+ /tmp
+ ~~~~
    + CategoryInfo          : ObjectNotFound: (/tmp:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException

PS C:\Users\USER\Documents\GitAdvancedExercises> git status
>>
HEAD detached at f72a3c8
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   readme.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\USER\Documents\GitAdvancedExercises> 
```
### challenge 7
```bash
PS C:\Users\USER\Documents\GitAdvancedExercises> git checkout main   
M       readme.md
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)
PS C:\Users\USER\Documents\GitAdvancedExercises> git tag v1.0
PS C:\Users\USER\Documents\GitAdvancedExercises> 
```
### challenge 8
```bash
PS C:\Users\USER\Documents\GitAdvancedExercises> git tag 
v1.0
PS C:\Users\USER\Documents\GitAdvancedExercises> git tag -d v1.0
Deleted tag 'v1.0' (was f72a3c8)
PS C:\Users\USER\Documents\GitAdvancedExercises>
```
### challenge 9
```bash
PS C:\Users\USER\Documents\GitAdvancedExercises> git push origin main
>>
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (6/6), 614 bytes | 102.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
To https://github.com/Vanessa694/GitAdvancedExercises
   8445766..f72a3c8  main -> main
PS C:\Users\USER\Documents\GitAdvancedExercises> 
```
### challenge 10
```bash
PS C:\Users\USER\Documents\GitAdvancedExercises> git pull origin main
>>
From https://github.com/Vanessa694/GitAdvancedExercises
 * branch            main       -> FETCH_HEAD
Already up to date.
PS C:\Users\USER\Documents\GitAdvancedExercises> 
```





