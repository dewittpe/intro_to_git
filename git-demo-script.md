# Create a new project directory on your computer
mkdir newproject
cd newproject

# initialize the git repo
git intit

# check the status of the repo
git status

# create a file
echo "This is a very important file." > important.txt

# check the status of the repo again
git status

# add the file to the staging area
git add important.txt

# check the status again
git status

# commit the file to the repo
git commit -m "initial commit with important file"

# add some more files
echo "# README Files are important" > README.md
echo "Second important analysis file" > important02.txt
echo "another line in the file" >> important02.txt
mkdir data
cp ... data into the repo ... just copy a set of files into the repo

# check the status 
git status

# add only one or two files to the staging area
git add file1 file2

# status
git status

# commit
git commit

# check the commit log
git log

# note that this log can be customized, these are specific to my ~/.gitconfig
# file
git lg1
git lg2

# Edit a file (make a really stupid edit)
vim ....

# check the diff
git diff file

# check out the file to remove really stupid edit
git checkout file

# edit the file with something smart, remove something and add something
git diff
git add file
git commit -m "..."

# mv files into a new directory
mkdir ....
git mv file file
git rm file
git status
git commit
git log
git lg1

# add files that need to be ignored...  add .log file to a directory
mkdir compiled
report/report.pdf
report/report.log
git status 
echo "*.log\n*.swp" > .gitignore
git status

--------------------------------------------------------------------------
# Working with a remote
--------------------------------------------------------------------------

open a webbrowser, open up cbcgit.ucdenver.edu:8443, 
login as yourself, 
create a new repo
add the repo to the the work above 
push the above to the remote
show the result in the new repo

--------------------------------------------------------------------------
# Working with "others"
--------------------------------------------------------------------------

start by showing ~/.gitconfig
git config -l

ssh into your machine in 406
ssh optiplex

clone the repo
git config -l
make a few changes and at least two commits
push changes.

logout of optiplex and move back to the inspiron
git fetch
git lg1
git status
git merge origin/master   (This with a fast forward)

git blame

ssh back to optiplex
edit files, without and with merge conflic
git fetch
git merge
fix issues

git tag 


--------------------------------------------------------------------------
# Working with Branches
--------------------------------------------------------------------------

git branch



