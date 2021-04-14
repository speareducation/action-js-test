# Github Actions for JS Test & Lint


## run-tests

Runs `yarn lint` and `yarn test --coverage` using scripts from package.json. Usually this would be eslint
and Jest.

_This action should probably not be used directly_, see test-and-notify

Example:

```

```

### Inputs

* `output-path` - Path or name of directory to store results, default './.ci-results'

### Outputs

* `lint-result` - "PASS" if linting check passed, "FAIL" if problems found
* `lint-result-emoji` - Emoji code representation of lint result
* `lint-success` - Boolean of lint result
* `lint-summary` - Text summary of lint results
* `test-result` - "PASS" if all tests passed, "FAIL" if problems found
* `test-result-emoji` - Emoji code representation of test result
* `test-success` - Boolean of test result
* `test-coverage` - Test coverage summary
* `test-summary` - Text summary of test results
