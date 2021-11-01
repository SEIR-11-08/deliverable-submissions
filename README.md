# Submitting Deliverables

We will have you follow these steps when copying down the deliverable assignments and then submitting them.

## Pulling Down the Assignment 

<br/>

1. From the class schedule, click on the link for the deliverable assignment you want to start working on. (Right clicking on the link will give you the option to open in a new tab.)

![Link from class schedule](./images/class-schedule.png)

<br/>

-----------------------------------------

This will take you to the repo for that assignment. _Notice the top right corner indicates that the repo is on the class account and not your own account._

![Assignment repo](./images/assignment-repo-class-account.png)

<br/>

2. From here click on the "Fork" button in the top right corner of the page. This will Create a copy of the repository on your own account.

![Assignment repo](./images/assignment-repo-fork.png)

<br/>

---

3. From there you will prompted with a popup asking where you would like to "fork" the repo to. Select your own github account here.

![Assignment repo](./images/where-to-fork.png)

It will take a few seconds to copy the repository over from the classroom account to your own account.

---

We should now see the repository copied over. _Notice the top right corner indicates that you are now looking at the repository on your own account and not the class account._

![Assignment repo](./images/repo-on-our-account.png)

At this point we want to copy the repository from our account onto our own computers locally.

4. Click on the green button that says code. It should bring up a drop down with the Git URL for the repository on our own account. Click on the clipboard icon to copy the Git URL to your clipboard.


![Copy git url](./images/copy-git-url.png)
<p><strong>** Note:</strong> Be sure to click on "SSH" before copying the url!</p>

---

If you haven't already, create a directory in your `sei` directory called `deliverables` to store all of your deliverable assignments.

5. In your terminal navigate to your `deliverables` directory and type `git clone` and then paste in the Git URL you copied from your clipboard.

The command will look something like this.
```bash
git clone git@github.com:msolorio-ga/HW-Loops-Conditionals.git
```
Run that command and git will create a new directory with the name shown in the URL. In this case the directory will be called HW-Loops-Conditionals.

If everything went through successfully you should be able to see the new directory created by running the `ls` command.

<br/>

![see new directory](./images/see-new-dir.png)

<br/>
By running `git clone <your-git-url>`, you've copied, or "cloned", the repository from your Github account to your own your own computer.

6. Use the `cd` command to step into your cloned repository.

7. Once inside the repository run `ls -a`.

You should see all of the files that exist in the repository. You will also notice `.git`. This indicates that this is infact a Git repository. Git has 
already been initialized and we do not need to run `git init`.

<br/>

![cd into directory](./images/cd-into-dir.png)

<br/>

---

<br/>

8. Running `git remote -v` will list out all of the remotes for the repository. It should display an origin remote that points to the Git URL you cloned from.

When you are ready to push your work back to Github you will push to this origin remote.

![origin remote](./images/origin-remote.png)

<br/>

From here, you are ready to start working on the assignment.

<br/>

---

<br/>

## Working on the Assignment

<br/>

1. Open the repository in your code editor.

2. Follow the instructions for the assignment, committing your work as needed.

<br/>

<details>
  <summary>A Reminder on Commands for Staging and Committing</summary>

  <br/>

  To move your changes to the staging area
  ```bash
  git add -A
  ```
  To commit your changes
  ```bash
  git commit -m 'write a message here that describes your changes'
  ```
</details>

<br/>

---

<br/>

## Submitting the Assignment

<br/>

Once you've completed all of the assignment double check that all of your work has been committed.

1. Run `git status`.

- If the output shows you files in red or green, add your changes to the staging area and/or commit your changes first. Then run `git status` to check if it went through.

- If the output of `git status` says "nothing to commit, working tree clean", all your work has been committed and you are ready to push your work to Github. 🙌

<br/>

---

<br/>

2. Run `git push origin main`. After a second or two you will see an output that looks like this.

<br/>

![git push origin master](./images/git-push.png)
<p><strong>** Note:</strong> The picture says "master" but you should use "main"!</p>

<br/>

3. You can now go back to the repository on your Github account. If you don't have it open any more you can click on your profile icon in the top right, and click on 'Your repositories' in the dropdown. From there you can find the repository for the assignment.

The page should indicate that this is the repository from your account.

<br/>

![repo on your account](./images/repo-our-account.png)

<br/>

---

<br/>

4. From this page, click on the "Pull requests" tab.

<br/>

![pull request tab](./images/pull-request-tab.png)

<br/>

---

<br/>

You will be taken to the "pull requests" page for the repo.

5. From here click on the green "New pull request" button.

<br/>

![new pull request](./images/new-pull-request.png)

<br/>

---

<br/>

6. You'll be taken to another page to create your pull request. Here you will be able to confirm that you're making a pull request from the repository on _your account_ into the repository on the _class account_. It should look something like this.

![confirm pull request](./images/confirm-pull-request.png)

<br/>

---

<br/>

7. Once confirmed click the green "Create pull request" button.

From there it will take you to a page to add a title to your pull request. Type your name here and click "Create pull request" from this page.

<br/>

![title pull request](./images/title-pull-request.png)

From there you are all set! You've just sumbitted the deliverable assignment.

You can double check that your pull request has been made by visiting the "Pull requests tab".

![pull request tab](./images/double-check.png)

From there you should your pull request on the list.
