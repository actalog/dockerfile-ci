# Dockerfile CI

Continuous Integration for Dockerfile

## Getting started

```yml
name: CI

on:
  - push

jobs:
  node-ci:
    name: Node CI
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: gabrielrufino/dockerfile-ci@v1
        with:
          image-name: gabrielrufino/image
```
