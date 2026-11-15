# Token authorization

KeyAuth rejected the session before the overlay started.

This is an auth problem, not a Discord overlay problem. The splash shows **KeyAuth failed (0xA06)** or a token / license message.

1. Confirm the key is for Ascendency and has not expired.
2. Check the PC clock is correct (wrong date breaks auth).
3. Disable VPN for the login, then retry.
4. Delete `%LOCALAPPDATA%\asc\cred.json` and paste the key again.
5. If it still says the token must be provided, the application token on the KeyAuth side is wrong — that is staff-only. Open a ticket.

See [0xA06 — KeyAuth failed](../errors/0xa06.md).
