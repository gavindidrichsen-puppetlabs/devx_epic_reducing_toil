# devx_epic_reducing_toil

## Description

Maintaining puppet code, e.g., keeping modules up-to-date, is for many organizations a very difficult activity.  Over the years both `puppetlabs` and `vopupuli` organizations have attempted to reduce this maintenance toil with various tools.  Some of these tools are collected here for reference and to encourage further development.

## Design Decisions

<!-- adrlog -->

* [ADR-0001](doc/adr/0001-record-architecture-decisions.md) - Record architecture decisions
* [ADR-0002](doc/adr/0002-use-meta-to-collect-related-existing-work.md) - Use meta to collect related existing work

<!-- adrlogstop -->

## Setup

* [meta](https://github.com/mateodelnorte/meta-npm)

## Usage

* Checkout all child repositories. For more information on `meta` see [ADR-0002](doc/adr/0002-use-meta-to-collect-related-existing-work.md).

```bash
meta git update
```

## Contributing

If making a change to code warrants more explanation, then consider adding a separate design decision with `adr new "Do this so that"` and updating the root README with `adr-log -i README.md -d doc`.  For mor information see [ADR-0001](doc/adr/0001-record-architecture-decisions.md).
