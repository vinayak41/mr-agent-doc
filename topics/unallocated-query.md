# Unallocated query

An unallocated query has no team and no employee. It is still in the active sales process, and it is not a resubmission.

## How it is recognized

A query is an unallocated query when all four are true:

1. It has no assigned team.
2. It has no assigned employee.
3. Its sales stage is not a [closed stage](closed-stage.md).
4. `is_resubmitted` is false.

A query with an assigned team is not an unallocated query. A query with an assigned employee is not an unallocated query. A query in a closed stage is not an unallocated query. A query with `is_resubmitted` true is not an unallocated query.
