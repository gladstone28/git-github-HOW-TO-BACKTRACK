link to lesson:
https://www.codecademy.com/journeys/full-stack-engineer/paths/fscj-22-building-interactive-websites/tracks/fscj-22-git-and-github-part-i/modules/wdcp-22-important-git-operations-da30bb5a-8cd0-4294-b963-9841dd1c22db/lessons/git-backtracking/exercises/git-checkout-1

HOW TO BACKTRACK
git checkout
5 min
What if you decide to change the ghost’s line in the working directory, but then decide you wanted to discard that change?

You could rewrite the line how it was originally, but what if you forgot the exact wording? The command

```
git checkout HEAD filename

```
will restore the file in your working directory to look exactly as it did when you last made a commit.

Here, filename again is the actual name of the file. If the file is named changes.txt, the command would be
```
git checkout HEAD changes.txt
```

### Instructions
Checkpoint 1 Passed
1. Change the ghost’s words in some way. Here’s a fun suggestion:

Ghost: 
My hour is almost come,
When I to sulphurous and tormenting balloons
Must render up myself. 

Checkpoint 2 Passed
2. From the terminal, use git diff to see the difference between scene-5.txt as it appears in the working directory vs. how it appears in your last commit.

You may need to press q on your keyboard to restore the terminal.

Checkpoint 3 Passed
3. Use the new Git command to restore the file in your working directory to look as it did when you last made a commit.

Close the scene-5.txt file and then re-open it to see that the changes you had previously made to the ghost’s line have been discarded.

Hint


To revert changes that you have made to a file, use the following command:

git checkout HEAD filename
