# Support Engineering Toolkit

Production-minded automation for endpoint management, identity, security,
migrations, diagnostics, and repeatable support operations.

## Why this repository exists

I do not want to be the engineer who heroically fixes the same problem forever.
These tools are built to contain the immediate issue, capture enough evidence
to understand the real failure, and make the next occurrence safer or
unnecessary.

The intended operator is not only the person who wrote the script. Tools should
check state before changing it, fail clearly, log what they did, and give a
newer technician enough context to act without guessing.

## Repository map

- scripts/endpoint-management
- scripts/identity-and-access
- scripts/security-hardening
- scripts/software-deployment
- scripts/diagnostics-and-remediation
- scripts/networking-and-voip
- scripts/microsoft-365
- scripts/utilities
- docs

## Safety and provenance

The default refactor process excludes any source file that produces a security
or redistribution finding. The detailed scan report is intentionally kept
outside this Git repository.