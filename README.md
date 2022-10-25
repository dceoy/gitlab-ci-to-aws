gitlab-ci-to-aws
================

Toolkit for CI/CD from GitLab to AWS

[![Lint](https://github.com/dceoy/gitlab-ci-to-aws/actions/workflows/lint.yml/badge.svg)](https://github.com/dceoy/gitlab-ci-to-aws/actions/workflows/lint.yml)

Installation
------------

1.  Check out the repository.

    ```sh
    $ git clone git@github.com:dceoy/gitlab-ci-to-aws.git
    $ cd gitlab-ci-to-aws
    ```

2.  Install [Rain](https://github.com/aws-cloudformation/rain) and set `~/.aws/config` and `~/.aws/credentials`.

3.  Create an AWS IAM user group for CI/CD.

    ```sh
    $ rain deploy src/iam.cfn.yml ci-iam
    ```
