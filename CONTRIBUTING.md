# Contributing to Programming Club, DAU Repositories

First off, thank you for considering a contribution to **Programming Club, DAU**! Student contributions are what make our club projects thriving learning environments for everyone at **Dhirubhai Ambani University**.

Whether you are fixing a typo, resolving a bug, or building a new feature, your help is warmly welcomed.

---

## General Guidelines & Etiquette

- **Be Inclusive & Kind**: We are all students learning together. Be patient with beginners and open to feedback.
- **Ask Questions Early**: If you are unsure about how to implement something or need help with Git, reach out in the issue discussion or contact maintainers via [programming-club@dau.ac.in](mailto:programming-club@dau.ac.in).
- **Follow the Code of Conduct**: Ensure all interactions remain respectful and constructive by reviewing our [Code of Conduct](./CODE_OF_CONDUCT.md).

---

## Development Workflow

We follow a standard Git feature-branch workflow. Follow these steps to work on a project:

### 1. Find or Create an Issue
Before writing code, check the repository's issue tracker:
- If an issue exists, leave a comment expressing your interest to work on it (`"I'd like to work on this issue!"`).
- If you notice a new bug or have a feature idea, open a new issue using our issue templates first.

### 2. Fork & Clone
Fork the repository to your GitHub account and clone it locally:

```bash
git clone https://github.com/<your-username>/<repository-name>.git
cd <repository-name>
```

Add the original repository as an `upstream` remote:

```bash
git remote add upstream https://github.com/ProgrammingClub-DAU/<repository-name>.git
```

### 3. Create a Feature Branch
Always create a new branch from `main` (or `master`) for your work. Do not work directly on the default branch.

```bash
git checkout main
git pull upstream main
git checkout -b <branch-name>
```

#### Branch Naming Conventions
Use descriptive, prefix-based names for your branches:

- `feat/short-description` — New features (e.g., `feat/user-login`)
- `fix/short-description` — Bug fixes (e.g., `fix/nav-bar-overlap`)
- `docs/short-description` — Documentation improvements (e.g., `docs/update-setup-guide`)
- `refactor/short-description` — Code refactoring without functionality changes (e.g., `refactor/api-handler`)
- `chore/short-description` — Build scripts, dependencies, or maintenance (e.g., `chore/update-deps`)

### 4. Make Changes & Commit
Write your code, following project formatting and coding standards. Keep commits atomic (focused on a single logical change).

#### Commit Message Conventions
We follow the **Conventional Commits** specification. Format your commit messages as follows:

```
<type>(<optional scope>): <short description>
```

**Allowed Types:**
- `feat`: A new feature for the user
- `fix`: A bug fix
- `docs`: Documentation changes only
- `style`: Formatting changes that do not affect code logic (white-space, linting)
- `refactor`: Code restructuring without changing external behavior
- `test`: Adding missing tests or correcting existing tests
- `chore`: Maintenance tasks, dependency updates, or build configuration

**Examples:**
- `feat(auth): add Google OAuth login flow`
- `fix(dashboard): resolve state leak in chart component`
- `docs(readme): add installation steps for Linux users`

### 5. Push Changes & Open a Pull Request
Push your branch to your remote fork:

```bash
git push origin <branch-name>
```

Then submit a Pull Request (PR) against the `main` branch of the official `ProgrammingClub-DAU` repository:
- Give your PR a clear, descriptive title.
- Fill out all sections of the [Pull Request Template](./PULL_REQUEST_TEMPLATE.md).
- Link the relevant issue using GitHub keywords (e.g., `Closes #42` or `Fixes #15`).

---

## Code Review Process

1. **Initial Automated Checks**: Ensure linting, formatting, and build scripts pass.
2. **Peer Review**: A club project maintainer or peer will review your PR. They may ask for minor changes or suggestions.
3. **Iterate**: Make requested adjustments locally, commit them, and push to the same branch. The PR will update automatically.
4. **Merge**: Once approved by at least one maintainer, your PR will be merged into `main`!

---

## Coding Style Expectations

- **Clean & Readable**: Code should be readable and self-explanatory where possible.
- **Linting & Formatting**: Run repository linters/formatters (e.g., Prettier, ESLint, Black, or `clang-format`) before committing.
- **Documentation**: Comment complex logic and keep README/setup instructions up to date.
- **No Unused Code**: Clean up debug `console.log` statements, unused variables, and commented-out code snippets before opening a PR.

---

## Best Practices for Student Contributors

- **Start Small**: If you are new to the codebase, look for issues tagged `good first issue`.
- **Sync Regularly**: Rebase or pull changes from `upstream/main` regularly to avoid git merge conflicts.
- **Test Your Work**: Test your code manually or with existing unit tests before submitting your PR.
- **Have Fun**: Open source is a team effort and a continuous learning journey!

If you run into any blockers or have suggestions to improve this guide, feel free to contact us at [programming-club@dau.ac.in](mailto:programming-club@dau.ac.in).
