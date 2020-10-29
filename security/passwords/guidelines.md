# Password Creation Guidelines

- [Dropbox Password Creation Guidelines](https://help.dropbox.com/accounts-billing/create-delete/secure-password)

# Password Storage Guidelines
- Hashed with a Salt (not encrypted, and **never** plaintext):
    - Why? Encryption is reversible:
      - Developers can see your credentials
      - Anyone who gains access to that developers' credentials
      - Any hacker that finds the encryption key.
        - How did the hacker find the encryption key?
        - That's right, *the developer posted it on GitHub* :facepalm: 
    - [Hashing libraries](https://security.stackexchange.com/questions/211/how-to-securely-hash-passwords/31846#31846)
      - Why shouldn't you create your own hashing / encryption library? Maintenance is the biggest fighter of security. Don't try to recreate the wheel. Especially when the wheel is already rolling down the hill and the leading experts in security are trying to create the next fight in security: Quantum Computers.

## Source
- [StackOverflow to the Rescue](https://security.stackexchange.com/questions/211/how-to-securely-hash-passwords/31846#31846)
