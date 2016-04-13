# git-standup

> Recall what you did on the last working day ..or be nosy and find what someone else did.

## Original project

This is a fork of the [git-standup](https://github.com/kamranahmedse/git-standup) from kamranahmedse. 
Got and check it out if you feel the original verison is more suitable for your needs;

## Install

You can install it either using CURL

```bash
$ curl -L https://raw.githubusercontent.com/Kerruba/git-standup/master/installer.sh | sudo sh
```

Or by cloning and manually installing it

```bash
$ git clone https://github.com/Kerruba/git-standup.git
$ cd git-standup
$ sudo make install
```

## Usage

All you have to do is run `git standup` in a repository or a folder containing multiple repositories

## Single Repository Usage

Head to the project repository and run

```bash
$ git standup
```

<!-- ![git standup](http://i.imgur.com/wyo4s9E.gif) -->

## Multiple Repository Usage
Open a directory having multiple repositories and run

```bash
$ git standup
```

<!-- ![git standup](http://i.imgur.com/RT25cT9.gif) -->

This will show you all your commits since the last working day in all the repositories inside. 


## Standup options

This fork of the repo let you define both the span you want to look for and the author. I've did this because I need more control
on which logs I want to return;

You can define a specific "since" variable:

```bash
# Considering commits in the last 2 weeks
$ git standup "last 2 weeks"
```

You can have a look to other people commits:

```bash
# Considering commits from 'John Doe' in the last 2 weeks
$ git standup "last 2 weeks" "John Doe"

# Considering yesterday commits from 'John Doe'
$git standup "" "John Doe"
```

## Motivation

The original version of the command is great, but not suitable for all my cases. Since I have to fill weekly reports about my job,
I found it easier to specify the time interval I want to check in order to "remember" what I've done;

## License

MIT © [Kamran Ahmed](http://kamranahmed.info)
