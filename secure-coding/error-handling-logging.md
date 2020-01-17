# Error Handling and Logging

- Handle all errors
- No stacktrace or database errors on the screen
- Never fail into an unknown state. Fail safe - Fail close
- Rollback to any transaction it was performing
- Log errors
- Don't show if its username or password
- Security-related errors (login fail, access control failures, server-side input validation failures) should issue a system alert
- Log Bruteforce attempts (10 successive failed login in under 1 minute or 100 or more failed attempts in on 24h period)
- Log all security related events

Logs must contain:

- type of event
- when the event happened
- the source (IP) X-Forwarded-For header ?
- the outcome of the event
- if possible the identity of any individuals associated

Using and protecting logs:

- protect log files, audit trails and the backups
- uniform logs in the same place, readable by the SIEM
- Only authorized indiduals should have logs access
- Logs should be stored encrypted
- Logs should be accessible by the incident response team
- Logs should be stored on a secure server / area
- Kigs should be incorporated in the backup strategy
- Treat logs and media like sensitive information
