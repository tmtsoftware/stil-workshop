# stil-workshop
Workshop scratch area for demo purposes

* author: [Emmanuel Joliet](ejoliet@ipac.caltech.edu)

## Demos

Will demo:

* github tool: graphs, pull request, code review
* commits and pushes
* branches and merging

In order to do that, git concept will be introduced such as:

* git clone
* fork
* commits, pushes
* branching

## Hands-on

Participants will then do the follwoing steps:

* clone the repos locally on their end (need git software installed)
  * `git clone https://i[username]@github.com/tmtsoftware/stil-workshop.git`   
  * default landing branch should be `master`
   * `git status` to check on which branch you are

* create your feature/ticket branch from `master` 
  * `git checkout -b [branch name]`
* edit and change one line of the file in this repos named [scratch.txt](scratch.txt)
* Persist your changes in your branch: add/commit
  * `git add .`
  * `git commit -m"[your message]"`
* continue changing/adding/commit and check the differences:
  * `git diff`
  * Check your commit history: `git log` or more fancy `git log --decorate --graph`

* OPTIONAL: if no commit to be made, at that point, you can: pull or rebase
  * after pulling, check branches pulled: `git branch --all`

* Once done, push to server (`-u` means start tracking)
  * `git push -u origin [branch name]`

* in github.com, button 'pull request' should appear
  * I will pick one and show a pull request / code review
  * I will show how to request changes (and what to do)
  * Go ahead and play around

* OPTIONAL if request change, need to go to the branch, and
  * change file, git add / commit / (rebase -i to squash) / push

* show approve changes and merge from github

* if merge conflict (tipycally same line have changed in the meantime: github will suggest commands and guidelines to solve and merge locally

### References:

* [Git documentation](https://git-scm.com/docs)
* [Github guides](https://guides.github.com)
* [Useful git tips & tricks](https://git-scm.com/book/en/v1/Git-Basics-Tips-and-Tricks)
* [Leave message in Slack #workshop](https://tmt-stil.slack.com/messages/C4JV40FRD)

