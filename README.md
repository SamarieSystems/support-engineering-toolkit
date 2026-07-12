# Support Engineering Toolkit

Production-minded automation for the ugly middle ground between "the ticket is closed" and "the problem is actually gone."

This repository contains PowerShell and systems tooling built around a simple goal: solve the immediate problem, understand why it happened, and leave behind something safer, clearer, and easier for the next person to use.

I work in support-heavy systems engineering environments where problems rarely stay inside one clean boundary. A user issue may cross endpoint state, identity, policy, networking, security tooling, application behavior, and deployment history before the real failure becomes visible. These tools are the reusable pieces that came out of that work.

## What this repository is

This is a curated portfolio of operational automation for:

* Endpoint management and device enrollment
* Identity and access administration
* Security hardening and remediation
* Software deployment and removal
* Diagnostics and evidence collection
* Microsoft 365 administration
* Networking and VoIP troubleshooting
* Repeatable support operations

It is not intended to be a dump of every script I have ever touched.

A tool belongs here when it demonstrates a useful problem, a deliberate approach, and a result another technician can understand and repeat.

## How I think about support engineering

A ticket is often a symptom, not the whole problem.

The immediate fix matters because a person is blocked right now. The work is not finished, though, until I have answered some version of these questions:

1. What actually failed?
2. Why was the failure difficult to identify?
3. What evidence would make the next occurrence easier to diagnose?
4. Can the repair be made safe and repeatable?
5. Can a newer technician use the result without depending on tribal knowledge?
6. Can the issue be prevented instead of repeatedly serviced?

The best outcome is not becoming faster at fixing the same failure forever. It is making that failure less likely to reach another user.

## Repository map

```text
support-engineering-toolkit/
|-- README.md
|-- SECURITY.md
|-- LICENSE_REVIEW_REQUIRED.md
|-- CONTRIBUTING.md
|-- docs/
|   |-- repository-map.md
|   |-- design-principles.md
|   `-- script-catalog.md
|-- scripts/
|   |-- endpoint-management/
|   |-- identity-and-access/
|   |-- security-hardening/
|   |-- software-deployment/
|   |-- diagnostics-and-remediation/
|   |-- networking-and-voip/
|   |-- microsoft-365/
|   `-- utilities/
`-- tests/
```

Scripts are grouped by the operational problem they solve, not merely by programming language.

## Quality bar

Not every script will need the same level of engineering, but portfolio-ready tools should aim for the following:

* Detect current state before making changes
* Validate prerequisites and permissions
* Support safe re-runs whenever practical
* Fail clearly instead of producing mystery success
* Log meaningful decisions and outcomes
* Avoid embedding credentials or environment-specific secrets
* Separate configuration from executable logic
* Document expected inputs, outputs, and rollback
* Preserve attribution and licensing information
* Explain the user or support problem the tool was built to solve

## Public code and sanitization

Public versions are sanitized and may differ from the original internal implementation.

Customer names, employer identifiers, tenant IDs, internal domains, deployment keys, private addresses, credentials, proprietary runbooks, and production-specific paths do not belong in this repository.

Some tools may be rewritten from the ground up before publication when the original implementation contains environment-specific or third-party material that should not be redistributed.

## Provenance and licensing

No repository-wide software license is applied automatically.

Each published script must be reviewed for ownership, attribution, and redistribution rights. A file adapted from vendor documentation, an RMM library, Microsoft sample code, an employer repository, or another project must retain the required notices and may need to remain unpublished.

See [LICENSE_REVIEW_REQUIRED.md](LICENSE_REVIEW_REQUIRED.md).

## Using the scripts

Read the documentation beside a script before running it.

Operational automation can make broad system changes quickly. Test in a lab or limited scope first, confirm required permissions, and understand the rollback path. Unless a script explicitly says otherwise, assume it is provided as a technical portfolio artifact rather than a supported production product.

## What this repository demonstrates

Beyond the individual tools, this repository is meant to show how I approach technical work:

* User impact comes before tool worship
* Root cause matters more than closing the ticket quickly
* Automation should transfer knowledge, not hide it
* Clear output is part of the solution
* Junior technicians deserve usable tools and understandable documentation
* A durable fix is better than permanent heroics

## Related project

[Time Clock Manager](https://github.com/SamarieSystems/time-clock-manager) is maintained separately because it is a complete user-facing application rather than an operational script collection.

## Status

This repository is being rebuilt as a clean, sanitized portfolio from several years of support engineering and systems automation work. Scripts are being reviewed individually before publication.
