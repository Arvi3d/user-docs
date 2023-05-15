# License policies

Group administrators can set license policies to define Snyk behavior for treating license issues. For example, you can allow or disallow packages with certain license types, to avoid using packages containing incompatible licenses.

You can [create a license policy and rules](create-a-license-policy-and-rules.md) for your Group.

### Initial default policy

An initial policy is created automatically and set as the default, to help you get started quickly with license policy management. This default policy is a baseline to answer the requirements of multiple types of applications (such as SaaS, distributed, and so on), and may be used as a starting point to calibrate additional license policies.&#x20;

The default license policy contains the standard **Snyk Default License Policy**, but the rules can be edited to match your preferences.

{% hint style="warning" %}
The default policy does not endorse or criticize any license, and should not be treated as legal guidance.
{% endhint %}

Any new Organizations that are created in your group are automatically added to the default policy. When an Organization is created, it can be moved to a different policy.
