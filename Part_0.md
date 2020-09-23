# Unix/Git (10/8)

Workshop Recording: [here](__insert-link-here__)

Workshop Slides: [here](__insert-link-here__)

In this workshop, we learned about Unix and Git. Specifically, we completed our **Installations**, and then learned about **Unix**, and **mGit**.

We used these ideas to:
- [x] Install Git, Git Bash (for Windows), Node.js + npm
- [x] Learn how to navigate around files using Unix or Git Bash commands
- [x] Learn how to add, push/pull, and branch with Git
- [x] Create a branch of the Pokemon Generator using Git


## Installations:

### Git

For Mac users: (download instructions) (link)

For Windows: (download instructions) (link)

## Git Bash (for Windows users ONLY)

Here are the download instructions: (download instructions) (link)

## Node.js + npm

For Mac users: (download instructions) (link)

For Windows: (download instructions) (link)


## What is Unix?

Unix is a computer operating system (OS). It allows you to move around your computer, select files, and execute commands.

Unix is the default OS on Mac computers. For Windows users, the default OS is Microsoft Windows OS, which is not as prevalent in tech industry. This is why Windows users will be using Git Bash, similar OS to Unix, which should have been downloaded in the previous step.

A programmer can access a computer's OS through the Command Line Interface (CLI) or the command line. This is where we enter commands.

In Hack School, we will be using Unix, through the command line, to access and modify files.


### Directories and File Systems

A **file system** is a system that your computer uses to store data. Without a file system, your computer would just dump all your files into one giant box, and you would have a really difficult time trying to sort all the files on your computer!

Most OS, including Unix, use **directories** to organize data. On the user interface, directories are often referred to as "folders".

You can see an example of the Unix file system below:

<img src="https://i.stack.imgur.com/zZp99.png" alt="file-system-diagram">

The `/` at the top of the diagram represents the **root directory**. As the name implies, it is the beginning of the system, where everything originates from.

Directly below the root directory are eleven other directores named `bin`, `dev`, `etc`, `home`, and others. These directories are considered **subdirectories** or **children** of the root directory.

Below the `home` directory are two other directories `mthomas` and `stu1`. These directories are the **subdirectories** or **children** of `home`. Accordingly, you can refer to `home` as the **parent directory** of `mthomas` and `stu1`.

#### File Paths

Unix's file system of directories allows you to locate a file or directory by listing its parent directories, separated by `/`. This is called a **path**.

There are two types of paths: **root paths** and **local paths**.

**Root paths** start at the root directory. For example, the root path to the directory `bin` would be `/home/mthomas/bin`. You start at the root `/` directory; then you move down to the `home` directory; then you move to the `mthomas` directory; and that's where you would find `bin`.

<details> 
  <summary> Try it yourself!: What is the root path to <code>foo</code>?</summary>
   The path would be: <code>/home/mthomas/class_stuff/foo</code>.
</details>

**Local paths** start at the directory that you are currently located in. This only works if you are in a parent directory containing where you want to go. 

For example, if you were in `mthomas`, you cannot use a local path to get to `stu1`. You would have to use a root path to get to `stu1`.

However, if you were in `mthomas`, you could get to `foo` using a local path. That local path would be `/class_stuff/foo`. That is because you are already located in `/home/mthomas`.

For convenient coding, most of the time you will want to use a root directory so the program is never confused on where files are located.

### Unix Commands

A **command** are word(s) that are sent to the command line. The command line then takes our commands, compiles them into binary, and then sends it to the computer operating system to do something.

Here are a few Unix commands that you can use on your command line (either Unix or Git Bash).

#### Where are you? Use `pwd`!

The command `pwd` is used to determine where you are in the Unix file system. `pwd` stands for **present working directory**.

This is an example of someone using `pwd` on their computer:

<img src="https://codeforwin.org/wp-content/uploads/2019/02/pwd-command-linux-min.jpg" alt="pwd_screenshot">

The `$` marks the end of their user account name (`bandnapaikaray` on their localhost network). On the first line, you can see that they used `pwd`.

Their command line returned `/home/bandnapaikaray`.

You should recognize this as a root path!

This is a fairly default `pwd` result: the user is currently inside their computer (`/`), inside one of the accounts (`home`), and specifically inside the `bandnapaikaray` account.

<details> 
  <summary> Try it yourself!: If you were in the <code>class_stuff</code> directory, what would <code>pwd</code> return?</summary>
  <code>pwd</code> would return <code>/home/mthomas/class_stuff</code>.
</details>


#### Navigating directories using `cd`

The `cd` command is used to navigate the Unix file system. `cd` stands for **current directory**. It can be used two ways.

##### `cd ..`

This command moves from the current directory to parent directory. On the diagram above, you would be moving up one level.

For example, if you were currently in the `/bin` directory, you could use `cd ..` in the command line to move into the parent (in this case, `mthomas`) directory.


##### `cd [path]`

This command moves from a current directory to another directory.


## What is Git?

<img src="https://cdn.afterdawn.fi/v3/news/original/github-logo.png" alt="github logo" height=10% width=10%>

Git is a very popular version-control software used during software development. It is used for tracking changes and making sure your software always has backups, in case someone messes up. Data in Git is stored in a file system with directories, just like with Unix (although directories in Git are called **repositories**.)

We access Git using either Git Bash or Unix.

In Hack School, we will be using Git to make a personal branch of the Pokemon Generator.

### Configuring Git on your computer

First, make sure you have Git downloaded on your computer!

Next (ignoring the $ symbol: remember, that marks the end of a username), enter these two commands:
```
$ git config --global user.name "FirstName LastName"
```
and then
```
$ git config --global user.email "email@domain.com"
```
These will configure Git on your computer (that is: tell your computer what account you are using on Git).


### Adding and committing

You can **add** files using the `git add` command. In Git, adding files means moving files to your *staging area*.

You can think of your *staging area* as your Git checkout basket. While you can make personalize changes and select what you want to upload, **adding** on Git does not actually do anything to your Git repository. You'll need to commit to effect changes in your code.

#### `git add`

`git add` is a Git command that takes an input file(s) and adds them to your staging area.

You can use `git add` in a variety of different ways, including:

`git add new-file.txt`, where you add a file "new-file.txt" to your staging area;

`git add new-file1.txt newfile2.txt` where you can add multiple files to your staging area, if the file names are given and separated by spaces;

or even `git add --all`, where all updated or modified files get sent to your staging area.


<details> 
  <summary> Extra Credit: How to remove files from your staging area? </summary>
  Added something you don't want to send to your staging area? Try using the <code>rm</code> command: <code> rm --cached file_name.txt </code>. You'll need to add <code>--cached</code> to tell Git that the file you want to remove ("file_name.txt") is already cached (that is, it's already in the staging area).
</details>

Now you've added file(s) to your staging area. The next step is to move these changed file(s) to your local repository: where your Git code lives on your computer.


#### `git commit`

`git commit` is a Git command that takes the input file(s) from the staging area and adds them to your local repository.

Usually, you'll want to use this command:
```
git commit -m "this is a message"
```
By adding `-m`, you can add a message attached to your commit. This is especially useful so you can make notes of what you changed, so if you ever have to go back through your code to hunt down a previous version, you don't have to manually look through "commit 405" to "commit 500" to see what changes you made.

Congratulations! You have moved files from your staging area to your local repository (computer).


### What is a remote repository?

A remote repository is where software is stored online.

<img src="https://qph.fs.quoracdn.net/main-qimg-a161bdd97e4e0de40d999ac222fe2008" alt="remote repository diagram">

By moving your code from a local repository to a remote repository, you put your code on the Internet. That allows your GitHub profile to show the code. It also allows other collaboraters to access the new code.

Some examples of Main Idea 1 are:

#### `(Code Command #1)`

`Code Command #1` is a (insert descriptor here). It takes (input) and (does output).

```
example code here
```


## Project Implementation

### Task 1

We want to do (insert task here) for our Pokemon generator.

For that, we use **main idea 1** and **main idea 2**.

```
example code here
```

<details> 
  <summary> Hint #1: </summary>
   Try doing this: <code> code </code>
</details>

## Simple Resources:

**Main Idea 1**:

Site #1: (link)

Site #2: (link)
