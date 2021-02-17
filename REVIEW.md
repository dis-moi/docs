# Review process
> This is a general process, a project specific process must be documented in its own repository.

We rely on peer review as much as possible :
> https://en.wikipedia.org/wiki/Peer_review

Try to be as benevolent as possible when reviewing your peers. 
Someone theorized about *Egoless programming* which fits our overall philosophy quite well.
> https://en.wikipedia.org/wiki/Egoless_programming

## Branch
When starting to work on a subject on any project, the first thing to do is creating your own branch.
The base branch should be `master` and the new branch should reflect the subject you are working on:
- a new feature must be prefixed by `feat/` ex: `feat/new-contribution-form`
- a bug fix can be prefiexed by `fix/`
Or `chore`, `docs` or any other word you see fit!

> We use Conventional commits for commit messages, and this branch naming is inspired by the keywords used there

## Commits
For commit messages we use the Conventional commits convention.
Beware, a single commit shouldn't break anything (whether the test, or the app, or anything).
We should be able to check out any commits and run the app without any issues.
Also, we should try to keep commits small. Try to include only the smallest amount of change that keeps it atomic. In other words, let's create commits that only do one thing.

> When unsure just squash everything.

## History
Keep your history clean! There can be many commits or only one, as long as the story told is consistent.
If you the history doesn't feel right, just be a negationist and use (and abuse) `git rebase -i`. 
Just as long as you don't overwrite other people's history it's fine (really).

And if you feel like, feel freer to `squash` your branch history into a single commit.

## Pull/Merge request
When ready you can open a Pull Request targeting the main branch.
> BTW shall we rename `master` to `main`?

OR not! You can open the PR as soon as you create your branch, 
this can be relevant to keep other team members posted. 
Just be sure to add the WIP keyword somewhere in the title and/or add the `WIP` label to your PR.

> Also if your PR relates to an issue in any way, don't forget to mention it (#42 for issue number 42)
> https://www.conventionalcommits.org/en/v1.0.0-beta.2/#commit-message-for-a-fix-using-an-optional-issue-number

> __Ultimate tip__ If your branch only contains one commit with a title and a body:
> ```
> doc: Add review document draft
> At last, here's the long-awaited documentation!
> ```
> The title and description of the PR will use this information.

## Reviewer - *the peer*
Depending on the subject of the PR, you can assign non-technical people as reviewers:
- member of the product team to review the docs, user stories or screenshots
- member of the comms team to review spelling, relevance of keyword use, images and wording
- member of UX-UI or graphical team to review images, screenshots, design and user stories in practice 
> to do this in the best way possible, feature branches should be deployed and testable somewhere.

- At least 2 reviewers should be assigned to a PR.
- Reviewers!
  - Please be diligent with your reviews! From our experience, PR which aren't reviewed quickly tend to wait... wait.. sometimes for months...even years! (I just closed a 7 year old PR recently)
  - Tip: If you don't understand anything you're reading, you might not be the right person for the job! And that's OK! 
  Just let us know and we'll help you understand or choose another person suited to the task (at least try to look for typos :) )
  - We love our work to be read by others (who said egoless?!) so please try to show you care and leave some comments in the diff!
- A PR should be merged in the next 72h? at most
- You must have at least one approval to merge a PR

### Unwritten rules (so far)
Mind the state of the review :
- approve
- comment
- request changes

If the PR is approved, it's approved period, even if there are comments left, its just mean it's not these notices aren't that important after all.
If one of the reviewers requests changes, the changes must be applied or the reviewer must be convinced otherwise until the PR is approved.
Once changes are applied, the PR author should then request a re-review (there is a button for that).

## Resources
There are plenty of excellent resources out there, so feel free to add anything relevant here.

## Tools
Any tools that could help folks to become a Git, Github power user?

- [Managing your work on GitHub](https://docs.github.com/en/github/managing-your-work-on-github)
- [Using Git](https://docs.github.com/en/github/using-git)
- [A Step-by-Step Guide to Git](https://opensource.com/article/18/1/step-step-guide-git)
- [How to become a Git expert](https://www.freecodecamp.org/news/how-to-become-a-git-expert-e7c38bf54826/)
