# Git Commit Message Prompt

This prompt guides you in creating a clear, concise, and informative Git commit message.

## 0. Commit Type Prefix

Prefix your commit message with a type to categorize the change. This helps in understanding the nature of the commit at a glance.

*   **feat:** A new feature
*   **fix:** A bug fix or behavior adjustment
*   **docs:** Documentation only changes
*   **style:** Changes that do not affect the meaning of the code (white-space, formatting, missing semicolons, etc.)
*   **refactor:** A code change that neither fixes a bug nor adds a feature
*   **perf:** A code change that improves performance
*   **test:** Adding missing tests or correcting existing tests
*   **build:** Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)
*   **ci:** Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs)
*   **chore:** Other changes that don't modify src or test files
*   **revert:** Reverts a previous commit

### Example:

```
feat: Add user profile editing functionality
fix: Correct off-by-one error in pagination
docs: Update README with new installation instructions
```

## 1. What Changed?

Provide a brief, objective summary of the changes introduced in this commit. Focus on *what* was modified, added, or removed.

*   **Instructions:** Describe the changes in a direct and factual manner. Avoid subjective language.
*   **To view changes:** Run `git diff --staged` to see staged changes, or `git diff HEAD` to see all changes since the last commit.

### Example:

```
- Refactored user authentication module.
- Added input validation for registration form.
- Fixed a bug where user sessions were not expiring correctly.
```

## 2. Why It Changed?

Explain the reason or motivation behind the changes. Focus on *why* these changes were necessary, what problem they solve, or what new functionality they enable.

*   **Instructions:** Provide context and justification for the changes. Link to issues or requirements if applicable.

### Example:

```
- To improve maintainability and separate concerns within the authentication logic.
- To prevent invalid data submission and enhance security.
- To resolve reported issue #123 where users remained logged in indefinitely.
```
