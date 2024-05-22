# Learn to use git as a Gizmo to Impress Your Friends and Terrify Your Enemies

## types of complexity

Broadening our git vocabulary can be one of the keys for managing all this complexity that we are dealing with daily.

* Processor architecture
* OS
* Languages
* Domain
* Supplier
* Release cycle

## scope

* referring to and tracking commits
* ways to work with branches (rebase, merge, cherry-pick, rerere)
* debugging with git (blame, bisect)
* classic workflows

## not in the scope

* github and other "bare repos"
* hooks
* submodules/subtrees
* IDE integration and git clients

## get the chapters

```bash
git clone --recurse-submodules git@github.com:s-zaj/gizmo.git
```

## adding chapters

Each chapter is a little sandboxed nested root which is registered as a submodule. The motivation is to have a little demo repository that is designed for play with the topics included

```bash
cd ../chapters
mkdir 01_commits
cd 01_commits
git init
git echo "Submodule repository" > README.md
git add README.md
git commit -m "initial submodule commit"
cd ../..
git submodule add -- <absolute path to repo> chapters/01_commits
```
