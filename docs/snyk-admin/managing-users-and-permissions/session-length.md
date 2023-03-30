# Session length

By default, inactive logged-in users are automatically logged out after 30 days to protect any account from being exposed inadvertently through user inactivity.

You can change this 30-day default period, setting session length for any time between 5 minutes and 30 days.

{% hint style="info" %}
Users who belong to multiple Groups are always logged out automatically after the shortest time configured for any of those Groups.
{% endhint %}

## Configure session length for a Snyk Group

Group admins can change the default session length of the maximum, 30 days, to any value from 5 minutes to 30 days.

### **Prerequisites for configuring session length**

You must be an administrator of the Group to update the session length.

This feature is available to plans that support Groups. See [pricing plans](https://snyk.io/plans/) for more details.

### **Steps to configure session length**

1. Log in to your Snyk account and navigate to the Group for which you want o configure session length.
2. Navigate to **Settings** to update the Group settings.
3. In the **Session expiration** area, enter values for the session length:

<figure><img src="../../.gitbook/assets/uuid-21093b2a-7003-b47a-cb62-2e6dd147323e-en.png" alt="Group settings, change Session expiration"><figcaption><p>Group settings, change Session expiration</p></figcaption></figure>

When session length expiration has been configured, tracking of session length starts within 60 seconds or when a user logs in, whichever comes first.
