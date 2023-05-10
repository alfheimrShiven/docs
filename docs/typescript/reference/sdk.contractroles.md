---
slug: /reference/sdk.contractroles
title: ContractRoles class
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

# ContractRoles class

Handle contract permissions

## Example

```javascript
const contract = await sdk.getContract("{{contract_address}}");
const rolesAndMembers = await contract.roles.getAll();
await contract.roles.grantRole("admin", "0x...");
```

## Constructors

| Constructor                                                                   | Modifiers | Description                                                       |
| ----------------------------------------------------------------------------- | --------- | ----------------------------------------------------------------- |
| [(constructor)(contractWrapper, roles)](./sdk.contractroles._constructor_.md) |           | Constructs a new instance of the <code>ContractRoles</code> class |

## Properties

| Property                                          | Modifiers | Type          | Description |
| ------------------------------------------------- | --------- | ------------- | ----------- |
| [featureName](./sdk.contractroles.featurename.md) |           | "Permissions" |             |

## Methods

| Method                                                      | Modifiers | Description                                                                                                                                                                                                                                                                                                                                                                                         |
| ----------------------------------------------------------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [get(role)](./sdk.contractroles.get.md)                     |           | Call this to get a list of addresses that are members of a specific role.                                                                                                                                                                                                                                                                                                                           |
| [getAll()](./sdk.contractroles.getall.md)                   |           | Call this to get get a list of addresses for all supported roles on the contract.                                                                                                                                                                                                                                                                                                                   |
| [grant(role, address)](./sdk.contractroles.grant.md)        |           | Call this to grant a role to a specific address.                                                                                                                                                                                                                                                                                                                                                    |
| [revoke(role, address)](./sdk.contractroles.revoke.md)      |           | Call this to revoke a role from a specific address.                                                                                                                                                                                                                                                                                                                                                 |
| [setAll(rolesWithAddresses)](./sdk.contractroles.setall.md) |           | <p>Call this to OVERWRITE the list of addresses that are members of specific roles.</p><p>Every role in the list will be overwritten with the new list of addresses provided with them. If you want to add or remove addresses for a single address use [ContractRoles.grant()](./sdk.contractroles.grant.md) and [ContractRoles.revoke()](./sdk.contractroles.revoke.md) respectively instead.</p> |

**Signature:**

```typescript
export declare class ContractRoles<TContract extends IPermissions, TRole extends Role> implements DetectableFeature
```

**Implements:** DetectableFeature

## Remarks

Configure roles and permissions for a contract, to restrict certain actions.