# Team lead access to unallocated queries

A user with the role `TEAM LEAD` can access an [unallocated query](../topics/unallocated-query.md) when its source is allowed to that user's team, or when its source is allowed to that team's allowed teams. The same user can access a [team's unallocated query](../topics/teams-unallocated-queries.md) when that query is assigned to the team lead's team, or when it is assigned to one of the team lead's allowed teams.

## Unallocated query

A `TEAM LEAD` can access an unallocated query when either is true:

1. The query's source is allowed to the team lead's team.
2. The query's source is allowed to that team's allowed teams.

A `TEAM LEAD` cannot access an unallocated query when the source is allowed to neither the team lead's team nor that team's allowed teams.

## Team's unallocated queries

A `TEAM LEAD` can access a team's unallocated query when either is true:

1. The query is assigned to the team lead's team.
2. The query is assigned to one of the team lead's allowed teams.

A `TEAM LEAD` cannot access a team's unallocated query when it is assigned to neither the team lead's team nor the team lead's allowed teams.
