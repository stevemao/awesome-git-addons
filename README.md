# Awesome git addons [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated list of addons that extends git cli.

```
$ git bla
Something awesome happens!
```

Inspired by the [awesome](https://github.com/sindresorhus/awesome) list thing.


## Table of Contents

- [Git Extras](#git-extras)
- [git-flow](#gitflow-avh-edition)


## [Git Extras](https://github.com/tj/git-extras)

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
Deleted branch integration (was bfb8522).
Deleted remote-tracking branch remote/integration (was bfb8522).
To git@github.com:remote/gulp.git
 - [deleted]         integration
```

### delete-submodule

```
$ git delete-submodule lib/foo
```

### delete-tag

```
$ git delete-tag 0.0.1
Deleted tag '0.0.1' (was 08595cb)
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
Removing .DS_Store
Removing .editorconfig
Removing .gitignore
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


## [gitflow (AVH Edition)](https://github.com/petervanderdoes/gitflow)

### flow-init

```
$ git flow init

Which branch should be used for bringing forth production releases?
   - changelog
   - master
Branch name for production releases: [master]

Which branch should be used for integration of the "next release"?
   - changelog
Branch name for "next release" development: [master]
Production and integration branches should differ.
```

### flow-feature

```
$ git flow feature
$ git flow feature start awesome-feature
$ git flow feature finish awesome-feature
$ git flow feature delete awesome-feature

$ git flow feature publish awesome-feature
$ git flow feature pull remote awesome-feature
```

### flow-release

```
$ git flow release
$ git flow release start awesome-release
$ git flow release finish awesome-release
$ git flow release delete awesome-release
```

### flow-hotfix

```
$ git flow hotfix
$ git flow hotfix start awesome-release
$ git flow hotfix finish awesome-release
$ git flow hotfix delete awesome-release
```

### flow-support

```
$ git flow support
```


## [git-up](https://github.com/aanand/git-up)


## [hub](https://github.com/github/hub)


## [git-deploy](https://github.com/mislav/git-deploy)


## [bash-git-prompt](https://github.com/magicmonty/bash-git-prompt)


## [git-stree](https://github.com/tdd/git-stree)


## [git-subrepo](https://github.com/ingydotnet/git-subrepo)


## [git-archive-all](https://github.com/Kentzo/git-archive-all)


## [git-cal](https://github.com/k4rthik/git-cal)

```
$ git cal
    Aug   Sep     Oct     Nov       Dec     Jan       Feb     Mar     Apr     May       Jun     Jul     Aug
        ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼
    M   ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼
        ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼
    W ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼
      ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼
    F ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼
      ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼ ◼

                                                                                               Less ◼ ◼ ◼ ◼ ◼  More
1907: Total commits
  78: Days ( Apr 15 2015 - Jul  5 2015 ) - Longest streak excluding weekends
  35: Days ( May 17 2015 - Jun 20 2015 ) - Longest streak including weekends
   0: Days - Current streak
```


## [git-crypt](https://github.com/AGWA/git-crypt)


## [git-hooks](https://github.com/icefox/git-hooks)


## [git-imerge](https://github.com/mhagger/git-imerge)


## [git-lfs](https://github.com/github/git-lfs)


## [git-now](https://github.com/iwata/git-now)


## [git-plus](https://github.com/tkrajina/git-plus)


## [git-sh](https://github.com/rtomayko/git-sh)


## [git-test](https://github.com/spotify/git-test)


## [GitTracker](https://github.com/stevenharman/git_tracker)


## [legit](https://github.com/kennethreitz/legit)


## License

[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png)](http://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [Steve Mao](https://github.com/stevemao) has waived all copyright and related or neighboring rights to this work.
