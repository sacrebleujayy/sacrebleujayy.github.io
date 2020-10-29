# Stored Plaintext Passwords Test
How to tell if a site is storing your passwords in plaintext:
- Is the password display or returned to you anywhere on the site or from the site?
  - Places to look:
    - Account Settings -> Password
    - Password Reset / Recovery
    - Change Password
- Asynchronous Password Actions:
    - Emailed about password validation
- Passwords rejected for being similar:
    - The password may be encrypted (not plaintext), but it still means it is reversible.
- Fast Response time:
    - Scripted approach:
      > When you send an authentication request, you can measure the time it took for the server to answer. During that delay, with normal password hashing, the server must have computed the hash function. For better accuracy send many authentication requests; if the server can handle 100 requests per second then you know that whatever hashing they used requires no more than 1/100th of their CPU power.

## Sources
- [7Labs](https://7labs.io/tips-tricks/find-out-whether-a-website-hashes-your-password-or-not-security-tips.html)
- [StackOverflow](https://security.stackexchange.com/questions/44802/how-to-tell-if-a-site-is-securely-storing-passwords/44809)
