# Securing your cookies

- encrypted not encoded
- key stored on the server ( a secure location )
- use secure cookies for sessionID, tokens, account number...
- use the 'secure' attribute to send cookies
- HTTP Strict Transport Security Header
- Use HTTPOnly security header to block cookies from access attempts from client side-scripts

[JWS is NOT a secure cookie](https://www.youtube.com/watch?v=td-2rN4PgRw&feature=youtu.be), it's encoded, not encrypted
