link to lesson:

https://www.codecademy.com/journeys/full-stack-engineer/paths/fscj-22-building-interactive-websites/tracks/fscj-22-git-and-github-part-i/modules/wdcp-22-important-git-operations-da30bb5a-8cd0-4294-b963-9841dd1c22db/lessons/git-backtracking/exercises/git-reset-2


### HOW TO BACKTRACK

## git reset II

Creating a project is like hiking in a forest. Sometimes you take a wrong turn and find yourself lost.

Just like retracing your steps on that hike, Git enables you to rewind to the part before you made the wrong turn. You can do this with:

```
git reset commit_SHA

```
This command works by using the first 7 characters of the SHA of a previous commit. For example, if the SHA of the previous commit is 5d692065cf51a2f50ea8e7b19b5a7ae512f633ba, use:

```
git reset 5d69206

```
HEAD is now set to that previous commit.


### Instructions
Checkpoint 1 Passed
1. From the terminal, print out your Git commit log.

Note: If your cursor gets stuck in “git log” mode in the terminal, press q on your keyboard to escape.

2. From the terminal, enter the command to reset to a previous commit, using the first 7 characters of one of the past commit SHAs in your Git log.

Next, print the Git commit log again.

Notice anything interesting? The commits that came after the one you reset to are gone. The HEAD commit has been reassigned. You just changed history.

Hint

Make sure you don’t use the SHA of the most recent commit, as this will not result in anything resetting! You’ll need to use the SHA of a previous commit. You can use the dates in the log to determine the order in which the commits were published.

