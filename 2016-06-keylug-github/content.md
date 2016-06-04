class: center, middle

# How To GitHub

#### KeyLUG June 2016

Matt Layman [@mblayman](https://twitter.com/mblayman)

---

# Topics

1. Git
--

2. GitHub

---

# Why version control?

--

team-project
--
.v2.8
--
.johns-comments
--
.edit-3
--
.kates-redlines.7
--
.oh-please-stop-the-pain.docx

---

class: center, middle

# Git - A Primer

???
Here we'll cover a history of Git
and where it fits into the scheme of version control.

---

# FOSS VCS history

--
* rcs (1982)
--

* cvs (1990)
--

* svn (2000)
--

* bzr (2005) (distributed)
--

* hg (2005) (distributed)
--

* git (2005) (distributed)

--

and a host of others along the way

--

* 2005 was apparently a very good year
--

* Dishonorable mentions: ClearCase, Visual SourceSafe

---

# Distributed VCS (DVCS)

### What makes the distributed concept so powerful?

* Most operations are local to your machine<br>
  (i.e., OMG FAST)
* Incentivizes good development practices
  (short lived, feature branches)
* Resilient to data loss
--

¯\\\_(ツ)\_/¯ (mostly a nice side effect)

---

class: center, middle

# That's enough backstory

---

# Install

Ubuntu 16.04

```bash
$ sudo apt install git  # apt-get on older versions
```

Fedora

```bash
$ sudo yum install git-all
$ # YMMV, I don't run Fedora so I took this from the internet.
```

OS X

```bash
$ brew install git  # After doing the Homebrew install dance.
```

---

# Configure

```bash
$ git config --global user.name "Jane Smith"
$ git config --global user.email "jane.smith@gmail.com"
```

--

Global configuration data is stored in `~/.gitconfig`.

--

```ini
[user]
        name = Jane Smith
        email = jane.smith@gmail.com
[color]
        ui = true
```

--

For all the gory details

```bash
$ git config --help
```

---

class: center

# Let's Rock

![Vader Rockin' Out](rock.jpg)

---

# GitHub

It is *the* default place to look for Git repositories
in the software industry.

So... why?

---

# Because

* First to market?
* Clever product name?
* Cute mascot?

--

Honestly, it doesn't matter. They have developer mindshare.

---

# Make an account

https://github.com

--

**Seriously**
--
, if you don't have an account
--
, and you're a developer
--
, and you have a computer
with access to the internet right now
--


*Stop listening to me until you make an account!*

---

# Handle SSH keys

* Create an ssh key.
* Add your public key to GitHub.

https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/

---

class: center, middle

# Fork a repo

---

# Cloning

--

Your local clone should be the *upstream* repository.

--

IMO, this is an easier workflow than having a local clone
of your *forked* repository.

---

class: center, middle

# A Tale of Two Features

---

# Local upstream

1. Create a branch
2. Fix issue A
3. Get fix merged in GitHub (remote) master
4. **Pull to local master**
5. Create a branch
6. Fix issue B
7. Get fix merged in GitHub (remote) master

---

# Local forked

1. Create a branch
2. Fix issue A
3. Get fix merged in GitHub (remote) master
4. **Merge upstream master into forked master**
5. Create a branch
6. Fix issue B
7. Get fix merged in GitHub (remote) master

---

class: center, middle

# Pull Requests

They're great. Let's do some.

---

class: center, middle

# Thanks!

Matt Layman [@mblayman](https://twitter.com/mblayman)
