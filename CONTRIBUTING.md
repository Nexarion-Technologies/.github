# Contributing

Nexarion's public repositories are intentionally small, synthetic demonstrations of engineering patterns. Contributions that improve clarity, correctness, tests, portability, documentation, accessibility, or defensive behavior are welcome.

## Before opening a pull request

1. Open or reference an issue when the change affects behavior or public contracts.
2. Keep the change bounded to the repository's stated purpose.
3. Use synthetic data only.
4. Add or update tests and evidence when behavior changes.
5. Run the repository's documented validation commands.
6. Confirm that no secrets, private endpoints, tenant identifiers, client information, or internal topology are present.

## Do not submit

- credentials, tokens, certificates, connection strings, or `.env` files;
- real client, employee, customer, vendor, or financial records;
- screenshots or logs from private environments unless fully reconstructed with synthetic data;
- internal hostnames, private IP addresses, tenant IDs, account IDs, or production URLs;
- direct exports from private GitLab, n8n, SharePoint, QuickBooks, or other systems;
- code that adds unrestricted write, delete, execution, or approval authority without an explicit public design review.

## Pull-request expectations

A useful pull request explains:

- the problem being solved;
- the intended boundary and non-goals;
- validation performed;
- security and privacy considerations;
- evidence or tests demonstrating the result.

Repository-specific contribution instructions take precedence over this organization default.
