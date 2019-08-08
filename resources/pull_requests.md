Pull Requests
=============


Pull Request (PR) or Merge Request (MR) in GitLab, is a great
tool to review and discuss solutions and implementations.

All changes made in any repository should be integrated using a Pull Request.
This will help the entire team to know what is being delivered and help
each other in improving code quality and propagate knowledge between developers.

## Opening Pull Requests

### Title

You can use the following pattern for the title:

```
Example of a nice PR title
```

* Title must be capitalized and conjugated in the present
* Title must be 50 chars or less
* You don't need to worry about User Story number in the title, since it is present
in branch name

### Description

* Describe what you did/why you did it using description field remembering that reviewers need
your context to review your PR

We already have some Pull Requests templates according to the repository, feel free to
suggest enhancements for them.

### Labels

Labels are a great way to organize different types of PR

* Always use labels to allow filtering and better usability in listing
do code review
* Select a label that best describes the purpose of PR

### Reviewers

* You can select the whole team you're working with or people individually. As we use
[Pull Reminders](https://pullreminders.com/), it will take care about notifying everyone
* Sure that, if you want, you can indicate `Reviewers` that has more knowledge about that
piece of code you're changing or ask for some extra guidance on it
* Select as Reviewer who didn't participated of development of the code

### Assignees

Assignees are members that worked with you in your PR or specific issues.

* Select yourself and people that pair programmed with you

## Receiving reviews

As everyone will be able to review your changes, discussions will be raised, code samples will
be shown, experiences will be shared. Everything is part of the review process.

When opening a Pull Request and being reviewed, consider the following:

* Create a well-explained description. When writing, try to describe the changes to a person
who is not in the context of the problem
* If your change includes any UI changes, consider adding a screenshot on its description
* Answer to questions and comments that will come
* Don’t take it personally. Nobody is doing it in order to make you feel bad or let you
uncomfortable among other developers
* Always be humble. Learn from your mistakes and try to create notes of your common mistakes
if realize that you're committing it more than once or twice
* Make sure you fully understand the other alternatives before choosing one of them or keeping
the solution you’ve provided. If you did not fully understand why somebody asked you to change
something, ask for explanations and/or examples.
* Avoid interrupting your co-worker to ask for reviews if you already send it in your Slack's `#dev`
channel (except for `expedite` tasks).
* Be kind :green_heart:

## Reviewing Pull Requests

* Look out for code smells (From the Wikipedia definition: `[code smells] indicate weaknesses in design
that may be slowing down development or increasing the risk of bugs or failures in the future`) that
should be removed to avoid future problems with the apps.
* Share, whenever possible, different solutions for a given problem through pointing code examples.
The examples can come from another project or written by you just for illustration purposes.
* Don’t be afraid of asking for documentation when necessary. Many times the discussions generated
by a Pull Request should be added to the project in the form of documentation, even things related
to specific parts of the code or the development workflow of the project. We should not let important
decisions to exist only in the form of Pull Request comments since other
developers might have a hard time searching through old Pull Requests to find the reasons behind
an existing implementation or design.
* If in the middle of discussion you find something interesting to document, do it. The entire team
will be thankful for that.
* If the Pull Request goals and motivations aren’t clear for you, ask the Pull Request author for
a better description and explanations. Remember that Pull Requests aren’t only about adding code
but adding business knowledge too.
* Although the commits in a Pull Request are merged together they should be meaningful on their own.
Comment about better commit messages and point to relevant documentation when necessary
* Appreciate the quality of the work of your team
* Try to take the most of out the GitHub UI and the GitHub Flavored Markdown when reviewing code:
for highlighting snippets, doing references between commits and other issues and calling other
developers to join you in the review.
* Avoid commenting on commits directly instead of
the Pull Request diff, since it pollutes the Pull Request page and such comments won’t be
collapsed when the related lines get changed and/or fixed by a new commit.

### Source

Most of the explanation comes from [Plataformatec Guidelines](http://guidelines.plataformatec.com.br/pull-requests.html).

### Articles

If you want to read more about this subject, check these articles:

* [There’s a human on the other side of your code review](https://medium.com/@tadasant/theres-a-human-on-the-other-side-of-your-code-review-9732cc15bfee)
* [Unlearning toxic behaviors in a code review culture](https://medium.com/@sandya.sankarram/unlearning-toxic-behaviors-in-a-code-review-culture-b7c295452a3c)
