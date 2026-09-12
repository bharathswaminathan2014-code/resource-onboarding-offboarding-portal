# Portal v4 implementation notes

This version includes the requested User Management completion and the equivalent of the planned Dashboard Prompt 3 work directly in the source code.

## User Management
- Add and edit portal users with name, email, role, account, program, project and status.
- Seven roles retained: Executive, Senior Leader, Senior Manager, Manager, PMO, Operational User, Admin.
- Account → Program → Project cascading scope selection.
- Activate/deactivate users.
- Safe delete for custom users; seeded demo users and users referenced by lifecycle records cannot be destructively deleted.
- Existing seeded demo personas are preserved.

## Dashboard enhancement
- Existing Dashboard retained; no separate Executive Dashboard.
- Focused on onboarding/offboarding status and PMO visibility.
- Added date-range filtering.
- Requires Attention is derived from scoped pending/delayed/blocker records rather than hard-coded governance items.
- Account/program/project/location/manager/status filters remain.
- Upcoming onboarding/offboarding remains visible.
- Removed SLA/governance wording from the Dashboard presentation.
- Existing RBAC/scope model is respected.
- No AI, backend, database, SSO or new governance module added.
