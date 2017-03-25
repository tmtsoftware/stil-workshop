# stil-workshop
Workshop scratch area for demo purposes

* author: [Emmanuel Joliet](ejoliet@ipac.caltech.edu)

## Demos

Will demo:

* github tool: graphs, pull request, code review
* commits and pushes
* [branches and merging](https://www.atlassian.com/git/tutorials/using-branches)

In order to do that, git concept will be introduced such as:

* git clone
* fork
* commits, pushes
* branching

## Hands-on

Participants will then do the follwoing steps:

1. clone the repos locally on their end (need git software installed)
  * `git clone https://i[username]@github.com/tmtsoftware/stil-workshop.git`   
  * default landing branch should be `master`
    * `git status` to check on which branch you are

2. create your feature/ticket branch from `master` 
  * `git checkout -b [branch name]`
  * for example, let's take a  ticket from JIRA board [DEMOSS1](https://tmt-project.atlassian.net/secure/RapidBoard.jspa?rapidView=14&projectKey=DEMOSS1&view=planning&selectedIssue=DEMOSS1-15)
3. edit and change one line of the file in this repos named [scratch.txt](scratch.txt)
4. Persist your changes in your branch: add/commit
   1. `git add .`
   2. `git commit -m"[your message]"`
5. continue changing/adding/commit and check the differences:
   1. `git diff`
   2. Check your commit history: `git log` or more fancy `git log --decorate --graph`
   3. OPTIONAL: if no commit to be made, at that point, you can: pull or rebase
     * after pulling, check branches pulled: `git branch --all`
     * if `master` got new things, you will need to rebase in order to avoid conflict at the time you pull request

6. Once done, push to server (`-u` means start tracking)
  * First time push: `git push -u origin [branch name]`
  * Following pushes: `git push`

7. in github.com, button 'pull request' should appear
  * I will pick one and show a pull request / code review
  * I will show a case of how to [request changes](https://help.github.com/articles/about-pull-request-reviews/)  (and what to do)
  * OPTIONAL if request change, need to go to the branch, and
    * change file, git add / commit / (`rebase -i` to squash) / push (steps 3 to 6 above)
    * no rebase there because branch is already in server / no force push either

8. Show when approve changes and merge from github

9. if merge conflict (tipycally same line have changed in the meantime: github will suggest commands and guidelines to solve and merge locally

### References:

* [Git documentation](https://git-scm.com/docs)
* [Github guides](https://guides.github.com)
* [Useful git tips & tricks](https://git-scm.com/book/en/v1/Git-Basics-Tips-and-Tricks)
* [Leave message in Slack #workshop](https://tmt-stil.slack.com/messages/C4JV40FRD)

