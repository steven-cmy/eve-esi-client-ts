# CharactersCharacterIdWalletTransactionsGetInner

wallet transaction

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**client_id** | **number** |  | [default to undefined]
**date** | **string** | Date and time of transaction | [default to undefined]
**is_buy** | **boolean** |  | [default to undefined]
**is_personal** | **boolean** |  | [default to undefined]
**journal_ref_id** | **number** |  | [default to undefined]
**location_id** | **number** |  | [default to undefined]
**quantity** | **number** |  | [default to undefined]
**transaction_id** | **number** | Unique transaction ID | [default to undefined]
**type_id** | **number** |  | [default to undefined]
**unit_price** | **number** | Amount paid per unit | [default to undefined]

## Example

```typescript
import { CharactersCharacterIdWalletTransactionsGetInner } from 'eve-esi-client-ts';

const instance: CharactersCharacterIdWalletTransactionsGetInner = {
    client_id,
    date,
    is_buy,
    is_personal,
    journal_ref_id,
    location_id,
    quantity,
    transaction_id,
    type_id,
    unit_price,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
