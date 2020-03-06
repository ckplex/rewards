# Everything around PR's in [brave-core](https://github.com/brave/brave-core)


## Checklist for creating PR
- move issue that this PR is resolving in In Progress column on global board
- how to handle CI failure (with skip labels)
- draft PR (try to do it as soon as possible, don't wait for everything to be done so that you don't loose work)
- skip labels in general
- checklist that needs to be done
- assigning milestones
- uplifts
- commits (squashing and keeping clean history)
- review request via our tag (move it in Review column on global board)
- wait for CI before approving
- if you change code ask for re-review (no automatic review dismissal)
- you are responsible for PR to be reviewed
- always check CI (yes it can take multiple tries), if CI failed on not related things add a note to the PR

## Checklist for reviewing PR
- it follows our coding standard and chromium ones (https://google.github.io/styleguide/cppguide.html)
- CI passed or make sure that there is a note about failure 
- it has test plan in the PR
- it has `feature/rewards` label
- it has `QA/Yes` or `QA/No` on the issue that this PR is resolving
- always go through test plan locally so that you can confirm that is working as expecting
- try to find edge cases that PR could introduce
- if you have questions contact creator and go through the PR with him
