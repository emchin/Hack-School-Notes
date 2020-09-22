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


#### Navigating directories using `cd`

The `cd` command is used to navigate the Unix file system. `cd` stands for **current directory**. It can be used two ways.

##### `cd ..`

This command moves from the current directory to parent directory. On the diagram above, you would be moving up one level.

For example, if you were currently in the `/bin` directory, you could use `cd ..` in the command line to move into the parent (in this case, `mthomas`) directory.


##### `cd [path]`

This command moves from a current directory to another directory.


## What is [Workshop Name]?

[Workshop Name] is (insert general description here). It is used for (general purpose).

In Hack School, we will be using [Tool 1] to (purpose for project).

### Main Idea 1

Main Idea 1 is (explanation).

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
