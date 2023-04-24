# The basics

Your help is appreciated and welcome!

The _master_ branch is meant to hold the release code. At any time this should be 
identical to the code available on PyPI. 

PR's will be pushed on the _development_ branch if the actual package code is changed. When the time comes this branch
will be merged to the _master_ branch and a new release will be issued.

PR's that deal with documentation, and other adjacent files (README for example) can be pushed to the _master_ branch.

When submitting PR's please take into account:
* the project's goals
* PEP8 and the style guide below

# Testing

You can use tox to run tests locally. Example for the unit tests with Python version 3.7:

```console
tox -e py27
```

Otherwise, you can just push and the tests will be run by GitHub Actions.

# Style guide

Just run [*black*](https://black.readthedocs.io) on modified files before sending the PR. There is no need to reinvent the wheel here!

**Tip**: Add a pre-commit hook with `pip install pre-commit && pre-commit install`
