envsubst-orb
===

CircleCI orb to use envsubst command

https://circleci.com/orbs/registry/orb/sawadashota/envsubst

Usage
---

```yaml
orbs:
  envsubst: sawadashota/envsubst@volatile
version: 2.1
job:
  echo-version:
    image:
      - docker: circleci/python:3.8
    steps:
      - envsubst/install
      - run: which envsubst
```