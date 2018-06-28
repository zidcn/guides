# CONTRIBUTING

## High level guidelines:
- Be consistent.
- Be patient.
- Don't rewrite existing code to follow this guide. Unless you are doing code refactoring.
- Don't violate a guideline without a good reason.
- A reason is good when you can convince the team.
- Don't hesitate to ask when it's necessary. It's necessary when:
  - you've worked on a problem for some time.
  - you've tried the best you can.
  - you are not very confident or you have no idea at all.
  - you don't know what to do.

## Naming conventions
- Be consistent.
- Be short.
- Be accurate.
- Be explicit.
- Again, don't heisitate to ask when you need inspiration.

## Coding style
- Follow the existing code(good parts).
- When in doubt, check the following guides:
  - [ruby-style-guide](https://github.com/rubocop-hq/ruby-style-guide)
  - [rails-style-guide](https://github.com/rubocop-hq/rails-style-guide)
- Ask someone if you are still confusing.


## Workflow
We use GitHub issues with(out) milestones, PR, releases and a `CHANGELOG.md` to manage the development and releases in production.

### Releases and Changelog
1. Releases
    - We tag every release with a version number and update them on GitHub.
2. Changelog
    - We sumarizes changes in `CHANGELOG.md` under the corresponding version.
    - A version with date means it's been released to production already.
    - A version without date means we're still working on it.
    - You should never add/edit changes under a version with date.

### Issues and milestones
We always keep three milestones open:
- long term: has issues we are going to deal with for a long time.
- The next minor version: has issues we are currently working with. It will be closed once it's released.
- The next of next minor version: has issues scheduled for the next phase. A new future-plan milestone will be opened when it replaces the current-working milestone.

For example, the current release on production is v1.3.1. So we'll have the three milestones open:
- long term
- v1.4
- v1.5

Issues without a mileston means we haven't schedule it yet.


### Pull requests(PR)

1. Start a new branch(keep the name short, simple, and meaningful) from:
    - `master`: For small changes or a simple feature we want to deploy it very soon.
    - a feature branch: For big changes or a complex feature which need to be tested thoroughly.
2. Start coding and commiting. Remember rebase your working branch frequently from the base branch(`master` or the feature branch mentioned in 1.).
3. Before submit your PR
    - Rebase from the base branch(in 1.).
    - Improve/Re-organize your commit history using interactive rebase(`git rebase -i`). Some tips:
        - Decide which changes should be in which commit(s) wisely.
        - Squash redundent commits such as `Fix typo`
        - Write a [good commit message](https://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html). Example format:
            ```
            Present-tense summary under 50 characters

            * More information about commit (under 72 characters).
            * More information about commit (under 72 characters).

            http://project.management-system.com/ticket/123
            ```
    - Make sure all tests are passed(`rails test` and `rails test:system`)
4. Submit your PR
    - One issue/change one pull request.
    - Put necessary details in your comment and reference the related issue.
5. Ask person for a review:
    - Approval: your PR will be merged to the right branch.
    - Request changes: you should ammending your commits(or close the PR and start a new one) and repeat steps start with 3.