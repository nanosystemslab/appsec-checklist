# Command Register and Safety Review

| Command | Who/what may issue it | Preconditions | Safety limits | Interlock | Logged fields | Failure behavior |
|---|---|---|---|---|---|---|
| | | | | | | |

Required tests:
- Unauthorized user blocked.
- Wrong device ID blocked.
- Out-of-range command blocked.
- Replay/malformed command blocked or harmless.
- Command log created.
- Device enters safe state on connection loss or command failure.
