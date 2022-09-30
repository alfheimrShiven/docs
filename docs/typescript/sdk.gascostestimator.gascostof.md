---
slug: /sdk.gascostestimator.gascostof
title: GasCostEstimator.gasCostOf() method
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

## GasCostEstimator.gasCostOf() method

Estimates the cost of gas in native token of the current chain Pass in the same parameters as the contract's function.

## Example

```javascript
const costOfClaim = await nftDrop?.estimator.gasCostOf("claim", [
  "0x...", // receiver
  1, // quantity
  "0x...", // currency
  1, // price per token
  [], // proofs
  1, // proof max quantity per transaction
]);
```

**Signature:**

```typescript
gasCostOf(fn: keyof TContract["functions"] | (string & {}), args: Parameters<TContract["functions"][typeof fn]> | any[]): Promise<string>;
```

## Parameters

| Parameter | Type                                                                   | Description |
| --------- | ---------------------------------------------------------------------- | ----------- |
| fn        | keyof TContract\["functions"\] &#124; (string &amp; {})                |             |
| args      | Parameters&lt;TContract\["functions"\]\[typeof fn\]&gt; &#124; any\[\] |             |

**Returns:**

Promise&lt;string&gt;

the estimated price in native currency (ETH, MATIC, etc) of calling this function

## Remarks

Estimate the cost of gas in native token of the current chain