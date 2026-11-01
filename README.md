# Workflows

[Reusable workflows](https://docs.github.com/en/actions/learn-github-actions/reusing-workflows) for GitHub Actions.

## Usage

This is an example to release a Ruby gem when its version is bumped.

```yaml
name: release

on:
  push:
    branches:
      - main
    paths:
      - lib/**/version.rb

jobs:
  release:
    uses: r7kamura/workflows/.github/workflows/gem-release.yml@main
    permissions:
      contents: write
      id-token: write
```

See [.github/workflows](/.github/workflows) for more details.
