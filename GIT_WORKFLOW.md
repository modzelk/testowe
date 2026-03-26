# Git Workflow Documentation

##Overview
This document describes the Git workflow used for the `modzelk/carpoolingmobile` and `modzelk/carpooling` repositories.

### Branching Strategy
1. **Main Branch**: The `main` branch is the stable branch, which always contains production-ready code.
2. **Feature Branches**: For each new feature or bug fix, a new branch should be created from `main`. The convention for naming these branches is `feature/<feature-name>` or `bugfix/<bug-name>`.

### Pull Requests
1. **Creating a Pull Request**: Once work on a feature is complete, a pull request (PR) should be submitted to merge the feature branch into `main`.
2. **Review Process**: Pull requests should be reviewed by at least one other developer before being merged.
3. **Merging**: After approval, the PR can be merged into `main`. Always rebase with the latest `main` before merging.

### Release Process
1. **Preparation**: Ensure that the code in `main` is production-ready. Test thoroughly before proceeding.
2. **Tagging**: Once ready to release, create a new tag in the format `vX.X.X` that corresponds to the release version.
3. **Deployment**: After tagging, deploy the code from the `main` branch to production.

### Important Commands
```bash
# Clone repository
git clone <repository-url>

# Create a new feature branch
git checkout -b feature/<feature-name>

# Commit changes
git commit -m "Description of changes"

# Push changes to feature branch
git push origin feature/<feature-name>

# Create pull request on GitHub after pushing
```