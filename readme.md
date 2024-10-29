# Git
This an overview for git. You can come here for reference.

## How to get it
- **Windows**
Download the latest Git for Windows installer from [Windows Link](https://git-scm.com/download/win)
- **macOS**
Git is often pre-installed on macOS. To check, open Terminal and type ```git --version```. If it's not installed, you can download it from the App Store or using a package manager like [Homebrew](https://brew.sh/).
- **Linux**
Git is typically included in most Linux distributions. To check, open a terminal and type ```git --version```. If it's not installed, you can install it using your distribution's package manager (e.g., ```sudo apt install git``` on Ubuntu).

## Get help
```bash
git help
```

## Create new Repository
```bash
git init
```
This command with create an empty repo where you are. You can check where you are with the ```pwd``` command.

## Stage changes
```bash
git add [*]
```
\* can be the file, a folder, or if you want to add all you can use ``` git add .``` or if you want all the files and directories under another dictory you can use ```git add \path\to\folder\* ```.

## Commit changes
```bash
git commit -m "Message"
```
This will commit the sataged changes with the ```Message```. If you want to use the default editor to write your message you can use:
```bash
git commit -a
```

## Check the status
You can always check the current status of git using the following command:
```bash
git status
```

## Branches
### Create a new Branch
```bash
git branch [name]
```
### Switch to a branch
```bash
git checkout [name]
```
### See all the branches
```bash
git branch
```
### Change the name of current branch
```bash
git branch -M [new-name]
```
### Delete a branch
```bash
git branch -D [name]
```

## Merge
You can merge branches using the following command:
```bash
git merge [current_branch] [branch]
```
You can ommit the ```current_branch``` if you are already there. For example if you are in ```main``` and want to merge ```work``` you can write the following command if you are currently in the main branch:
```bash
git merge work
```

## Working with remote
### Add a remote
```bash
git remote add [name] <remote_url>
```
By convention the remote name is ```origin```.
### Push to remote
```bash
git push -u [remote] [branch]
```
For example this branch is ```lesson-git``` if we want to push it to our remote repo we can use:
```bash
git push -u origin lesson-git
```
### List remotes
```bash
git remote
```
### Fetch changes from remote
Fetch changes from the remote repository without merging
```bash
git fetch [remote]
```
If you don't provide the remote name it will use the default remote.
### Pull changes from remote
Fetch and merge changes from the remote repository
```bash
git pull [remote] [branch]
```

### Clone a remote repo
```bash
git clone [remote_url]
```

## More Information
### Ignore files or folders
If you want git to ignore tracking a folder or a file you can add them to the ```.gitignore``` file. This is usually the ```.env``` file.
### Undo changes
```bash
git revert
```
By default it will revert to last commit but you can use the commit to revert to.
```bash
git reset
```