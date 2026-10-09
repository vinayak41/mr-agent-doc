# Call log sets sales stage

## Summary

A newly logged call can move the primary query's sales stage. The stage follows the length of that call.

CONTACTING sits between NEW and CONNECTED.

## When it applies

The call updates only the [primary query](primary-query.md) for that contact. Other queries for the same contact stay as they are. If the contact has no primary query, the call does not change any stage.

A call longer than 10 seconds counts as a conversation. A call of 10 seconds or less counts as a short attempt. That includes a call with no recorded length.

## Rule

| Current stage | Call | New stage |
| --- | --- | --- |
| NEW | Longer than 10 seconds | CONNECTED |
| NEW | 10 seconds or less | CONTACTING |
| CONTACTING | Longer than 10 seconds | CONNECTED |
| CONTACTING | 10 seconds or less | Unchanged |
| Any later stage | Any length | Unchanged |

Examples:

1. The query is NEW and the call lasts 11 seconds. The stage becomes CONNECTED.
2. The query is NEW and the call lasts 10 seconds. The stage becomes CONTACTING.
3. The query is CONTACTING and the call lasts 11 seconds. The stage becomes CONNECTED.
4. The query is CONTACTING and the call lasts 4 seconds. The stage stays CONTACTING.
5. The query is PROPOSAL and the call lasts 30 seconds. The stage stays PROPOSAL.
