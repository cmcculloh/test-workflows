Please complete this checklist, and then delete it and all of the following before issuing your PR:

    - [ ] Ensure all tests are passing
    - [ ] Add appropriate labels to PR
    - [ ] Write a correctly formatted PR Title
    - [ ] Link to project management ticket and/or any relevant GH Issues
    - [ ] Write a thorough, but concise description that explains "what" and "why" changes were made
    - [ ] Link to any relevant resources you referenced/used
    - [ ] Delete all PR template text (including this checklist)

# Github labels

Please add the appropriate labels to your PR.

- **version:major**: Breaking Change
- **version:minor**: New Features, performance improvements, code refactors
- **version:patch**: Style changes, fixes
- **version:none**: DX (build, CI, chores, tests) or Documentation only

If you wish for your code to be deployed to the dev environment, add the **dev-deployment** label.

# Title:

    Should begin with project management ticket number (or NOTICKET) followed by a pipe (|) symbol
    Should not be more than 50 characters
    Should complete the sentence, "This commit..." or "If merged, this commit would..." (whichever is more comfortable)
    Can be written in [present simple, third person form](https://www.grammar.cl/Present/Verbs_Third_Person.htm)* or Imperative form
    Common present simple, third person verbs include (but are not limited to):
        - Fixes
        - Adds
        - Removes or Deletes
        - Corrects
        - Refactors
        - Changes
    Should begin with a capital letter
    Should not include trailing punctuation
    May include an emoji
    Compliant PR Titles:
        - JIRA-67927 | Adds yarn test:commit-title command
        - ABC67927 | Add information to the pull request template
        - 🔥 GH23 | Removes semantic commits
    Incompliant PR Titles:
        - Added information to the PR template.
        - chore: CM86827 | Add information to the PR template.
        - WIP EOD MONDAY
        - Can you guys merge this please???

# Description

    Should begin with a link to a project management ticket or "NO TICKET", eg: [TICKET123](https://jira.company.com/jira/browse/TICKET123)
    Should reference any relevant GH issues, eg: Closes #25
    Should explain what and why changes were made, but not how*
        The code explains _how_ all of this was done, so re-stating it is redundant
    If more than one thing is being accomplished, create a concise bullet-point list stating what the PR accomplishes
    State the reasoning behind decisions that were made. Especially if the "why" isn't obvious, or if answering the question, "Why did you do it _this_ way instead of _this more common_ way?"
    Include a link dump of relevant reference materials you utilized during development

*If for some reason the how is unavoidably confusing, it is recommended that you add the most concise comments possible in your code. Future developers looking at it asking "how??" are unlikely to look at PR descriptions to answer this question.

## Example Description

```
[JIRATicket](https://jira.kroger.com/jira/browse/)
Relates to #25

- Adds a PR template
- Adds DEV_NOTES.md to track ADRs (Architectural Design Rationales) starting with why we chose not to go with Conventional Commits

Right now our PRs are all over the place. Titles and descriptions vary wildly and often the first comment is asking a clarifying question or requesting a JIRA ticket number. This hopes to resolve that and get some consistency.

#### Link Dump
- https://www.conventionalcommits.org/en/v1.0.0/
- https://conjugator.reverso.net/conjugation-english-verb-add.html
- https://who-t.blogspot.com/2009/12/on-commit-messages.html
```
