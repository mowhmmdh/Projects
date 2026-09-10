# Enterprise Network Infrastructure & IT Operations — Case Study

**Author:** Mohammad Hossein Asgari Somarin  
**Focus:** Network infrastructure, IT operations, Windows/Linux administration, security hardening  
**Publication type:** Technical portfolio case study

> This case study describes technical responsibilities and problem-solving approaches in generalized form. Internal addresses, credentials, proprietary configurations, security-sensitive details, and confidential operational data are intentionally omitted.

## Context

Enterprise IT environments require more than basic connectivity. Day-to-day reliability depends on coordinated work across endpoint support, network infrastructure, identity services, servers, web services, monitoring, and security controls.

This case study documents a practical approach to supporting and improving an enterprise environment while keeping changes controlled, reversible, and documented.

## Scope of work

- IT help-desk and end-user technical support
- Network troubleshooting and infrastructure maintenance
- Passive network infrastructure: structured cabling, patch panels and rack organization
- Active network equipment administration and troubleshooting
- Windows Server and Active Directory operational support
- Linux server administration and service maintenance
- Firewall and network-security operations
- CCTV infrastructure troubleshooting and maintenance
- Internal web-service and reverse-proxy administration
- Technical documentation and change verification

## Methodology

### 1. Establish a baseline

Before changing production systems, identify the current topology, service dependencies, ownership, access paths, and failure domains. Record the current state so that a change can be verified and, when necessary, rolled back.

### 2. Separate symptoms from root causes

A user-facing incident is not treated as proof of a specific technical cause. Troubleshooting starts with a minimal hypothesis set and validates each layer independently: endpoint, DNS, network path, authentication, application, and service availability.

### 3. Prefer low-risk, reversible changes

Production changes are introduced in small steps. Configuration backups, before/after checks, explicit validation criteria, and rollback paths reduce the chance that troubleshooting itself becomes an outage.

### 4. Harden the environment in layers

Security is treated as a stack rather than a single firewall rule. Relevant controls include least privilege, secure administration, service exposure minimization, network segmentation, logging, update discipline, identity protection, and verification of externally reachable services.

### 5. Document what changed

Operational knowledge should not remain inside an individual administrator's memory. Significant changes are recorded with purpose, affected services, validation steps, and recovery notes.

## Example troubleshooting flow

When an internal service is reported as unavailable:

1. Confirm whether the issue affects one endpoint or multiple users.
2. Check name resolution and the expected destination.
3. Verify network reachability without changing production configuration.
4. Confirm that the destination service is listening and healthy.
5. Inspect reverse-proxy, firewall, or access-control behavior where applicable.
6. Review recent changes and logs.
7. Apply the smallest viable corrective change.
8. Validate from both the affected client and an independent test point.
9. Record the final state and rollback information.

## Security principles applied

- Minimize externally exposed services.
- Use HTTPS for public-facing web services where supported.
- Restrict management interfaces to trusted paths.
- Separate network roles where practical.
- Protect administrative credentials and avoid embedding secrets in documentation.
- Keep operating systems and server applications maintained.
- Treat DNS, identity, firewall, and reverse-proxy configuration as security-sensitive components.
- Validate changes after deployment instead of relying only on configuration syntax.

## What this case study demonstrates

The main engineering lesson is that reliable IT operations are a combination of troubleshooting discipline, infrastructure fundamentals, controlled change management, and security awareness. The same methodology can be reused across different vendors and enterprise environments.

## Evidence and reproducibility

Where possible, portfolio work should be supported by public technical documentation, sanitized configuration examples, diagrams, scripts, and version-controlled change history. Sensitive enterprise information is excluded from public materials.

## Author

**Mohammad Hossein Asgari Somarin** is an IT / Network & Infrastructure practitioner focused on practical networking, systems administration, infrastructure security, and IT operations.

Professional portfolio: https://mowhmmdh.github.io/  
GitHub: https://github.com/mowhmmdh  
LinkedIn: https://www.linkedin.com/in/mohammadhosseinasgari/
