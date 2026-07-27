# Public repository publication policy

## Purpose

Nexarion Technologies publishes selected engineering demonstrations to provide inspectable proof of technical patterns without exposing private operations, client environments, or proprietary implementation details.

## Required publication conditions

Public content must:

- use synthetic, generated, or explicitly approved public data;
- remove credentials, secrets, private keys, tokens, cookies, and connection strings;
- remove private IP addresses, internal hostnames, tenant IDs, account IDs, and non-public URLs;
- remove client, employee, customer, vendor, and confidential project identifiers;
- avoid direct copies of production exports and private repository history;
- state the read/write/execution boundary clearly;
- include validation, tests, or reproducible evidence appropriate to the claim;
- include a README, license, security guidance, and `.env.example` where configuration is required;
- preserve source provenance without revealing confidential sources.

## Prohibited public content

The following remains private unless separately reviewed and approved:

- detailed Keystone specifications and internal project taxonomy;
- network diagrams, host inventories, firewall rules, and infrastructure topology;
- production workflow exports, service configurations, or database schemas containing sensitive implementation detail;
- client contracts, proposals, correspondence, financial records, or support evidence;
- model prompts, policies, or execution logic that expose proprietary operating controls;
- live integrations with consequential write, payment, identity, security, or trading authority.

## Sanitization review

Before publication or release:

1. scan for credentials and private identifiers;
2. inspect repository history, not only the current tree;
3. verify that examples and screenshots are synthetic;
4. run tests and static validation;
5. verify manifests and generated evidence;
6. review links, badges, package names, and metadata for old private namespaces;
7. record the approved public scope in the release notes.

## Intellectual-property boundary

An open-source license applies only to the files intentionally published under that license. It does not license private repositories, client materials, unpublished Keystone specifications, business methods, branding, trademarks, or non-public implementation work.
