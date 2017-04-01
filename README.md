# stil-workshop
Workshop scratch area for demo purposes

* author: [Emmanuel Joliet](https://tmt-stil.slack.com/team/ejoliet)

## Demo

The demo will cover:

* github tool: graphs, pull request, code review
* commits and pushes
* [branches and merging](https://www.atlassian.com/git/tutorials/using-branches)

Participants will need [Git](https://git-scm.com/) installed and some knowledge of `git` commands in order to follow the tutorial.

## Hands-on

Participants will be guided through the following steps:

1. **clone** the repos locally on their end (need git software installed)
  * `git clone https://[username]@github.com/tmtsoftware/stil-workshop.git`   
  * default landing branch should be `master` (default per repos)
    * `git status` to check on which branch you are

2. create your feature/ticket **branch** from `master` 
  * `git checkout -b [branch name]`, required unique branch name, usually formatted as `ISSUE-ID-meaningful-short-description`
    * For demo, let's append github `USERNAME` to branch name
  * for example, let's take a  ticket from JIRA board [DEMOSS1](https://tmt-project.atlassian.net/secure/RapidBoard.jspa?rapidView=14&projectKey=DEMOSS1&view=planning&selectedIssue=DEMOSS1-15)
    * my branch name will be DEMOSS1-EJOLIET-bug-fix
3. edit and **change** one line of the file in this repos named [scratch.txt](scratch.txt)
4. **commit** your changes in your branch: add/commit
    1. `git add scratch.txt`
    2. `git commit -m"[your message]"`
5. continue changing/adding/commit and check the differences:
    1. `git diff HEAD~0`
    2. Check your commit history: `git log` or more fancy `git log --decorate --graph`
    3. *OPTIONAL*: if no commit to be made, at that point, you can: pull or rebase
     * after pulling, check branches pulled: `git branch --all`
     * if `master` got new things, you will need to rebase in order to avoid conflict at the time you pull request

6. Once done of changes, **push** to server (`-u` means start tracking)
  * First time push: `git push -u origin [branch name]`
  * Your local branch is now synced with remote
  * Next pushes: `git push`

7. **Pull Request**: in github.com, button 'pull request' should appear
  * Show a pull request / code review
  * *OPTIONAL* Show a case of how to [request changes](https://help.github.com/articles/about-pull-request-reviews/)  (and what to do)
    * if request change, need to go to the branch, and
        * change file, git add / commit / (`rebase -i` to squash) / push (steps 3 to 6 above)
        * no rebase there because branch is already in server / no force push either

8. Show when approve changes and merge from github
  * Branch can be deleted from github after merged

9. OPTIONAL: If merge conflict (typically, same line have changed in the meantime: github will suggest commands and guidelines to solve and merge locally

10. Once merged, typically the branch can be deleted from github from the same pull request page.


### Need Help?

* [Installing Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
* [Git documentation](https://git-scm.com/docs)
* [Github guides](https://guides.github.com)
* [Useful git tips & tricks - autocompletion!](https://git-scm.com/book/en/v1/Git-Basics-Tips-and-Tricks)
* [Pull request template](https://help.github.com/articles/creating-a-pull-request-template-for-your-repository/)
* [Leave message in Slack #workshop](https://tmt-stil.slack.com/messages/C4JV40FRD)
* [Slack me](https://tmt-stil.slack.com/messages/@ejoliet)
