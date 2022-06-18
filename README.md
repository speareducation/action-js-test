# Github Actions for JS Test & Lint

## run-tests

Runs `npm run lint` and `npm run test --coverage` using scripts from package.json. Usually this would be eslint
and Jest.

### Inputs

* `output-path` - Path or name of directory to store results, default: ./.ci-results
* `lint-results-file` - Filename for lint results, default: js-lint-results.txt
* `test-results-file` - Filename for test results, default: js-test-results.txt
* `pr-comment-file` - Filename for PR comment, default: js-pr-comment.md
* `email-file` - Filename for email body, default: js-overview-email.txt

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
