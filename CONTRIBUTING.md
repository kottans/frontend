[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)
  
# Contributing

We want to encourage all students and mentors to get involved
with the development of this course. The materials here are
mostly developed and curated by the mentors team but we admit
that we may miss things, or occasionally get them wrong.
We've put together some guidelines that should help you
get started with making contributions.

Thanks for helping improve this course for everyone!

## Questions, concerns, or issues

If you've got a question or problem that you think others may
have, then please read this first.

The GitHub issue tracker is our preferred channel for dealing
with these questions. It keeps questions public and allows
others to pitch in with potential solutions,
it also means everything is documented for the future.
This should not be used for personal questions or issues
unfit for public discussion, in those instances we encourage
you to contact the member of mentors team responsible for
this course.

Before submitting a new issue, use the GitHub search
(or just browse through [open issues](https://issues) or
[closed issues](https://issues?q=is%3Aissue+is%3Aclosed))
to see if it has already been submitted before.
If it hasn't, then go ahead and create a new one.
When creating a new issue, please spend some time
creating an identifiable and specific
title, then provide as much detail as possible in the main
description.

Examples of bad titles:
* _Problem with materials for current phase_
* _Question about the course_
* _Just a thought..._
* _Can't complete one task_

Examples of good titles:
* _Task Intro to JS: broken Extra materials link_
* _Assignment Pizza App submission of 30th Feburary is incorrect_
* _Object-Oriented JavaScript missing source repository_

## Amendments, corrections, and contributions

Contributions are so gratefully received. If you've noticed
an error, or would like to add additional resources then
please use a pull request. To ensure your pull request
is accepted as quickly as possible, please take a moment
to check the following guidelines. Once a pull request
has been submitted, it can be reviewed by fellow students
and mentors. When a mentor (or normally at least two)
thinks it looks good, it'll be accepted and merged in.

### General guidelines

* Ensure any added resources are properly cited like similar
  material. This may be adding a link to the resource in
  a task description, or appending a full citation to
  an assignment.
* If you're adding a task then, please, do the following:
  - use either of existing tasks as a template
  - give a suggested task file some meaningful name
  - place the task file under `tasks/`
  - follow the structure common for all tasks
  - keep badges
  - also list the task in [`tasks/README.md`](tasks/README.md).
    If you aren't sure to what phase to add the task to, then
    just list it somewhere under
    **New tasks suggested for the remote phase** or
    **To Be Assigned** sections. Please, feel free adding any
    comments.
* In your PR comment give a comprehensive description of
  what and why you're suggesting to add, or refer to an issue
  (e.g. `Resolves #121`).

### Commits

Please ensure your PR initially has 1 or 2 commits,
3 as a maximum. Otherwise please squash your commits
into fewer well separated commits.
It's important that commits are atomic to keep the history clean.
Below you will find a short guide on squashing commits into a clean history. 
Please read through and follow [Chris Beams's - How to write a git commit message](http://chris.beams.io/posts/git-commit/).

1. Run `git log --oneline master..your-branch-name | wc -l`
   to see how many commits there are on your branch.
1. Run `git rebase -i HEAD~#` where # is the number
   of commits you have done on your branch.
1. Use the interactive rebase to edit your history.
   Unless you have good reason to keep more than one
   commit, it is best to mark the first commit
   with 'r' (reword) and the others with 's' (squash).
   This lets you keep the first commit only, but change
   the message.

If your commit resolves some issue then please refer the issue.
This will get issue closed automatically upon merge.
Commit message example:

```
Fixed broken link to w3schools in Intro to HTML & CSS

Resolves #111
```

Note a blank line before `Resolves...`. Everything after a
blank line will be considered supplementary information
not normally required to show up when anyone browses
commits history with compact output.

### Never made any Pull Requests before?

Piece of cake!

Consider completing
[Kent C. Dodds' How to Contribute to an Open Source Project on GitHub course](https://egghead.io/courses/how-to-contribute-to-an-open-source-project-on-github)
(14 lessons, each ~3 mins long)

## Credits

- [BlueHatbRit/EDU-CONTRIBUTING.md](https://gist.github.com/BlueHatbRit/3bd366313f7ca2c7d2537d927ec970e8)
- [PurpleBooth/Good-CONTRIBUTING.md-template.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426)
