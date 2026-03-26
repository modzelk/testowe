# Repository Overview

This document provides an overview of the repository structure and guidelines for the **carpoolingmobile** and **carpooling** repositories.

## Branches Overview

### Carpooling Mobile Repository
- **main**: The stable version of the application, suitable for release.
- **mobile**: Branch for mobile-specific features and improvements.
- **develop**: Integration branch for features that are ready to be tested.
- **frontend**: Contains all frontend-related development.
- **backend**: Contains all backend-related development.

### Carpooling Repository
- **main**: The stable version of the application for the web.
- **mobile**: This branch may not be applicable for this repository but is included for consistency.
- **develop**: The latest features and fixes that are being prepared for the next release.
- **frontend**: Contains all frontend-related development.
- **backend**: Contains all backend-related development.

## Merge Strategies

- **Merge Commit**: Use this for feature branches that need to retain history.
- **Squash Merge**: Suitable for small features or fixes where detailed history isn't necessary. All commits will be combined into a single commit.
- **Rebase and Merge**: Use this for a clean history. It places the changes from the feature branch on top of the main branch, maintaining a linear history.

## Branching Conventions

- Branch names should be descriptive and follow the pattern: `feature/<feature-name>` or `bugfix/<bug-description>`.
- Always create new branches off of `develop` for new features or bug fixes.

## Commit Message Format

- **Format**: `[TYPE] Description of the change`
- **Types**: `feat` for new features, `fix` for bug fixes, `docs` for documentation changes, `style` for formatting (non-code), `refactor` for code improvements without changing behavior, and `test` for adding or updating tests.

## Protection Rules

- Branches like `main` and `develop` are protected, preventing direct pushes.
- All changes must go through pull requests to ensure code review before merging.
- Require status checks to pass before merging into protected branches.

## Additional References
- Ensure to review the [contribution guidelines](#) for further details.
- Check the [repository wiki](#) for documentation and further instructions.