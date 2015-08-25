# Awesome git addons [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated list of addons that extends git.

Inspired by the [awesome](https://github.com/sindresorhus/awesome) list thing.


## Table of Contents

- [Git Extras](#git-extras)


## [Git Extras](https://github.com/tj/git-extras) - Little git extras.

### squash

```
$ git squash fixed-cursor-styling "Fixed cursor styling"
$ git squash 95b7c52
$ git squash HEAD~3
```

### summary

```
$ git summary

 project  : git
 repo age : 10 years
 active   : 11868 days
 commits  : 40530
 files    : 2825
 authors  :
 15401	Junio C Hamano                  38.0%
  1844	Jeff King                       4.5%
```

### line-summary

```
$ git line-summary

 project  : gulp
 lines    : 3900
 authors  :
 1040 Contra                    26.7%
  828 Sindre Sorhus             21.2%
```

### effort

```
$ git effort

  file                                          commits    active days

  .gitattributes............................... 3          3
  .gitignore................................... 265        226
  .mailmap..................................... 47         40
```

### authors

```
$ git authors
Contra <contra@maricopa.edu>
Eric Schoffstall <contra@wearefractal.com>
Sindre Sorhus <sindresorhus@gmail.com>
```

### changelog

```
$ git changelog
## 3.9.0

- add babel support
- add transpiler fallback support
- add support for some renamed transpilers (livescript, etc)
- add JSCS
- update dependecies (liftoff, interpret)
- documentation tweaks

## 3.8.11

- fix node 0.12/iojs problems
- add node 0.12 and iojs to travis
- update dependencies (liftoff, v8flags)
- documentation tweaks
```

### commits-since

```
$ git commits-since yesterday
... changes since yesterday
TJ Holowaychuk - Fixed readme
```

### count

```
$ git count
total 855
```

### create-branch

```
$ git create-branch development
```

### delete-branch

```
$ git delete-branch integration
```

### delete-submodule

```
$ git delete-submodule lib/foo
```

### delete-tag

```
$ git delete-tag 0.0.1
```

### delete-merged-branches

```
$ git delete-merged-branches
Deleted feature/themes (was c029ab3).
Deleted feature/live_preview (was a81b002).
Deleted feature/dashboard (was 923befa).
```

### fresh-branch

```
$ git fresh-branch docs
```

### guilt

```
$ git guilt `git log --until="3 weeks ago" --format="%H" -n 1` HEAD
Paul Schreiber                +++++++++++++++++++++++++++++++++++++++++++++(349)
spacewander                   +++++++++++++++++++++++++++++++++++++++++++++(113)
Mark Eissler                  ++++++++++++++++++++++++++
```

### merge-into

```
$ git merge-into master
```

### graft

```
$ git graft new_feature master
```

### alias

```
$ git alias last "cat-file commit HEAD"
$ git alias
last = cat-file commit HEAD
```

### ignore

```
$ git ignore build "*.o" "*.log"
... added 'build'
... added '*.o'
... added '*.log'
```

### info

```
$ git info

    ## Remote URLs:

    origin              git@github.com:sampleAuthor/git-extras.git (fetch)
    origin              git@github.com:sampleAuthor/git-extras.git (push)

    ## Remote Branches:

    origin/HEAD -> origin/master
    origin/myBranch

    ## Local Branches:

    myBranch
    * master

    ## Most Recent Commit:

    commit e3952df2c172c6f3eb533d8d0b1a6c77250769a7
    Author: Sample Author <sampleAuthor@gmail.com>

    Added git-info command.

    Type 'git log' for more commits, or 'git show <commit id>' for full commit details.

    ## Configuration (.git/config):

    color.diff=auto
    color.status=auto
```

### fork

```
$ git fork LearnBoost/expect.js
```

### release

```
$ git release 0.1.0
```

### contrib

```
$ git contrib visionmedia
visionmedia (18):
  Export STATUS_CODES
  Replaced several Array.prototype.slice.call() calls with Array.prototype.unshift.call()
  Moved help msg to node-repl
```

### repl

```
$ git repl

git> ls-files
History.md
Makefile
```

### undo

```
$ git undo
```

### gh-pages

```
$ git gh-pages
```

### scp

```
$ git scp staging HEAD
```

### setup

```
$ git setup
```

### touch

```
$ git touch index.js
```

### obliterate

```
$ git obliterate secrets.json
```

### feature|refactor|bug|chore

```
$ git feature dependencies
$ git feature finish dependencies
```

### local-commits

```
$ git local-commits
commit 5f00a3c1bb71876ebdca059fac96b7185dea5467
Merge: 7ad3ef9 841af4e
Author: Blaine Bublitz <blaine@iceddev.com>
Date:   Thu Aug 20 11:35:15 2015 -0700

    Merge pull request #1211 from JimiHFord/patch-1

    Update guidelines.md

commit 841af4ee7aaf55b505354d0e86d7fb876d745e26
Author: Jimi Ford <JimiHFord@users.noreply.github.com>
Date:   Thu Aug 20 11:55:38 2015 -0400

    Update guidelines.md

    fixed typo
```

### archive-file

```
$ git archive-file
Building archive on branch "master"
Saved to "gulp.v3.9.0-36-g47cb6b0.zip" ( 60K)
```

### missing

```
$ git missing master
< d14b8f0 only on current checked out branch
> 97ef387 only on master
```

### lock

```
$ git lock config/database.yml
```

### locked

```
$ git locked
config/database.yml
```

### unlock

```
$ git unlock config/database.yml
```

### reset-file

```
$ git reset-file README.md HEAD^
Reset 'README.md' to HEAD^
```

### pr

```
$ git pr 226
From https://github.com/tj/git-extras
 * [new ref]       refs/pulls/226/head -> pr/226
Switched to branch 'pr/226'
```

### root

```
$ git root
/GitHub/git
```

### delta

```
$ git delta
README.md
```

### merge-repo

```
$ git merge-repo git@github.com:tj/git-extras.git master .
git fetch git@github.com:tj/git-extras.git master
warning: no common commits
remote: Counting objects: 3507, done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 3507 (delta 1), reused 0 (delta 0), pack-reused 3502
Receiving objects: 100% (3507/3507), 821.12 KiB | 286.00 KiB/s, done.
Resolving deltas: 100% (1986/1986), done.
From github.com:tj/git-extras
 * branch            master     -> FETCH_HEAD
Added dir 'git-merge-repo.E95m0gj'
No local changes to save
```

### psykorebase

```
$ git psykorebase master
$ git psykorebase --continue
$ git psykorebase master feature
```


## [gitflow](https://github.com/nvie/gitflow) - git extensions to provide high-level repository operations for Vincent Driessen's branching model.

## [git-up](https://github.com/aanand/git-up) - Fetch and rebase all locally-tracked remote branches.

## [hub](https://github.com/github/hub) - Extend git with extra features and commands that make working with GitHub easier.

## [git-deploy](https://github.com/mislav/git-deploy) - git deployment made easy.

## [bash-git-prompt](https://github.com/magicmonty/bash-git-prompt) - An informative and fancy bash prompt for Git users.

## [git-stree](https://github.com/tdd/git-stree) - A better git subtree helper command.

## [git-subrepo](https://github.com/ingydotnet/git-subrepo) - git Submodule Alternative.

## [git-archive-all](https://github.com/Kentzo/git-archive-all) - A python script wrapper for git-archive that archives a git superproject and its submodules, if it has any.

## [git-cal](https://github.com/k4rthik/git-cal) - Github like contributions calendar on terminal.

## [git-crypt](https://github.com/AGWA/git-crypt) - Transparent file encryption in git.

## [gitflow (AVH Edition)](https://github.com/petervanderdoes/gitflow) - This fork adds functionality not added to the original branch.

## [git-hooks](https://github.com/icefox/git-hooks) - A tool to manage project, user, and global Git hooks for multiple git repositories.

## [git-imerge](https://github.com/mhagger/git-imerge) - Incremental merge for git.

## [git-lfs](https://github.com/github/git-lfs) - git extension for versioning large files.

## [git-now](https://github.com/iwata/git-now) - A temporary commit tool for git.

## [git-plus](https://github.com/tkrajina/git-plus) - git utilities.

## [git-sh](https://github.com/rtomayko/git-sh) - A customized bash environment suitable for git work.

## [git-test](https://github.com/spotify/git-test) - Run tests on each distinct tree in a revision list, skipping versions whose contents have already been tested.

## [GitTracker](https://github.com/stevenharman/git_tracker) - A git hook that will scan your current branch name looking for something it recognizes as a Pivotal Tracker story number.

## [legit](https://github.com/kennethreitz/legit) - git for Humans.
