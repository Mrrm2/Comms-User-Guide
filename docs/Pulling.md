# Pulling and Resolving Merge Conflicts

Since GitHub is a collaborative platform, others can contribute to a repository as well. You may find that the copy of the repository on your computer is different from what is on GitHub. Therefore, it is important to know how to pull changes from a remote repository and resolve merge conflicts. This guide will walk you through the process of pulling changes from a remote repository and resolving merge conflicts.

## Pulling from a remote repository

1. First, navigate to the directory on your local machine where you want to store the files from the repository. You can do this in the terminal or command prompt by using the “cd” command. For example, type “cd Documents/GitHub/my-repo” to navigate to a directory called “my-repo” in your “Documents/GitHub” folder.

2. Next, use the “git clone” command to clone the repository from GitHub to your local machine. To do this, copy the URL of the repository from GitHub and paste it into the terminal after the “git clone” command. For example, type “git clone https://github.com/username/repo.git” to clone a repository called “repo” from a user called “username” on GitHub.

3. After cloning the repository, navigate into the repository’s directory using the “cd” command. For example, type “cd repo” to enter the “repo” directory.

4. Use the “git pull” command to pull any changes made to the repository since you cloned it. For example, type “git pull origin master” to pull changes from the “master” branch of the repository. This will update your local repository with the latest changes from GitHub.

5. If there are any merge conflicts between the changes you pulled and the changes you made locally, you will need to resolve them before you can commit and push your changes back to GitHub. You can check if there are any conflicts by using the “git status” command. Conflicts will be marked as “both modified” or “unmerged” files. If there are no conflicts, you can skip to the next section.

## Resolving merge conflicts

1. To resolve conflicts, open the file(s) with conflicts in a text editor and look for the conflict markers, which look like “<<<<<<<”, “=======”, and “>>>>>>>”. These markers indicate where the changes from both sides of the conflict begin and end.

2. Edit the file to resolve the conflict by keeping the changes you want and deleting the markers and conflicting lines. Save the file.

3. After resolving all conflicts, add the changes to the staging area using the “git add” command. For example, type “git add file-with-conflicts.txt” to add a file called “file-with-conflicts.txt” to the staging area.

4. Use the “git commit” command to commit the changes with a message describing the conflict resolution. For example, type “git commit -m ‘Resolve merge conflict in file-with-conflicts.txt’”.

5. Finally, use the “git push” command to push your changes back to GitHub. For example, type “git push origin master” to push changes to the “master” branch of the repository.
