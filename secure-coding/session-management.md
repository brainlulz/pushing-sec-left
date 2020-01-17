# Session management

- Use tools from your framework
- Session ID passed over encrypted channels
- Session ID at least 128 characters long
- Random session ID (use a tool to get a random)
- Destroy session after loggout
- Only use sessionID to identify the session
- Suspicious activity if unknown sessionID, block ID
- Never pass the sessionID in url but secure cookie
- Regenerate SessionID during auth, reauth or privilege level change
- The sessionID should have an end time
