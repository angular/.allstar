# Allstar configuration for GoogleContainerTools

[Allstar](https://github.com/ossf/allstar) is a security-policy GitHub app. It is
installed for all repositories in the Angular organization. This repository contains the root
configuration for the app.

## Enabled Repos

Currently Allstar is enabled on only the following repositories:

- [angular/.allstar](https://github.com/angular/.allstar)
- [angular/angular](https://github.com/angular/angular)
- [angular/angular-cli](https://github.com/angular/angular-cli)
- [angular/components](https://github.com/angular/components)
- [angular/dev-infra](https://github.com/angular/dev-infra)

In the future AllStar is planned to be enabled for all repositories in the Angular organization.

## Policy Configuration

These are the settings required to be in compliance

### [Branch Protection](branch_protection.yaml)

|                         |         |
| ----------------------- | ------- |
| Enforce default branch  | true    |
| Other enforced branches | `*.*.x` |
| Require approval        | false   |
| Dismiss stale reviews   | false   |
| Block force push        | true    |

### [Outside Collaborators](outside.yaml)

- Push access not allowed.
- Admin access not allowed.

### [SECURITY.md](security.yaml)

- SECURITY.md required.

### [Binary Artifacts](binary_artifacts.yaml)

- No binary artifacts are allowed to be commited to the repository.
