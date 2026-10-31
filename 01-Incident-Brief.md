# Incident Brief: Password Spraying and Account Takeover

## Your role
You are a junior CTI/SOC analyst supporting the security team at Northbridge University. The SOC has received a report that several dormant Service Desk accounts may have been accessed by an unauthorised person.

## Initial report
The university observed multiple failed sign-in attempts against several unused Service Desk accounts. One sign-in later succeeded. The accounts had weak passwords that had not been changed since initial setup. After the successful sign-in, an unfamiliar MFA method was enrolled and the account was used to access the university SharePoint environment. The university's IT team has blocked the suspected unauthorised access.

The initial report also mentions residential proxy infrastructure. A separate staff member reported a sign-in problem during the same period.

## Your mission
Investigate the supplied evidence and prepare a short team assessment for the SOC lead. Your job is not to identify a real-world threat actor. Your job is to explain what the evidence supports, what remains uncertain, and what the university should do next.

## Scope
- Three Service Desk accounts are in scope.
- Identity-provider sign-in records, MFA audit records and SharePoint audit records are supplied.
- A small IOC/context sheet is supplied.
- Some data is deliberately incomplete. One event is included as a potential benign lead; do not assume every unusual event is malicious.

## Evidence discipline
For each conclusion, ask:
1. What exactly does the evidence show?
2. Which source supports it?
3. Is this a fact, an interpretation or an unknown?
4. What further evidence would confirm it?
