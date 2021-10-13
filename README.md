clang-format mirror
===================

Mirror of `clang-format` package for pre-commit.

For pre-commit: see https://github.com/pre-commit/pre-commit

For clang-format: see https://github.com/ssciwr/clang-format-wheel

In comparison to other available pre-commit hooks for clang-format, this one installs clang-format from Python wheels.
This makes it usable without additional installation requirements - e.g. in pre-commit CI.

### Using clang-format with pre-commit

Add this to your `.pre-commit-config.yaml` for a project containing C, C++, C# or CUDA files:

```yaml
-   repo: https://github.com/pre-commit/mirrors-clang-format
    rev: ''  # Use the tag you want to point at
    hooks:
    -   id: clang-format
```

The available tags match the released versions of `clang-format`. All minor versions >= 10.0 are available.
By default, the hook uses a local `.clang-format` style file, but you could provide a different style
by overriding `args:`. If you do so, be sure you include `-i`. If you override types, be sure to use
`types_or:`. See the pre-commit docs for more information.
