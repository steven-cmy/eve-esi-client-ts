# CorporationsCorporationIdWalletsDivisionTransactionsGetInner

wallet transaction

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**client_id** | **number** |  | [default to undefined]
**date** | **string** | Date and time of transaction | [default to undefined]
**is_buy** | **boolean** |  | [default to undefined]
**journal_ref_id** | **number** | -1 if there is no corresponding wallet journal entry | [default to undefined]
**location_id** | **number** |  | [default to undefined]
**quantity** | **number** |  | [default to undefined]
**transaction_id** | **number** | Unique transaction ID | [default to undefined]
**type_id** | **number** |  | [default to undefined]
**unit_price** | **number** | Amount paid per unit | [default to undefined]

## Example

```typescript
import { CorporationsCorporationIdWalletsDivisionTransactionsGetInner } from 'eve-esi-client-ts';

const instance: CorporationsCorporationIdWalletsDivisionTransactionsGetInner = {
    client_id,
    date,
    is_buy,
    journal_ref_id,
    location_id,
    quantity,
    transaction_id,
    type_id,
    unit_price,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
