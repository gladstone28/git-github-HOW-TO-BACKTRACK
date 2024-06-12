link to lesson:

https://www.codecademy.com/journeys/full-stack-engineer/paths/fscj-22-building-interactive-websites/tracks/fscj-22-git-and-github-part-i/modules/wdcp-22-important-git-operations-da30bb5a-8cd0-4294-b963-9841dd1c22db/lessons/git-backtracking/exercises/git-reset-1


### HOW TO BACKTRACK

## git reset I

Great! The files you’ve added to the staging area belong in the same commit.

What if, before you commit, you accidentally delete an important line from scene-2.txt? Unthinkingly, you add scene-2.txt to the staging area. The file change is unrelated to the Larry/Laertes swap and you don’t want to include it in the commit.

We can unstage that file from the staging area using

```
git reset HEAD filename

```
This command resets the file in the staging area to be the same as the HEAD commit. It does not discard file changes from the working directory, it just removes them from the staging area.

Instructions
Checkpoint 1 Passed
1. To try out the new command, let’s make a mistake on purpose!

The code editor is open to scene-2.txt. Delete any line from the file and click Run.

Checkpoint 2 Passed
2. From the terminal, add scene-2.txt to the Git staging area.

Checkpoint 3 Passed
3. Now check the status of the Git project.

In the output, notice scene-2.txt under “Changes to be committed”.

Checkpoint 4 Passed
4. Use the new Git command to unstage scene-2.txt from the staging area.

Notice in the output, “Unstaged changes after reset”:

```
M   scene-2.txt

```
- M is short for “modification”

5. Now that changes made to scene-2.txt have been booted out of the staging area, you’re ready to commit. From the terminal, make a commit to save the Larry/Laertes name swap in hamlet.

