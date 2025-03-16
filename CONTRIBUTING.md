# Contributing Guide

Thank you very much for your interest in contributing to this project! To make the contribution process as smooth as possible, please follow the guidelines below.

## Getting Started

### 1. Fork the Repository

First, fork the repository to your GitHub account. This will create your own copy of the repository.

### 2. Clone the Repository

Clone the repository you just forked to your local machine:

```bash
git clone https://github.com/your-username/file-zenith-web.git
cd file-zenith-web
```

### 3. Add Upstream Remote

To keep your repository in sync with the original repository, add the upstream remote:

```bash
git remote add upstream https://github.com/code-cracks/file-zenith-web.git
```

### 4. Create a New Branch

Before you start working, make sure to create a new branch. Branch names should follow the "functionality type/functionality description" format:

```bash
git checkout -b feat/feature-description
```

Branch types can be:

- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation
- `style`: Styling
- `refactor`: Code refactoring
- `perf`: Performance improvement
- `test`: Testing
- `chore`: Other changes

For example: `feat/home`, `fix/login-bug`, `docs/api-guide`

## Development Workflow

### 1. Install Dependencies

Before you start developing, install all dependencies:

```bash
pnpm install
```

### 2. Run the Project

To ensure you are developing in a properly running environment, start the project:

```bash
pnpm dev
```

### 3. Development Guidelines

Please follow these development guidelines:

- Ensure code is clear and concise.
- Follow the project's code style and standards (using ESLint and Prettier).
- If you add new features, please write corresponding tests.
- If you fix bugs, please add tests to prevent them from reoccurring.

### 4. Code Checking and Formatting

Before committing your changes, make sure you have properly formatted and linted the code:

```bash
pnpm lint
pnpm format
```

You can also run type checking to ensure type safety:

```bash
pnpm type-check
```

### 5. Commit Changes

This project uses commitlint and commitizen to standardize commit messages. Please use the following command to commit your changes:

```bash
pnpm commit
```

This will start an interactive commit process that guides you through selecting a commit type (such as feat, fix, docs, etc.) and filling in the commit message. Here's a guide for filling out each field:

1. **Select the type of change**:

   - Use arrow keys to select the type that best fits your changes
   - Commit types include:
     - `feat`: 🚀 A new feature
     - `fix`: 🧩 A bug fix
     - `docs`: 📚 Documentation only changes
     - `style`: 🎨 Changes that do not affect the meaning of the code
     - `refactor`: ♻️ A code change that neither fixes a bug nor adds a feature
     - `perf`: ⚡️ A code change that improves performance
     - `test`: ✅ Adding or modifying tests
     - `build`: 📦️ Changes that affect the build system or external dependencies
     - `ci`: 🎡 Changes to CI configuration
     - `chore`: 🔨 Other changes that don't modify src or test files
     - `revert`: ⏪️ Reverts a previous commit

2. **Denote the SCOPE of this change (optional)**:

   - This is optional and indicates what area your change affects
   - Can be a component name, file name, feature area, etc.
   - If your change affects multiple areas or you're unsure, select "empty"
   - If you need a custom scope, select "custom" and enter your own scope

3. **Write a SHORT, IMPERATIVE tense description of the change**:

   - Describe your change in a short sentence
   - Use imperative mood, e.g., "add user login feature" instead of "added user login feature"
   - No need to capitalize the first letter or add a period at the end

4. **Provide a LONGER description of the change (optional)**:

   - This is optional and provides more details about your change
   - Can describe the reason for the change, implementation details, etc.
   - Use "|" to break new lines

5. **List any BREAKING CHANGES (optional)**:

   - If your change breaks existing APIs or functionality, describe it here
   - Provide details about the breaking change and migration instructions
   - Use "|" to break new lines

6. **List any ISSUES by this change**:

   - If your change is related to any issues, list them here
   - Format as "#IssueNumber", e.g., "#31", "#34"

7. **Are you sure you want to proceed with the commit above?**:
   - Review your commit message and select "yes" if everything looks correct

After completing these steps, your commit message will be formatted and committed to the repository.

### 6. Sync Your Branch

Before you submit your changes, make sure your branch is up to date:

```bash
git fetch upstream
git rebase upstream/main
```

### 7. Push Your Branch

Push your branch to your own repository:

```bash
git push origin feat/feature-description
```

### 8. Create a Pull Request

On GitHub, navigate to your forked repository and click the "Compare & pull request" button. Make sure to describe your changes in detail.

## Code Review

All Pull Requests will be reviewed. Please keep the following points in mind:

- Is your code clear and easy to understand?
- Have you followed the project's code style and standards?
- Have you added appropriate tests?
- Are your changes compatible with the existing code?

## Frequently Asked Questions

### How to Report a Bug?

If you find a bug, please create an issue on GitHub and describe the bug and the steps to reproduce it as detailed as possible.

### How to Request a New Feature?

If you have a suggestion for a new feature, please create an issue on GitHub and describe your suggestion and its potential use in detail.

## Contact Us

If you have any questions or need help, please ask on GitHub or create an Issue.
