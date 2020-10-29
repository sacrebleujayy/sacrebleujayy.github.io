# Login Guidelines
Guidelines for making sure your login page and processing is secure.

The login page is the single protection to the customer from hackers. If a hacker can figure out how to get you or the login page to return your session cookie, you are fracked.

## Protect Customers from Brute Force & Dictionary Attacks
Implement a Captcha. Implement rate limiting. Implement account lockout. Implement *something*. Whatever you do, do not leave the login page open to brute force, social engineering, dictionary attacks.
