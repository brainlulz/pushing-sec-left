# Authentication

Use features provided in your programming framework and test the implementation.

- If password based Auth = follow [NIST Password Standard](https://pages.nist.gov/800-63-3/sp800-63b.html)
- Pricinipe of least privilege, even for apps
- Salt and hash password before storing, not encrypted
- Encrypt password in transit (https only)
- Re-auth for sensitive features
- Prevent against bruteforce
- Mask password while entering it on the screen
- Validate authorization of the user on new page and action using whitelinsting
- Hidden is not protected or safe
- Log login fails and errors
- Log bruteforce with IP, notify the account owner
