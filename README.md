# @actalog/dockerfile-ci

[![CI](https://github.com/actalog/dockerfile-ci/actions/workflows/ci.yml/badge.svg)](https://github.com/actalog/dockerfile-ci/actions/workflows/ci.yml)
[![CD](https://github.com/actalog/dockerfile-ci/actions/workflows/cd.yml/badge.svg)](https://github.com/actalog/dockerfile-ci/actions/workflows/cd.yml)

Continuous Integration for Dockerfile

## Getting started

```yml
name: CI

on:
  - pull_request
  - push

permissions:
  pull-requests: write

jobs:
  dockerfile-ci:
    name: Dockerfile CI
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: actalog/dockerfile-ci@v2
        with:
          image-name: actalog/image
```
