# Visual Studio Code extension authentication

To scan your projects you must authenticate with Snyk. The extension uses your Snyk API token for authentication. To store the token securely, Snyk uses [Secret Storage API](https://code.visualstudio.com/api/references/vscode-api#SecretStorage), which uses the system's keychain to manage the token.

## Logging in

To authenticate follow these steps:

1.  Once the extension is installed, click on the Snyk Icon in the left navigation bar:

    <img src="../../../.gitbook/assets/image (130) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (2) (1) (1) (1) (6).png" alt="" data-size="original">
2.  Click **Connect VS Code with Snyk**. The extension relies on the Snyk authentication API and asks you to authenticate your machine against the Snyk web application:

    <img src="../../../.gitbook/assets/image (147) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (2).png" alt="" data-size="original">
3. Click **Authenticate**.
4.  After successful authentication, view the confirmation message.

    <img src="../../../.gitbook/assets/image (154) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (2).png" alt="" data-size="original">
5. Close the browser window and return to VS Code. VS Code is now reading and saving the authentication on your local machine.

## Switching accounts

To re-authenticate with a different account, follow these steps:

1. Run the provided `Snyk: Log Out` command.
2. Once logged out, click **Connect VS Code with Snyk** to authenticate with the different account.

![Snyk: Log Out](../../../.gitbook/assets/logging-out-command.png)

Or you run `Snyk: Set Token` command and set your token in the text field manually.

![Set token manually](<../../../.gitbook/assets/image (224) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png>)

## Requirements for Linux and Unix

When authenticating with Snyk, users have the option to copy the authentication URL to their clipboard.

For Linux and Unix users, this requires that the `xclip` or `xsel` utility be installed.
