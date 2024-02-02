# Janus IDP Project Governance

## Triagers

Triagers assess newly-opened issues in the [janus-idp/backstage-plugins][] and [janus-idp/backstage-showcase][] repositories. The GitHub team for Janus IDP triagers is `@janus-idp/issue-triage`.

Triagers are given the "Triage" GitHub role and have:

* Ability to label issues and pull requests
* Ability to comment, close, and reopen issues and pull requests

## Maintainers

Janus IDP maintainers maintain the `janus-idp/*` GitHub repositories. The GitHub team for Janus IDP maintainers is `@janus-idp/maintainers`.

Additionally per-area maintainer GitHub teams exist. These teams own individual plugins or repositories via `CODEOWNERS` files. All project area specific maintainer teams are child teams of the `@janus-idp/maintainers`.

Maintainers have:

* Commit access to the repository they co-maintain.

Both maintainers and non-maintainers may propose changes to the Janus IDP source code. The mechanism to propose such a change is a GitHub pull request. Maintainers review and merge pull requests.

Single maintainer must approve a pull request before the pull request can be merged. Approving a pull request indicates that the maintainer accepts responsibility for the change. Approval must be from maintainer who are not authors of the change.

If a maintainer opposes a proposed change, then the change cannot land. The exception is if the TSC votes to approve the change despite the opposition. Usually, involving the TSC is unnecessary. Often, discussions or further changes result in collaborators removing their opposition.

## Technical Steering Committee

A subset of the maintainers forms the Technical Steering Committee (TSC). The TSC has final authority over this project, including:

* Technical direction
* Project governance and process (including this policy)
* Contribution policy
* GitHub repository hosting
* Conduct guidelines
* Maintaining the list of maintainers

A GitHub team for TSC is `@janus-idp/steering`. This group has admin access to all repositories within the organization.

## Maintainer activities

* Helping users and novice contributors
* Contributing code and documentation changes that improve the project
* Reviewing and commenting on issues and pull requests
* Participation in working groups
* Merging pull requests

The TSC can remove inactive maintainers or provide them with _emeritus_ status. Emeriti may request that the TSC restore them to active status.

A maintainer is automatically made emeritus (and removed from active maintainer status) if it has been more than 12 months since the contributor has authored or approved a commit that has landed.

The status of each individual maintainer is subjected to review by TSC annually.

## Maintainer nominations

Existing maintainers can nominate someone to become a maintainer. Nominees should have significant and valuable contributions across the Janus IDP organization.

To nominate a new maintainer, open an issue in the [janus-idp/.github][] repository. Provide a summary of the nominee's contributions. For example:

* Commits in the `janus-idp/*` repositories
  * Use the link `https://github.com/janus-idp/REPO/commits?author=GITHUB_ID`
* Pull requests and issues opened in the `janus-idp/*` repositories
  * Use the link `https://github.com/janus-idp/REPO/issues?q=author:GITHUB_ID`
* Comments on pull requests and issues in the `janus-idp/*` repositories
  * Use the link `https://github.com/janus-idp/node/issues?q=commenter:GITHUB_ID`
* Reviews on pull requests in the `janus-idp/*` repositories
  * Use the link `https://github.com/janus-idp/node/pulls?q=reviewed-by:GITHUB_ID`
* Help provided to end-users and novice contributors
* Pull requests and issues opened throughout the Janus IDP organization
  * Use the link  `https://github.com/search?q=author:GITHUB_ID+org:janus-idp`
* Comments on pull requests and issues throughout the Janus IDP organization
  * Use the link `https://github.com/search?q=commenter:GITHUB_ID+org:janus-idp`
* Participation in other projects, teams, and working groups of the Janus IDP organization
* Other participation in the wider Janus IDP community

Mention `@janus-idp/maintainers` in the issue to notify other maintainers about the nomination.

The nomination passes if no maintainer oppose it after one week. Otherwise, the nomination fails.

Collaborators might overlook someone with valuable contributions. In that case, the contributor may open an issue or contact a maintainer to request a nomination.

Collaborators who authored a plugin that was accepted by the Janus IDP community as a code donation automatically become maintainers of said plugin.

## Onboarding

After the nomination passes, a TSC member onboards the new maintainer.

## Consensus seeking process

The TSC follows a [Consensus Seeking][] decision-making model.

## Annual Access Review

The TSC will review access to repositories at least annually. The purpose of this review is to ensure that only authorized individuals have access to the repositories and that they have the appropriate permissions.

During the review, the TSC will:

1. Verify the list of people with access to the repositories and their respective permissions.
2. Check for any unauthorized access, such as team members who have left the project but still have write access to the repositories.
3. Document the date of the review, the list of repositories reviewed, and the results of the review.

If any unauthorized access is detected, the TSC will take corrective actions and consult the Red Hat Information Security team that offered their assistance and support.

The TSC will maintain records of review results, including the date the review was performed and any changes made to repository access.

## Project areas

Janus IDP community defines following project areas that have separate maintainers group

### Plugins

The [janus-idp/backstage-plugins][] repository has an maintainers group for the whole plugin ecosystem. The GitHub team for Janus IDP plugin maintainers is `@janus-idp/maintainers-plugins`. This group is a child of `@janus-idp/maintainers`. The group has a write access to the [janus-idp/backstage-plugins][] and is set to be the default `CODEOWNER` on this repository.

Individual plugins can have their own maintainers, separate from the rest. This is defined via `CODEOWNERS`.

### Showcase

The `@janus-idp/maintainers-showcase` GitHub team maintains the [janus-idp/backstage-showcase][] repository. This team has a write access to that repository. This team is the default `CODEOWNER` for this repository.

### Helm


https://github.com/orgs/redhat-developer/teams/rhdh-helm

The `@redhat-developer/rhdh-helm` GitHub team has write access to, and maintains, the https://github.com/redhat-developer/rhdh-chart repo. This team is the default `CODEOWNER` for this repository.

### GPTs

The maintainers group for golden path templates stored in the [janus-idp/software-templates][] has a separate GitHub team named `@janus-idp/maintainers-gpt`. This team has a write access to the [janus-idp/software-templates][] repository. This team is the default `CODEOWNER` for this repository.

### Demo

The `@janus-idp/maintainers-demo` GitHub team maintains the [janus-idp/demo-setup][]. This team has a write accesss to the that repository. This team is the default `CODEOWNER` for this repository.

### Community website

The `@janus-idp/maintainers-website` GitHub team maintains the [janus-idp/janus-idp.github.io][]. This team has a write accesss to the that repository. This team is the default `CODEOWNER` for this repository.

### Blog

There is one more distinct maintainer team within the [janus-idp/janus-idp.github.io][] repository overseeing the blog content. This team has a write accesss to the that repository. This team is the default `CODEOWNER` for this repository. This group has a GitHub team named `@janus-idp/maintainers-blog` and is the `CODEOWNER` for all `.md` and `.mdx` files within this repository.


### Documentation

A separate maintainers group exist across all the repositories with authority over all `.md` and `.mdx` file changes. This team has a separate `@janus-idp/maintainers-docs` GitHub team.

### QE

The `@janus-idp/maintainers-qe` GitHub team maintains the [janus-idp/showcase-e2e][]. This team has a write accesss to the that repository. This team is the default `CODEOWNER` for this repository.

[Consensus Seeking]: https://en.wikipedia.org/wiki/Consensus-seeking_decision-making
[janus-idp/backstage-plugins]: https://github.com/janus-idp/backstage-plugins
[janus-idp/backstage-showcase]: https://github.com/janus-idp/backstage-showcase
[janus-idp/helm-backstage]: https://github.com/janus-idp/helm-backstage
[janus-idp/software-templates]: https://github.com/janus-idp/software-templates
[janus-idp/demo-setup]: https://github.com/janus-idp/demo-setup
[janus-idp/janus-idp.github.io]: https://github.com/janus-idp/janus-idp.github.io
[janus-idp/showcase-e2e]: https://github.com/janus-idp/showcase-e2e
