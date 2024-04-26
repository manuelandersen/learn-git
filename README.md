# Learning Git trough using Git

So, this is a github repo that im using to learn git and github.

## First step

We use:

```
git init 
```

to initiate a git repository. This means that our local folder will be tracked by git.  

The second thing we do is go to github and create a repository. We use:

```
git remote add origin url
```

where url is the url of the repository we just created.

We then create a python file called `first-file.py` and we just write in this a simple print:

```python
print("This is the first file")
```

we use:

```
git add .
```

to add this file to our repository. Then we use:

```
git commit -m "message"
```
to commit this files we added to the repository. You need to write in `"message"` a concise description of what you commit. Then we use:

```
git push origin master
```
to push our commit to the github repository. This changes will be in the `master` branch.

### Checking what is going on

At any point you can do:

```
git status
```
to now where the code you have write are in terms of git tracking.

You can also do:

```
git log
```

to get a recor of all the changes and commits your code had over time. To exit this log just press `q`.

# Making a new branch

Sometimes you want to work on some new feature or try a different version of your code, but dont want to change the code until you know that the feature works. So you make a "copy" of your actual code and work in that copy. This is called a new branch. Your make a new one by doing:

```
git checkout -b new-branch
```

where `new-branch` is the name of the new branch you want to make.