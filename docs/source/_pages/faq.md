# Frequently Asked Questions (FAQ)

:::{warning}
:name: faq-disclaimer

Please note that the views expressed here are, for the most part, opinions only. They reflect design decisions made by the maintainers of the package. They are neither right nor wrong, but chosen to best support development of the package. All are subject to change at any time.
:::

## Why Rebase and Squash Merge?

Commits to the `main` branch should leave the project in a working state. The `main` branch is the project's single source of truth for the latest developments to the codebase and users may (and often will) clone and use the latest commit to `main`. When creating a feature, fixing a bug, etc., multiple logical changes are often required. For example, tests and documentation are usually needed and possibly even updates to ci functionality, to name a few. Since commits should represent a single logical change, pull requests are used in practice to create a single stable change (e.g. creating a new feature) that consists of multiple logical changes (e.g. add functionality, create tests, update documentation, etc.), each of which might by themselves leave the project in an incomplete (i.e. unstable) state (Note that pull requests are also, obviously, used for performing code reviews). For this reason, commits in a pull request are squashed into a single commit before being merged into `main`. The same also goes for the `release` branch and when creating `hotfixes`.

The reason for rebasing is even more straightforward. For one thing, commits to the `main` branch must always be on top of the latest version of `main` (hence merge conflicts must be resolved). Furthermore, if dates when the pull request was created and at what point in the history are required, this is all stored in the pull request itself. However, the only history that matters are the final (squashed) commits that have been merged into `main` for end use. This is analogous to a change made to a document in a document control system in a regulated industry. If the change is begun at revision B of the document and the document is subsequently updated to revisions C and D before the change is completed, the originator updates his or her change with the revisions from C and D and submits it as revision E. The end user sees a linear progression from revision B to E and the details of the changes that went into E, including the dates and times individual changes were made, are stored in the change order.
