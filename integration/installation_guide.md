This integration will allow users to sign in by verifying ownership of an NFT.

## Prerequisites

1. An Auth0 account and tenant. [Sign up for free](https://auth0.com/signup).

## Set up Sign in with Vula Labs

Register your client by sending a POST to https://login.vulalabs.com/oauth/register with the body:

{
"email": "example@email.com",
"name": "example",
"redirectUris": ["https://example.com/oauth/callback],
"homepageUri": "https://example.com"
}

In the response will be the Client ID and Client Secret to use in the Connection setup steps below.

## Add the Connection

1. Select **Add Integration** (at the top of this page).
2. Read the necessary access requirements, and select **Continue**.
3. Configure the integration using the following fields:
   * Client ID obtained in the previous section
   * Client Secret obtained in the previous section
4. Select the **Permissions** needed for your applications.
5. Choose and configure whether to sync user profile attributes at each login.
6. Select **Create**.
7. In the **Applications** view, choose the Applications that should use this Connection to log in.

## Test connection

You're ready to [test this Connection](https://auth0.com/docs/authenticate/identity-providers/test-connections).
