# pylint-action

## How to use

```
jobs:
  codelint:
    if: github.event_name == 'pull_request'
    runs-on: ubuntu-latest

    steps:
      - name: Check-out
        uses: actions/checkout@v3
        with:
          fetch-depth: 1

      - name: Poetry install
        uses: wintero92/poetry-install-action@v1

      - name: Pylint
        uses: wintero92/pylint-action@v1
```

## Inputs

See `action.yaml` for possible inputs.