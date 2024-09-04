# whywaita/is-installed-xcode-action

[![CI](https://github.com/whywaita/is-installed-xcode-action/actions/workflows/ci.yml/badge.svg)](https://github.com/whywaita/is-installed-xcode-action/actions/workflows/ci.yml)

whywaita/is-installed-xcode-action checks to see if the same Xcode version as GitHub-hosted is installed.

## Usage

```yaml
- uses: whywaita/is-installed-xcode-version@v1
  with:
    success-on-miss: false  # Optional
```

Please see [actions.yml](https://github.com/whywaita/is-installed-xcode-version/blob/main/action.yml) about input parameters.

## Motivation

The GitHub-hosted runner installs Xcode under the conditions specified in [actions/runner-images](https://github.com/actions/runner-images/blob/59a0b3727b675f4d29713127bca7726492d7a085/README.md#L121).

This action checks whether the self-hosted runner is in the same state as the GitHub-hosted runner when providing the macOS runner.
