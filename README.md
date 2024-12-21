# Dockerfile CI

Continuous Integration for Dockerfile

## Getting started

```yml
name: CI

on:
  - push

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
