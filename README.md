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
