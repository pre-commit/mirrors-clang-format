clang-format mirror
===================

Mirror of `clang-format` package for pre-commit.

For pre-commit: see https://github.com/pre-commit/pre-commit

For clang-format: see https://github.com/ssciwr/clang-format-wheel


### Using clang-format with pre-commit

Add this to your `.pre-commit-config.yaml`:

```yaml
-   repo: https://github.com/pre-commit/mirrors-clang-format
    rev: ''  # Use the sha / tag you want to point at
    hooks:
    -   id: clang-format
```

Use `clang-format-diff` to format only the modified portions of the code, rather than the entire changed files.

```yaml
-   repo: https://github.com/pre-commit/mirrors-clang-format
    rev: ''  # Use the sha / tag you want to point at
    hooks:
    -   id: clang-format-diff
```
