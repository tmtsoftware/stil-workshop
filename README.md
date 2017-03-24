# stil-workshop
Workshop scratch area for demo purposes

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
** `git clone https://i[username]@github.com/tmtsoftware/stil-workshop.git`   
** check your landing branch: `git status`, should be `master`
* create branch from `master` 
** `git checkout -b [branch name]
* edit and change one line of the file named [scratch.txt](scratch.txt)
* add/commit
** `git add .`
** `git commit -m"[your message]"`
* continue changing/adding/commit and check the differences:
** `git diff`
* OPTIONAL: if no commit to be made, at that point, you can: pull or rebase
* Once done, push to server
** `git push -u origin [branch name] 
* in github.com, button 'pull request' should appear
* will pick one and show a pull request / code review
* show how to request changes (and what to do)
** change file/ add / commit / push
* show approve changes and merge from github
* if conflict: see github for guidelines

### References:

* [Git documentation](https://git-scm.com/docs)
* [Github guides](https://guides.github.com)
* [Emmanuel Joliet](ejoliet@ipac.caltech.edu)
* [Slack workshop](https://tmt-stil.slack.com/messages/C4JV40FRD)

