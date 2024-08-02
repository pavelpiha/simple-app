# Application Style Guide

## Code Style

1. **Components**:

- Use only standalone Angular components.
- Use only OnPush Change Detection strategy.
- Common components should be stored in `src/app/common`
- Metadata properties in @Component decorator should be sorted by next order:

```
 selector,
 templateUrl,
 styleUrls,
 changeDetection,
 standalone,
 imports,
 '...all the rest properties'
```

2. **Models and DAO services**:

- Use Angular property naming convention.
- Use camel case for property naming.
- Use `src/app/shared` folder for storing Models and DAO services. Use model scope folder structure example:

3. **Comments**: Code should not contain commented out code.

4. **File names**: File names should follow Angular file naming convention.

## Git

1. **Commit Messages**: Use the [Conventional Commits](https://www.conventionalcommits.org/) format.
2. **Strict Commit Messages**

- For self review use such commit message. example: "chore: self review"
- For resolving conflicts use such commit message. example: "chore: resolve review commits"
- For bug fixes use `fix` prefix and the ticket identifier in the scope. example: "fix(DDIAAS-8888): remove feature"

3. **Branch Naming strategy**: Use descriptive branch names. Branches should start with prefixes: feature|fix[/-]
   (example: `feature/add-login-button`, `feature-implement-dropdown-for-user-form`, , `fix/fix-login-error`).

## Pull Requests

1. **PR Description**: Provide a detailed description of the changes in the PR. Include the purpose of the PR and any relevant context.
2. **Main branch restrictions**: pull request to the 'main' branch should be raised from a branch that starts with 'feature/' or 'fix/'
