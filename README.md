# Workflows

Reusable workflows for GitHub Actions.

## Usage

This is an example to run tests on Rust project.

```yaml
name: test

on:
  pull_request:
  push:
    branches:
      - main

jobs:
  test:
    uses: r7kamura/workflows/.github/workflows/rust-test.yml@main
```

See [.github/workflows](/.github/workflows) for more details.
