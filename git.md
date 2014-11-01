### Commit Messages

Good commit messages should have a concise message in present tense and lowercase, preferably with a prepended subsystem for easy clarity of history.
Due to the use of GitHub, they should also be no longer than 50 characters, so that it does not wrap into the description.

If the commit fixes an existing GitHub issue, the description should contain `Fixes #<issue number>` or `Closes #<issue number>`, so that the issue can be automatically closed once merged in.
`Fixes` should be used for issues or bugs. `Closes` should be used for all other things.

```
guides: add git guidelines

Closes #15
Closes #10
```

### Pull Requests

Maintainers should try to avoid using the GitHub `Merge pull request` button when possible. Doing so causes un-necesary nonlinearities, making the git history difficult to understand by putting commits in order of their commit date, rather than merge date.

A more reasonable and readable way of doing things is to grab Pull Requests by piping a patch grabbed by `curl` into `git am`, and amending if necessary, before commiting.

Doing so also preserves the git author, while showing the related maintainer as the commiter.

#### Simple example

```bash
$ curl https://github.com/<org>/<repo>/pull/<num>.patch | git am
$ # possibly do fixups
$ git commit --amend # edit message at this time
```

#### Complex example

Sometimes Pull Requests may be based off of old branches or commits, and may need rebasing, and other fixups.
This example covers most complex cases.

```bash
$ git checkout -b pr <pr-commit-base>
$ curl https://github.com/<org>/<repo>/pull/<num>.patch | git am
$ git rebase -i master # squash everything together
$ # possibly do fixups
$ git commit --amend # edit message at this time
$ git checkout master
$ git merge --ff-only pr
$ git branch -D pr
```
