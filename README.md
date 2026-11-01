# Workflows

[Reusable workflows](https://docs.github.com/en/actions/learn-github-actions/reusing-workflows) for GitHub Actions.

## Usage

This is an example to run RuboCop on Ruby project.

```yaml
name: rubocop

on:
  pull_request:
  push:
    branches:
      - main

jobs:
  rubocop:
    uses: r7kamura/workflows/.github/workflows/ruby-rubocop.yml@main
```

See [.github/workflows](/.github/workflows) for more details.
