# `git-blame-bob`

`git-blame-bob` is a simple `git` plugin that lets you target the blame for code
you did or didn't write.

## Motivation

Ever wonder, **_Who wrote this garbage code?_** Sure, you could find out with `git blame`,
but even if it wasn't *Bob*:

* Maybe **Bob** approved that garbage in code review.
* Maybe **Bob** could've mentored the author on writing less-garbagey code.
* Maybe **Bob** helped foster a culture of shipping garbage.
* Maybe **Bob** put pressure on deadlines that lead to the garbaginess.
* ~~Maybe~~ **Bob**'s written things **much, much worse**.

Code completely yanked from [git-self-blame](https://github.com/JacobEvelyn/git-self-blame). Credit goes there.

![It works, I swear.](https://user-images.githubusercontent.com/1114569/36355517-754d5ff0-14b2-11e8-9ca1-7a51150bca37.gif)

## Features

* Symlink or change the name of the script to match your coworkers. Bob's out this week, better prepare: ```ln -s git-blame-bob git-blame-vivian```
* Doesn't change your `git` history or configuration or anything else. This is a real tool, not some joke to mess up your whole repo.
* Definitely works in Bash and Zsh. Probably works in most other shells?
* Accepts any arguments that `git blame` accepts.
* Can be safely run in parallel with other `git` commands (including
  other `git self-blame` commands).

## Installation

```bash
git clone https://github.com/ccraciun/git-blame-bob.git
cd git-blame-bob
export PATH=$PATH:$(pwd)

# If you want to actually use this more than once, add this
# to your PATH in a more permanent place, like your
# `~/.bashrc` or `~/.zshrc` files.
```

## How does it work?

There's a handy walkthrough
[in the source](https://github.com/JacobEvelyn/git-self-blame/blob/master/git-self-blame)!

## Who are you?
I'm just a guy who had an idea and stole the code from Jacob. In Jacob's words:
> I do a lot of [humor writing](https://medium.com/@jacobevelyn) and
> [tech writing](https://medium.freecodecamp.org/@jacobevelyn) and
> [code writing](https://github.com/JacobEvelyn), and you can blame me for all
of it.
