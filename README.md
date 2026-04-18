## eve-esi-client-ts@1.1.1

This generator creates TypeScript/JavaScript client that utilizes [axios](https://github.com/axios/axios). The generated Node module can be used in the following environments:

Environment
* Node.js
* Webpack
* Browserify

Language level
* ES5 - you must have a Promises/A+ library installed
* ES6

Module system
* CommonJS
* ES6 module system

It can be used in both TypeScript and JavaScript. In TypeScript, the definition will be automatically resolved via `package.json`. ([Reference](https://www.typescriptlang.org/docs/handbook/declaration-files/consumption.html))

### Building

To build and compile the typescript sources to javascript use:
```
npm install
npm run build
```

### Publishing

First build the package then run `npm publish`

### Consuming

navigate to the folder of your consuming project and run one of the following commands.

_published:_

```
npm install eve-esi-client-ts@1.1.1 --save
```

_unPublished (not recommended):_

```
npm install PATH_TO_GENERATED_PACKAGE --save
```

### Documentation for API Endpoints

All URIs are relative to *https://esi.evetech.net*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*AllianceApi* | [**getAlliances**](docs/AllianceApi.md#getalliances) | **GET** /alliances | List all alliances
*AllianceApi* | [**getAlliancesAllianceId**](docs/AllianceApi.md#getalliancesallianceid) | **GET** /alliances/{alliance_id} | Get alliance\&#39;s public information
*AllianceApi* | [**getAlliancesAllianceIdCorporations**](docs/AllianceApi.md#getalliancesallianceidcorporations) | **GET** /alliances/{alliance_id}/corporations | List alliance\&#39;s corporations
*AllianceApi* | [**getAlliancesAllianceIdIcons**](docs/AllianceApi.md#getalliancesallianceidicons) | **GET** /alliances/{alliance_id}/icons | Get alliance icon
*AssetsApi* | [**getCharactersCharacterIdAssets**](docs/AssetsApi.md#getcharacterscharacteridassets) | **GET** /characters/{character_id}/assets | Get character assets
*AssetsApi* | [**getCorporationsCorporationIdAssets**](docs/AssetsApi.md#getcorporationscorporationidassets) | **GET** /corporations/{corporation_id}/assets | Get corporation assets
*AssetsApi* | [**postCharactersCharacterIdAssetsLocations**](docs/AssetsApi.md#postcharacterscharacteridassetslocations) | **POST** /characters/{character_id}/assets/locations | Get character asset locations
*AssetsApi* | [**postCharactersCharacterIdAssetsNames**](docs/AssetsApi.md#postcharacterscharacteridassetsnames) | **POST** /characters/{character_id}/assets/names | Get character asset names
*AssetsApi* | [**postCorporationsCorporationIdAssetsLocations**](docs/AssetsApi.md#postcorporationscorporationidassetslocations) | **POST** /corporations/{corporation_id}/assets/locations | Get corporation asset locations
*AssetsApi* | [**postCorporationsCorporationIdAssetsNames**](docs/AssetsApi.md#postcorporationscorporationidassetsnames) | **POST** /corporations/{corporation_id}/assets/names | Get corporation asset names
*CalendarApi* | [**getCharactersCharacterIdCalendar**](docs/CalendarApi.md#getcharacterscharacteridcalendar) | **GET** /characters/{character_id}/calendar | List calendar event summaries
*CalendarApi* | [**getCharactersCharacterIdCalendarEventId**](docs/CalendarApi.md#getcharacterscharacteridcalendareventid) | **GET** /characters/{character_id}/calendar/{event_id} | Get an event
*CalendarApi* | [**getCharactersCharacterIdCalendarEventIdAttendees**](docs/CalendarApi.md#getcharacterscharacteridcalendareventidattendees) | **GET** /characters/{character_id}/calendar/{event_id}/attendees | Get attendees
*CalendarApi* | [**putCharactersCharacterIdCalendarEventId**](docs/CalendarApi.md#putcharacterscharacteridcalendareventid) | **PUT** /characters/{character_id}/calendar/{event_id} | Respond to an event
*CharacterApi* | [**getCharactersCharacterId**](docs/CharacterApi.md#getcharacterscharacterid) | **GET** /characters/{character_id} | Get character\&#39;s public information
*CharacterApi* | [**getCharactersCharacterIdAgentsResearch**](docs/CharacterApi.md#getcharacterscharacteridagentsresearch) | **GET** /characters/{character_id}/agents_research | Get agents research
*CharacterApi* | [**getCharactersCharacterIdBlueprints**](docs/CharacterApi.md#getcharacterscharacteridblueprints) | **GET** /characters/{character_id}/blueprints | Get blueprints
*CharacterApi* | [**getCharactersCharacterIdCorporationhistory**](docs/CharacterApi.md#getcharacterscharacteridcorporationhistory) | **GET** /characters/{character_id}/corporationhistory | Get corporation history
*CharacterApi* | [**getCharactersCharacterIdFatigue**](docs/CharacterApi.md#getcharacterscharacteridfatigue) | **GET** /characters/{character_id}/fatigue | Get jump fatigue
*CharacterApi* | [**getCharactersCharacterIdMedals**](docs/CharacterApi.md#getcharacterscharacteridmedals) | **GET** /characters/{character_id}/medals | Get medals
*CharacterApi* | [**getCharactersCharacterIdNotifications**](docs/CharacterApi.md#getcharacterscharacteridnotifications) | **GET** /characters/{character_id}/notifications | Get character notifications
*CharacterApi* | [**getCharactersCharacterIdNotificationsContacts**](docs/CharacterApi.md#getcharacterscharacteridnotificationscontacts) | **GET** /characters/{character_id}/notifications/contacts | Get new contact notifications
*CharacterApi* | [**getCharactersCharacterIdPortrait**](docs/CharacterApi.md#getcharacterscharacteridportrait) | **GET** /characters/{character_id}/portrait | Get character portraits
*CharacterApi* | [**getCharactersCharacterIdRoles**](docs/CharacterApi.md#getcharacterscharacteridroles) | **GET** /characters/{character_id}/roles | Get character corporation roles
*CharacterApi* | [**getCharactersCharacterIdStandings**](docs/CharacterApi.md#getcharacterscharacteridstandings) | **GET** /characters/{character_id}/standings | Get standings
*CharacterApi* | [**getCharactersCharacterIdTitles**](docs/CharacterApi.md#getcharacterscharacteridtitles) | **GET** /characters/{character_id}/titles | Get character corporation titles
*CharacterApi* | [**postCharactersAffiliation**](docs/CharacterApi.md#postcharactersaffiliation) | **POST** /characters/affiliation | Character affiliation
*CharacterApi* | [**postCharactersCharacterIdCspa**](docs/CharacterApi.md#postcharacterscharacteridcspa) | **POST** /characters/{character_id}/cspa | Calculate a CSPA charge cost
*ClonesApi* | [**getCharactersCharacterIdClones**](docs/ClonesApi.md#getcharacterscharacteridclones) | **GET** /characters/{character_id}/clones | Get clones
*ClonesApi* | [**getCharactersCharacterIdImplants**](docs/ClonesApi.md#getcharacterscharacteridimplants) | **GET** /characters/{character_id}/implants | Get active implants
*ContactsApi* | [**deleteCharactersCharacterIdContacts**](docs/ContactsApi.md#deletecharacterscharacteridcontacts) | **DELETE** /characters/{character_id}/contacts | Delete contacts
*ContactsApi* | [**getAlliancesAllianceIdContacts**](docs/ContactsApi.md#getalliancesallianceidcontacts) | **GET** /alliances/{alliance_id}/contacts | Get alliance contacts
*ContactsApi* | [**getAlliancesAllianceIdContactsLabels**](docs/ContactsApi.md#getalliancesallianceidcontactslabels) | **GET** /alliances/{alliance_id}/contacts/labels | Get alliance contact labels
*ContactsApi* | [**getCharactersCharacterIdContacts**](docs/ContactsApi.md#getcharacterscharacteridcontacts) | **GET** /characters/{character_id}/contacts | Get contacts
*ContactsApi* | [**getCharactersCharacterIdContactsLabels**](docs/ContactsApi.md#getcharacterscharacteridcontactslabels) | **GET** /characters/{character_id}/contacts/labels | Get contact labels
*ContactsApi* | [**getCorporationsCorporationIdContacts**](docs/ContactsApi.md#getcorporationscorporationidcontacts) | **GET** /corporations/{corporation_id}/contacts | Get corporation contacts
*ContactsApi* | [**getCorporationsCorporationIdContactsLabels**](docs/ContactsApi.md#getcorporationscorporationidcontactslabels) | **GET** /corporations/{corporation_id}/contacts/labels | Get corporation contact labels
*ContactsApi* | [**postCharactersCharacterIdContacts**](docs/ContactsApi.md#postcharacterscharacteridcontacts) | **POST** /characters/{character_id}/contacts | Add contacts
*ContactsApi* | [**putCharactersCharacterIdContacts**](docs/ContactsApi.md#putcharacterscharacteridcontacts) | **PUT** /characters/{character_id}/contacts | Edit contacts
*ContractsApi* | [**getCharactersCharacterIdContracts**](docs/ContractsApi.md#getcharacterscharacteridcontracts) | **GET** /characters/{character_id}/contracts | Get contracts
*ContractsApi* | [**getCharactersCharacterIdContractsContractIdBids**](docs/ContractsApi.md#getcharacterscharacteridcontractscontractidbids) | **GET** /characters/{character_id}/contracts/{contract_id}/bids | Get contract bids
*ContractsApi* | [**getCharactersCharacterIdContractsContractIdItems**](docs/ContractsApi.md#getcharacterscharacteridcontractscontractiditems) | **GET** /characters/{character_id}/contracts/{contract_id}/items | Get contract items
*ContractsApi* | [**getContractsPublicBidsContractId**](docs/ContractsApi.md#getcontractspublicbidscontractid) | **GET** /contracts/public/bids/{contract_id} | Get public contract bids
*ContractsApi* | [**getContractsPublicItemsContractId**](docs/ContractsApi.md#getcontractspublicitemscontractid) | **GET** /contracts/public/items/{contract_id} | Get public contract items
*ContractsApi* | [**getContractsPublicRegionId**](docs/ContractsApi.md#getcontractspublicregionid) | **GET** /contracts/public/{region_id} | Get public contracts
*ContractsApi* | [**getCorporationsCorporationIdContracts**](docs/ContractsApi.md#getcorporationscorporationidcontracts) | **GET** /corporations/{corporation_id}/contracts | Get corporation contracts
*ContractsApi* | [**getCorporationsCorporationIdContractsContractIdBids**](docs/ContractsApi.md#getcorporationscorporationidcontractscontractidbids) | **GET** /corporations/{corporation_id}/contracts/{contract_id}/bids | Get corporation contract bids
*ContractsApi* | [**getCorporationsCorporationIdContractsContractIdItems**](docs/ContractsApi.md#getcorporationscorporationidcontractscontractiditems) | **GET** /corporations/{corporation_id}/contracts/{contract_id}/items | Get corporation contract items
*CorporationApi* | [**getCorporationsCorporationId**](docs/CorporationApi.md#getcorporationscorporationid) | **GET** /corporations/{corporation_id} | Get corporation\&#39;s public information
*CorporationApi* | [**getCorporationsCorporationIdAlliancehistory**](docs/CorporationApi.md#getcorporationscorporationidalliancehistory) | **GET** /corporations/{corporation_id}/alliancehistory | Get alliance history
*CorporationApi* | [**getCorporationsCorporationIdBlueprints**](docs/CorporationApi.md#getcorporationscorporationidblueprints) | **GET** /corporations/{corporation_id}/blueprints | Get corporation blueprints
*CorporationApi* | [**getCorporationsCorporationIdContainersLogs**](docs/CorporationApi.md#getcorporationscorporationidcontainerslogs) | **GET** /corporations/{corporation_id}/containers/logs | Get all corporation ALSC logs
*CorporationApi* | [**getCorporationsCorporationIdDivisions**](docs/CorporationApi.md#getcorporationscorporationiddivisions) | **GET** /corporations/{corporation_id}/divisions | Get corporation divisions
*CorporationApi* | [**getCorporationsCorporationIdFacilities**](docs/CorporationApi.md#getcorporationscorporationidfacilities) | **GET** /corporations/{corporation_id}/facilities | Get corporation facilities
*CorporationApi* | [**getCorporationsCorporationIdIcons**](docs/CorporationApi.md#getcorporationscorporationidicons) | **GET** /corporations/{corporation_id}/icons | Get corporation icon
*CorporationApi* | [**getCorporationsCorporationIdMedals**](docs/CorporationApi.md#getcorporationscorporationidmedals) | **GET** /corporations/{corporation_id}/medals | Get corporation medals
*CorporationApi* | [**getCorporationsCorporationIdMedalsIssued**](docs/CorporationApi.md#getcorporationscorporationidmedalsissued) | **GET** /corporations/{corporation_id}/medals/issued | Get corporation issued medals
*CorporationApi* | [**getCorporationsCorporationIdMembers**](docs/CorporationApi.md#getcorporationscorporationidmembers) | **GET** /corporations/{corporation_id}/members | Get corporation members
*CorporationApi* | [**getCorporationsCorporationIdMembersLimit**](docs/CorporationApi.md#getcorporationscorporationidmemberslimit) | **GET** /corporations/{corporation_id}/members/limit | Get corporation member limit
*CorporationApi* | [**getCorporationsCorporationIdMembersTitles**](docs/CorporationApi.md#getcorporationscorporationidmemberstitles) | **GET** /corporations/{corporation_id}/members/titles | Get corporation\&#39;s members\&#39; titles
*CorporationApi* | [**getCorporationsCorporationIdMembertracking**](docs/CorporationApi.md#getcorporationscorporationidmembertracking) | **GET** /corporations/{corporation_id}/membertracking | Track corporation members
*CorporationApi* | [**getCorporationsCorporationIdRoles**](docs/CorporationApi.md#getcorporationscorporationidroles) | **GET** /corporations/{corporation_id}/roles | Get corporation member roles
*CorporationApi* | [**getCorporationsCorporationIdRolesHistory**](docs/CorporationApi.md#getcorporationscorporationidroleshistory) | **GET** /corporations/{corporation_id}/roles/history | Get corporation member roles history
*CorporationApi* | [**getCorporationsCorporationIdShareholders**](docs/CorporationApi.md#getcorporationscorporationidshareholders) | **GET** /corporations/{corporation_id}/shareholders | Get corporation shareholders
*CorporationApi* | [**getCorporationsCorporationIdStandings**](docs/CorporationApi.md#getcorporationscorporationidstandings) | **GET** /corporations/{corporation_id}/standings | Get corporation standings
*CorporationApi* | [**getCorporationsCorporationIdStarbases**](docs/CorporationApi.md#getcorporationscorporationidstarbases) | **GET** /corporations/{corporation_id}/starbases | Get corporation starbases (POSes)
*CorporationApi* | [**getCorporationsCorporationIdStarbasesStarbaseId**](docs/CorporationApi.md#getcorporationscorporationidstarbasesstarbaseid) | **GET** /corporations/{corporation_id}/starbases/{starbase_id} | Get starbase (POS) detail
*CorporationApi* | [**getCorporationsCorporationIdStructures**](docs/CorporationApi.md#getcorporationscorporationidstructures) | **GET** /corporations/{corporation_id}/structures | Get corporation structures
*CorporationApi* | [**getCorporationsCorporationIdTitles**](docs/CorporationApi.md#getcorporationscorporationidtitles) | **GET** /corporations/{corporation_id}/titles | Get corporation titles
*CorporationApi* | [**getCorporationsNpccorps**](docs/CorporationApi.md#getcorporationsnpccorps) | **GET** /corporations/npccorps | Get npc corporations
*CorporationProjectsApi* | [**getCorporationsProjectsContribution**](docs/CorporationProjectsApi.md#getcorporationsprojectscontribution) | **GET** /corporations/{corporation_id}/projects/{project_id}/contribution/{character_id} | Get your project contribution
*CorporationProjectsApi* | [**getCorporationsProjectsContributors**](docs/CorporationProjectsApi.md#getcorporationsprojectscontributors) | **GET** /corporations/{corporation_id}/projects/{project_id}/contributors | List project contributors
*CorporationProjectsApi* | [**getCorporationsProjectsDetail**](docs/CorporationProjectsApi.md#getcorporationsprojectsdetail) | **GET** /corporations/{corporation_id}/projects/{project_id} | Get project details
*CorporationProjectsApi* | [**getCorporationsProjectsListing**](docs/CorporationProjectsApi.md#getcorporationsprojectslisting) | **GET** /corporations/{corporation_id}/projects | List corporation projects
*DogmaApi* | [**getDogmaAttributes**](docs/DogmaApi.md#getdogmaattributes) | **GET** /dogma/attributes | Get attributes
*DogmaApi* | [**getDogmaAttributesAttributeId**](docs/DogmaApi.md#getdogmaattributesattributeid) | **GET** /dogma/attributes/{attribute_id} | Get attribute information
*DogmaApi* | [**getDogmaDynamicItemsTypeIdItemId**](docs/DogmaApi.md#getdogmadynamicitemstypeiditemid) | **GET** /dogma/dynamic/items/{type_id}/{item_id} | Get dynamic item information
*DogmaApi* | [**getDogmaEffects**](docs/DogmaApi.md#getdogmaeffects) | **GET** /dogma/effects | Get effects
*DogmaApi* | [**getDogmaEffectsEffectId**](docs/DogmaApi.md#getdogmaeffectseffectid) | **GET** /dogma/effects/{effect_id} | Get effect information
*FactionWarfareApi* | [**getCharactersCharacterIdFwStats**](docs/FactionWarfareApi.md#getcharacterscharacteridfwstats) | **GET** /characters/{character_id}/fw/stats | Overview of a character involved in faction warfare
*FactionWarfareApi* | [**getCorporationsCorporationIdFwStats**](docs/FactionWarfareApi.md#getcorporationscorporationidfwstats) | **GET** /corporations/{corporation_id}/fw/stats | Overview of a corporation involved in faction warfare
*FactionWarfareApi* | [**getFwLeaderboards**](docs/FactionWarfareApi.md#getfwleaderboards) | **GET** /fw/leaderboards | List of the top factions in faction warfare
*FactionWarfareApi* | [**getFwLeaderboardsCharacters**](docs/FactionWarfareApi.md#getfwleaderboardscharacters) | **GET** /fw/leaderboards/characters | List of the top pilots in faction warfare
*FactionWarfareApi* | [**getFwLeaderboardsCorporations**](docs/FactionWarfareApi.md#getfwleaderboardscorporations) | **GET** /fw/leaderboards/corporations | List of the top corporations in faction warfare
*FactionWarfareApi* | [**getFwStats**](docs/FactionWarfareApi.md#getfwstats) | **GET** /fw/stats | An overview of statistics about factions involved in faction warfare
*FactionWarfareApi* | [**getFwSystems**](docs/FactionWarfareApi.md#getfwsystems) | **GET** /fw/systems | Ownership of faction warfare systems
*FactionWarfareApi* | [**getFwWars**](docs/FactionWarfareApi.md#getfwwars) | **GET** /fw/wars | Data about which NPC factions are at war
*FittingsApi* | [**deleteCharactersCharacterIdFittingsFittingId**](docs/FittingsApi.md#deletecharacterscharacteridfittingsfittingid) | **DELETE** /characters/{character_id}/fittings/{fitting_id} | Delete fitting
*FittingsApi* | [**getCharactersCharacterIdFittings**](docs/FittingsApi.md#getcharacterscharacteridfittings) | **GET** /characters/{character_id}/fittings | Get fittings
*FittingsApi* | [**postCharactersCharacterIdFittings**](docs/FittingsApi.md#postcharacterscharacteridfittings) | **POST** /characters/{character_id}/fittings | Create fitting
*FleetsApi* | [**deleteFleetsFleetIdMembersMemberId**](docs/FleetsApi.md#deletefleetsfleetidmembersmemberid) | **DELETE** /fleets/{fleet_id}/members/{member_id} | Kick fleet member
*FleetsApi* | [**deleteFleetsFleetIdSquadsSquadId**](docs/FleetsApi.md#deletefleetsfleetidsquadssquadid) | **DELETE** /fleets/{fleet_id}/squads/{squad_id} | Delete fleet squad
*FleetsApi* | [**deleteFleetsFleetIdWingsWingId**](docs/FleetsApi.md#deletefleetsfleetidwingswingid) | **DELETE** /fleets/{fleet_id}/wings/{wing_id} | Delete fleet wing
*FleetsApi* | [**getCharactersCharacterIdFleet**](docs/FleetsApi.md#getcharacterscharacteridfleet) | **GET** /characters/{character_id}/fleet | Get character fleet info
*FleetsApi* | [**getFleetsFleetId**](docs/FleetsApi.md#getfleetsfleetid) | **GET** /fleets/{fleet_id} | Get fleet information
*FleetsApi* | [**getFleetsFleetIdMembers**](docs/FleetsApi.md#getfleetsfleetidmembers) | **GET** /fleets/{fleet_id}/members | Get fleet members
*FleetsApi* | [**getFleetsFleetIdWings**](docs/FleetsApi.md#getfleetsfleetidwings) | **GET** /fleets/{fleet_id}/wings | Get fleet wings
*FleetsApi* | [**postFleetsFleetIdMembers**](docs/FleetsApi.md#postfleetsfleetidmembers) | **POST** /fleets/{fleet_id}/members | Create fleet invitation
*FleetsApi* | [**postFleetsFleetIdWings**](docs/FleetsApi.md#postfleetsfleetidwings) | **POST** /fleets/{fleet_id}/wings | Create fleet wing
*FleetsApi* | [**postFleetsFleetIdWingsWingIdSquads**](docs/FleetsApi.md#postfleetsfleetidwingswingidsquads) | **POST** /fleets/{fleet_id}/wings/{wing_id}/squads | Create fleet squad
*FleetsApi* | [**putFleetsFleetId**](docs/FleetsApi.md#putfleetsfleetid) | **PUT** /fleets/{fleet_id} | Update fleet
*FleetsApi* | [**putFleetsFleetIdMembersMemberId**](docs/FleetsApi.md#putfleetsfleetidmembersmemberid) | **PUT** /fleets/{fleet_id}/members/{member_id} | Move fleet member
*FleetsApi* | [**putFleetsFleetIdSquadsSquadId**](docs/FleetsApi.md#putfleetsfleetidsquadssquadid) | **PUT** /fleets/{fleet_id}/squads/{squad_id} | Rename fleet squad
*FleetsApi* | [**putFleetsFleetIdWingsWingId**](docs/FleetsApi.md#putfleetsfleetidwingswingid) | **PUT** /fleets/{fleet_id}/wings/{wing_id} | Rename fleet wing
*FreelanceJobsApi* | [**getCharactersFreelanceJobsListing**](docs/FreelanceJobsApi.md#getcharactersfreelancejobslisting) | **GET** /characters/{character_id}/freelance-jobs | List character freelance jobs
*FreelanceJobsApi* | [**getCharactersFreelanceJobsParticipation**](docs/FreelanceJobsApi.md#getcharactersfreelancejobsparticipation) | **GET** /characters/{character_id}/freelance-jobs/{job_id}/participation | Get character freelance job participation
*FreelanceJobsApi* | [**getCorporationsFreelanceJobsListing**](docs/FreelanceJobsApi.md#getcorporationsfreelancejobslisting) | **GET** /corporations/{corporation_id}/freelance-jobs | List corporation freelance jobs
*FreelanceJobsApi* | [**getCorporationsFreelanceJobsParticipants**](docs/FreelanceJobsApi.md#getcorporationsfreelancejobsparticipants) | **GET** /corporations/{corporation_id}/freelance-jobs/{job_id}/participants | List participants of a freelance job
*FreelanceJobsApi* | [**getFreelanceJobsDetail**](docs/FreelanceJobsApi.md#getfreelancejobsdetail) | **GET** /freelance-jobs/{job_id} | Get freelance job details
*FreelanceJobsApi* | [**getFreelanceJobsListing**](docs/FreelanceJobsApi.md#getfreelancejobslisting) | **GET** /freelance-jobs | List freelance jobs
*IncursionsApi* | [**getIncursions**](docs/IncursionsApi.md#getincursions) | **GET** /incursions | List incursions
*IndustryApi* | [**getCharactersCharacterIdIndustryJobs**](docs/IndustryApi.md#getcharacterscharacteridindustryjobs) | **GET** /characters/{character_id}/industry/jobs | List character industry jobs
*IndustryApi* | [**getCharactersCharacterIdMining**](docs/IndustryApi.md#getcharacterscharacteridmining) | **GET** /characters/{character_id}/mining | Character mining ledger
*IndustryApi* | [**getCorporationCorporationIdMiningExtractions**](docs/IndustryApi.md#getcorporationcorporationidminingextractions) | **GET** /corporation/{corporation_id}/mining/extractions | Moon extraction timers
*IndustryApi* | [**getCorporationCorporationIdMiningObservers**](docs/IndustryApi.md#getcorporationcorporationidminingobservers) | **GET** /corporation/{corporation_id}/mining/observers | Corporation mining observers
*IndustryApi* | [**getCorporationCorporationIdMiningObserversObserverId**](docs/IndustryApi.md#getcorporationcorporationidminingobserversobserverid) | **GET** /corporation/{corporation_id}/mining/observers/{observer_id} | Observed corporation mining
*IndustryApi* | [**getCorporationsCorporationIdIndustryJobs**](docs/IndustryApi.md#getcorporationscorporationidindustryjobs) | **GET** /corporations/{corporation_id}/industry/jobs | List corporation industry jobs
*IndustryApi* | [**getIndustryFacilities**](docs/IndustryApi.md#getindustryfacilities) | **GET** /industry/facilities | List industry facilities
*IndustryApi* | [**getIndustrySystems**](docs/IndustryApi.md#getindustrysystems) | **GET** /industry/systems | List solar system cost indices
*InsuranceApi* | [**getInsurancePrices**](docs/InsuranceApi.md#getinsuranceprices) | **GET** /insurance/prices | List insurance levels
*KillmailsApi* | [**getCharactersCharacterIdKillmailsRecent**](docs/KillmailsApi.md#getcharacterscharacteridkillmailsrecent) | **GET** /characters/{character_id}/killmails/recent | Get a character\&#39;s recent kills and losses
*KillmailsApi* | [**getCorporationsCorporationIdKillmailsRecent**](docs/KillmailsApi.md#getcorporationscorporationidkillmailsrecent) | **GET** /corporations/{corporation_id}/killmails/recent | Get a corporation\&#39;s recent kills and losses
*KillmailsApi* | [**getKillmailsKillmailIdKillmailHash**](docs/KillmailsApi.md#getkillmailskillmailidkillmailhash) | **GET** /killmails/{killmail_id}/{killmail_hash} | Get a single killmail
*LocationApi* | [**getCharactersCharacterIdLocation**](docs/LocationApi.md#getcharacterscharacteridlocation) | **GET** /characters/{character_id}/location | Get character location
*LocationApi* | [**getCharactersCharacterIdOnline**](docs/LocationApi.md#getcharacterscharacteridonline) | **GET** /characters/{character_id}/online | Get character online
*LocationApi* | [**getCharactersCharacterIdShip**](docs/LocationApi.md#getcharacterscharacteridship) | **GET** /characters/{character_id}/ship | Get current ship
*LoyaltyApi* | [**getCharactersCharacterIdLoyaltyPoints**](docs/LoyaltyApi.md#getcharacterscharacteridloyaltypoints) | **GET** /characters/{character_id}/loyalty/points | Get loyalty points
*LoyaltyApi* | [**getLoyaltyStoresCorporationIdOffers**](docs/LoyaltyApi.md#getloyaltystorescorporationidoffers) | **GET** /loyalty/stores/{corporation_id}/offers | List loyalty store offers
*MailApi* | [**deleteCharactersCharacterIdMailLabelsLabelId**](docs/MailApi.md#deletecharacterscharacteridmaillabelslabelid) | **DELETE** /characters/{character_id}/mail/labels/{label_id} | Delete a mail label
*MailApi* | [**deleteCharactersCharacterIdMailMailId**](docs/MailApi.md#deletecharacterscharacteridmailmailid) | **DELETE** /characters/{character_id}/mail/{mail_id} | Delete a mail
*MailApi* | [**getCharactersCharacterIdMail**](docs/MailApi.md#getcharacterscharacteridmail) | **GET** /characters/{character_id}/mail | Return mail headers
*MailApi* | [**getCharactersCharacterIdMailLabels**](docs/MailApi.md#getcharacterscharacteridmaillabels) | **GET** /characters/{character_id}/mail/labels | Get mail labels and unread counts
*MailApi* | [**getCharactersCharacterIdMailLists**](docs/MailApi.md#getcharacterscharacteridmaillists) | **GET** /characters/{character_id}/mail/lists | Return mailing list subscriptions
*MailApi* | [**getCharactersCharacterIdMailMailId**](docs/MailApi.md#getcharacterscharacteridmailmailid) | **GET** /characters/{character_id}/mail/{mail_id} | Return a mail
*MailApi* | [**postCharactersCharacterIdMail**](docs/MailApi.md#postcharacterscharacteridmail) | **POST** /characters/{character_id}/mail | Send a new mail
*MailApi* | [**postCharactersCharacterIdMailLabels**](docs/MailApi.md#postcharacterscharacteridmaillabels) | **POST** /characters/{character_id}/mail/labels | Create a mail label
*MailApi* | [**putCharactersCharacterIdMailMailId**](docs/MailApi.md#putcharacterscharacteridmailmailid) | **PUT** /characters/{character_id}/mail/{mail_id} | Update metadata about a mail
*MarketApi* | [**getCharactersCharacterIdOrders**](docs/MarketApi.md#getcharacterscharacteridorders) | **GET** /characters/{character_id}/orders | List open orders from a character
*MarketApi* | [**getCharactersCharacterIdOrdersHistory**](docs/MarketApi.md#getcharacterscharacteridordershistory) | **GET** /characters/{character_id}/orders/history | List historical orders by a character
*MarketApi* | [**getCorporationsCorporationIdOrders**](docs/MarketApi.md#getcorporationscorporationidorders) | **GET** /corporations/{corporation_id}/orders | List open orders from a corporation
*MarketApi* | [**getCorporationsCorporationIdOrdersHistory**](docs/MarketApi.md#getcorporationscorporationidordershistory) | **GET** /corporations/{corporation_id}/orders/history | List historical orders from a corporation
*MarketApi* | [**getMarketsGroups**](docs/MarketApi.md#getmarketsgroups) | **GET** /markets/groups | Get item groups
*MarketApi* | [**getMarketsGroupsMarketGroupId**](docs/MarketApi.md#getmarketsgroupsmarketgroupid) | **GET** /markets/groups/{market_group_id} | Get item group information
*MarketApi* | [**getMarketsPrices**](docs/MarketApi.md#getmarketsprices) | **GET** /markets/prices | List market prices
*MarketApi* | [**getMarketsRegionIdHistory**](docs/MarketApi.md#getmarketsregionidhistory) | **GET** /markets/{region_id}/history | List historical market statistics in a region
*MarketApi* | [**getMarketsRegionIdOrders**](docs/MarketApi.md#getmarketsregionidorders) | **GET** /markets/{region_id}/orders | List orders in a region
*MarketApi* | [**getMarketsRegionIdTypes**](docs/MarketApi.md#getmarketsregionidtypes) | **GET** /markets/{region_id}/types | List type IDs relevant to a market
*MarketApi* | [**getMarketsStructuresStructureId**](docs/MarketApi.md#getmarketsstructuresstructureid) | **GET** /markets/structures/{structure_id} | List orders in a structure
*MetaApi* | [**getMetaChangelog**](docs/MetaApi.md#getmetachangelog) | **GET** /meta/changelog | Get changelog
*MetaApi* | [**getMetaCompatibilityDates**](docs/MetaApi.md#getmetacompatibilitydates) | **GET** /meta/compatibility-dates | Get compatibility dates
*MetaApi* | [**getMetaStatus**](docs/MetaApi.md#getmetastatus) | **GET** /meta/status | Get health status
*PlanetaryInteractionApi* | [**getCharactersCharacterIdPlanets**](docs/PlanetaryInteractionApi.md#getcharacterscharacteridplanets) | **GET** /characters/{character_id}/planets | Get colonies
*PlanetaryInteractionApi* | [**getCharactersCharacterIdPlanetsPlanetId**](docs/PlanetaryInteractionApi.md#getcharacterscharacteridplanetsplanetid) | **GET** /characters/{character_id}/planets/{planet_id} | Get colony layout
*PlanetaryInteractionApi* | [**getCorporationsCorporationIdCustomsOffices**](docs/PlanetaryInteractionApi.md#getcorporationscorporationidcustomsoffices) | **GET** /corporations/{corporation_id}/customs_offices | List corporation customs offices
*PlanetaryInteractionApi* | [**getUniverseSchematicsSchematicId**](docs/PlanetaryInteractionApi.md#getuniverseschematicsschematicid) | **GET** /universe/schematics/{schematic_id} | Get schematic information
*RoutesApi* | [**postRoute**](docs/RoutesApi.md#postroute) | **POST** /route/{origin_system_id}/{destination_system_id} | Get route between two systems
*SearchApi* | [**getCharactersCharacterIdSearch**](docs/SearchApi.md#getcharacterscharacteridsearch) | **GET** /characters/{character_id}/search | Search on a string
*SkillsApi* | [**getCharactersCharacterIdAttributes**](docs/SkillsApi.md#getcharacterscharacteridattributes) | **GET** /characters/{character_id}/attributes | Get character attributes
*SkillsApi* | [**getCharactersCharacterIdSkillqueue**](docs/SkillsApi.md#getcharacterscharacteridskillqueue) | **GET** /characters/{character_id}/skillqueue | Get character\&#39;s skill queue
*SkillsApi* | [**getCharactersCharacterIdSkills**](docs/SkillsApi.md#getcharacterscharacteridskills) | **GET** /characters/{character_id}/skills | Get character skills
*SovereigntyApi* | [**getSovereigntyCampaigns**](docs/SovereigntyApi.md#getsovereigntycampaigns) | **GET** /sovereignty/campaigns | List sovereignty campaigns
*SovereigntyApi* | [**getSovereigntyMap**](docs/SovereigntyApi.md#getsovereigntymap) | **GET** /sovereignty/map | List sovereignty of systems
*SovereigntyApi* | [**getSovereigntyStructures**](docs/SovereigntyApi.md#getsovereigntystructures) | **GET** /sovereignty/structures | List sovereignty structures
*StatusApi* | [**getStatus**](docs/StatusApi.md#getstatus) | **GET** /status | Retrieve the uptime and player counts
*UniverseApi* | [**getUniverseAncestries**](docs/UniverseApi.md#getuniverseancestries) | **GET** /universe/ancestries | Get ancestries
*UniverseApi* | [**getUniverseAsteroidBeltsAsteroidBeltId**](docs/UniverseApi.md#getuniverseasteroidbeltsasteroidbeltid) | **GET** /universe/asteroid_belts/{asteroid_belt_id} | Get asteroid belt information
*UniverseApi* | [**getUniverseBloodlines**](docs/UniverseApi.md#getuniversebloodlines) | **GET** /universe/bloodlines | Get bloodlines
*UniverseApi* | [**getUniverseCategories**](docs/UniverseApi.md#getuniversecategories) | **GET** /universe/categories | Get item categories
*UniverseApi* | [**getUniverseCategoriesCategoryId**](docs/UniverseApi.md#getuniversecategoriescategoryid) | **GET** /universe/categories/{category_id} | Get item category information
*UniverseApi* | [**getUniverseConstellations**](docs/UniverseApi.md#getuniverseconstellations) | **GET** /universe/constellations | Get constellations
*UniverseApi* | [**getUniverseConstellationsConstellationId**](docs/UniverseApi.md#getuniverseconstellationsconstellationid) | **GET** /universe/constellations/{constellation_id} | Get constellation information
*UniverseApi* | [**getUniverseFactions**](docs/UniverseApi.md#getuniversefactions) | **GET** /universe/factions | Get factions
*UniverseApi* | [**getUniverseGraphics**](docs/UniverseApi.md#getuniversegraphics) | **GET** /universe/graphics | Get graphics
*UniverseApi* | [**getUniverseGraphicsGraphicId**](docs/UniverseApi.md#getuniversegraphicsgraphicid) | **GET** /universe/graphics/{graphic_id} | Get graphic information
*UniverseApi* | [**getUniverseGroups**](docs/UniverseApi.md#getuniversegroups) | **GET** /universe/groups | Get item groups
*UniverseApi* | [**getUniverseGroupsGroupId**](docs/UniverseApi.md#getuniversegroupsgroupid) | **GET** /universe/groups/{group_id} | Get item group information
*UniverseApi* | [**getUniverseMoonsMoonId**](docs/UniverseApi.md#getuniversemoonsmoonid) | **GET** /universe/moons/{moon_id} | Get moon information
*UniverseApi* | [**getUniversePlanetsPlanetId**](docs/UniverseApi.md#getuniverseplanetsplanetid) | **GET** /universe/planets/{planet_id} | Get planet information
*UniverseApi* | [**getUniverseRaces**](docs/UniverseApi.md#getuniverseraces) | **GET** /universe/races | Get character races
*UniverseApi* | [**getUniverseRegions**](docs/UniverseApi.md#getuniverseregions) | **GET** /universe/regions | Get regions
*UniverseApi* | [**getUniverseRegionsRegionId**](docs/UniverseApi.md#getuniverseregionsregionid) | **GET** /universe/regions/{region_id} | Get region information
*UniverseApi* | [**getUniverseStargatesStargateId**](docs/UniverseApi.md#getuniversestargatesstargateid) | **GET** /universe/stargates/{stargate_id} | Get stargate information
*UniverseApi* | [**getUniverseStarsStarId**](docs/UniverseApi.md#getuniversestarsstarid) | **GET** /universe/stars/{star_id} | Get star information
*UniverseApi* | [**getUniverseStationsStationId**](docs/UniverseApi.md#getuniversestationsstationid) | **GET** /universe/stations/{station_id} | Get station information
*UniverseApi* | [**getUniverseStructures**](docs/UniverseApi.md#getuniversestructures) | **GET** /universe/structures | List all public structures
*UniverseApi* | [**getUniverseStructuresStructureId**](docs/UniverseApi.md#getuniversestructuresstructureid) | **GET** /universe/structures/{structure_id} | Get structure information
*UniverseApi* | [**getUniverseSystemJumps**](docs/UniverseApi.md#getuniversesystemjumps) | **GET** /universe/system_jumps | Get system jumps
*UniverseApi* | [**getUniverseSystemKills**](docs/UniverseApi.md#getuniversesystemkills) | **GET** /universe/system_kills | Get system kills
*UniverseApi* | [**getUniverseSystems**](docs/UniverseApi.md#getuniversesystems) | **GET** /universe/systems | Get solar systems
*UniverseApi* | [**getUniverseSystemsSystemId**](docs/UniverseApi.md#getuniversesystemssystemid) | **GET** /universe/systems/{system_id} | Get solar system information
*UniverseApi* | [**getUniverseTypes**](docs/UniverseApi.md#getuniversetypes) | **GET** /universe/types | Get types
*UniverseApi* | [**getUniverseTypesTypeId**](docs/UniverseApi.md#getuniversetypestypeid) | **GET** /universe/types/{type_id} | Get type information
*UniverseApi* | [**postUniverseIds**](docs/UniverseApi.md#postuniverseids) | **POST** /universe/ids | Bulk names to IDs
*UniverseApi* | [**postUniverseNames**](docs/UniverseApi.md#postuniversenames) | **POST** /universe/names | Get names and categories for a set of IDs
*UserInterfaceApi* | [**postUiAutopilotWaypoint**](docs/UserInterfaceApi.md#postuiautopilotwaypoint) | **POST** /ui/autopilot/waypoint | Set Autopilot Waypoint
*UserInterfaceApi* | [**postUiOpenwindowContract**](docs/UserInterfaceApi.md#postuiopenwindowcontract) | **POST** /ui/openwindow/contract | Open Contract Window
*UserInterfaceApi* | [**postUiOpenwindowInformation**](docs/UserInterfaceApi.md#postuiopenwindowinformation) | **POST** /ui/openwindow/information | Open Information Window
*UserInterfaceApi* | [**postUiOpenwindowMarketdetails**](docs/UserInterfaceApi.md#postuiopenwindowmarketdetails) | **POST** /ui/openwindow/marketdetails | Open Market Details
*UserInterfaceApi* | [**postUiOpenwindowNewmail**](docs/UserInterfaceApi.md#postuiopenwindownewmail) | **POST** /ui/openwindow/newmail | Open New Mail Window
*WalletApi* | [**getCharactersCharacterIdWallet**](docs/WalletApi.md#getcharacterscharacteridwallet) | **GET** /characters/{character_id}/wallet | Get a character\&#39;s wallet balance
*WalletApi* | [**getCharactersCharacterIdWalletJournal**](docs/WalletApi.md#getcharacterscharacteridwalletjournal) | **GET** /characters/{character_id}/wallet/journal | Get character wallet journal
*WalletApi* | [**getCharactersCharacterIdWalletTransactions**](docs/WalletApi.md#getcharacterscharacteridwallettransactions) | **GET** /characters/{character_id}/wallet/transactions | Get wallet transactions
*WalletApi* | [**getCorporationsCorporationIdWallets**](docs/WalletApi.md#getcorporationscorporationidwallets) | **GET** /corporations/{corporation_id}/wallets | Returns a corporation\&#39;s wallet balance
*WalletApi* | [**getCorporationsCorporationIdWalletsDivisionJournal**](docs/WalletApi.md#getcorporationscorporationidwalletsdivisionjournal) | **GET** /corporations/{corporation_id}/wallets/{division}/journal | Get corporation wallet journal
*WalletApi* | [**getCorporationsCorporationIdWalletsDivisionTransactions**](docs/WalletApi.md#getcorporationscorporationidwalletsdivisiontransactions) | **GET** /corporations/{corporation_id}/wallets/{division}/transactions | Get corporation wallet transactions
*WarsApi* | [**getWars**](docs/WarsApi.md#getwars) | **GET** /wars | List wars
*WarsApi* | [**getWarsWarId**](docs/WarsApi.md#getwarswarid) | **GET** /wars/{war_id} | Get war information
*WarsApi* | [**getWarsWarIdKillmails**](docs/WarsApi.md#getwarswaridkillmails) | **GET** /wars/{war_id}/killmails | List kills for a war


### Documentation For Models

 - [AllianceDetail](docs/AllianceDetail.md)
 - [AllianceId](docs/AllianceId.md)
 - [AlliancesAllianceIdContactsGetInner](docs/AlliancesAllianceIdContactsGetInner.md)
 - [AlliancesAllianceIdContactsLabelsGetInner](docs/AlliancesAllianceIdContactsLabelsGetInner.md)
 - [AlliancesAllianceIdIconsGet](docs/AlliancesAllianceIdIconsGet.md)
 - [CaptureFwComplex](docs/CaptureFwComplex.md)
 - [CharacterId](docs/CharacterId.md)
 - [CharactersAffiliationPostInner](docs/CharactersAffiliationPostInner.md)
 - [CharactersCharacterIdAgentsResearchGetInner](docs/CharactersCharacterIdAgentsResearchGetInner.md)
 - [CharactersCharacterIdAssetsGetInner](docs/CharactersCharacterIdAssetsGetInner.md)
 - [CharactersCharacterIdAssetsLocationsPostInner](docs/CharactersCharacterIdAssetsLocationsPostInner.md)
 - [CharactersCharacterIdAssetsLocationsPostInnerPosition](docs/CharactersCharacterIdAssetsLocationsPostInnerPosition.md)
 - [CharactersCharacterIdAssetsNamesPostInner](docs/CharactersCharacterIdAssetsNamesPostInner.md)
 - [CharactersCharacterIdAttributesGet](docs/CharactersCharacterIdAttributesGet.md)
 - [CharactersCharacterIdBlueprintsGetInner](docs/CharactersCharacterIdBlueprintsGetInner.md)
 - [CharactersCharacterIdCalendarEventIdAttendeesGetInner](docs/CharactersCharacterIdCalendarEventIdAttendeesGetInner.md)
 - [CharactersCharacterIdCalendarEventIdGet](docs/CharactersCharacterIdCalendarEventIdGet.md)
 - [CharactersCharacterIdCalendarGetInner](docs/CharactersCharacterIdCalendarGetInner.md)
 - [CharactersCharacterIdClonesGet](docs/CharactersCharacterIdClonesGet.md)
 - [CharactersCharacterIdClonesGetHomeLocation](docs/CharactersCharacterIdClonesGetHomeLocation.md)
 - [CharactersCharacterIdClonesGetJumpClonesInner](docs/CharactersCharacterIdClonesGetJumpClonesInner.md)
 - [CharactersCharacterIdContactsGetInner](docs/CharactersCharacterIdContactsGetInner.md)
 - [CharactersCharacterIdContractsContractIdBidsGetInner](docs/CharactersCharacterIdContractsContractIdBidsGetInner.md)
 - [CharactersCharacterIdContractsContractIdItemsGetInner](docs/CharactersCharacterIdContractsContractIdItemsGetInner.md)
 - [CharactersCharacterIdContractsGetInner](docs/CharactersCharacterIdContractsGetInner.md)
 - [CharactersCharacterIdCorporationhistoryGetInner](docs/CharactersCharacterIdCorporationhistoryGetInner.md)
 - [CharactersCharacterIdFatigueGet](docs/CharactersCharacterIdFatigueGet.md)
 - [CharactersCharacterIdFittingsGetInner](docs/CharactersCharacterIdFittingsGetInner.md)
 - [CharactersCharacterIdFittingsGetInnerItemsInner](docs/CharactersCharacterIdFittingsGetInnerItemsInner.md)
 - [CharactersCharacterIdFittingsPost](docs/CharactersCharacterIdFittingsPost.md)
 - [CharactersCharacterIdFleetGet](docs/CharactersCharacterIdFleetGet.md)
 - [CharactersCharacterIdFwStatsGet](docs/CharactersCharacterIdFwStatsGet.md)
 - [CharactersCharacterIdFwStatsGetKills](docs/CharactersCharacterIdFwStatsGetKills.md)
 - [CharactersCharacterIdFwStatsGetVictoryPoints](docs/CharactersCharacterIdFwStatsGetVictoryPoints.md)
 - [CharactersCharacterIdIndustryJobsGetInner](docs/CharactersCharacterIdIndustryJobsGetInner.md)
 - [CharactersCharacterIdKillmailsRecentGetInner](docs/CharactersCharacterIdKillmailsRecentGetInner.md)
 - [CharactersCharacterIdLocationGet](docs/CharactersCharacterIdLocationGet.md)
 - [CharactersCharacterIdLoyaltyPointsGetInner](docs/CharactersCharacterIdLoyaltyPointsGetInner.md)
 - [CharactersCharacterIdMailGetInner](docs/CharactersCharacterIdMailGetInner.md)
 - [CharactersCharacterIdMailLabelsGet](docs/CharactersCharacterIdMailLabelsGet.md)
 - [CharactersCharacterIdMailLabelsGetLabelsInner](docs/CharactersCharacterIdMailLabelsGetLabelsInner.md)
 - [CharactersCharacterIdMailListsGetInner](docs/CharactersCharacterIdMailListsGetInner.md)
 - [CharactersCharacterIdMailMailIdGet](docs/CharactersCharacterIdMailMailIdGet.md)
 - [CharactersCharacterIdMedalsGetInner](docs/CharactersCharacterIdMedalsGetInner.md)
 - [CharactersCharacterIdMedalsGetInnerGraphicsInner](docs/CharactersCharacterIdMedalsGetInnerGraphicsInner.md)
 - [CharactersCharacterIdMiningGetInner](docs/CharactersCharacterIdMiningGetInner.md)
 - [CharactersCharacterIdNotificationsContactsGetInner](docs/CharactersCharacterIdNotificationsContactsGetInner.md)
 - [CharactersCharacterIdNotificationsGetInner](docs/CharactersCharacterIdNotificationsGetInner.md)
 - [CharactersCharacterIdOnlineGet](docs/CharactersCharacterIdOnlineGet.md)
 - [CharactersCharacterIdOrdersGetInner](docs/CharactersCharacterIdOrdersGetInner.md)
 - [CharactersCharacterIdOrdersHistoryGetInner](docs/CharactersCharacterIdOrdersHistoryGetInner.md)
 - [CharactersCharacterIdPlanetsGetInner](docs/CharactersCharacterIdPlanetsGetInner.md)
 - [CharactersCharacterIdPlanetsPlanetIdGet](docs/CharactersCharacterIdPlanetsPlanetIdGet.md)
 - [CharactersCharacterIdPlanetsPlanetIdGetLinksInner](docs/CharactersCharacterIdPlanetsPlanetIdGetLinksInner.md)
 - [CharactersCharacterIdPlanetsPlanetIdGetPinsInner](docs/CharactersCharacterIdPlanetsPlanetIdGetPinsInner.md)
 - [CharactersCharacterIdPlanetsPlanetIdGetPinsInnerContentsInner](docs/CharactersCharacterIdPlanetsPlanetIdGetPinsInnerContentsInner.md)
 - [CharactersCharacterIdPlanetsPlanetIdGetPinsInnerExtractorDetails](docs/CharactersCharacterIdPlanetsPlanetIdGetPinsInnerExtractorDetails.md)
 - [CharactersCharacterIdPlanetsPlanetIdGetPinsInnerExtractorDetailsHeadsInner](docs/CharactersCharacterIdPlanetsPlanetIdGetPinsInnerExtractorDetailsHeadsInner.md)
 - [CharactersCharacterIdPlanetsPlanetIdGetPinsInnerFactoryDetails](docs/CharactersCharacterIdPlanetsPlanetIdGetPinsInnerFactoryDetails.md)
 - [CharactersCharacterIdPlanetsPlanetIdGetRoutesInner](docs/CharactersCharacterIdPlanetsPlanetIdGetRoutesInner.md)
 - [CharactersCharacterIdPortraitGet](docs/CharactersCharacterIdPortraitGet.md)
 - [CharactersCharacterIdRolesGet](docs/CharactersCharacterIdRolesGet.md)
 - [CharactersCharacterIdSearchGet](docs/CharactersCharacterIdSearchGet.md)
 - [CharactersCharacterIdShipGet](docs/CharactersCharacterIdShipGet.md)
 - [CharactersCharacterIdStandingsGetInner](docs/CharactersCharacterIdStandingsGetInner.md)
 - [CharactersCharacterIdTitlesGetInner](docs/CharactersCharacterIdTitlesGetInner.md)
 - [CharactersCharacterIdWalletJournalGetInner](docs/CharactersCharacterIdWalletJournalGetInner.md)
 - [CharactersCharacterIdWalletTransactionsGetInner](docs/CharactersCharacterIdWalletTransactionsGetInner.md)
 - [CharactersDetail](docs/CharactersDetail.md)
 - [CharactersFreelanceJobsListing](docs/CharactersFreelanceJobsListing.md)
 - [CharactersFreelanceJobsParticipation](docs/CharactersFreelanceJobsParticipation.md)
 - [CharactersSkillqueueSkill](docs/CharactersSkillqueueSkill.md)
 - [CharactersSkills](docs/CharactersSkills.md)
 - [CharactersSkillsSkill](docs/CharactersSkillsSkill.md)
 - [ConstellationId](docs/ConstellationId.md)
 - [ContractsPublicBidsContractIdGetInner](docs/ContractsPublicBidsContractIdGetInner.md)
 - [ContractsPublicItemsContractIdGetInner](docs/ContractsPublicItemsContractIdGetInner.md)
 - [ContractsPublicRegionIdGetInner](docs/ContractsPublicRegionIdGetInner.md)
 - [CorporationCorporationIdMiningExtractionsGetInner](docs/CorporationCorporationIdMiningExtractionsGetInner.md)
 - [CorporationCorporationIdMiningObserversGetInner](docs/CorporationCorporationIdMiningObserversGetInner.md)
 - [CorporationCorporationIdMiningObserversObserverIdGetInner](docs/CorporationCorporationIdMiningObserversObserverIdGetInner.md)
 - [CorporationId](docs/CorporationId.md)
 - [CorporationItemDelivery](docs/CorporationItemDelivery.md)
 - [CorporationsCorporationIdAlliancehistoryGetInner](docs/CorporationsCorporationIdAlliancehistoryGetInner.md)
 - [CorporationsCorporationIdAssetsGetInner](docs/CorporationsCorporationIdAssetsGetInner.md)
 - [CorporationsCorporationIdBlueprintsGetInner](docs/CorporationsCorporationIdBlueprintsGetInner.md)
 - [CorporationsCorporationIdContactsGetInner](docs/CorporationsCorporationIdContactsGetInner.md)
 - [CorporationsCorporationIdContainersLogsGetInner](docs/CorporationsCorporationIdContainersLogsGetInner.md)
 - [CorporationsCorporationIdContractsGetInner](docs/CorporationsCorporationIdContractsGetInner.md)
 - [CorporationsCorporationIdCustomsOfficesGetInner](docs/CorporationsCorporationIdCustomsOfficesGetInner.md)
 - [CorporationsCorporationIdDivisionsGet](docs/CorporationsCorporationIdDivisionsGet.md)
 - [CorporationsCorporationIdDivisionsGetHangarInner](docs/CorporationsCorporationIdDivisionsGetHangarInner.md)
 - [CorporationsCorporationIdDivisionsGetWalletInner](docs/CorporationsCorporationIdDivisionsGetWalletInner.md)
 - [CorporationsCorporationIdFacilitiesGetInner](docs/CorporationsCorporationIdFacilitiesGetInner.md)
 - [CorporationsCorporationIdFwStatsGet](docs/CorporationsCorporationIdFwStatsGet.md)
 - [CorporationsCorporationIdFwStatsGetKills](docs/CorporationsCorporationIdFwStatsGetKills.md)
 - [CorporationsCorporationIdFwStatsGetVictoryPoints](docs/CorporationsCorporationIdFwStatsGetVictoryPoints.md)
 - [CorporationsCorporationIdIconsGet](docs/CorporationsCorporationIdIconsGet.md)
 - [CorporationsCorporationIdIndustryJobsGetInner](docs/CorporationsCorporationIdIndustryJobsGetInner.md)
 - [CorporationsCorporationIdMedalsGetInner](docs/CorporationsCorporationIdMedalsGetInner.md)
 - [CorporationsCorporationIdMedalsIssuedGetInner](docs/CorporationsCorporationIdMedalsIssuedGetInner.md)
 - [CorporationsCorporationIdMembersTitlesGetInner](docs/CorporationsCorporationIdMembersTitlesGetInner.md)
 - [CorporationsCorporationIdMembertrackingGetInner](docs/CorporationsCorporationIdMembertrackingGetInner.md)
 - [CorporationsCorporationIdOrdersGetInner](docs/CorporationsCorporationIdOrdersGetInner.md)
 - [CorporationsCorporationIdOrdersHistoryGetInner](docs/CorporationsCorporationIdOrdersHistoryGetInner.md)
 - [CorporationsCorporationIdRolesGetInner](docs/CorporationsCorporationIdRolesGetInner.md)
 - [CorporationsCorporationIdRolesHistoryGetInner](docs/CorporationsCorporationIdRolesHistoryGetInner.md)
 - [CorporationsCorporationIdShareholdersGetInner](docs/CorporationsCorporationIdShareholdersGetInner.md)
 - [CorporationsCorporationIdStarbasesGetInner](docs/CorporationsCorporationIdStarbasesGetInner.md)
 - [CorporationsCorporationIdStarbasesStarbaseIdGet](docs/CorporationsCorporationIdStarbasesStarbaseIdGet.md)
 - [CorporationsCorporationIdStarbasesStarbaseIdGetFuelsInner](docs/CorporationsCorporationIdStarbasesStarbaseIdGetFuelsInner.md)
 - [CorporationsCorporationIdStructuresGetInner](docs/CorporationsCorporationIdStructuresGetInner.md)
 - [CorporationsCorporationIdStructuresGetInnerServicesInner](docs/CorporationsCorporationIdStructuresGetInnerServicesInner.md)
 - [CorporationsCorporationIdTitlesGetInner](docs/CorporationsCorporationIdTitlesGetInner.md)
 - [CorporationsCorporationIdWalletsDivisionJournalGetInner](docs/CorporationsCorporationIdWalletsDivisionJournalGetInner.md)
 - [CorporationsCorporationIdWalletsDivisionTransactionsGetInner](docs/CorporationsCorporationIdWalletsDivisionTransactionsGetInner.md)
 - [CorporationsCorporationIdWalletsGetInner](docs/CorporationsCorporationIdWalletsGetInner.md)
 - [CorporationsDetail](docs/CorporationsDetail.md)
 - [CorporationsFreelanceJobsListing](docs/CorporationsFreelanceJobsListing.md)
 - [CorporationsFreelanceJobsParticipants](docs/CorporationsFreelanceJobsParticipants.md)
 - [CorporationsFreelanceJobsParticipantsParticipant](docs/CorporationsFreelanceJobsParticipantsParticipant.md)
 - [CorporationsProjectsContribution](docs/CorporationsProjectsContribution.md)
 - [CorporationsProjectsContributors](docs/CorporationsProjectsContributors.md)
 - [CorporationsProjectsContributorsContributor](docs/CorporationsProjectsContributorsContributor.md)
 - [CorporationsProjectsDetail](docs/CorporationsProjectsDetail.md)
 - [CorporationsProjectsDetailConfiguration](docs/CorporationsProjectsDetailConfiguration.md)
 - [CorporationsProjectsDetailConfigurationcapturefwcomplex](docs/CorporationsProjectsDetailConfigurationcapturefwcomplex.md)
 - [CorporationsProjectsDetailConfigurationcapturefwcomplexLocationsInner](docs/CorporationsProjectsDetailConfigurationcapturefwcomplexLocationsInner.md)
 - [CorporationsProjectsDetailConfigurationdamageship](docs/CorporationsProjectsDetailConfigurationdamageship.md)
 - [CorporationsProjectsDetailConfigurationdamageshipIdentitiesInner](docs/CorporationsProjectsDetailConfigurationdamageshipIdentitiesInner.md)
 - [CorporationsProjectsDetailConfigurationdamageshipShipsInner](docs/CorporationsProjectsDetailConfigurationdamageshipShipsInner.md)
 - [CorporationsProjectsDetailConfigurationdefendfwcomplex](docs/CorporationsProjectsDetailConfigurationdefendfwcomplex.md)
 - [CorporationsProjectsDetailConfigurationdeliveritem](docs/CorporationsProjectsDetailConfigurationdeliveritem.md)
 - [CorporationsProjectsDetailConfigurationdeliveritemDockingLocationsInner](docs/CorporationsProjectsDetailConfigurationdeliveritemDockingLocationsInner.md)
 - [CorporationsProjectsDetailConfigurationdeliveritemItemsInner](docs/CorporationsProjectsDetailConfigurationdeliveritemItemsInner.md)
 - [CorporationsProjectsDetailConfigurationdestroynpc](docs/CorporationsProjectsDetailConfigurationdestroynpc.md)
 - [CorporationsProjectsDetailConfigurationdestroyship](docs/CorporationsProjectsDetailConfigurationdestroyship.md)
 - [CorporationsProjectsDetailConfigurationearnloyaltypoints](docs/CorporationsProjectsDetailConfigurationearnloyaltypoints.md)
 - [CorporationsProjectsDetailConfigurationlostship](docs/CorporationsProjectsDetailConfigurationlostship.md)
 - [CorporationsProjectsDetailConfigurationmanufactureitem](docs/CorporationsProjectsDetailConfigurationmanufactureitem.md)
 - [CorporationsProjectsDetailConfigurationmatcherarchetype](docs/CorporationsProjectsDetailConfigurationmatcherarchetype.md)
 - [CorporationsProjectsDetailConfigurationmatchercorporation](docs/CorporationsProjectsDetailConfigurationmatchercorporation.md)
 - [CorporationsProjectsDetailConfigurationmatcherfaction](docs/CorporationsProjectsDetailConfigurationmatcherfaction.md)
 - [CorporationsProjectsDetailConfigurationmatchersignature](docs/CorporationsProjectsDetailConfigurationmatchersignature.md)
 - [CorporationsProjectsDetailConfigurationminematerial](docs/CorporationsProjectsDetailConfigurationminematerial.md)
 - [CorporationsProjectsDetailConfigurationminematerialMaterialsInner](docs/CorporationsProjectsDetailConfigurationminematerialMaterialsInner.md)
 - [CorporationsProjectsDetailConfigurationremoteboostshield](docs/CorporationsProjectsDetailConfigurationremoteboostshield.md)
 - [CorporationsProjectsDetailConfigurationremoterepairarmor](docs/CorporationsProjectsDetailConfigurationremoterepairarmor.md)
 - [CorporationsProjectsDetailConfigurationsalvagewreck](docs/CorporationsProjectsDetailConfigurationsalvagewreck.md)
 - [CorporationsProjectsDetailConfigurationscansignature](docs/CorporationsProjectsDetailConfigurationscansignature.md)
 - [CorporationsProjectsDetailConfigurationshipinsurance](docs/CorporationsProjectsDetailConfigurationshipinsurance.md)
 - [CorporationsProjectsDetailConfigurationunknown](docs/CorporationsProjectsDetailConfigurationunknown.md)
 - [CorporationsProjectsDetailContribution](docs/CorporationsProjectsDetailContribution.md)
 - [CorporationsProjectsDetailCreator](docs/CorporationsProjectsDetailCreator.md)
 - [CorporationsProjectsDetailDetails](docs/CorporationsProjectsDetailDetails.md)
 - [CorporationsProjectsDetailProgress](docs/CorporationsProjectsDetailProgress.md)
 - [CorporationsProjectsDetailProject](docs/CorporationsProjectsDetailProject.md)
 - [CorporationsProjectsDetailReward](docs/CorporationsProjectsDetailReward.md)
 - [CorporationsProjectsListing](docs/CorporationsProjectsListing.md)
 - [Cursor](docs/Cursor.md)
 - [DamageShip](docs/DamageShip.md)
 - [DefendFwComplex](docs/DefendFwComplex.md)
 - [DeliverItem](docs/DeliverItem.md)
 - [DestroyNpc](docs/DestroyNpc.md)
 - [DestroyShip](docs/DestroyShip.md)
 - [DogmaAttributesAttributeIdGet](docs/DogmaAttributesAttributeIdGet.md)
 - [DogmaDynamicItemsTypeIdItemIdGet](docs/DogmaDynamicItemsTypeIdItemIdGet.md)
 - [DogmaDynamicItemsTypeIdItemIdGetDogmaAttributesInner](docs/DogmaDynamicItemsTypeIdItemIdGetDogmaAttributesInner.md)
 - [DogmaDynamicItemsTypeIdItemIdGetDogmaEffectsInner](docs/DogmaDynamicItemsTypeIdItemIdGetDogmaEffectsInner.md)
 - [DogmaEffectsEffectIdGet](docs/DogmaEffectsEffectIdGet.md)
 - [DogmaEffectsEffectIdGetModifiersInner](docs/DogmaEffectsEffectIdGetModifiersInner.md)
 - [EarnLoyaltyPoint](docs/EarnLoyaltyPoint.md)
 - [ErrorDetail](docs/ErrorDetail.md)
 - [FactionId](docs/FactionId.md)
 - [FleetsFleetIdGet](docs/FleetsFleetIdGet.md)
 - [FleetsFleetIdMembersGetInner](docs/FleetsFleetIdMembersGetInner.md)
 - [FleetsFleetIdWingsGetInner](docs/FleetsFleetIdWingsGetInner.md)
 - [FleetsFleetIdWingsGetInnerSquadsInner](docs/FleetsFleetIdWingsGetInnerSquadsInner.md)
 - [FleetsFleetIdWingsPost](docs/FleetsFleetIdWingsPost.md)
 - [FleetsFleetIdWingsWingIdSquadsPost](docs/FleetsFleetIdWingsWingIdSquadsPost.md)
 - [FreelanceJobsDetail](docs/FreelanceJobsDetail.md)
 - [FreelanceJobsDetailAccessandvisibility](docs/FreelanceJobsDetailAccessandvisibility.md)
 - [FreelanceJobsDetailBroadcastlocations](docs/FreelanceJobsDetailBroadcastlocations.md)
 - [FreelanceJobsDetailConfiguration](docs/FreelanceJobsDetailConfiguration.md)
 - [FreelanceJobsDetailConfigurationParametersValue](docs/FreelanceJobsDetailConfigurationParametersValue.md)
 - [FreelanceJobsDetailContribution](docs/FreelanceJobsDetailContribution.md)
 - [FreelanceJobsDetailCreator](docs/FreelanceJobsDetailCreator.md)
 - [FreelanceJobsDetailCreatorcharacter](docs/FreelanceJobsDetailCreatorcharacter.md)
 - [FreelanceJobsDetailCreatorcorporation](docs/FreelanceJobsDetailCreatorcorporation.md)
 - [FreelanceJobsDetailDetails](docs/FreelanceJobsDetailDetails.md)
 - [FreelanceJobsDetailFreelancejob](docs/FreelanceJobsDetailFreelancejob.md)
 - [FreelanceJobsDetailParameterboolean](docs/FreelanceJobsDetailParameterboolean.md)
 - [FreelanceJobsDetailParametercorporationitemdelivery](docs/FreelanceJobsDetailParametercorporationitemdelivery.md)
 - [FreelanceJobsDetailParametermatcher](docs/FreelanceJobsDetailParametermatcher.md)
 - [FreelanceJobsDetailParametermatchervalue](docs/FreelanceJobsDetailParametermatchervalue.md)
 - [FreelanceJobsDetailParameteroptions](docs/FreelanceJobsDetailParameteroptions.md)
 - [FreelanceJobsDetailProgress](docs/FreelanceJobsDetailProgress.md)
 - [FreelanceJobsDetailRestrictions](docs/FreelanceJobsDetailRestrictions.md)
 - [FreelanceJobsDetailReward](docs/FreelanceJobsDetailReward.md)
 - [FreelanceJobsListing](docs/FreelanceJobsListing.md)
 - [FwLeaderboardsCharactersGet](docs/FwLeaderboardsCharactersGet.md)
 - [FwLeaderboardsCharactersGetKills](docs/FwLeaderboardsCharactersGetKills.md)
 - [FwLeaderboardsCharactersGetKillsActiveTotalInner](docs/FwLeaderboardsCharactersGetKillsActiveTotalInner.md)
 - [FwLeaderboardsCharactersGetKillsLastWeekInner](docs/FwLeaderboardsCharactersGetKillsLastWeekInner.md)
 - [FwLeaderboardsCharactersGetKillsYesterdayInner](docs/FwLeaderboardsCharactersGetKillsYesterdayInner.md)
 - [FwLeaderboardsCharactersGetVictoryPoints](docs/FwLeaderboardsCharactersGetVictoryPoints.md)
 - [FwLeaderboardsCharactersGetVictoryPointsActiveTotalInner](docs/FwLeaderboardsCharactersGetVictoryPointsActiveTotalInner.md)
 - [FwLeaderboardsCharactersGetVictoryPointsLastWeekInner](docs/FwLeaderboardsCharactersGetVictoryPointsLastWeekInner.md)
 - [FwLeaderboardsCharactersGetVictoryPointsYesterdayInner](docs/FwLeaderboardsCharactersGetVictoryPointsYesterdayInner.md)
 - [FwLeaderboardsCorporationsGet](docs/FwLeaderboardsCorporationsGet.md)
 - [FwLeaderboardsCorporationsGetKills](docs/FwLeaderboardsCorporationsGetKills.md)
 - [FwLeaderboardsCorporationsGetKillsActiveTotalInner](docs/FwLeaderboardsCorporationsGetKillsActiveTotalInner.md)
 - [FwLeaderboardsCorporationsGetKillsLastWeekInner](docs/FwLeaderboardsCorporationsGetKillsLastWeekInner.md)
 - [FwLeaderboardsCorporationsGetKillsYesterdayInner](docs/FwLeaderboardsCorporationsGetKillsYesterdayInner.md)
 - [FwLeaderboardsCorporationsGetVictoryPoints](docs/FwLeaderboardsCorporationsGetVictoryPoints.md)
 - [FwLeaderboardsCorporationsGetVictoryPointsActiveTotalInner](docs/FwLeaderboardsCorporationsGetVictoryPointsActiveTotalInner.md)
 - [FwLeaderboardsCorporationsGetVictoryPointsLastWeekInner](docs/FwLeaderboardsCorporationsGetVictoryPointsLastWeekInner.md)
 - [FwLeaderboardsCorporationsGetVictoryPointsYesterdayInner](docs/FwLeaderboardsCorporationsGetVictoryPointsYesterdayInner.md)
 - [FwLeaderboardsGet](docs/FwLeaderboardsGet.md)
 - [FwLeaderboardsGetKills](docs/FwLeaderboardsGetKills.md)
 - [FwLeaderboardsGetKillsActiveTotalInner](docs/FwLeaderboardsGetKillsActiveTotalInner.md)
 - [FwLeaderboardsGetKillsLastWeekInner](docs/FwLeaderboardsGetKillsLastWeekInner.md)
 - [FwLeaderboardsGetKillsYesterdayInner](docs/FwLeaderboardsGetKillsYesterdayInner.md)
 - [FwLeaderboardsGetVictoryPoints](docs/FwLeaderboardsGetVictoryPoints.md)
 - [FwLeaderboardsGetVictoryPointsActiveTotalInner](docs/FwLeaderboardsGetVictoryPointsActiveTotalInner.md)
 - [FwLeaderboardsGetVictoryPointsLastWeekInner](docs/FwLeaderboardsGetVictoryPointsLastWeekInner.md)
 - [FwLeaderboardsGetVictoryPointsYesterdayInner](docs/FwLeaderboardsGetVictoryPointsYesterdayInner.md)
 - [FwStatsGetInner](docs/FwStatsGetInner.md)
 - [FwStatsGetInnerKills](docs/FwStatsGetInnerKills.md)
 - [FwStatsGetInnerVictoryPoints](docs/FwStatsGetInnerVictoryPoints.md)
 - [FwSystemsGetInner](docs/FwSystemsGetInner.md)
 - [FwWarsGetInner](docs/FwWarsGetInner.md)
 - [GroupId](docs/GroupId.md)
 - [GroupId1](docs/GroupId1.md)
 - [GroupId2](docs/GroupId2.md)
 - [IncursionsGetInner](docs/IncursionsGetInner.md)
 - [IndustryFacilitiesGetInner](docs/IndustryFacilitiesGetInner.md)
 - [IndustrySystemsGetInner](docs/IndustrySystemsGetInner.md)
 - [IndustrySystemsGetInnerCostIndicesInner](docs/IndustrySystemsGetInnerCostIndicesInner.md)
 - [InsurancePricesGetInner](docs/InsurancePricesGetInner.md)
 - [InsurancePricesGetInnerLevelsInner](docs/InsurancePricesGetInnerLevelsInner.md)
 - [KillmailsKillmailIdKillmailHashGet](docs/KillmailsKillmailIdKillmailHashGet.md)
 - [KillmailsKillmailIdKillmailHashGetAttackersInner](docs/KillmailsKillmailIdKillmailHashGetAttackersInner.md)
 - [KillmailsKillmailIdKillmailHashGetVictim](docs/KillmailsKillmailIdKillmailHashGetVictim.md)
 - [KillmailsKillmailIdKillmailHashGetVictimItemsInner](docs/KillmailsKillmailIdKillmailHashGetVictimItemsInner.md)
 - [KillmailsKillmailIdKillmailHashGetVictimItemsInnerItemsInner](docs/KillmailsKillmailIdKillmailHashGetVictimItemsInnerItemsInner.md)
 - [KillmailsKillmailIdKillmailHashGetVictimPosition](docs/KillmailsKillmailIdKillmailHashGetVictimPosition.md)
 - [LostShip](docs/LostShip.md)
 - [LoyaltyStoresCorporationIdOffersGetInner](docs/LoyaltyStoresCorporationIdOffersGetInner.md)
 - [LoyaltyStoresCorporationIdOffersGetInnerRequiredItemsInner](docs/LoyaltyStoresCorporationIdOffersGetInnerRequiredItemsInner.md)
 - [Manual](docs/Manual.md)
 - [ManufactureItem](docs/ManufactureItem.md)
 - [MarketsGroupsMarketGroupIdGet](docs/MarketsGroupsMarketGroupIdGet.md)
 - [MarketsPricesGetInner](docs/MarketsPricesGetInner.md)
 - [MarketsRegionIdHistoryGetInner](docs/MarketsRegionIdHistoryGetInner.md)
 - [MarketsRegionIdOrdersGetInner](docs/MarketsRegionIdOrdersGetInner.md)
 - [MarketsStructuresStructureIdGetInner](docs/MarketsStructuresStructureIdGetInner.md)
 - [Matcher](docs/Matcher.md)
 - [MetaChangelog](docs/MetaChangelog.md)
 - [MetaChangelogEntry](docs/MetaChangelogEntry.md)
 - [MetaCompatibilityDates](docs/MetaCompatibilityDates.md)
 - [MetaStatus](docs/MetaStatus.md)
 - [MetaStatusRoutestatus](docs/MetaStatusRoutestatus.md)
 - [MineMaterial](docs/MineMaterial.md)
 - [ModelBoolean](docs/ModelBoolean.md)
 - [ModelError](docs/ModelError.md)
 - [Options](docs/Options.md)
 - [PostCharactersCharacterIdFittingsRequest](docs/PostCharactersCharacterIdFittingsRequest.md)
 - [PostCharactersCharacterIdFittingsRequestItemsInner](docs/PostCharactersCharacterIdFittingsRequestItemsInner.md)
 - [PostCharactersCharacterIdMailLabelsRequest](docs/PostCharactersCharacterIdMailLabelsRequest.md)
 - [PostCharactersCharacterIdMailRequest](docs/PostCharactersCharacterIdMailRequest.md)
 - [PostCharactersCharacterIdMailRequestRecipientsInner](docs/PostCharactersCharacterIdMailRequestRecipientsInner.md)
 - [PostFleetsFleetIdMembersRequest](docs/PostFleetsFleetIdMembersRequest.md)
 - [PostUiOpenwindowNewmailRequest](docs/PostUiOpenwindowNewmailRequest.md)
 - [PutCharactersCharacterIdCalendarEventIdRequest](docs/PutCharactersCharacterIdCalendarEventIdRequest.md)
 - [PutCharactersCharacterIdMailMailIdRequest](docs/PutCharactersCharacterIdMailMailIdRequest.md)
 - [PutFleetsFleetIdMembersMemberIdRequest](docs/PutFleetsFleetIdMembersMemberIdRequest.md)
 - [PutFleetsFleetIdRequest](docs/PutFleetsFleetIdRequest.md)
 - [PutFleetsFleetIdSquadsSquadIdRequest](docs/PutFleetsFleetIdSquadsSquadIdRequest.md)
 - [RegionId](docs/RegionId.md)
 - [RemoteBoostShield](docs/RemoteBoostShield.md)
 - [RemoteRepairArmor](docs/RemoteRepairArmor.md)
 - [Route](docs/Route.md)
 - [RouteConnection](docs/RouteConnection.md)
 - [RouteRequestBody](docs/RouteRequestBody.md)
 - [SalvageWreck](docs/SalvageWreck.md)
 - [ScanSignature](docs/ScanSignature.md)
 - [ShipInsurance](docs/ShipInsurance.md)
 - [SolarSystemId](docs/SolarSystemId.md)
 - [SovereigntyCampaignsGetInner](docs/SovereigntyCampaignsGetInner.md)
 - [SovereigntyCampaignsGetInnerParticipantsInner](docs/SovereigntyCampaignsGetInnerParticipantsInner.md)
 - [SovereigntyMapGetInner](docs/SovereigntyMapGetInner.md)
 - [SovereigntyStructuresGetInner](docs/SovereigntyStructuresGetInner.md)
 - [StationId](docs/StationId.md)
 - [StatusGet](docs/StatusGet.md)
 - [StructureId](docs/StructureId.md)
 - [TypeId](docs/TypeId.md)
 - [TypeId1](docs/TypeId1.md)
 - [TypeId2](docs/TypeId2.md)
 - [UniverseAncestriesGetInner](docs/UniverseAncestriesGetInner.md)
 - [UniverseAsteroidBeltsAsteroidBeltIdGet](docs/UniverseAsteroidBeltsAsteroidBeltIdGet.md)
 - [UniverseBloodlinesGetInner](docs/UniverseBloodlinesGetInner.md)
 - [UniverseCategoriesCategoryIdGet](docs/UniverseCategoriesCategoryIdGet.md)
 - [UniverseConstellationsConstellationIdGet](docs/UniverseConstellationsConstellationIdGet.md)
 - [UniverseFactionsGetInner](docs/UniverseFactionsGetInner.md)
 - [UniverseGraphicsGraphicIdGet](docs/UniverseGraphicsGraphicIdGet.md)
 - [UniverseGroupsGroupIdGet](docs/UniverseGroupsGroupIdGet.md)
 - [UniverseIdsPost](docs/UniverseIdsPost.md)
 - [UniverseIdsPostAgentsInner](docs/UniverseIdsPostAgentsInner.md)
 - [UniverseIdsPostAlliancesInner](docs/UniverseIdsPostAlliancesInner.md)
 - [UniverseIdsPostCharactersInner](docs/UniverseIdsPostCharactersInner.md)
 - [UniverseIdsPostConstellationsInner](docs/UniverseIdsPostConstellationsInner.md)
 - [UniverseIdsPostCorporationsInner](docs/UniverseIdsPostCorporationsInner.md)
 - [UniverseIdsPostFactionsInner](docs/UniverseIdsPostFactionsInner.md)
 - [UniverseIdsPostInventoryTypesInner](docs/UniverseIdsPostInventoryTypesInner.md)
 - [UniverseIdsPostRegionsInner](docs/UniverseIdsPostRegionsInner.md)
 - [UniverseIdsPostStationsInner](docs/UniverseIdsPostStationsInner.md)
 - [UniverseIdsPostSystemsInner](docs/UniverseIdsPostSystemsInner.md)
 - [UniverseMoonsMoonIdGet](docs/UniverseMoonsMoonIdGet.md)
 - [UniverseNamesPostInner](docs/UniverseNamesPostInner.md)
 - [UniversePlanetsPlanetIdGet](docs/UniversePlanetsPlanetIdGet.md)
 - [UniverseRacesGetInner](docs/UniverseRacesGetInner.md)
 - [UniverseRegionsRegionIdGet](docs/UniverseRegionsRegionIdGet.md)
 - [UniverseSchematicsSchematicIdGet](docs/UniverseSchematicsSchematicIdGet.md)
 - [UniverseStargatesStargateIdGet](docs/UniverseStargatesStargateIdGet.md)
 - [UniverseStargatesStargateIdGetDestination](docs/UniverseStargatesStargateIdGetDestination.md)
 - [UniverseStarsStarIdGet](docs/UniverseStarsStarIdGet.md)
 - [UniverseStationsStationIdGet](docs/UniverseStationsStationIdGet.md)
 - [UniverseStructuresStructureIdGet](docs/UniverseStructuresStructureIdGet.md)
 - [UniverseStructuresStructureIdGetPosition](docs/UniverseStructuresStructureIdGetPosition.md)
 - [UniverseSystemJumpsGetInner](docs/UniverseSystemJumpsGetInner.md)
 - [UniverseSystemKillsGetInner](docs/UniverseSystemKillsGetInner.md)
 - [UniverseSystemsSystemIdGet](docs/UniverseSystemsSystemIdGet.md)
 - [UniverseSystemsSystemIdGetPlanetsInner](docs/UniverseSystemsSystemIdGetPlanetsInner.md)
 - [UniverseTypesTypeIdGet](docs/UniverseTypesTypeIdGet.md)
 - [Unknown](docs/Unknown.md)
 - [WarsWarIdGet](docs/WarsWarIdGet.md)
 - [WarsWarIdGetAggressor](docs/WarsWarIdGetAggressor.md)
 - [WarsWarIdGetAlliesInner](docs/WarsWarIdGetAlliesInner.md)
 - [WarsWarIdGetDefender](docs/WarsWarIdGetDefender.md)


<a id="documentation-for-authorization"></a>
## Documentation For Authorization


Authentication schemes defined for the API:
<a id="OAuth2"></a>
### OAuth2

- **Type**: OAuth
- **Flow**: accessCode
- **Authorization URL**: https://login.eveonline.com/v2/oauth/authorize
- **Scopes**: 
 - **esi-access.read_lists.v1**: esi-access.read_lists.v1
 - **esi-activities.read_character.v1**: esi-activities.read_character.v1
 - **esi-alliances.read_contacts.v1**: esi-alliances.read_contacts.v1
 - **esi-assets.read_assets.v1**: esi-assets.read_assets.v1
 - **esi-assets.read_corporation_assets.v1**: esi-assets.read_corporation_assets.v1
 - **esi-calendar.read_calendar_events.v1**: esi-calendar.read_calendar_events.v1
 - **esi-calendar.respond_calendar_events.v1**: esi-calendar.respond_calendar_events.v1
 - **esi-characters.read_agents_research.v1**: esi-characters.read_agents_research.v1
 - **esi-characters.read_blueprints.v1**: esi-characters.read_blueprints.v1
 - **esi-characters.read_contacts.v1**: esi-characters.read_contacts.v1
 - **esi-characters.read_corporation_roles.v1**: esi-characters.read_corporation_roles.v1
 - **esi-characters.read_fatigue.v1**: esi-characters.read_fatigue.v1
 - **esi-characters.read_freelance_jobs.v1**: esi-characters.read_freelance_jobs.v1
 - **esi-characters.read_fw_stats.v1**: esi-characters.read_fw_stats.v1
 - **esi-characters.read_loyalty.v1**: esi-characters.read_loyalty.v1
 - **esi-characters.read_medals.v1**: esi-characters.read_medals.v1
 - **esi-characters.read_notifications.v1**: esi-characters.read_notifications.v1
 - **esi-characters.read_standings.v1**: esi-characters.read_standings.v1
 - **esi-characters.read_titles.v1**: esi-characters.read_titles.v1
 - **esi-characters.write_contacts.v1**: esi-characters.write_contacts.v1
 - **esi-clones.read_clones.v1**: esi-clones.read_clones.v1
 - **esi-clones.read_implants.v1**: esi-clones.read_implants.v1
 - **esi-contracts.read_character_contracts.v1**: esi-contracts.read_character_contracts.v1
 - **esi-contracts.read_corporation_contracts.v1**: esi-contracts.read_corporation_contracts.v1
 - **esi-corporations.read_blueprints.v1**: esi-corporations.read_blueprints.v1
 - **esi-corporations.read_contacts.v1**: esi-corporations.read_contacts.v1
 - **esi-corporations.read_container_logs.v1**: esi-corporations.read_container_logs.v1
 - **esi-corporations.read_corporation_membership.v1**: esi-corporations.read_corporation_membership.v1
 - **esi-corporations.read_divisions.v1**: esi-corporations.read_divisions.v1
 - **esi-corporations.read_facilities.v1**: esi-corporations.read_facilities.v1
 - **esi-corporations.read_freelance_jobs.v1**: esi-corporations.read_freelance_jobs.v1
 - **esi-corporations.read_fw_stats.v1**: esi-corporations.read_fw_stats.v1
 - **esi-corporations.read_medals.v1**: esi-corporations.read_medals.v1
 - **esi-corporations.read_projects.v1**: esi-corporations.read_projects.v1
 - **esi-corporations.read_standings.v1**: esi-corporations.read_standings.v1
 - **esi-corporations.read_starbases.v1**: esi-corporations.read_starbases.v1
 - **esi-corporations.read_structures.v1**: esi-corporations.read_structures.v1
 - **esi-corporations.read_titles.v1**: esi-corporations.read_titles.v1
 - **esi-corporations.track_members.v1**: esi-corporations.track_members.v1
 - **esi-fittings.read_fittings.v1**: esi-fittings.read_fittings.v1
 - **esi-fittings.write_fittings.v1**: esi-fittings.write_fittings.v1
 - **esi-fleets.read_fleet.v1**: esi-fleets.read_fleet.v1
 - **esi-fleets.write_fleet.v1**: esi-fleets.write_fleet.v1
 - **esi-industry.read_character_jobs.v1**: esi-industry.read_character_jobs.v1
 - **esi-industry.read_character_mining.v1**: esi-industry.read_character_mining.v1
 - **esi-industry.read_corporation_jobs.v1**: esi-industry.read_corporation_jobs.v1
 - **esi-industry.read_corporation_mining.v1**: esi-industry.read_corporation_mining.v1
 - **esi-killmails.read_corporation_killmails.v1**: esi-killmails.read_corporation_killmails.v1
 - **esi-killmails.read_killmails.v1**: esi-killmails.read_killmails.v1
 - **esi-location.read_location.v1**: esi-location.read_location.v1
 - **esi-location.read_online.v1**: esi-location.read_online.v1
 - **esi-location.read_ship_type.v1**: esi-location.read_ship_type.v1
 - **esi-mail.organize_mail.v1**: esi-mail.organize_mail.v1
 - **esi-mail.read_mail.v1**: esi-mail.read_mail.v1
 - **esi-mail.send_mail.v1**: esi-mail.send_mail.v1
 - **esi-markets.read_character_orders.v1**: esi-markets.read_character_orders.v1
 - **esi-markets.read_corporation_orders.v1**: esi-markets.read_corporation_orders.v1
 - **esi-markets.structure_markets.v1**: esi-markets.structure_markets.v1
 - **esi-planets.manage_planets.v1**: esi-planets.manage_planets.v1
 - **esi-planets.read_customs_offices.v1**: esi-planets.read_customs_offices.v1
 - **esi-search.search_structures.v1**: esi-search.search_structures.v1
 - **esi-skills.read_skillqueue.v1**: esi-skills.read_skillqueue.v1
 - **esi-skills.read_skills.v1**: esi-skills.read_skills.v1
 - **esi-structures.read_character.v1**: esi-structures.read_character.v1
 - **esi-structures.read_corporation.v1**: esi-structures.read_corporation.v1
 - **esi-ui.open_window.v1**: esi-ui.open_window.v1
 - **esi-ui.write_waypoint.v1**: esi-ui.write_waypoint.v1
 - **esi-universe.read_structures.v1**: esi-universe.read_structures.v1
 - **esi-wallet.read_character_wallet.v1**: esi-wallet.read_character_wallet.v1
 - **esi-wallet.read_corporation_wallets.v1**: esi-wallet.read_corporation_wallets.v1

