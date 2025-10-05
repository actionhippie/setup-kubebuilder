# setup-kubebuilder

[![Current Tag](https://img.shields.io/github/v/tag/actionhippie/setup-kubebuilder?sort=semver)](https://github.com/actionhippie/setup-kubebuilder) [![Testing Build](https://github.com/actionhippie/setup-kubebuilder/workflows/testing/badge.svg)](https://github.com/actionhippie/setup-kubebuilder/actions/workflows/testing.yml)

[GitHub Action](https://github.com/features/actions) to install the
[Kubebuilder][kubebuilder] binary.

## Usage

```yml
name: Example

on:
  - push
  - pull_request

jobs:
  test:
    runs-on: ubuntu-latest

    steps:
      - uses: actions/checkout@v2

      - uses: actionhippie/setup-kubebuilder@v1

      - run: kubebuilder --help
```

## Inputs

### `version`

Version of the Kubebuilder binary

## Outputs

None

## Security

If you find a security issue please contact thomas@webhippie.de first.

## Contributing

Fork -> Patch -> Push -> Pull Request

## Authors

* [Thomas Boerger](https://github.com/tboerger)

## License

Apache-2.0

## Copyright

```console
Copyright (c) 2024 Thomas Boerger <thomas@webhippie.de>
```

[kubebuilder]: https://book.kubebuilder.io/
