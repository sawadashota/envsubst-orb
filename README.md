envsubst-orb [![CircleCI](https://circleci.com/gh/sawadashota/envsubst-orb/tree/master.svg?style=svg)](https://circleci.com/gh/sawadashota/envsubst-orb/tree/master)
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
      - docker: circleci/python:3.12
    steps:
      - envsubst/install
      - run: which envsubst
```