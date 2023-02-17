# Using Snyk IaC with the Web UI

## View project vulnerabilities

Use Snyk IaC with the [Snyk Web UI](../../getting-started/quickstart/create-a-snyk-account/snyk-web-ui.md) to find and fix issues in configuration files.

1. In your **Projects** area, select the project to open
2. Snyk IaC displays information and issue cards for that project:

![](<../../.gitbook/assets/image (2) (3) (1) (1) (1) (1) (1) (1) (1) (2).png>)

Information available shows standard Snyk Project information (see [introduction-to-snyk-projects](../../manage-issues/introduction-to-snyk-projects/ "mention")), including:

* Snapshot information showing when the project was last tested.
* **Overview**, **History** and **Settings** information. For example, use the **History** section to view previous snapshots of projects.
* Filters on the left of the screen.

## Issue card details

Each issue card shows specific details about that issue:

![](<../../.gitbook/assets/Screenshot 2022-05-23 at 14.24.14.png>)

Card details include:

* The severity level (for example, **H** for high) and the name of the issue (for example, **Non-encrypted S3 Bucket**).
* The **ID** of the security rule (e.g. **SNYK-CC-TF-4**): click the link to view more information in the [Snyk Security Rules](https://snyk.io/security-rules).
* A **snippet** of your code showing the exact area that is vulnerable.
* The exact **path** of the issue.
* More details, such as:
  * a short **description** of the issue
  * the **impact** of the issue
  * the **remediation** advice to resolve the issue

Click **Full details** to see a preview of the full code:

![](<../../.gitbook/assets/Screenshot 2022-05-23 at 14.24.20.png>)

Click **Ignore** to ignore this vulnerability (see [Ignore Issues](../../manage-issues/issue-management/ignore-issues.md))

### Notes

* Terraform Cloud and Helm will not show a code snippet, but just the card details. They will also not have a **Full details** button to show the preview of the full code.\
  Examples:

![](<../../.gitbook/assets/image (114) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (2).png>)

![Terraform Cloud](<../../.gitbook/assets/image (100) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (4).png>)

* In some cases that we can not identify the exact line of the vulnerable path in the file, we will not show a code snippet, but an info message and the card details. If able to, we will show the **Full details** button so that a preview of the full code can be seen.\
  Example:

![](<../../.gitbook/assets/Screenshot 2022-05-23 at 14.28.07 (1).png>)

![](<../../.gitbook/assets/Screenshot 2022-05-23 at 14.28.17 (1).png>)
