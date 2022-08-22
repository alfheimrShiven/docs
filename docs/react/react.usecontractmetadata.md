---
slug: /react.usecontractmetadata
title: useContractMetadata() function
hide_title: true
displayed_sidebar: react
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

## useContractMetadata() function

> This feature is currently in beta and may change based on feedback that we receive.

Use this to get the contract metadata for a (built-in or custom) contract.

## Example

```javascript
const {
  data: contractMetadata,
  isLoading,
  error,
} = useContractMetadata("{{contract_address}}");
```

**Signature:**

```typescript
export declare function useContractMetadata(
  contractAddress: RequiredParam<ContractAddress>,
): import("@tanstack/react-query").UseQueryResult<
  {
    [x: string]: import("@thirdweb-dev/sdk/dist/browser").Json;
    description?: string | undefined;
    image?: any;
    external_link?: string | undefined;
    name: string;
  },
  unknown
>;
```

## Parameters

| Parameter       | Type                                                                                           | Description                          |
| --------------- | ---------------------------------------------------------------------------------------------- | ------------------------------------ |
| contractAddress | [RequiredParam](./react.requiredparam.md)&lt;[ContractAddress](./react.contractaddress.md)&gt; | the address of the deployed contract |

**Returns:**

import("@tanstack/react-query").UseQueryResult&lt;{ \[x: string\]: import("@thirdweb-dev/sdk/dist/browser").Json; description?: string \| undefined; image?: any; external_link?: string \| undefined; name: string; }, unknown&gt;

a response object that includes the contract metadata of the deployed contract