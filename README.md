# Atomist Vulnerability and Advisory DB

This repository contains private advisories to be managed as part of the Atomist
Vulnerability Database. Information in this repository will not be part of the
global Atomist Vulnerability Database.

Advisories are managed in JSON files placed in directories of this repository.

## Managing Advisories

### Adding Advisories

Creating new advisories can be achieved by either creating a new JSON advisory
file in the `main` branch by manually or by opening a new GitHub issue
using the [_New advisory_](ADVISORY_TEMPLATE.json) issue template. Once the
issue is raised, a pull request with a new skeleton advisory JSON file is
opened.

The content of advisory JSON files strictly follows the schema defined in
[Open Source Vulnerability (OSV) format](https://ossf.github.io/osv-schema/).
Take a look at the
[GitHub Advisory Database](https://github.com/github/advisory-database/tree/main/advisories/github-reviewed)
for examples of advisories.

### Updating Advisories

To update an advisory, change the corresponding JSON advisory file either
directly in the `main` branch of this repository or raise a pull request
with your updates.

Once the changes are committed to the `main` branch, the advisory will get
updated in the database automatically. A GitHub Check will indicate the
successful update of the advisory.

### Deleting Advisories

Deleting an advisory from the database can be achieved by removing the
corresponding JSON advisory file from the `main` branch of this
repository.

> 💡 Only additions, changes and removals of JSON advisory files in the
> repository's default branch are being processed and mirrored into the
> database.
