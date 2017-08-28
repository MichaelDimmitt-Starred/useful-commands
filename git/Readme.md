# Github_Map_Closing_Notes

git add .; git commit --amend --no-edit; git push --force-with-lease;


### My development environment remote information for a project
remote origin commit information can be found in the linked issue:
<br>https://github.com/Swuber/unf-swuber_web_app_phoenix/issues/4

### Check out the first time I needed to use SVN instead of git.
neat way I get a part of a repository without the whole enchillada:
<br>https://github.com/MichaelDimmitt/sc/blob/master/install.sh

### Update a Branch
<pre>git remote add upstream https://github.com/whoever/whatever.git;
git rebase upstream/master;
git push -f origin master;</pre>

### Updating Forked Repository
<pre>git remote add upstream https://github.com/whoever/whatever.git;
git pull upstream master;
git rebase upstream/master;
git push -f origin master;
</pre>
In one command:
<pre>git remote add upstream https://github.com/whoever/whatever.git;git pull upstream master;git rebase upstream/master;git push -f origin master;</pre>

<b>Alternate</b><br>https://stackoverflow.com/questions/7244321/how-do-i-update-a-github-forked-repository
<pre>git remote add upstream https://github.com/whoever/whatever.git;
git fetch upstream master;
git checkout master;
git rebase upstream/master;
git push -f origin master;
</pre>

### Git LFS (large files)
<pre>brew install git-lfs;
git lfs install;
git lfs track "*.iso";
git add .gitattributes;
git lfs ls-files;
https://github.com/git-lfs/git-lfs?utm_source=gitlfs_site&utm_medium=repo_link&utm_campaign=gitlfs
</pre>

### Cherrypicking
http://stackoverflow.com/questions/9339429/what-does-cherry-picking-a-commit-with-git-mean
1) Make sure you are on the branch you want apply the commit to.
 ```git checkout master```
2) Execute the following:
 ```git cherry-pick <commit-hash>```

```git notes copy <fromcommithash> <tocommithash>```

simplify into single command:
git checkout branch; git cherry-pick <commit-hash>git notes copy <fromcommithash> <tocommithash>
### how github handles repo names
```
github allows [A-Za-z0-9_.-], and transforms all other characters to "-"
when we were getting each file name
we needed to check immediately if it passed and ignore/not create repo if it failed.
```

### when rebasing a large number of commits (implemented in next header)
```
if squashing make changes on a seperate branch
then, do not merge;
instead preserve the old copy of master renaming
and then change the rebased branch to master
(implemented in next header: how to change master branch)
```
### how to change master branch
```
git branch -m master old-master
git branch -m seotweaks master
git push -f origin master
git push origin master:master --force
```

```
If you want to rename the current branch, you can do:

git branch -m newname
```

### warning regarding github map, in view mode.
```
submodules are only for viewing.
edits should be performed by cloning
and pushing particular repositories.
```

### updating a map
```
git clone --recursive https://github.com/MichaelDimmitt/Research.git
cd Research/;git submodule update --remote --merge;
git add .;git commit -m "applied updat operation git submodule update --remote --merge”;git push;
git clone --recursive https://github.com/MichaelDimmitt/Research.git;
```

### Additional Information coming soon.
#### secrets ... people may be warned
```
git rebase -i 504faf7d0b72c6d8e6fc0279a40fb39143d6d0ad
vi README.md
git add .
git commit --amend --author="MichaelDimmitt <michaelgdimmitt@gmail.com>" --no-edit
git rebase --continue
git push --force-with-lease
```
