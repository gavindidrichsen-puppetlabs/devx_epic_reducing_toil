# 1. Record architecture decisions

Date: 2024-07-03

## Status

Accepted

## Context

We need to record the architectural decisions made on this project.

## Decision

We will use Architecture Decision Records, as [described by Michael Nygard](http://thinkrelevance.com/blog/2011/11/15/documenting-architecture-decisions).

If making a change to code warrants more explanation, then consider adding a separate design decision document or `ADR`:

* [adr-tools](https://github.com/npryce/adr-tools)
* [adr-log](https://github.com/adr/adr-log)

Follow these steps to add a new design decision and update the README:

```bash
# initialize the ADR directory
adr init

# create a new design decision, e.g., `adr new "Title of your design decision"`
adr new "Do whiteboard wednesday talks" 

# fill in the "Context", "Decision", and "Consequences" of the new doc
vim doc/adr/0002-do-whiteboard-wednesday-talks.md

# update the `README.md` table of contents to include the newest design decision
adr-log -i README.md -d doc
```

## Consequences

See Michael Nygard's article, linked above. For a lightweight ADR toolset, see Nat Pryce's [adr-tools](https://github.com/npryce/adr-tools).
