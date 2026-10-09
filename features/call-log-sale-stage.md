# Call log sets sales stage

## Summary

A newly logged call can move the primary query's sales stage. The stage follows the length of that call.

Contacting sits between New and Connected.

## When it applies

The call updates only the [primary query](primary-query.md) for that contact. Other queries for the same contact stay as they are. If the contact has no primary query, the call does not change any stage.

A call longer than 10 seconds counts as a conversation. A call of 10 seconds or less counts as a short attempt. That includes a call with no recorded length.

## Rule

| Current stage | Call | New stage |
| --- | --- | --- |
| New | Longer than 10 seconds | Connected |
| New | 10 seconds or less | Contacting |
| Contacting | Longer than 10 seconds | Connected |
| Contacting | 10 seconds or less | Unchanged |
| Any later stage | Any length | Unchanged |

Examples:

1. The query is New and the call lasts 11 seconds. The stage becomes Connected.
2. The query is New and the call lasts 10 seconds. The stage becomes Contacting.
3. The query is Contacting and the call lasts 11 seconds. The stage becomes Connected.
4. The query is Contacting and the call lasts 4 seconds. The stage stays Contacting.
5. The query is Proposal and the call lasts 30 seconds. The stage stays Proposal.
