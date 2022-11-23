Create a `.github/CODEOWNERS` file and take a look at the example [here](https://github.com/ethanthorpe-pin/protected-branch-example). For your instance you may want the following contents

```
*   @JitMaharaj @JimThorpePIN
```

In the GitHub repo, go to `Settings` -> `Branches` -> `Branch protection rules` -> `Add rule`. Set `Branch name pattern` to `main`. For the rules, I recommend the following.

```
☑ Require a pull request before merging
    ☑ Require approvals
        Set to 1
    ☑ Dismiss stale pull request approvals when new commits are pushed
    ☑ Require review from Code Owners
    ☑ Require approval of the most recent push
☑ Require status checks to pass before merging
    ☑ Require branches to be up to date before merging
☐ Require conversation resolution before merging
☐ Require signed commits
☐ Require linear history
☐ Require deployments to succeed before merging
☐ Lock branch
☑ Do not allow bypassing the above settings

☐ Allow force pushes
☐ Allow deletions
```
