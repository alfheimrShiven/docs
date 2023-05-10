---
slug: /reference/sdk.erc1155.get
title: Erc1155.get() method
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

# Erc1155.get() method

Get a single NFT Metadata

## Example

```javascript
const nft = await contract.erc1155.get(0);
```

**Signature:**

```typescript
get(tokenId: BigNumberish): Promise<NFT>;
```

## Parameters

| Parameter | Type         | Description                        |
| --------- | ------------ | ---------------------------------- |
| tokenId   | BigNumberish | the tokenId of the NFT to retrieve |

**Returns:**

Promise&lt;[NFT](./sdk.nft.md)&gt;

The NFT metadata