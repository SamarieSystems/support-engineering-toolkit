# Design principles

## Support is a signal

Repeated tickets indicate a system, product, policy, or knowledge-transfer
failure. The immediate fix matters, but it should also produce evidence for a
durable fix.

## Expected script behavior

- Detect state before changing it.
- Prefer idempotent operations.
- Log decisions and results.
- Exit safely when prerequisites are missing.
- Explain errors in language an operator can act on.
- Make rollback explicit when practical.
- Preserve attribution and licensing.