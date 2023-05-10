# Usage settings

Select **Settings** > **Usage** to view Snyk usage details in your Group or Organization, including:

* [Test usage](usage-settings.md#test-usage): the number of tests used
* [Contributing developers](usage-settings.md#contributing-developers): the number of developers contributing to Projects
* [Projects](usage-settings.md#projects): Project test usage settings (can be viewed and modified)

## Test usage

The **Test Usage** section shows how many tests you are using over the current billing period:

<figure><img src="../../.gitbook/assets/test-usage.png" alt="Test usage data" width="563"><figcaption><p>Test usage data</p></figcaption></figure>

{% hint style="info" %}
Test limits vary for Snyk products and plans. See the [plans page](https://snyk.io/plans/) for details.
{% endhint %}

{% hint style="info" %}
See [What counts as a test?](https://support.snyk.io/hc/en-us/articles/360000925418-What-counts-as-a-test-) for details of how Snyk counts tests.
{% endhint %}

## Contributing developers

{% hint style="info" %}
The integrations for which Snyk has developer counts are GitHub, GitHub Enterprise, GitLab and the Snyk CLI.
{% endhint %}

Snyk defines contributing developers as developers having made a commit to a private repo monitored by Snyk in the last 90 days.

The **Contributing developers for Git and CLI integrations** section shows contributing developer counts, both at the org level and the group level.

The counts indicate the number of contributing developers to the default branch of the private repos connected with the integration.

Snyk does not count contributions to public (open source) repos currently as the pricing model is based on the number of contributing developers to private repositories.

For example:

<figure><img src="../../.gitbook/assets/image__10_.png" alt="Contributing developers counts"><figcaption><p>Contributing developers counts</p></figcaption></figure>

* **Total unique contributors across all integrations:** the number of contributors across all the integrations in your Snyk account. Contributing developers are only counted once, even if they have contributed to multiple integrations or multiple repositories.
* **Breakdown by integration**: the number of contributors, Organizations, and repos in that integration.

Each contributor is **counted by** the **author** email field, which is set within the local Git configuration in the developer’s machine.

## Projects

The **Projects** section shows test usage settings for your Projects:

### Bulk actions

For **Bulk actions**, select relevant Projects, then for the selected Projects, select **Delete**, **Activate** or **Deactivate**:

<figure><img src="../../.gitbook/assets/usage-projects-bulk-actions.png" alt="Bulk actions on Projects" width="563"><figcaption><p>Bulk actions on Projects</p></figcaption></figure>

### Set test frequency

You can set the frequency of testing for each Project.&#x20;

For each entry, you can select the frequency of testing for that Project (never, daily, or weekly) as applicable to the type of Project, Open Source, Code analysis, Container, or IaC:

<figure><img src="../../.gitbook/assets/usage-projects-single.png" alt="Select test frequency"><figcaption><p>Select test frequency</p></figcaption></figure>

{% hint style="info" %}
The default test frequency and limitations are as follows:

* Open Source: The default is daily.
* Code analysis Projects: The default is weekly; daily is not available. To test your code daily, submit a request to [Snyk Support.](https://support.snyk.io/hc/en-us/requests)
* Container: The default is daily.
* IaC: The default is weekly.
{% endhint %}

Click **Deactivate** to never test, and also remove webhooks and stop showing the Project’s results in reporting.
