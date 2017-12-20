
Creating a new repo in git can be done only via the webpage
login using prakashanand.email@gmail.com with pass test1234!
once logged in, create a repo using the options on the website
NOTE: Your root folder in github is "papython", so all of your projects will have https://github.com/papython as the default github path


Checking in your project for the first time

login to your linux account
mkdir test_project
cd test_project
Initialize the local directory as a Git repository.
git init
# Adds the files in the local repository and stages them for commit. To unstage a file, use 'git reset HEAD YOUR-FILE'.
git add .
# Commits the tracked changes and prepares them to be pushed to a remote repository. To remove this commit and modify 
the file, use 'git reset --soft HEAD~1' and commit and add the file again.git commit -m "First commit"
git commit -m "First commit"

Next, you want to upload your files to github.com
At the top of your GitHub repository's Quick Setup page on the website, click  to copy the remote repository URL. e.g. https://github.com/papython/python_REST.git
In the linux command prompt, add the URL for the remote repository where your local repository will be pushed. This has to be done only once and gets stored in the .git/conf file.
git remote add origin https://github.com/papython/python_REST.git
# Sets the new remote
git remote -v
# Verifies the new remote URL
Push the changes in your local repository to GitHub.
git push origin master
# Pushes the changes in your local repository up to the remote repository you specified as the origin


Here is an example of the full process

mkdir test
cd test
echo "testing file1">test1
echo "testing file2">test2
git init
git add .
git commit -m "my comments"
git remote add origin https://github.com/papython/<repo name>
git push origin master

