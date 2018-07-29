---
title: Git
tags: programming vcs
---

{% include stub %}

{% include wikilink topic="Git (software)" %}

Using git without a server
--------------------------

When in an environment that doesn't have internet access, you can push and pull
code to/from a place on your filesystem (such as a USB drive). This is great
for sharing code at a competition.

First, you need to create a 'bare' repo to push/pull to. Insert your USB drive, let's say you're on Windows and the drive is E. Open a terminal.

```
E:
git init --bare repo
```

Next, you have to point your source checkout to it (do this from each computer that needs it). To do this, you need to create a 'remote' in your local checkout. You've probably noticed that when using git we often type the word 'origin'. Turns out, this is the default remote usually created when you initially clone a repo.

```
cd path\to\repo
git remote add usb E:\repo
```

Finally, you have to push code to it. The idea is `git push <remote name> <branch name>`. So...

```
git push usb master
```

Pulling is the same.

```
git pull usb master
```

You can do all of your normal git things. Just where you would often type 'origin', you can type 'usb' now. There are some shortcuts and some limited gotchas, but it's been in my experience the best way to share code at a competition without using internet.
