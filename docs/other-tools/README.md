# Snyk Tools

## Scope of Snyk Tools

Snyk Tools help with specific "pain points" that may not be addressed by Snyk product functionality, regardless of whether you use Snyk through the Web UI, CLI, API, or an integration.

{% hint style="info" %}
You must have a [Snyk Account](https://snyk.io/login?cta=sign-up\&loc=nav\&page=support\_docs\_page) with populated projects to use Snyk Tools.
{% endhint %}

## Available Snyk Tools

### Key Tools

Snyk provides full documentation for the following key Snyk Tools:

* [snyk-api-import (docs)](tool-snyk-api-import/): Bulk import projects into Snyk in a robust, paced way. Repo: [snyk-api-import](https://github.com/snyk-tech-services/snyk-api-import)
* [snyk-delta (docs)](tool-snyk-delta.md): Get the delta between two Snyk snapshots. Repo: [snyk-delta](https://github.com/snyk-tech-services/snyk-delta)
* [snyk-filter (docs)](tool-snyk-filter.md): Takes the JSON output from the Snyk CLI, and applies custom filtering of the results. Repo: [snyk-filter](https://github.com/snyk-tech-services/snyk-filter)
* [jira-tickets-for-new-vulns (docs)](tool-jira-tickets-for-new-vulns.md): Sync your Snyk monitored projects and auto-open JIRA tickets for issues. Repo: [jira-tickets-for-new-vulns](https://github.com/snyk-tech-services/jira-tickets-for-new-vulns)
* [snyk-scm-contributors-count (docs)](snyk-scm-contributors-count-cli-tool/): Count contributors for your SCM repos with commits in the last 90 days. Repo: [snyk-scm-contributors-count](https://github.com/snyk-tech-services/snyk-scm-contributors-count).

### Additional Snyk Tools

For additional Snyk Tools, **refer to the repos** for usage instructions:

* [snyk-disallow](https://github.com/snyk-tech-services/snyk-disallow): Get a viewer token for the Snyk Group to get a read|test-only token for CI or similar systems.
* [snyk-prevent-gh-commit-status](https://github.com/snyk-tech-services/snyk-prevent-gh-commit-status): POST commit status of a PR the result of [snyk-delta](https://github.com/snyk-tech-services/snyk-delta) executed in the CI.
* [snyk-cr-monitor](https://github.com/snyk-tech-services/snyk-cr-monitor): Gather Docker repos to test, then iterate through results, to run multiple jobs simultaneously.
* [backstage-plugin-snyk](https://github.com/snyk-tech-services/backstage-plugin-snyk): Plugin to display security details from Snyk.
* [snyk-api-ts-client](https://github.com/snyk-tech-services/snyk-api-ts-client): Snyk API Typescript client.
* [snyk-transitive-ignore](https://github.com/snyk-tech-services/snyk-transitive-ignore): Generate the Snyk ignore policy dynamically based on a provided list of packages.
* [snyk-user-sync-tool](https://github.com/snyk-tech-services/snyk-user-sync-tool): Add, remove, and sync user memberships.
* [snyk-licenses-texts](https://github.com/snyk-tech-services/snyk-licenses-texts): Provides Organization level licenses used, copyrights, and dependencies data.
* [snyk-request-manager](https://github.com/snyk-tech-services/snyk-request-manager): Rate controlled and retry enabled request manager to interact with Snyk APIs.
* [snyk2spdx](https://github.com/snyk-tech-services/snyk2spdx): Convert the Snyk CLI output to SPDX format.
* [snyk-repo-issue-tracker](https://github.com/snyk-tech-services/snyk-repo-issue-tracker): A python script / module that allows for generating a changeset of issues between runs against the Snyk project issues API.
*   [snyk-repo-diff:](https://github.com/snyk-tech-services/snyk-repo-diff) Helps answer which repositories aren't monitored by Snyk.

    This works by retrieving a list of all projects in a given Snyk Group (all projects in all orgs belonging to the same Snyk Group) and associating them with a list of repositories found in a given GitHub Organization (see below section on GitLab support),
* [snyk-issues-to-csv](https://github.com/snyk-tech-services/snyk-issues-to-csv): A python script that uses the PySnyk module along with the Pandas modules to collect all issues from the report API and combine them into a single CSV for an entire group.
* [snyk-bulk](https://github.com/snyk-tech-services/snyk-bulk): Recursively scan source repositories for open source vulnerabilities with the Snyk CLI, outside of a build environment.
* [snyk-bulk-action-scripts](https://github.com/snyk-tech-services/snyk-bulk-action-scripts): A collection of scripts to edit integration settings for every organization in a group in Snyk.
* [snyk-deps-to-csv](https://github.com/snyk-tech-services/snyk-deps-to-csv): Collects all dependencies from all orgs in a group and outputs to a CSV file.

## Tool ideas

Do you have an idea for a tool? If so, check out [Snyk Apps](../integrations/snyk-apps/), which provides an opportunity to mold your Snyk experience to suit your specific needs. You can also contact [Snyk Support](https://support.snyk.io/hc/en-us/) with questions.
