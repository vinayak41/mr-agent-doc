# Primary query

A contact can have more than one query. One of them is the primary query. A rule that follows a call uses that query only. The other queries for the same contact stay as they are.

## How it is chosen

A query is primary when both are true:

1. Its sales stage is not Lost, Booked, or Cancelled.
2. It has an assigned employee.

A query in Lost, Booked, or Cancelled is not primary. A query with no assigned employee is not primary.

If no query meets both, the contact has no primary query.

## Open question

- If more than one query meets both, which one is the primary query?
