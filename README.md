# install-bob-action

Installs [bob](https://bob.build/) on GitHub Actions.

## Features

You can specify bob release version via `version`.

## Usage

Create `.github/workflows/test.yml` in your repo with the following contents:

```yaml
name: "Test bob install action"
on:
  pull_request:
  push:
jobs:
  tests:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2.4.0
      - uses: benchkram/bob-install-action@v1
        with:
          version: 0.4.0
      - run: bob --version
```
