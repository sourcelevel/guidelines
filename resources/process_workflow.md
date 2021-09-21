Process Workflow
================

## Introduction

In this section we want to describe our process to create the User Stories and tasks in the Shortcut board.

### User Story cards

Each card in Shortcut is called User Story (Story), it can be:

*   Feature
*   Chore
*   Bug

`Chores` are the things you have to do that don’t actually change your product.

Examples include paying down technical debt, improving test coverage,
upgrading library dependencies, research, devops tasks like spinning up new servers,
database maintenance, operational tasks, writing scripts to automate those tasks, etc.

We like to create the `Feature type` as SMART tasks instead of INVEST stories, so we can move short but meaningful tasks through the Shortcut board.

Each Feature task is linked to an Epic card, but we create this Epic card as an INVEST Story.

Pay attention to the SMART meaning so you can create a nice described/sized task:

*   Specific: The goal should target a specific area of improvement or answer a specific need.
*   Measurable: The goal must be quantifiable, or at least allow for measurable progress.
*   Attainable: The goal should be realistic, based on available resources and existing constraints.
*   Relevant: The goal should align with other business objectives to be considered worthwhile.
*   Time-bound: The goal must have a deadline or defined end.

Be sure not to create a task such as "create a input field", or "create an API", because it may be too small and you may miss the point of what you are developing.

All SMART tasks should be linked to a User Story, which should be properly detailed with its goal (it can be written using the User Story pattern), Acceptance criteria, and BDD if necessary.

We are following Gherkin syntax to describe our User Stories:

### Title:

```
[Verb] [What] [Where]

Examples:
- Fix typo in Dangerzone
- Investigate problems in GitLab Sync
- Add search field to repositories listing in Dangerzone
```

### Description:

```
- Scenario:
- Given
- And
- When
- Then
```

### Epic cards

The type Epic will be considered INVEST Stories to us.

You can follow the script in this link to create the User Story text and the BDD scenarios: https://forrest.netlify.com/#/

Pay attention to what INVEST stands for:

*   Independent (of all others)
*   Negotiable (not a specific contract for features)
*   Valuable (or vertical)
*   Estimable (to a good approximation)
*   Small (so you won't take months to complete a single User Story)
*   Testable (in principle, even if there isn’t a test for it yet)

## Stages

*   Unscheduled
*   Ready for Development
*   In Development
*   Ready for Review
*   Ready for Test
*   In Test
*   Ready for Deploy
*   Completed

### Unscheduled

Everyone is welcome to create stories in this column, feel free to suggest new features,
adjustments or report bugs. It's important to detail stories as much as possible, to
guarantee that everyone has enough information to work on it.

You can upload files to use as example, add labels and select the project for it.

### Ready for Development

All story cards are prioritized based on importance vs effort to accomplish it.

### In Development

When the User Story is in this stage and due some reason it can't be moved to
Ready For Review stage, add `blocked` label to the card leaving it in this stage.
Also, comment on the User Story card explaining why it got blocked.

### Ready for Review

When moving cards to this stage, you should have a working solution and an open Pull
Request available for review.

### Ready for Test

After your Pull Request is approved or all comments answered, you can move
the story card to this stage then someone will test it.
