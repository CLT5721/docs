---
slug: /sdk.vote.vote
title: Vote.vote() method
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

## Vote.vote() method

Vote

## Example

```javascript
// The proposal ID of the proposal you want to vote on
const proposalId = "0";
// The vote type you want to cast, can be VoteType.Against, VoteType.For, or VoteType.Abstain
const voteType = VoteType.For;
// The (optional) reason for the vote
const reason = "I like this proposal!";

await contract.vote(proposalId, voteType, reason);
```

**Signature:**

```typescript
vote(proposalId: string, voteType: VoteType, reason?: string): Promise<TransactionResult>;
```

## Parameters

| Parameter  | Type                          | Description                                           |
| ---------- | ----------------------------- | ----------------------------------------------------- |
| proposalId | string                        | The proposal to cast a vote on.                       |
| voteType   | [VoteType](./sdk.votetype.md) | The position the voter is taking on their vote.       |
| reason     | string                        | <i>(Optional)</i> (optional) The reason for the vote. |

**Returns:**

Promise&lt;[TransactionResult](./sdk.transactionresult.md)&gt;

## Remarks

Vote on an active proposal