# Security policy

Do not open a public issue containing credentials, customer information,
internal hostnames, private IP addresses, tenant identifiers, or production
logs.

Before publishing or contributing code:

- Replace credentials with parameters or environment variables.
- Replace customer and employer names with neutral examples.
- Remove internal domains, UNC paths, and private addresses.
- Confirm that third-party code permits redistribution.
- Scan Git history, not only the current working tree.

If a credential was committed, rotate or revoke it first. Deleting the visible
line does not remove it from repository history.