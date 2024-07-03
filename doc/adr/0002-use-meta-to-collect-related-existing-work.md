# 2. Use meta to collect related existing work

Date: 2024-07-03

## Status

Accepted

## Context

Members of puppet and the community have already attempted to solve a number of module maintenance challenges like updating module dependencies, removing old dependencies, and comparing the impact of changes.  To make it easier for others to review and work on these related repositories I wanted to collect them together under one coordinating or "parent" repository.

[meta](https://github.com/mateodelnorte/meta-npm) is an effective tool for creating such a parent.  I have used this tool for other collections.

## Decision

Therefore, I decided to use `meta` to collect diverse repositories in one place for reference.

## Consequences

Now sharing a collection of related repositories is easy.  Adding new ones to the collection is very simple.  See below to get started with this repository:

```bash
# gather all the child repositories
meta git update

# add a new child repository beneath a directory
meta import my/collection/cool_repo https://github.com/organization/cool_repo.git

# run a command on all repositories
meta exec 'git checkout -b fix_a_problem_branch'
```
