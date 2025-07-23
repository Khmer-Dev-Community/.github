# 🤝 Contributing to the [Platform Repository Name]

We're thrilled you're interested in contributing to the Khmer Development Community's [Platform Repository Name]! Your contributions help us build a stronger, more vibrant tech ecosystem in Cambodia.

This document outlines guidelines for contributing to this specific repository. Please take a moment to review it before making your first contribution.

## 🌟 How to Contribute

We welcome contributions of all kinds, including but not limited to:

* **Code:** New features, bug fixes, performance improvements.
* **Documentation:** Updates, clarifications, new guides.
* **Bug Reports:** Identifying and reporting issues.
* **Feature Requests:** Suggesting new ideas.
* **Community Support:** Helping others, answering questions.

### 🐛 Reporting Bugs

If you find a bug, please help us by [opening a new issue](https://github.com/Khmer-Dev-Community/[Platform-Repository-Name]/issues/new?assignees=&labels=bug&projects=&template=bug_report.md&title=). Before opening a new issue, please:

1.  **Search existing issues:** Check if the bug has already been reported.
2.  **Provide detailed information:**
    * A clear and concise description of the bug.
    * Steps to reproduce the behavior.
    * Expected behavior vs. actual behavior.
    * Screenshots or videos (if applicable).
    * Your operating system, browser, and relevant software versions.

### ✨ Suggesting Enhancements (Feature Requests)

Have an idea for a new feature or improvement? We'd love to hear it! Please [open a new issue](https://github.com/Khmer-Dev-Community/[Platform-Repository-Name]/issues/new?assignees=&labels=enhancement&projects=&template=feature_request.md&title=). When suggesting an enhancement, please:

1.  **Search existing issues:** Check if a similar idea has already been proposed.
2.  **Describe the enhancement:** Clearly explain the feature and why it would be beneficial.
3.  **Provide examples:** If possible, illustrate how the feature would be used.

## 💻 Code Contributions (The Fork & Pull Request Workflow)

We use the standard GitHub "fork and pull request" workflow for all code contributions.

1.  **Fork the Repository:**
    * Go to `https://github.com/Khmer-Dev-Community/[Platform-Repository-Name]`
    * Click the "Fork" button in the top right corner. This creates a copy of the repository under your GitHub account.

2.  **Clone Your Fork:**
    * Open your terminal/command prompt.
    * Clone your *fork* to your local machine:
        ```bash
        git clone [https://github.com/YOUR_USERNAME/](https://github.com/YOUR_USERNAME/)[Platform-Repository-Name].git
        cd [Platform-Repository-Name]
        ```
    * Replace `YOUR_USERNAME` with your GitHub username.

3.  **Set Upstream Remote (One-time setup):**
    * Add the original Khmer-Dev-Community repository as an "upstream" remote. This allows you to pull changes from the main project.
        ```bash
        git remote add upstream [https://github.com/Khmer-Dev-Community/](https://github.com/Khmer-Dev-Community/)[Platform-Repository-Name].git
        ```

4.  **Create a New Branch:**
    * Always work on a new branch for your contributions. Use a descriptive name (e.g., `feature/add-user-profile`, `bugfix/login-issue`).
        ```bash
        git checkout main # Or 'master', depending on the primary branch name
        git pull upstream main # Sync with the latest changes from the main repo
        git checkout -b your-new-branch-name
        ```

5.  **Make Your Changes:**
    * Implement your feature, fix the bug, or update documentation.
    * Ensure your code adheres to our [Coding Style & Conventions](#coding-style-conventions) (see below).
    * **Write tests** for new features or bug fixes whenever applicable.
    * **Update documentation** if your changes affect existing features or add new ones.

6.  **Test Your Changes:**
    * Before committing, run all relevant tests to ensure your changes haven't introduced regressions.
    * [Add specific instructions here, e.g., `npm test`, `yarn test`, `php artisan test`, etc.]

7.  **Commit Your Changes:**
    * Stage your changes:
        ```bash
        git add .
        ```
    * Commit with a clear and concise message. Follow our [Commit Message Guidelines](#commit-message-guidelines).
        ```bash
        git commit -m "feat: Add new user registration flow"
        # or
        git commit -m "fix: Resolve incorrect user count on dashboard"
        ```

8.  **Push to Your Fork:**
    * Push your new branch to your forked repository on GitHub:
        ```bash
        git push origin your-new-branch-name
        ```

9.  **Create a Pull Request (PR):**
    * Go to your forked repository on GitHub. You should see a prominent "Compare & pull request" button.
    * Click it to start the PR creation process.
    * **Ensure the base repository is `Khmer-Dev-Community/[Platform-Repository-Name]` and the base branch is `main` (or `master`).** Your head repository should be your fork and your new branch.
    * **Fill out the Pull Request template thoroughly:**
        * Provide a clear title (matching your commit message style).
        * Describe the changes you've made and why.
        * Reference any related issues (e.g., `Closes #123`, `Fixes #456`).
        * Include screenshots or GIFs if it's a visual change.

10. **Review Process:**
    * Maintainers will review your PR. They may ask for changes or clarification.
    * Be responsive to feedback. Once approved, your changes will be merged!

## 📝 Commit Message Guidelines

We use a conventional commit style for clear and consistent commit history. This helps with automatic changelog generation and understanding the project's evolution.

**Format:** `<type>(<scope>): <subject>`

* **`<type>`:**
    * `feat`: A new feature
    * `fix`: A bug fix
    * `docs`: Documentation only changes
    * `style`: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc.)
    * `refactor`: A code change that neither fixes a bug nor adds a feature
    * `perf`: A code change that improves performance
    * `test`: Adding missing tests or correcting existing tests
    * `build`: Changes that affect the build system or external dependencies (e.g., npm, yarn)
    * `ci`: Changes to our CI configuration files and scripts
    * `chore`: Other changes that don't modify src or test files
    * `revert`: Reverts a previous commit
* **`<scope>` (optional):** The part of the codebase affected (e.g., `auth`, `ui`, `database`, `frontend`, `backend`).
* **`<subject>`:** A concise, imperative mood description (e.g., "add," "fix," "update") with no period at the end.

**Examples:**

* `feat(users): Add user profile page`
* `fix(login): Resolve incorrect password error message`
* `docs: Update README with contribution guidelines`
* `refactor(api): Streamline error handling logic`

## 📏 Coding Style & Conventions

To maintain a consistent and readable codebase, please adhere to the following (or link to more detailed style guides):

* **[Specific Language/Framework] Style Guide:** [Link to ESLint config, Prettier config, or internal style guide document, e.g., "Follow our ESLint rules."]
* **Indentation:** Use [e.g., 2 spaces or 4 spaces] for indentation.
* **Naming Conventions:** [e.g., camelCase for variables, PascalCase for components, kebab-case for CSS classes].
* **Comments:** Use comments to explain complex logic, but prefer self-documenting code.
* **Linting/Formatting:** Ensure your code passes all linting checks. We recommend setting up your editor to format code on save using [e.g., Prettier or ESLint auto-fix].

## 🛡️ Code of Conduct

Please review our [Code of Conduct](link-to-your-CODE_OF_CONDUCT.md) for information on our community's behavioral expectations. We are committed to providing a welcoming and inclusive environment for everyone.

## 🙏 Thank You!

Your contributions are vital to the success of the Khmer Development Community. We appreciate your time, effort, and dedication to helping us build something great for Cambodia!

---

*This document is inspired by best practices in open-source projects.*
