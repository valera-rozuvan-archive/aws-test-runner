# aws-test-runner

## wip has moved

Future work on this repository has moved to the monorepo [valera-rozuvan/howtos](https://github.com/valera-rozuvan/howtos). This repo is archived for historic purposes (to preserve commit history). Navigate over to [howtos/aws-test-runner](https://github.com/valera-rozuvan/howtos/tree/main/aws-test-runner) to see updates (if any).

## introduction

AWS test runner that can go on running as long as necessary

## Pre-requisites

In the file `run-tests.sh` update thie following ENV variables:

```text
ROLE_ARN
DEVICE_SERIAL_NUMBER
```

In the file `run-tests-suite.sh` update the test file name ENV variable:

```text
TEST_FILE_NAME
```

And also the full path to the test in the function invocation on line 26:

```text
show_simplified_logs "functional_tests/jest/aws-lambda-invocation.tests.ts"
```

TODO: Make the above also an ENV variable.

## Running

Simply launch the Bash script `run-tests.sh`.

## License

This project is licensed under the MIT License. See [LICENSE](./LICENSE) for more details.
