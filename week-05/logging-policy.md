# Logging policy
- INFO: successful business events using opaque resource IDs.
- WARN: rejected user/business operation that does not indicate a server fault.
- ERROR: unexpected failures with exception context, without exposing request secrets.
- Never log passwords, authorization headers, payment-card details, tokens or full personal records.
- Return a generic internal error message to clients; retain diagnostic detail only in protected server logs.
