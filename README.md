# Git-and-Github-Intro
Brief Intro of GIT AND GITHUB with basic commands and tutorial

## GIT
Version control system is a tool (software) that helps to track changes in code 
GIT is a version control system. It is 
- Popular
- free and open source
- fast and scalable

Used primarily to
- track the history : history of features or code in your project and can rollback to previos version of your project
- collaborate : when you collaborate in a team on a project, it is important to track on which features, what changes, whom has did it and which changes should be accepted in the production

## GITHUB  
Website that allows developers to store and manage their code using GIT.We upload the project in folders called Repositories(or Repo) on github. Also you can watch other people's repo's,clone and download it etc.

### Step 1 - Create Repo

You will see a readme.md file once a repo is created

**Readme** file is stored as Readme.md where `".md"` stands for `markdown`, there is a message against the README.md file on slight right, upon initial setting up of repo, this will always contain the message `"initial commit"`

You can go on the edit option, do some editing and select commit changes. You may additionally add a message while doing this change which will reflect on the repo as well


### Step 2 - Setting up GIT
1. Download VS CODE
2. Download GITBASH (ON WINDOWS) / TERMINAL (ON MAC)

Once installed, check for git version using git bash
> `git --version`
This will output the version and will confirm installation of git on your system

You can also run a few scripts like `ls` - This will output all the folders and files in your current directory, `pwd` - will provide current directly path, '`clear` - to clear output on the git bash terminal, `-Get-ChildItem -Force` - to get all the items in current directory including the hidden ones or alternatively use `dir -Force` for the same command.


### Step 3 - Configuring GIT
Telling GIT which account do we need to make changes on github

1. Setting USER NAME
- `git config -- global user.name "Your_User_Name`

2. Setting EMAIL
- `git config -- global user.email "email_address`

3. To check the status of setup
- `git config --list`

### <span style= 'color:red'>You can also use the git commands in your VS CODE Terminal </span>

### GIT COMMANDS
1. clone - cloning a repository on our local machine
  - `git clone <-some link>`
  - Go to your repo, click on code button (in green) select HTTPS block and copy the link there and use that link in the clone command to copy your repo in local machine

2. status - display the state of your code
  - `git status`
  - Suppose you have made some changes in your project (in any file), and saved it, then although the changes have been made locally in the system, they will not reflect on the github repo. When you use the `git status` command, it will reflect which files have been changed or modified, are they up-to-date or require some additional operations.

Whenever you modified or changed somethin in your project, from there it is a two step process : 
1. Add 
2. Commit
If you do not use these two commands, the status will keep on showing there are some modified files in the project

There are 4 kinds of statuses that `git status` will show
1. Untracked - You added a new file, saved it but haven't added and commit it to the main brand
2. modified - some changes in the previously present files in repo
3. staged - file is added but not committed in the repo
4. unmodified - unchanged