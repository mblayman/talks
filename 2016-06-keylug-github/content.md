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

# Step 1

Make an account at https://github.com.

--

**Seriously**, 
--
if you don't have an account, 
--
and you're a developer, 
--
and you have a computer
with access to the internet right now, 
--
*stop listening to me until you make an account*.

---

# Step 2

Create an ssh key and add your public key to GitHub.

https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/
