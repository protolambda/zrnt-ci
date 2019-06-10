# ZRNT CI

CI utils for [ZRNT](https://github.com/protolambda/zrnt)

## Primary Dockerfile

This is a custom Golang docker image for testing,
 it is lightweight (alpine linux), and supports:
- Git
- Git LFS (to pull in test vectors)
- tar, gzip
- curl (to pull in scripts / data)
- make
- bash: for scripting & coverage report upload (codecov)
- gotestsum: for nice formatting of test runs,
 and building the test report in Junit-style XML.

```bash
docker build -t protolambda/zrnt-ci-primary:1.0.0 primary
```
