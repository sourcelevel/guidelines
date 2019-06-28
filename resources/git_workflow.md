Git Workflow
============

We follow some patterns on creating branches and this is related to our workflow in `ClubHouse`.

If you didn't read [Pull Requests](https://github.com/sourcelevel/guidelines/blob/master/resources/pull_requests.md), we recommend to read it before this guide.

## Introduction

### User Story

Each card in ClubHouse is called User Story (Story), it can be:

* Feature
* Chore
* Bug

`Chores` are the things you have to do that don’t actually change your product.

Examples include paying down technical debt, improving test coverage,
upgrading library dependencies, research, devops tasks like spinning up new servers,
database maintenance, operational tasks, writing scripts to automate those tasks, etc.

### Stages

* Unscheduled
* Ready for Development
* In Development
* Ready for Review
* Ready for Test
* In Test
* Ready for Deploy
* Completed

#### Unscheduled

Everyone is welcome to create stories in this column, feel free to suggest new features,
adjustments or report bugs. Its important to detail stories as much as possible, to
guarantee that everyone has enough information to work on it.

You can upload files to use as example, add labels and select the project for it.

#### Ready for Development

All story cards are prioritized based on importance vs effort to accomplish it.

#### Ready for Review

When moving cards to this stage, you should have a working solution and an open Pull
Request available for review.

#### Ready for Test

After your Pull Request is approved or all comments answered, you can move
the story card to this stage then someone will test it.

## Branches

We work with a single stable branch: `master`. Everything that is merged into it, we assume that already passed in the `Test phase` properly.

Now that you're familiar with `User Story`, let's understand how it reflects our branches and accordingly to our Pull Requests:

### User Story

#### User Story card

First, we create a branch using `master` as the base with the following pattern:

* `chddd/user-story-card-title`

Where `ddd` stands for Story Card number in ClubHouse, check some examples of naming User Story branches:

* `ch897/collect-issues-line-numbers`
* `ch569/edit-reviewer-author`
* `ch642/clustering-contribution-data`

#### More than a single branch

If you realize that a single branch won't be enough, you can create more branches to detail
your work of this User Story card. For example, let us imagine the following scenario:

We have a User Story `Collect issues line numbers` which its number in ClubHouse is `123`.

![https://github.com/sourcelevel/guidelines/blob/master/images/user_story_flow.png](https://github.com/sourcelevel/guidelines/blob/master/images/user_story_flow.png)

In this case, we can start creating the branch for it using `master` as the base:

```
git checkout -b ch123/collect-issues-line-numbers
```

After analyzing the requirements we noticed that a single Pull Request would carry too many
changes. So we've decided to break down our changes in n pull requests, to do so we start
creating a new branch using `ch123/collect-issues-line-numbers` as the base, then create the
new one:

```
git checkout -b ch123/xz-add-database-migrations
```

Where `xz` stands for initials of developer, check some examples of naming sub User Story branches:

* `ch321/wt-fix-reviews-count-in-repository-page`
* `ch781/gg-remove-sales-machine-from-subscriptions`

If you developed that change in pair programming, you can use both initials ordered alphabetically:

* `ch821/gg-wt-add-call-to-action-to-landing-page`

Note that you're able to open new branches and Pull Requests as you consider necessary on working in a User Story card.
To decide that, always keep in mind: how easy would be to review your code, so Pull Request size will be your guide.