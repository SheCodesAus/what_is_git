<center>

<img src=./img/logo.png />

<h1><img src=./img/git_icon.png width="100" /> Git and GitHub <img src=./img/github_icon.png width="100" /></h1>

</center>

Hopefully you've already taken a look at [our introductory video on Git and GitHub](). (If you haven't, have a watch after class!)

This lesson is a practical introduction to using Git and GitHub. It will give you a chance to use the tools we outlined in the video. 

Don't worry if you're still feeling confused by the end of class - the best way to get comfortable with these skills is to practise them, and there'll be plenty of opportunity for that throughout this course!

```diff
- need to add a link to the video once it's finished
```

<h2>Table of Contents</h2>

- [  Section 1: Git](#--section-1-git)
  - [1.1 🧹 Some Housekeeping 🧹](#11--some-housekeeping-)
    - [Step 1.1.1 🏡 Go To Your Home Directory 🏡](#step-111--go-to-your-home-directory-)
    - [Step 1.1.2 🎓 Make Sure You Have A Directory For Your Class Work 🎓](#step-112--make-sure-you-have-a-directory-for-your-class-work-)
    - [Step 1.1.3 🧭 Navigate Into Your Classwork Directory 🧭](#step-113--navigate-into-your-classwork-directory-)
    - [Step 1.1.4 📁 Create A Directory For Today's Work 📁](#step-114--create-a-directory-for-todays-work-)
  - [1.2 - 🌄 Initialisation 🌄](#12----initialisation-)
    - [Step 1.2.1 🗂️ Initialise The Directory As A Git Repo 🗂️](#step-121-️-initialise-the-directory-as-a-git-repo-️)
    - [Step 1.2.2 👀 Inspecting Our New Git Repo 👀](#step-122--inspecting-our-new-git-repo-)
  - [Step 1.3 🌱 The Initial Commit 🌱](#step-13--the-initial-commit-)
    - [Step 1.3.1 📄 Create A Blank File 📄](#step-131--create-a-blank-file-)
    - [Step 1.3.2 🕵️ Check The Status 🕵️](#step-132-️-check-the-status-️)
    - [Step 1.3.3 📥 Add The New File To The "Staging Area" 📥](#step-133--add-the-new-file-to-the-staging-area-)
    - [Step 1.3.4 💾 Make The Commit 💾](#step-134--make-the-commit-)
  - [1.4 🪴 A Second Commit 🪴](#14--a-second-commit-)
    - [Step 1.4.1 📝 Adding Some Code 📝](#step-141--adding-some-code-)
    - [Step 1.4.1 🕵️ Check The Status Again 🕵️](#step-141-️-check-the-status-again-️)
    - [Step 1.4.2 📥 Add To Staging Again 📥](#step-142--add-to-staging-again-)
    - [Step 1.4.3 💾 Make That Commit! 💾](#step-143--make-that-commit-)
  - [1.5 ⏳ A Pause To Take Stock ⏳](#15--a-pause-to-take-stock-)
  - [1.6 🌵 Create A Feature Branch 🌵](#16--create-a-feature-branch-)
    - [Step 1.6.1 🌱 Create The New Branch 🌱](#step-161--create-the-new-branch-)
    - [Step 1.6.2 🕵️ Take A Look At The Current Branches 🕵️](#step-162-️-take-a-look-at-the-current-branches-️)
    - [Step 1.6.3 ➡️ Check Out The New Branch ➡️](#step-163-️-check-out-the-new-branch-️)
  - [1.7 🛠️ Develop A Feature 🛠️](#17-️-develop-a-feature-️)
    - [Step 1.7.1 📝 Write The Code 📝](#step-171--write-the-code-)
    - [Step 1.7.2 📥 Stage The Changes 📥](#step-172--stage-the-changes-)
    - [Step 1.7.3 💾 Make The Commit 💾](#step-173--make-the-commit-)
  - [1.8 ⏳ Pause Again: What Did We Just Do? ⏳](#18--pause-again-what-did-we-just-do-)
  - [1.9 ⛙ Merge The Feature Branch Into Main ⛙](#19--merge-the-feature-branch-into-main-)
    - [Step 1.9.1 ⬅️ Check Out The Main Branch ⬅️](#step-191-️-check-out-the-main-branch-️)
    - [Step 1.9.2 ⛙ Merge Away! ⛙](#step-192--merge-away-)
  - [1.10 ⏳ Pause Pt. 3: The Pausening ⏳](#110--pause-pt-3-the-pausening-)
- [ Section 2: Github](#-section-2-github)
  - [2.1 ⏫ Uploading A Repo ⏫](#21--uploading-a-repo-)
    - [Step 2.1.1 🌤️ Create A Repo In The Cloud 🌤️](#step-211-️-create-a-repo-in-the-cloud-️)
    - [Step 2.1.2 📋 Copy The Address For Your Cloud Repo 📋](#step-212--copy-the-address-for-your-cloud-repo-)
    - [Step 2.1.3 🔗 Link Your Local Repo To The Remote 🔗](#step-213--link-your-local-repo-to-the-remote-)
    - [Step 2.1.4 ⬆️ "Push" Your Changes To The Remote ⬆️](#step-214-️-push-your-changes-to-the-remote-️)
  - [2.2 ⏳ Pause: Did It Work? ⏳](#22--pause-did-it-work-)
  - [2.3 🔄 Workflow Moving Forward 🔄](#23--workflow-moving-forward-)
  - [2.3 ⏬ Downloading A Repo ⏬](#23--downloading-a-repo-)

## <img src=./img/git_icon.png width="100"/>  Section 1: Git
Git is a "version control" tool. This means we can use it to keep track of and manage changes that we make to our code. 

Git lets us safely try out modifications to code, without losing the version that works. It also allows us to "stitch together" all the best bits from various versions of our software. 

This might sound a bit abstract, so let's work through an example together.

---

### 1.1 🧹 Some Housekeeping 🧹
If you followed the instructions in our first ever lesson to the letter, you will have created a conveniently-located folder to hold your classwork. Let's check that it exists now:

<details>

<summary>

#### Step 1.1.1 🏡 Go To Your Home Directory 🏡

</summary>

---

Open the terminal, and issue the following command:

```bash
cd ~
```

> :information_source: **NOTE** :information_source:\
> That squiggly line is called a "tilde" (pronounced "til-duh"). You can type it by holding `Shift`, and then pressing the button next to the number 1 at the top of your keyboard.

This command navigates you to your "home" directory. That's the directory set aside for your personal files and folders.

---

</details>

<details>

<summary>

#### Step 1.1.2 🎓 Make Sure You Have A Directory For Your Class Work 🎓

</summary>

---

Enter this command:

```bash
ls
```

This will print the contents of your home directory on the screen. You should see a directory listed among them called `she_codes/`. 

> :exclamation: **IMPORTANT** :exclamation:\
> If you don't see one, you can create it now with:
>
> ```bash
> mkdir she_codes
> ```

---


</details>


<details>

<summary>

#### Step 1.1.3 🧭 Navigate Into Your Classwork Directory 🧭

</summary>

---

Now that we're certain that your `she_codes` directory exists, navigate into it with this command:

```bash
cd she_codes
```

---

</details>


<details>

<summary>

#### Step 1.1.4 📁 Create A Directory For Today's Work 📁

</summary>

---

We need a directory to hold our work for this lesson. You can create one and simultaneously navigate into it by entering the following command:

```bash
mkdir git_and_github && cd $_
```

> :information_source: **NOTE** :information_source:\
> `$_` is a little trick to let us avoid typing `git_and_github` twice. It is like saying "use that last value that I gave you again" to the shell. 
> 
> So this command says: "create a directory called `git_and_github`, and then immediately change directory into that same folder".

You should now be here:
```
~/
|
├─ she_codes/
| |
| ├─git_and_github/   <--- You are here
```

Ok, we are now ready to begin! What we just did is a good way to begin any class where we work on a new project. Jump to your classword directory, and then make a new folder to hold the code for that project.

---


</details>

---

### 1.2 - 🌄 Initialisation 🌄

We are going to turn our `git_and_github/` directory into a "Git Repository". That's what we call a directory that is version controlled with Git. 

This is another good thing to do each time we start work on something new.

<details>

<summary>

#### Step 1.2.1 🗂️ Initialise The Directory As A Git Repo 🗂️

</summary>

---

Run the following command:

```bash
git init
```

This "initialises" the folder as a Git repo. 

---

</details>

<details>

<summary>

#### Step 1.2.2 👀 Inspecting Our New Git Repo 👀

</summary>

---

This step isn't required every time you initialise a new repo, but it's useful this time just to see what that command did. Let's look at the contents of our new repo with this command:

```bash
ls -A
```

> :information_source: **NOTE** :information_source:\
> The `-A` there is a "flag". It adds optional extra functionality to the command. In this case, we are asking the shell to list ALL of the contents of the current directory, including hidden files and folders.

Here's what you should see:

![The terminal, with an output that just says `.git/`](./img/ls_results.png)

Hidden files and directories have names that begin with a dot. We can see that Git has created a hidden directory for us called `.git/`. This directory stores all the files that Git uses for keeping track of changes to our files. We don't need to open it right now - Git will handle it for us.

> :stop_sign: **CAUTION** :stop_sign:\
> We **won't** be working *inside* the `.git/` directory. It is just there to let Git do its thing. We will be creating all of the files and folders we need inside the `git_and_github/` directory, and `.git/` will just sit there alongside them. Watching. Waiting. 👀👀👀

> :warning: **WARNING** :warning:\
> Try to avoid a situation where one Git repo gets created *inside another one*. This can cause some very weird and confusing problems. 
>
> **Correct Structure:**  
> In general, you want to keep all the files for each project inside one "umbrella" directory, and make that umbrella directory your git repo. When you start a new project, make a new umbrella directory for it, next to your other projects. Like this:
>
> ```
> she_codes/
> ├─ html_intro/
> │  ├─ index.html
> │  ├─ styles.css
> |
> ├─ git_and_github/        <--- This is a git repo!
> │  ├─ README.md
> │  ├─ .git/
> |
> ├─ profile_site_project/  <--- This is a git repo!
> │  ├─ index.html
> │  ├─ styles.css
> │  ├─ README.md
> │  ├─ .git/
> ```

---

</details>

---

### Step 1.3 🌱 The Initial Commit 🌱
Git handles changes that we make to our files by storing them in "commits". Each commit represents a set of changes - a bit like a snapshot of our progress. 

We need to create an initial commit, so that we have a "starting point" to build on for our future changes. 

<details>

<summary>

#### Step 1.3.1 📄 Create A Blank File 📄

</summary>

---

Let's create a blank file to be in our initial commit. Run the following command:

```bash
touch README.md
```

> :information_source: **NOTE** :information_source:\
> The `touch` command creates a new file with the name supplied.

Now open the current directory in VS Code like so:

```bash
code .
```

Here's what you should see:

![A blank file called `README.md` in VS Code](./img/blank_file.png)

---

</details>

<details>

<summary>

#### Step 1.3.2 🕵️ Check The Status 🕵️

</summary>

---

We won't be adding any code yet - we'll let our initial commit just contain a blank file. Jump back into the terminal and run the following command:

```bash
git status
```

Here's what you should see:

![The results of running `git status` in the terminal - `README.md` is marked as an untracked file.](./img/initial_status.png)

So, Git can see that we have created a new file in the repository, but it isn't yet keeping track of those changes. If we want to add them to a commit, we need to put them in Git's "staging area". This is a holding zone for the changes we add to our commits.

---

</details>

<details>

<summary>

#### Step 1.3.3 📥 Add The New File To The "Staging Area" 📥

</summary>

---

To stage changes to a file, we use the `git add` command. Give it a go:

```bash
git add README.md
```

Now try checking the status again:

```bash
git status
```

![The results of running `git status` in the terminal - `README.md` is now marked as a change to be committed.](./img/second_status.png)

Looking good!

---

</details>

<details>

<summary>

#### Step 1.3.4 💾 Make The Commit 💾

</summary>

---

We are now ready to make our first commit! Here's the command:

```bash
git commit -m "initial commit"
```

> :information_source: **NOTE** :information_source:\
> The `-m` flag lets us add a "commit message" - a little explanation of what changes are in this commit. The text inside the quotation marks is the message. It's important to supply a message every time - Git will make your life difficult if you don't.

Here's the result of running that command:

![The result of creating our first commit.](./img/initial_commit.png)

Nice! We have a blank canvas to build on now. 

---

</details>

---

### 1.4 🪴 A Second Commit 🪴
Let's make a real change now!

<details>

<summary>

#### Step 1.4.1 📝 Adding Some Code 📝

</summary>

---

Go back to VS Code, add some text to `README.md`, and save the file. Here's a suggestion for what you can add:

```md
# Git Demonstration
Here are some useful commands for Git:
* `git init`: initialises a directory as a Git repo
* `git status`: checks the status of a Git repo
* `git add some_file_name`: adds `some_file_name` to staging
* `git commit -m "some message"`: creates a Git commit with "some message" as the commit message 
```

Don't forget to save the file!

> :information_source: **NOTE** :information_source:\
> The code we have added is in a language called "Markdown". It's quite extremely useful, and we will see it again in this course. Luckily, Markdown is so close to normal English that we don't need to be familiar with it to understand what's being said here.

---

</details>

<details>

<summary>

#### Step 1.4.1 🕵️ Check The Status Again 🕵️

</summary>

---

Let's check the status again! 

```bash
git status
```

![The results of running `git status` a third time. This time there are more unstaged changes to `README.md`.](./img/third_status.png)

Our new changes have been noticed by Git, but once again they aren't automatically staged. This is good, because sometimes there will be new changes that we don't want to add to our next commit! In this case, though, we **do** want to include this change in our next commit, so...

---

</details>

<details>

<summary>

#### Step 1.4.2 📥 Add To Staging Again 📥

</summary>

---

Add that change to staging! Same command as before:

```bash
git add README.md
```

Just to prove that it worked, let's check the status again. You don't need to do this every time, but it's a good demonstration for now:

```bash
git status
```

![The results of running status yet again. This time the changes to our file have been added to staging.](./img/second_staging.png)

Note that before our staged changes were marked with `new file:`, whereas now they register as `modified:`. Git is savvy!

---

</details>

<details>

<summary>

#### Step 1.4.3 💾 Make That Commit! 💾

</summary>

---

k, let's make our second commit. This time we need to include a different message:

```bash
git commit -m "added some useful hints on how to use Git to the README"
```

![The results of our second Git commit. This time the commit notes that 6 insertions were made.](./img/second_commit.png)

---

</details>

---

### 1.5 ⏳ A Pause To Take Stock ⏳
Let's just take a look at what we've done so far. In the pre-work video entitled "What Is Git", you were shown a graph that looked like this, depicting some commits:

![Three commits represented as a graph.](./img/what_is_git_video/7_graph_head.drawio.png)

We can't get quite such a pretty representation in the terminal, but we can get close. Try running this command:

```bash
git log --graph
```

Here's what I see:

![The Git graph, represented in the command line. Two commits are represented by asterisks, tagged with details describing them, and linked by a dotted line.](./img/git_log.png)

This is pretty much what we had above - it has just been rotated by 90 degrees, and rendered as text-art. The initial commit is at the bottom, and our second commit is above it. Each commit is represented by an asterisk. 

Of course, the working tree isn't represented in our command line graph. But the working tree is just "the current state of our code", and we can see that by looking at the files in VS Code!

Not bad!

> :information_source: **NOTE** :information_source:\
> In the "What Is Git" video, we mentioned that Git can be used to revert a previous mistake. We won't be demonstrating that here, because we don't want to get bogged down. If you'd like to see a demo of that (plus some other helpful techniques), [take a look at our video on useful Git techniques]().

```diff
- ^^Gonna need to make that video then too...
```

---

### 1.6 🌵 Create A Feature Branch 🌵
We've got some good progress in our repo here. We'd like to add some more, but we don't want to risk breaking what we already have by adding untested new code.

We've only been operating on the main branch so far. Let's create a new branch to hold our new changes. Once we are happy with them, we can merge them in.

A branch that we create to add new content or functionality to our code is called a "feature branch". In this case the feature that we're adding will just be more text in the `README.md` file, but that's ok! From little things, big things grow.

<details>

<summary>

#### Step 1.6.1 🌱 Create The New Branch 🌱

</summary>

---

Run the following command in the terminal:

```bash
git branch my_new_branch
```

> :information_source: **NOTE** :information_source:\
> Here `my_new_branch` is the name we are giving to our new branch!

---

</details>

<details>

<summary>

#### Step 1.6.2 🕵️ Take A Look At The Current Branches 🕵️

</summary>

---

Just so we are orientated, let's see what branches we have right now. To do this, you can run this command:

```bash
git branch
```

Since we didn't supply the name of a new branch, Git will just list all the currently available branches for us.

![A list of current branches in the terminal. There are two: `main`, and `my_new_branch`.](./img/current_branches.png)

The asterisk here indicates that we are currently operating on the `main` branch. If we want to work on our new feature in the other branch, we'll need to change that...

---

</details>


<details>

<summary>

#### Step 1.6.3 ➡️ Check Out The New Branch ➡️

</summary>

---

When we swap to a different branch in Git, we call it "checking out" the branch. We can do it with the following command:

```bash
git checkout my_new_branch
```

---

</details>

---

### 1.7 🛠️ Develop A Feature 🛠️
We created this branch to introduce new code into the repo, so let's do it!

<details>

<summary>

#### Step 1.7.1 📝 Write The Code 📝

</summary>

---

Hop back over to VS Code. You should see the same contents in the `README.md` file as you did before, since right now our two branches are identical to one another. 

Let's change that. Here's a modification to make to the file:

```diff
# Git Demonstration
Here are some useful commands for Git:
* `git init`: initialises a directory as a Git repo
* `git status`: checks the status of a Git repo
* `git add some_file_name`: adds `some_file_name` to staging
* `git commit -m "some message"`: creates a Git commit with "some message" as the commit message 

+ Some more commands:
+ * `git log --graph`: displays a graph of the commits in your repo
+ * `git branch`: lists the current branches in your repo
+ * `git branch some_branch_name`: creates a new branch called "some_branch_name"
+ * `git checkout some_branch_name`: moves the HEAD to the most recent commit on the branch called "some_branch_name"
```

Make sure you save your work!

---

</details>


<details>

<summary>

#### Step 1.7.2 📥 Stage The Changes 📥

</summary>

---

You can use `git status` to check what files have changed if you'd like. That's a good idea when you've made complex changes or it has been a while since your last commit.

In this case, though, we know exactly what has changed, and there's only one file we need to stage. So let's run that command:

```bash
git add README.md
```

---

</details>

<details>

<summary>

#### Step 1.7.3 💾 Make The Commit 💾

</summary>

---

This should be getting familiar! Here's that command again, this time with a different commit message:

```bash
git commit -m "added some extra examples of git commands to the readme"
```

---

</details>

---

### 1.8 ⏳ Pause Again: What Did We Just Do? ⏳

We just branched off an "alternate timeline" from our main branch, and added a commit to it. That means that we have two possible states for our repository, and we can flip back and forth between them by swapping branches.

The state of our repo now looks something like this:

![A diagram showing the "my_new_branch" branch forking off from the "main" branch.](./img/before_merge.drawio.png)

> :information_source: **NOTE** :information_source:\
> We're showing it to you in this format because the Git log graph doesn't draw lines where there are no commits. So it won't show you the forking path, since the `main` branch hasn't has any commits since the one marked with a blue circle here.
>
> You can still take a look at the Git graph, it'll just be a bit less helpful.

---

### 1.9 ⛙ Merge The Feature Branch Into Main ⛙
It's go time! Our "feature" is complete, and we are happy with how it looks, so let's merge it into the "canonical" version of our code - the `main` branch.

<details>

<summary>

#### Step 1.9.1 ⬅️ Check Out The Main Branch ⬅️

</summary>

---

To start with, we have to jump back to the `main` branch, since we want to merge our changes into it. 

You can do that with this command:

```bash
git checkout main
```

> :exclamation: **IMPORTANT** :exclamation:\
> The batch we are **in** is always the batch that will have changes applied to it in a merge. So, since we want to add the changes *from* `my_new_branch` *to* `main`, we needed to "check out" the main branch before merging!

---

</details>

<details>

<summary>

#### Step 1.9.2 ⛙ Merge Away! ⛙

</summary>

---


Ok, time to merge. Here's the command for that:

```bash
git merge my_new_branch
```

Here's what you should see:

![The result of the merge - the readout says "1 file changed, 7 insertions, 1 deletion".](./img/merge.png)


---

</details>

---

### 1.10 ⏳ Pause Pt. 3: The Pausening ⏳

Where are we now? What have we done so far?

1. We had some code on our main branch.
1. We split off a feature branch to test some new code.
1. We liked our new code, so we merged it into the main version.

Here's a diagram representing where we are at:

![A diagram depicting a feature branch splitting off from `main`, having a new commit added to it, and then merging back in.](./img/merge_diagram.drawio.png)

> :information_source: **NOTE** :information_source:\
> As before, you can take a look in the Git log, but since it doesn't draw lines that con't have commits in them, the bottom path between our blue commit and the merge won't appear.

This is great. But right now, all of the code is stored on your computer. What happens if you drop your laptop off a bridge? And if someone else wants to contribute to your work, how can they send you their additions?

For that we'll need something extra...

---

## <img src=./img/github_icon.png width="100" /> Section 2: Github

Github is a cloud-based version control tool. It combines with Git to give you super-powered control over your code, from anywhere on the planet.

With GitHub, you can upload your Git repositories to the internet, share them with whomever you want, and choose who is allowed to make changes to them.

Today we will just cover the basics, but later on down the line we will come back and expand our powers.

---

### 2.1 ⏫ Uploading A Repo ⏫

Right now we have a repository on our machine that we want to get onto GitHub. We'll look at how to do that first. Then later on we will show you how to get a repo from GitHub onto your local machine.

<details>

<summary>

#### Step 2.1.1 🌤️ Create A Repo In The Cloud 🌤️

</summary>

---

Head to [GitHub](https://github.com/). You may need to log into your account for this.

> :exclamation: **IMPORTANT** :exclamation:\
> If you haven't set one a GitHub account yet, now is the time! Then, after class you should check the [student handbook]() for information on how to get set up with a GitHub Student account. You'll need one later in the course!

Oh the main homepage you'll find a `New` button in the left hand pane like so:

![The New Repo button on GitHub](./img/new_repo_button.png)

Give it a click, and assign your repository a useful name. I recommend `"intro_to_git"`. 

> :stop_sign: **CAUTION** :stop_sign:\
> You can add a description if you want, but you should leave the rest of the form blank for now. We will be uploading content from our computer, so we don't want to block it with autogenerated content from GitHub.

Here's how your form should look when you submit it:

![The Create Repository form on GitHub](./img/create_repo.png)

---

</details>

```diff
- Need to add a link to the student handbook when in the section above
```

<details>

<summary>

#### Step 2.1.2 📋 Copy The Address For Your Cloud Repo 📋

</summary>

---

Clicking the `Create Repository` button should redirect you to your new repo. It will be empty for now, so you'll just see a screen with some `"Quick Setup"` tips.

Near the top of the page is a link you can copy. Grab it now - we are about to need it.

![The empty repository screen with the repo link circled.](img/link_to_copy.png)

---

</details>

<details>

<summary>

#### Step 2.1.3 🔗 Link Your Local Repo To The Remote 🔗

</summary>

---

The git repository you have on your local machine is called your **"local"** repo. The one on GitHub is called the **"remote"** repo.

We want to establish a link between them so that we can sync up the changes between them.

Jump into the terminal again, and run the following command, pasting the link you just copied from GitHub in the relevant spot:

```bash
git remote add origin YOUR_PASTED_LINK_HERE
```

This establishes the link between the repositories. Your local repo now knows that there is a repository on GitHub to match it. 

> :information_source: **NOTE** :information_source:\
> We told Git that the remote repo should be labelled `"origin"` here because that's considered normal practise, but technically you could call it anything. You'd just need to swap the new name into the command. 
> 
> Most of the time `"origin"` is the right choice unless you're doing something complicated.

---

</details>

<details>

<summary>

#### Step 2.1.4 ⬆️ "Push" Your Changes To The Remote ⬆️

</summary>

---

Let's send all our changes up to Github, so that it contains a backup of all the work we've done so far. 

The command for that is easy:

```bash
git push origin main
```

> :information_source: **NOTE** :information_source:\
> We specify `main` here, because we are pushing just the main branch. We could push a different branch if we wanted, but we don't have any other branches we care about right now. 
>
> We've also named the remote repo we are pushing to - as expected, it's `origin`!

---

</details>

---

### 2.2 ⏳ Pause: Did It Work? ⏳
Refresh the browser page on GitHub. You should see the readme file that you wrote locally.

You'll note that the Markdown code we created has been tastefully rendered. Nifty!

![The successfully pushed code displayed on GitHub](./img/successfully_pushed.png)

Under the green `<> Code` button, you can see that we've made three commits on this file. (In my case, I made them last week, because I've been working on this lesson for a little while.) 

We can also see from the top left that we are on the `main` branch, and that only one branch has been pushed to this remote repo so far.

If there were more files in the repo we would be able to explore them too, but let's keep things simple for now.

---

### 2.3 🔄 Workflow Moving Forward 🔄
Once you have established a local repo and hooked it up to GitHub, where do you go from there?

Here's a normal workflow.
1. Make a new branch to experiment with changes on.
2. Make incremental commits on the branch until you've completed the modification you set out to make. 
3. Merge the feature branch into `main` once you're satisfied.
4. Push your branches to Github often, to make sure they're backed up.
5. Once one feature is completed, start work on a new one!

---

### 2.3 ⏬ Downloading A Repo ⏬
Now that we've covered the case where you created the repo on your home machine and needed to back it up on GitHub, let's cover the other alternative.

What if you have a repo on GitHub that you want to copy down onto your local machine? 

Luckily, it's quite easy.

<details>

<summary>



</summary>

---



---

</details>

<details>

<summary>



</summary>

---



---

</details>