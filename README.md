# bob-install-action

Installs [bob](https://bob.build/) on GitHub Actions.

## Features

You can specify bob release version via `version`.

## Usage
```yaml
steps:
  - uses: benchkram/bob-install-action@v1
    with:
      version: 0.4.0
  - run: bob --version
```
