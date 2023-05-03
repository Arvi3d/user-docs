# Authentication for the Eclipse plugin

Once the CLI is downloaded you will be redirected to the browser to authenticate and then connect the IDE with your account.

## Steps in authentication

* You get a notification that a browser window will open (lower right).

![Notification, browser window opening for authentication](<../../../.gitbook/assets/Screenshot 2022-05-13 at 11.29.37.png>)

* Once you are redirected to the browser for authentication, click **Authenticate**.

![Authenticate](<../../../.gitbook/assets/Screenshot 2022-05-13 at 11.30.02.png>)

* You should see a successful message saying you've been authenticated.

![Confirmation of authentication](<../../../.gitbook/assets/Screenshot 2022-05-13 at 11.30.30.png>)

* Going back to the IDE, you should see a confirmation that the IDE has been successfully connected and the API token has been securely stored (lower right).

![Confirmation of connection](<../../../.gitbook/assets/Screenshot 2022-05-13 at 11.30.54.png>)

To verify that the Eclipse plugin is ready to start scanning, be sure the Snyk preferences show the following after the downloads and the authentication are done:

* Language server path that the Eclipse plugin will use
* Snyk CLI path that the Eclipse plugin will use
* Snyk API token, securely stored through the Eclipse's secure storage mechanism

![Snyk preferences](<../../../.gitbook/assets/image (132) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (2).png>)

## Configure the API token manually

You can provide the API token by copying it from your [account settings](https://app.snyk.io/account) and paste it into the Eclipse preferences Snyk API Token field. Click **Apply and Close** once the token has been set.

![Configure token](<../../../.gitbook/assets/image (139) (1) (1).png>)

## Next steps

Change the [configuration settings](https://docs.snyk.io/ide-tools/eclipse-plugin/configuration-of-the-eclipse-plugin) as needed and set the [environment variables](https://docs.snyk.io/ide-tools/eclipse-plugin/environment-variables-for-the-eclipse-plugin).
