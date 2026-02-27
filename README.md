# Security Automation – Authorized Access List Management (Python)

## Scenario
In an environment handling sensitive data, systems relied on an allow-list of IP addresses to control access to a restricted network. Over time, users changed roles or left the organization, but their IP addresses remained authorized. This created a security risk because outdated access permissions could allow unauthorized connections.

## Objective
Automate the removal of unauthorized IP addresses from the allow-list to maintain accurate access control and reduce the risk of stale permissions.

## Tools Used
- Python
- File handling
- List filtering logic

## Investigation / Process
1. Imported the file containing authorized IP addresses
2. Loaded a separate list containing IPs that should no longer have access
3. Converted file data into a workable list structure
4. Compared each allowed IP against the removal list
5. Removed any IP that should no longer be authorized
6. Rewrote the updated allow-list back to the system file

## Findings
Manual access management can easily leave outdated permissions in place.  
Automating verification ensures access lists stay accurate and reduces the chance of unauthorized access due to human error.

## Security Impact
This automation supports the principle of **least privilege** by ensuring only currently authorized users maintain access to sensitive systems. It also improves audit reliability by keeping access records consistent.

## Mitigation / Recommendation
Organizations should automate periodic validation of access control lists instead of relying on manual updates. Scheduled scripts or centralized identity management systems should enforce removal of outdated permissions.

---

Full detailed workflow available in attached project documentation.
