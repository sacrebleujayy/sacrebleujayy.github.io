# Login Guidelines
Guidelines for making sure your login page and processing is secure.

The login page is the single protection to the customer from hackers. If a hacker can figure out how to get you or the login page to return your session cookie, you are fracked.

## Use Someone Else's Login Functionality
Rather than risking having to maintain login functionality, use a SSO.

### SSO Providers
- [Amazon Cognito](https://aws.amazon.com/cognito/)
- OneLogin
- Okta

## Role Your Own
If you're going to decide to create your own login and do all the work

### Protect Customers from Brute Force & Dictionary Attacks
Implement a Captcha. Implement rate limiting. Implement account lockout. Implement *something*. Whatever you do, do not leave the login page open to brute force, social engineering, dictionary attacks.

### Review Password Guidelines
[Password Guidlines](../passwords/guidelines.md)
