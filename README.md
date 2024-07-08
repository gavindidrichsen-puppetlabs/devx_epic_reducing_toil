# devx_epic_reducing_toil

## Description

Maintaining puppet code, e.g., keeping modules up-to-date, is for many organizations a very difficult activity.  Over the years both `puppetlabs` and `vopupuli` organizations have attempted to reduce this maintenance toil with various tools.  Some of these tools are collected here for reference and to encourage further development.  The current list of repositories can be seen in the [.meta](.meta) and will look something like this:

```json
{
  "projects": {
    "building_blocks/catalog_impact/puppet-catalog-diff-viewer": "https://github.com/voxpupuli/puppet-catalog-diff-viewer.git",
    "building_blocks/catalog_impact/puppet-catalog_diff": "https://github.com/voxpupuli/puppet-catalog_diff.git",
    "building_blocks/dependabots/dependabot-core": "https://github.com/dependabot/dependabot-core.git",
    "building_blocks/dependabots/renovate": "https://github.com/renovatebot/renovate.git",
    "building_blocks/module_health/dependency_checker": "https://github.com/puppetlabs/dependency_checker.git",
    "building_blocks/module_health/puppet-ghostbuster": "https://github.com/voxpupuli/puppet-ghostbuster.git",
    "building_blocks/module_health/puppetfile-resolver": "https://github.com/puppetlabs/puppetfile-resolver.git",
    "building_blocks/module_health/r10k-resolve": "https://github.com/binford2k/r10k-resolve.git",
    "building_blocks/module_health/ra10ke": "https://github.com/building_blocks/module_health/ra10ke.git",
    "building_blocks/testing/onceover": "https://github.com/voxpupuli/onceover.git"
  }
}
```

## Design Decisions

<!-- adrlog -->

* [ADR-0001](doc/adr/0001-record-architecture-decisions.md) - Record architecture decisions
* [ADR-0002](doc/adr/0002-use-meta-to-collect-related-existing-work.md) - Use meta to collect related existing work

<!-- adrlogstop -->

## Setup

Ensure the folowing is installed

* [meta](https://github.com/mateodelnorte/meta-npm)

## Usage

```bash
# checkout all child repositories
meta git update
```

## Contributing

If making a change to code warrants more explanation, then consider adding a separate design decision with `adr new "Do this so that"` and updating the root README with `adr-log -i README.md -d doc`.  For more information see [ADR-0001](doc/adr/0001-record-architecture-decisions.md).
