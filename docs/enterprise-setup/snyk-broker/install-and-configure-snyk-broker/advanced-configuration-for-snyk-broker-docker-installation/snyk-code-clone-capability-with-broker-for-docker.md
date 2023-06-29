# Snyk Code - Clone capability with Broker for Docker

{% hint style="info" %}
**Feature availability**

The environment variable to enable Git clone capabilities is currently in closed beta. Contact your Snyk account management team to find out more.
{% endhint %}

By default, the Git clone capabilities required by Snyk Code are disabled. To grant Broker access to perform a Git clone of your repository, add the environment variable: `ACCEPT_CODE=true`.

Example:

```
docker run --restart=always \
           -p 8000:8000 \
           -e BROKER_TOKEN=secret-broker-token \
           -e GITHUB_TOKEN=secret-github-token \
           -e PORT=8000 \
           -e BROKER_CLIENT_URL=http://my.broker.client:8000 \
           -e ACCEPT_CODE=true
       snyk/broker:github-com
```

This adds the necessary `accept` rules for your choice of Git server. These rules are in the [client templates in the Broker GitHub repository](https://github.com/snyk/broker/tree/master/client-templates).

If custom `accept` rules are required, you can provide a custom `accept.json`.

Example:

```console
docker run --restart=always \
           -p 8000:8000 \
           -e BROKER_TOKEN=secret-broker-token \
           -e GITHUB_TOKEN=secret-github-token \
           -e PORT=8000 \
           -e BROKER_CLIENT_URL=http://my.broker.client:8000 \
           -e ACCEPT=/myFolder/accept.json
       snyk/broker:github-com
```

If you are using a custom `accept` file from a separate folder, with the `ACCEPT` environment variable, you cannot use the `ACCEPT_CODE` mechanism.

You can find the relevant `accept.json` for each of the Git integrations in [Adding custom allowlist for Docker installation](adding-custom-allowlist-for-docker-installation.md).

If you want to customize the `accept.json`, add this snippet to your custom `accept.json`

```
{
    "//": "used to redirect requests to snyk git client",
    "method": "any",
    "path": "/snykgit/*",
    "origin": "${GIT_CLIENT_URL}"
}
```

This snippet is valid for all Git integrations.
