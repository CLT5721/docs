---
slug: /react.usedelayedreveallazymint
title: useDelayedRevealLazyMint() function
hide_title: true
displayed_sidebar: react
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

## useDelayedRevealLazyMint() function

> This feature is currently in beta and may change based on feedback that we receive.

Use this to lazy mint a batch of delayed reveal NFTs on your [DropContract](./react.dropcontract.md)

**Signature:**

```typescript
export declare function useDelayedRevealLazyMint<TContract extends NFTContract>(
  contract: RequiredParam<TContract>,
  onProgress?: (progress: UploadProgressEvent) => void,
): import("@tanstack/react-query").UseMutationResult<
  import("@thirdweb-dev/sdk").TransactionResultWithId<never>[],
  unknown,
  DelayedRevealLazyMintInput,
  unknown
>;
```

## Parameters

| Parameter  | Type                                                       | Description                                                                                |
| ---------- | ---------------------------------------------------------- | ------------------------------------------------------------------------------------------ |
| contract   | [RequiredParam](./react.requiredparam.md)&lt;TContract&gt; | an instance of a [NFTContract](./react.nftcontract.md) with the drop extension             |
| onProgress | (progress: UploadProgressEvent) =&gt; void                 | <i>(Optional)</i> an optional callback that will be called with the progress of the upload |

**Returns:**

import("@tanstack/react-query").UseMutationResult&lt;import("@thirdweb-dev/sdk").TransactionResultWithId&lt;never&gt;\[\], unknown, [DelayedRevealLazyMintInput](./react.delayedreveallazymintinput.md), unknown&gt;

a mutation object that can be used to lazy mint a batch of NFTs