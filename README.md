# actions-test
.github/workflows/test.yml
yaml

name: Calculator Test

on:
  push:
  workflow_dispatch:

jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - name: Check calculation
        run: python -c "assert 1 + 1 == 2"
