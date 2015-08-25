# Awesome git addons [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated list of addons that extends git.

Inspired by the [awesome](https://github.com/sindresorhus/awesome) list thing.


## Table of Contents

- [Git Extras](#git-extras)


## [git-extras](https://github.com/tj/git-extras) - Little git extras.

### squash

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
  1400	Shawn O. Pearce                 3.5%
  1109	Linus Torvalds                  2.7%
   819	Nguyễn Thái Ngọc Duy            2.0%
   769	Johannes Schindelin             1.9%
   762	Jonathan Nieder                 1.9%
```

### line-summary

```
$ git line-summary

 project  : gulp
 lines    : 3900
 authors  :
 1040 Contra                    26.7%
  828 Sindre Sorhus             21.2%
  289 Rob Richardson            7.4%
  198 Blaine Bublitz            5.1%
  134 Eric Schoffstall          3.4%
  128 Dmitry Mazuro             3.3%
  109 Joel Kemp                 2.8%
   87 Vsevolod Strukchinsky     2.2%
   78 Terin Stock               2.0%
```

### effort

```
$ git effort

  file                                          commits    active days

  .gitattributes............................... 3          3
  .gitignore................................... 265        226
  .mailmap..................................... 47         40
  COPYING...................................... 2          2
  Documentation/.gitattributes................. 1          1
  Documentation/.gitignore..................... 12         12
  Documentation/CodingGuidelines............... 55         45
  Documentation/Makefile....................... 178        144
  Documentation/RelNotes/1.5.0.1.txt........... 1          1
```

### authors

```
$ git authors
Contra <contra@maricopa.edu>
Eric Schoffstall <contra@wearefractal.com>
Sindre Sorhus <sindresorhus@gmail.com>
Blaine Bublitz <blaine@iceddev.com>
Rob Richardson <robrich@robrich.org>
Eric Schoffstall <contra@maricopa.edu>
contra <contra@maricopa.edu>
Tyler Kellen <tyler@sleekcode.net>
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
$ git commits-since
... commits since last week
```

### count

```
$ git count
total 855
```

### create-branch

### delete-branch

### delete-submodule

### delete-tag

### delete-merged-branches

### fresh-branch

### guilt

### merge-into

### graft

### alias

### ignore

### info

### fork

### release

### contrib

### repl

### undo

### gh-pages

### scp

### setup

### touch

### obliterate

### feature|refactor|bug|chore

### local-commits

### archive-file

### missing

### lock

### locked

### unlock

### reset-file

### pr

### root

### delta

### merge-repo

### psykorebase


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
