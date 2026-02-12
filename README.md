# gha_experiments

Experiments re GitHub actions

Using "phpcs_full":

```yml
name: Coding standards
on: [pull_request]
jobs:
  coding_standards:
    timeout-minutes: 10
    runs-on: ubuntu-latest
    steps:
      - name: Run PHP_CodeSniffer
        uses: indigoxela/gha_experiments/actions/phpcs_full@main
```

Available (optional) parameters:

- php_version: defaults to 8.3
- fail_on_warnings: defaults to true
