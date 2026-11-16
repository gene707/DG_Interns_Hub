# SIEM Lab Triage Notes

> Complete all bracketed fields from the actual SIEM events. These are templates, not confirmed incident records.

## Finding 1: SSH Authentication Failures

- **Who:** `[Kali source IP]`, account `labuser`
- **What:** Repeated failed SSH password attempts
- **When:** `[first/last timestamps]`
- **Where:** Ubuntu `[host/IP]`, TCP/22
- **Why:** Authorized Hydra test if it matches the test window; otherwise, possible password guessing.
- **Verdict:** True positive for brute-force activity only if events confirm it; maliciousness is not implied.
- **Next step:** Verify authorization, check for successful login, preserve authentication logs, and reset/remove the temporary account.

## Finding 2: TCP SYN Scan

- **Who:** `[source IP/owner]`
- **What:** SYN probes to `[ports]` recorded by `[UFW/network sensor]`
- **When:** `[timestamps]`
- **Where:** Ubuntu `[host/IP]`
- **Why:** Expected Nmap lab scan if source and time match; otherwise, possible reconnaissance.
- **Verdict:** True positive for scan behavior if validated; otherwise, undetermined.
- **Next step:** Verify the source and change window, inspect adjacent hosts/ports, and retain logs.

## Finding 3: FIM Modification

- **Who:** `[user/process]`
- **What:** `/opt/fim-lab/monitored.txt` modified
- **When:** `[FIM timestamp]`
- **Where:** Ubuntu agent `[hostname]`
- **Why:** Expected test change if authorized; otherwise, possible tampering.
- **Verdict:** True positive for file change; benign if it matches the test.
- **Next step:** Verify the operator/change, compare hashes, and restore the baseline if required.

## Evidence to Attach

For each finding, attach:

- Raw event
- Parsed fields
- Alert ID
- Screenshot filename
