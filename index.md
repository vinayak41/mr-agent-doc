# Index

Business rules for how a query moves through the sales process. Each page states the rule, when it applies, and what stays unchanged.

| Topic | Rule |
| --- | --- |
| [Closed stage](topics/closed-stage.md) | BOOKED, LOST, and CANCELLED are closed stages. A query in a closed stage has left the active sales process. |
| [Primary query](topics/primary-query.md) | Among a contact's queries, the primary one is not in a closed stage, and it has an assigned employee. |
| [Resubmission query](topics/resubmission-query.md) | When a contact has more than one query and at least one has an assigned employee, each other query with no assigned employee is a resubmission query. |
| [Unallocated query](topics/unallocated-query.md) | A query with no assigned team, no assigned employee, an open sales stage, and `is_resubmitted` false. |
| [Team's unallocated queries](topics/teams-unallocated-queries.md) | Queries assigned to a team, with no assigned employee, an open sales stage, and `is_resubmitted` false. |
| [Call log sets sales stage](topics/call-log-sale-stage.md) | A new call can move the primary query from NEW to CONTACTING or CONNECTED, based on call length. A short call leaves CONTACTING as it is. Any later stage is left unchanged. |
| [Query history](topics/query-history.md) | A history entry whose changed_by id matches the logged-in user aligns to the right. Any other user's entry aligns to the left. |
