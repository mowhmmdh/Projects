# Enterprise Network Infrastructure & IT Operations — Case Study

**Author:** Mohammad Hossein Asgari Somarin  
**Focus:** Network infrastructure, IT operations, Windows/Linux administration, security hardening

> This public case study intentionally excludes internal IP addresses, credentials, proprietary configurations, security-sensitive details, and confidential operational data.

## Context

Reliable enterprise IT operations depend on coordinated work across endpoint support, networking, identity, servers, web services, monitoring, and security controls.

This case study presents a generalized operational methodology used in practical enterprise IT work: establish a baseline, isolate the fault domain, make controlled changes, verify outcomes, and document the final state.

## Technical scope

- Enterprise help desk and end-user support
- Network troubleshooting and infrastructure maintenance
- Structured cabling, patch panels and rack organization
- Active network equipment administration
- Windows Server and Active Directory operations
- Linux server administration
- Firewall and network-security operations
- CCTV infrastructure maintenance
- Web service and reverse-proxy administration
- Technical documentation and change verification

## Operational methodology

### Baseline first

Map dependencies and record the current state before production changes. A baseline makes validation and rollback possible.

### Diagnose by layer

Separate endpoint, DNS, routing, authentication, application, and service-level symptoms instead of assuming a single root cause from the first user report.

### Change conservatively

Use small, reversible changes with explicit before/after checks. Production troubleshooting should not create a larger outage than the original incident.

### Harden in layers

Security is treated as a combination of least privilege, service exposure reduction, segmentation, secure administration, logging, patching, identity controls, and verification of public attack surfaces.

### Document the result

Record the purpose, affected service, validation steps, and recovery information for significant changes so operational knowledge is reproducible.

## Example incident workflow

1. Determine whether the failure is isolated or widespread.
2. Verify DNS resolution and the expected destination.
3. Test network reachability without modifying production settings.
4. Confirm the destination service and its dependencies are healthy.
5. Inspect firewall, reverse-proxy, and access-control behavior when relevant.
6. Review recent changes and service logs.
7. Apply the smallest corrective change.
8. Validate from the affected client and an independent test point.
9. Record the resulting configuration and rollback notes.

## Security principles

- Minimize exposed services.
- Prefer HTTPS for public-facing services.
- Restrict administrative access to trusted paths.
- Segment network roles where practical.
- Never publish secrets or sensitive infrastructure details.
- Keep operating systems and server software maintained.
- Treat DNS, identity, firewall, and reverse-proxy settings as security-sensitive.
- Validate deployed changes rather than relying only on configuration syntax.

## Evidence strategy

Public technical work is strongest when supported by reproducible documentation, sanitized configuration examples, architecture diagrams, scripts, and version-controlled history. Confidential enterprise information should remain private.

## Author

**Mohammad Hossein Asgari Somarin** — IT / Network & Infrastructure practitioner focused on networking, systems administration, infrastructure security, and IT operations.

Portfolio: https://mowhmmdh.github.io/  
GitHub: https://github.com/mowhmmdh  
LinkedIn: https://www.linkedin.com/in/mohammadhosseinasgari/
