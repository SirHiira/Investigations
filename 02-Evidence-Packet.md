# Evidence Packet — Northbridge University


## Exhibit A — Account inventory

| Account | Department label | Status at start of case | Last known purpose |
|---|---|---|---|
| `ukservicedesk` | UK Service Desk | Dormant | Legacy support mailbox |
| `deservicedesk` | DE Service Desk | Dormant | Legacy support mailbox |
| `ieservicedesk` | IE Service Desk | Dormant | Legacy support mailbox |
| `j.mwangi` | IT Support | Active | Staff support account |

The three Service Desk accounts were not expected to be used interactively during the period under review.

## Exhibit B — Identity sign-in event extract

Times are UTC. 

| Time (UTC) | Account | Result | Source IP | Client / application | Notes |
|---|---|---|---|---|---|
| 08:41 | ukservicedesk | Failure | 198.51.100.24 | Browser / Cloud portal | Invalid password |
| 08:42 | deservicedesk | Failure | 198.51.100.24 | Browser / Cloud portal | Invalid password |
| 08:43 | ieservicedesk | Failure | 198.51.100.24 | Browser / Cloud portal | Invalid password |
| 08:47 | ukservicedesk | Failure | 198.51.100.24 | Browser / Cloud portal | Invalid password |
| 08:48 | deservicedesk | Failure | 198.51.100.24 | Browser / Cloud portal | Invalid password |
| 08:49 | ieservicedesk | Failure | 198.51.100.24 | Browser / Cloud portal | Invalid password |
| 09:03 | ukservicedesk | Success | 198.51.100.24 | Browser / Cloud portal | MFA challenge satisfied |
| 09:17 | j.mwangi | Failure | 203.0.113.77 | Browser / Cloud portal | User reported password typo; successful login from usual office network at 09:21 (not shown) |

## Exhibit C — MFA audit extract

| Time (UTC) | Account | Event | Result | Details |
|---|---|---|---|---|
| 09:06 | ukservicedesk | Authentication method added | Success | New mobile authenticator registered |
| 09:08 | ukservicedesk | MFA method tested | Success | Registration completed |
| 09:10 | deservicedesk | Authentication method added | Denied | Policy blocked registration |

## Exhibit D — SharePoint audit extract

| Time (UTC) | Account | Activity | Result | Details |
|---|---|---|---|---|
| 09:12 | ukservicedesk | Sign in to SharePoint | Success | New browser session |
| 09:14 | ukservicedesk | Site viewed | Success | `Finance-Operations` |
| 09:16 | ukservicedesk | File viewed | Success | `Supplier-Payments-Q3.xlsx` |
| 09:19 | ukservicedesk | File downloaded | Success | `Supplier-Payments-Q3.xlsx` |
| 09:24 | ukservicedesk | Sharing link created | Success | Link scope recorded as “Anyone” |
| 09:31 | ukservicedesk | Session revoked by IT | Success | Containment action |


## Exhibit E — Analyst note

The SOC has not yet established:
- whether the downloaded spreadsheet was opened or copied elsewhere;
- whether the public sharing link was accessed by another person;
- whether the same source infrastructure was used for other university accounts;
- how the password was obtained;
- whether any other account or cloud application was accessed.

## Questions to keep in mind
- Do the events form a coherent sequence?
- Which account is most clearly compromised?
- Which event is a possible false lead?
- What is known about data access versus data exfiltration?
- What would you ask the identity and SharePoint administrators to preserve?
