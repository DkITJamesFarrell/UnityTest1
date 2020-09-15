
## Making Updates

Updates should consist of 3 steps.

1. Commit changes (using semantic message format outlined below)
2. `git push --follow-tags origin master`

### Semantic Commit Message Format

Each commit message consists of a header, a body and a footer. The header has a special format that includes a type and a subject:

`<type>(<optional scope>): <subject> <BLANK LINE> <optional body> // This may span multiple lines <BLANK LINE> <optional footer>`

***Note: The following guidelines are taken from the [Angular commit message guidelines](https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines)***

#### Type

Type must be one of the following:

- ***build***: Changes that affect the build system or external dependencies\ 
- ***ci***: Changes to our CI configuration files and scripts\ 
- ***docs***: Documentation only changes\ 
- ***feat***: A new feature\ 
- ***fix***: A bug fix\ 
- ***perf***: A code change that improves performance\ 
- ***refactor***: A code change that neither fixes a bug nor adds a feature\ 
- ***style***: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)\ 
- ***test***: Adding missing tests or correcting existing tests\

### Scope

***Note:*** Optional

A scope MAY be provided after a type. A scope MUST consist of a noun describing a section of the codebase surrounded by parenthesis, e.g., docs(readme):

#### Subject

The subject contains a succinct description of the change:

- use the imperative, present tense: "change" not "changed" nor "changes" 
- don't capitalize the first letter 
- no fullstop (.) at the end

#### Body

Just as in the subject, use the imperative, present tense: "change" not "changed" nor "changes". The body should include the motivation for the change and contrast this with previous behavior.

#### Footer

The footer should contain any information about Breaking Changes and is also the place to reference git issues that this commit Closes.

A commit that has a footer BREAKING CHANGE:, or appends a ! after the type/scope, introduces a breaking API change (correlating with MAJOR in semantic versioning).
