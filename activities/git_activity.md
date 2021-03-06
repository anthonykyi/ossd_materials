# `git` hands-on activity


Unless noted otherwise all content is released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).


## Notes for instructors

### Organization

Students should be working in groups of three, but they should not be working together. At the beginning of the class meeting, hand out cards to student. The card should have  a group name and member number (those combinations should be unique). A sample
set of 12-team cards is included in this repository.
Students in the same team, should be distributed within the room - this way they are collaborating using the repository only.

If your class size is not a multiple of three, then allow some groups to be of size 4. The activities for member 4 below are
limited and optional, so any team without member 4 will be just fine.

### Setup

Create an empty repository for each team in the class organization on GitHub. The students should have permissions to write to these repositories.



## Activity

### Introduction
In this activity, you will collaborate with two or three other people. All of you are going
to be working with the same repository.
As different team-members make changes to the content repositories you will encounter some
issues. The objective of this activity is to learn how to resolve different types of issues
that may arise when collaborating with other people.

### Instructions

- If the instructions below state "create a file and commit", you should create a file, then
add it to the staging area and commit using a descriptive message:

  ```
  git add FILE_NAME
  git commit -m "MESSAGE FOR THE COMMIT"
  ```
- If the instructions below state "push changes to the remote repository", you should make sure that all the latest changes are committed (see above) and then push those changes:  

  ```
  git push origin master
  ```

- If you run into any problems while completing different rounds of this activity, raise
your hand and we will try to help out as quickly as we can.

### Actual Activity

<table>
<tr> <th>round</th><th> member 1</th><th>  member 2</th><th>  member 3 </th><th>  member 4 </th> </tr>

<tr>
<td colspan=5 align=center>

__Working with multiple files and multiple users__

</td>
</tr>

<tr>
<td>1 </td>
<td colspan=4>  

clone the team repository to a local machine

`git clone REPO_URL`

</td>
</tr>
<tr>
<td>2 </td>
<td >

create a `README.md` fie, it should contain a top level heading with a team name, commit the file and push it to the remote repository  

</td>
<td>

create a `LICENSE.txt` file, select one of the available software licenses, commit the file and push it to the remote repository  

</td>
<td>

use [Wikimedia Commons](https://commons.wikimedia.org/) to locate an image that will serve as a mascot for your team; download the file, add it to the repository and commit the file, (remember where you got the file from, you will need that information later)

</td>
<td> </td>
</tr>
<tr>
<td>3 </td>
<td colspan=4>

- create a new empty file named with your own name (I would create a file called `joanna.md`), for example,
- add the file to the repository, commit and push changes to the remote repository,

</td>
</tr>
<tr>

<td colspan=5>

In the last two steps, most of you should have encountered some issues when you tried pushing to the remote.
Since several people push changes to the same repository, most of you tried to push after someone else modified that remote repository. In many cases `git` can figure out how to combine
the changes made by different people. But, you will need to execute `git pull` to update
your local copy of the repository to the latest version of the remote repository.

</td>
</tr>

<tr>
<td colspan=5 align=center>

__Resolving merge conflincts__

</td>
</tr>

<tr>
<td>4 </td>
<td colspan=4 >

- Run `git pull` to synchronize your local repository with the remote one.
- In your local repository you should have the file called `README.md` right now.
- Edit the `README.md` file by adding your name to the file right below the name of the
team.
- Commit the changes and push them to the remote repository.  
</td>
</tr>

<tr>
<td colspan=5>

At this point, multiple users modified the same lines of the same file. `git` can no
longer resolve these changes on its own. The human-user intervention is necessary.
This is a __merge conflict__. To resolve it, the user has to edit the file manually
and decide which of the changes should be merged and which should be removed.

As you are resolving the merge conflicts manually, make sure that all of your
team-mates names end up being listed in the `README.md` file exactly once.

</td>
</tr>

<tr>
<td colspan=5 align=center>

__Managing forks and remotes__

</td>
</tr>


<tr>
<td>5 </td>
<td colspan=4>

- fork the team's repository to your own account  

- add your own fork address as the remote for your local repository: in the local repository run the command

    `git remote add myfork URL_TO_THE_FORK`

    where `URL_TO_THE_FORM` is replaced by the actual url

- run the command

    `git remote -v`

    and record the results in the body of your file (the one with your name in it)

- commit the changes to the file that you just edited  and push them to the `myfork` remote

    `git push myfork master`

- look at the files stored in the original repository in the course organization and in
your private fork, they should be different

</td>

</tr>







<tr>
<td> </td>
<td>

</td>
<td>

</td>
<td>

</td>
<td>

</td>

</tr>




<tr>
<td>4 </td>
<td colspan=4>

</td>

</tr>


</table>
