# Git Best Practices
This document outlines the best practices for working with branches, commits, and pull requests in for Dictionarry.

## Branch Naming

When creating a new branch, follow these guidelines for branch naming:

- Use a descriptive name that reflects the purpose of the branch.
- Use hyphens (`-`) to separate words in the branch name.
- Prefix the branch name with the type of change:
  - `feature/`: For adding new features or enhancements.
  - `fix/`: For bug fixes or minor corrections.
  - `docs/`: For documentation updates.
  - `refactor/`: For code refactoring or performance improvements.

Examples:
- `feature/add-new-collection`
- `fix/update-incorrect-data`
- `docs/update-contributing-guidelines`
- `refactor/optimize-query-performance`

## Commits

When making commits, follow these best practices:

- Make small, focused commits that address a single logical change.
- Write clear and concise commit messages that describe the purpose of the change.
- Use the present tense and imperative mood in commit messages.
- Prefix the commit message with the type of change (e.g., `feat:`, `fix:`, `docs:`, `refactor:`).
- If necessary, provide additional details in the commit description.

Example commit message:
```
feat: Add new collection for user preferences

- Create UserPreferences collection
- Define schema for user preferences
- Add sample data for testing
```

## Pull Requests

When creating pull requests (PRs), adhere to the following guidelines:

- Give the PR a clear and descriptive title that summarizes the changes.
- Provide a detailed description of the changes made in the PR.
- Reference any related issues or tasks using the appropriate keywords (e.g., `Closes #123`, `Fixes #456`).
- Request review from relevant team members or maintainers.
- Address any feedback or comments received during the review process.
- Ensure that the PR is up to date with the target branch before merging.

Example pull request title and description:
```
Title: Add new collection for user preferences

Description:
This pull request adds a new collection to store user preferences in the Dictionarry database.

Changes:
- Created UserPreferences collection
- Defined schema for user preferences
- Added sample data for testing

Closes #123
```

## Merging and Deleting Branches

After a pull request has been reviewed and approved, follow these steps:

1. Merge the pull request into the target branch (usually `dev`).
2. Delete the source branch to keep the repository clean.

## Syncing with the Latest Changes

To ensure your local branch is up to date with the latest changes in the `dev` branch, regularly perform the following steps:

1. Switch to the `dev` branch:
   ```
   git checkout dev
   ```

2. Pull the latest changes from the remote repository:
   ```
   git pull origin dev
   ```

3. Switch back to your feature branch:
   ```
   git checkout your-branch-name
   ```

4. Make your changes and submit a PR: