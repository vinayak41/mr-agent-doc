# Team's unallocated queries

A team's unallocated queries belong to that team and to no employee. Each one is still in the active sales process, and it is not a resubmission.

## How it is recognized

A query is one of a team's unallocated queries when all four are true:

1. It has an assigned team.
2. It has no assigned employee.
3. Its sales stage is not a [closed stage](closed-stage.md).
4. `is_resubmitted` is false.

A query with no assigned team is not one of a team's unallocated queries. A query with an assigned employee is not one of them. A query in a closed stage is not one of them. A query with `is_resubmitted` true is not one of them.
