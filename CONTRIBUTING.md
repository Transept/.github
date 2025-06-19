# TRANSEPT GENERAL CONTRIBUTION GUIDE

This is a general guide for contributing to any Transept project. This should allow for any developer to easily apply changes to these projects without having to figure out how to apply changes to the code.

## Development Workflow

Transept uses a GitFlow inspired development process. 

- Canonical Main: the `main` branch shall be the latestest version of useable code similar to a "nightly" build. Any feature, bugfix or task branch should be branched off of main and be merged into main.
- Feature Branches: all changes should be made via feature branches and a PR. This should be a single chagne package that contains a new feature/improvment or bug fix. No work should ever be done directly done on `main`
- Releases: All realeases shall be tags that follow the format `v<version>` where the version follows the [semver](https://semver.org/) standard. If any maintence needs to be applied to a release then the big fix will be worked on, and cherry picked onto the tag and a new verision shall be created.

## Branch Names
In general there is no a strict branch name convention but it is prefered to use a prefex of the type of change you are making using a `/`. Examples: `feature/new-widgit`, `task/rename-variable`, `chore/update-changelog`


## PRs

All PRs should have an associated issue that describes the problem at hand. The PR is for discusing the changes made and should include testing to show that whatever problem was being solved is solved.

