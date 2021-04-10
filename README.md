# MakeFile
Single File script for adding files on staging area in git and commiting and then pushing to specified branch

# Steps
* Copy This file in directory which you want to perform this task on.
* Add this file to .gitignore so as to prevent it from getting pushed along with your project by writing `makefile` in .gitignore.
* Now open this file and in it's structure that is
<br>

```
git:
	git add .
	git commit -m "$m"
	git push -u origin master
```

**Here check your branch name and replace `master` with it**.
**Note : This will add add files to staging area.**

* To run this file make sure this file is in root of your project directory and run command

```
make git m="<YOUR_COMMIT_MESSAGE>">
```