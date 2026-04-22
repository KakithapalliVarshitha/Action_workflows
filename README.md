name: Test Workflow

on: push

jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4

      - name: Use my reusable action
        uses: ./.github/actions/setup-runtime
