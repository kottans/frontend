[![MIT Licensed][icon-mit]][license]
[![Awesome][icon-awesome]][awesome]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![Telegram][icon-chat]][chat]

# Advanced git
**Enhance your git skills**

This task is optional.
You don't need it to advance further in the course.
However, you will definitely apply newly acquired skills
in your future work.

## Pre-requisites

You already some have hands-on experience with:
 * [ ] creating, forking and cloning repos
 * [ ] committing changes
 * [ ] pulling, fetching and, hopefully, rebasing
 * [ ] basic branching
 * [ ] pushing to remotes
 * [ ] creating PR
 * [ ] collaborating with others and/or yourself :wink:

Basically, you have successfully completed this course
[entry task](git-intro.md) and
[git collaboration task](git-collaboration.md)

## Topics

1. Commit often. How often and why?
1. Branching for experiments and easy roll-back. Fail no fear!
1. Oh shit, git! Undoing things.
1. `merge` vs `rebase`. Which is when.
1. Squash 'em all!
1. Never, ever, ever rewrite history! Or?
1. Conflict resolution. Peace!
1. Collaboration work flows
1. Issue Driven Development

Some topics above are really short, others take time
for they are better comprehended when practising.

## Materials

 * At [Learn git branching](https://learngitbranching.js.org/)
   refresh your skills:
   - Main: Moving Work Around, Advanced Topics
   - Remote: all exercises
 * git flows
   - [A successful Git branching model @nvie](https://nvie.com/posts/a-successful-git-branching-model/)
   - [Issues with "nvie" git-flow](http://scottchacon.com/2011/08/31/github-flow.html)
   - [Understanding the GitHub flow](https://guides.github.com/introduction/flow/)
   - [Introduction to GitLab Flow](https://docs.gitlab.com/ee/workflow/gitlab_flow.html)
   - [git-flow vs github-flow vs gitlab-flow](https://stackoverflow.com/questions/18188492/what-are-the-pros-and-cons-of-git-flow-vs-github-flow/35915110#35915110)
   - [OneFlow - a Git branching model and workflow](https://www.endoflineblog.com/oneflow-a-git-branching-model-and-workflow)
   - [Comparing Workflows @Atlassian](https://www.atlassian.com/git/tutorials/comparing-workflows)
   - [DM Development Workflow with Git, GitHub, JIRA and Jenkins](https://developer.lsst.io/processes/workflow.html)
   - [Git Workflows for Pros: A Good Git Guide](https://www.toptal.com/git/git-workflows-for-pros-a-good-git-guide)
 * git automation tools:
   - [hub from github](https://hub.github.com/)
   - [gitflow-avh](https://github.com/petervanderdoes/gitflow-avh)
   - [git-town](https://github.com/Originate/git-town)
   - [lazygit](https://github.com/jesseduffield/lazygit)
   - [git aliases](https://git-scm.com/book/en/v2/Git-Basics-Git-Aliases)
   - [gitalias](https://github.com/GitAlias/gitalias)
 * [Advanced Git Tricks :clapper:](https://vimeo.com/49444883)
 * [Git Patterns and Anti-Patterns](https://dzone.com/refcardz/git-patterns-and-anti-patterns?chapter=1)
 * [Oh shit, git!](http://ohshitgit.com/)
 * [How to undo (almost) anything with Git](https://blog.github.com/2015-06-08-how-to-undo-almost-anything-with-git/)
 * [Flight rules for git](https://github.com/k88hudson/git-flight-rules)
 * [GitHub Learning Lab](https://lab.github.com/courses):
   - [Reviewing pull requests](https://lab.github.com/githubtraining/reviewing-pull-requests)
   - [Managing merge conflicts](https://lab.github.com/githubtraining/managing-merge-conflicts)
 * [Rebase techniques](https://gist.github.com/OleksiyRudenko/232e1ebe6ed0780fc69d7391723cc75b)
 * [Merging repos](https://gist.github.com/OleksiyRudenko/3324acdab15fff52955979522c878a3e) &
   [Repo import and export back](https://gist.github.com/OleksiyRudenko/86d378b56fe690e47a066b8eeb4ac5b2)
 * [How to publish `dist/*` only on github pages](https://gist.github.com/OleksiyRudenko/7e94aa2d18927e0c5e65b2b5a1c0e375)
 * [octotree](https://github.com/ovity/octotree) // [Chrome github navigation plug-in](https://chrome.google.com/webstore/detail/octotree/bkhaagjahfmjljalopjnoealnfndnagc?hl=en-US)
 * [Скринкаст по git :clapper::clapper::clapper:](https://learn.javascript.ru/screencast/git)
 * [A Visual Git Reference](https://marklodato.github.io/visual-git-guide/index-en.html)
 * [_placeholder for workshop videocast_](#)

---

## Side notes

You don't need to read the notes below. These
are rather a collection of possible theses.

<details><summary>TL;DR</summary>

* Commit often
  - break your code base into smaller files
  - scope a commit to an individual file;
    may be 2+ files if a new module is introduced
    and immediately used/referred to elsewhere
  - think of collaboration and possible conflicts
* Branching
  - branch, fail, checkout back
  - branch naming patterns; scoping using `/` delimiter
  - you may not need the branch after merger
  - specify the commit scope in a message; branches
    are just pointers
  - `git stash`
* Undoing things
  - `git branch`
  - `git reset --mixed|soft|hard`
  - `git revert`
  - cherry pick
* `merge` / `rebase`
  - `merge` vs `rebase`
  - `git merge --no-ff branch`
  - cherry picking
  - what actually `rebase` is
* Squash 'em all!
  - keep issue references on squash/fixup
  - rebasing work flow
* History rewriting
  - remote as a WIP storage
  - killing branches on remote
  - force pushing squashed
* Conflict resolution
  - update from target branch before merging into it
  - `merge` vs `rebase`, hello again
  - cross check the result using diff with a back-up
    branch
* Collaboration work flows
  - nvie, github, gitlab, fork-PR
  - tools: `git-town`, git aliases
  - shortcuts from JetBrains WebStorm
* Issue Driven Development
  - add a feature/enhancement as an issue
  - refer to the issue on commit
  - issues as tasks in your IDE
* Misc
  - git config/aliases collection
  - sub-tree, sub-repo
  - merging repos
  - `push-dir` to publish
  - gists...
  - Git Credentials Storage
  - tags, releases

</details>


[icon-chat]: https://img.shields.io/badge/chat-on%20telegram-blue.svg
[icon-mit]: https://img.shields.io/badge/license-MIT-blue.svg
[icon-awesome]: https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg

[license]: https://github.com/Kottans/web/blob/master/LICENSE.md
[awesome]: https://github.com/sindresorhus/awesome#front-end-development
[chat]: https://t.me/joinchat/CX8EF1JmLm9IM6J6oy2U7Q
