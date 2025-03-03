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

```
