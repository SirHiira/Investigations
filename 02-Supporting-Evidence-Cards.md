# Supporting Evidence Cards

These cards reorganise facts in the source scenario. They are not raw logs.

## Card A — Authentication
- Multiple failed login attempts targeted several unused Service Desk accounts.
- A successful login occurred after the failures.
**Supports:** suspicious authentication activity followed by successful account access.

## Card B — Account condition
- The accounts were not actively used.
- Their passwords were weak and had remained unchanged since initial setup.
**Supports:** poor account hygiene increased the risk of credential compromise.

## Card C — MFA change
- After the successful login, an unauthorised person enrolled an MFA method.
**Supports:** the account's authentication setup was changed after access. The exact MFA method and technical mechanism are not specified.

## Card D — Cloud access
- The unauthorised person accessed the organisation's SharePoint tenant.
- The organisation subsequently blocked the access.
**Supports:** cloud access occurred and response action was taken. The narrative does not establish whether files were downloaded or changed.

## Card E — Network clue
- Residential proxy IP addresses were noted as network indicators.
**Supports:** proxy infrastructure may have been involved. No actual IPs or direct correlation to a specific login are supplied.

## Evidence discipline
Separate known facts, reasonable interpretations and unknowns.
