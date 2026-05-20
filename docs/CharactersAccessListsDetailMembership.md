# CharactersAccessListsDetailMembership


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**alliances** | [**Array&lt;CharactersAccessListsDetailAllianceentry&gt;**](CharactersAccessListsDetailAllianceentry.md) | Alliances in the Access List | [default to undefined]
**allow_everyone** | **boolean** | Whether everyone is allowed unless blocked | [default to undefined]
**characters** | [**Array&lt;CharactersAccessListsDetailCharacterentry&gt;**](CharactersAccessListsDetailCharacterentry.md) | Characters in the Access List | [default to undefined]
**corporations** | [**Array&lt;CharactersAccessListsDetailCorporationentry&gt;**](CharactersAccessListsDetailCorporationentry.md) | Corporations in the Access List | [default to undefined]

## Example

```typescript
import { CharactersAccessListsDetailMembership } from 'eve-esi-client-ts';

const instance: CharactersAccessListsDetailMembership = {
    alliances,
    allow_everyone,
    characters,
    corporations,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
