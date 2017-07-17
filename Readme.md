# git Branching Test

Simulation of a git workflow following the article [A successful Git branching model](http://nvie.com/posts/a-successful-git-branching-model/) and how-tos from [here](https://docs-applications.readthedocs.io/en/latest/git.html#workflow-gitflow).

Note that some of the information here are in addition to the two sources above.

The workflow features two permanent branches, `master` and `development`. Other branches for hotfixes, features and releases should be deleted after they have been merged into the permanent branches - they are not deleted in this repository to showcase the workflow. Also, feature branches can be local and not pushed to the repository.

For deployment environments featuring development, QA, and production environments, each branch can be deployed to an environment as follows:

- development branch -> development environment
- release branches -> QA environment
- master branch -> production environment

### Sourcetree tips:
While merging branches, new commits should be created for better clarity. In Sourcetree, the option "Create a new commit even if fast-forward is possible" should be checked.

For automatic detailed commit messages, the option "Include messages from commits being merged in the merge commit" can be checked.

The option "Commit merge immediately" can be unchecked to avoid automatic commit messages.
