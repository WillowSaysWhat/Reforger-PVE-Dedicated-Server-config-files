# Reforger PVE Dedicated Server config files

Congratulations, you are about to make your own dedicated Arma Reforger PVE server.

This README hold the different code you will need to fill out the different .json files.

* [ConflictPVEvanilla.json](#conflictpvevanillajson)

## NOTE

This is Gramps Conflict PVER emixed Vanilla 2.0 gamemode. it is a mod found in the workshop. The mode id number and mod location is `{6DD58790690E9D29}Missions/ConflictPVERemixedVanilla2_US.conf`
This is important for the scenarioId section in the json. 

## Most important
Check the `version` of each mod. It is continuously changing, so your mods will quickly become outdated. The `version` on the mods below are going to be very old, check them against the ones in your game.

## conflictPVEvanilla.json

```json
{
	"bindAddress": "your pc IP.",
	"bindPort": 2001,
	"publicAddress": "your public IP.",
	"publicPort": 2001,
	"a2s": {
		"address": "your public IP again.",
		"port": 17777
	},
	"rcon": {
		"address": "your public IP again, again.",
		"port": 19999,
		"password": "admin password",
		"permission": "monitor",
		"blacklist": [],
		"whitelist": []
	},
	"game": {
		"name": "Relaxed ConflictPVE Remixed Vanilla Mod ",
		"password": "",
		"passwordAdmin": "admin123",
		"admins" : ["your steam account number", "firends steam account number" ],
		"scenarioId": "{6DD58790690E9D29}Missions/ConflictPVERemixedVanilla2_US.conf",
		"maxPlayers": 30,
		"visible": true,
		"crossPlatform": true,
   		 "supportedPlatforms": [
			"PLATFORM_PC",
      			"PLATFORM_XBL"
		],
		"gameProperties": {
			"serverMaxViewDistance": 2500,
			"serverMinGrassDistance": 50,
			"networkViewDistance": 1000,
			"disableThirdPerson": false,
			"fastValidation": true,
			"battlEye": true,
			"VONDisableUI": false,
			"VONDisableDirectSpeechUI": false,
			"VONCanTransmitCrossFaction": false
		},
		"mods": [
    {
        "modId": "5DBD560C5148E1DA",
        "name": "ACE Carrying",
        "version": "1.1.2"
    },
    {
        "modId": "5EB744C5F42E0800",
        "name": "ACE Chopping",
        "version": "1.1.5"
    },
    {
        "modId": "60C4C12DAE90727B",
        "name": "ACE Medical",
        "version": "1.1.0"
    },
    {
        "modId": "606C369BAC3F6CC3",
        "name": "ACE Finger",
        "version": "1.1.0"
    },
    {
        "modId": "60EAEA0389DB3CC2",
        "name": "ACE Trenches",
        "version": "1.1.0"
    },
    {
        "modId": "60C53A9372ED3964",
        "name": "ACE Compass",
        "version": "1.1.0"
    },
    {
        "modId": "60C4CE4888FF4621",
        "name": "ACE Core",
        "version": "1.1.2"
    },
    {
        "modId": "606B100247F5C709",
        "name": "Bacon Loadout Editor",
        "version": "1.2.8"
    },
    {
        "modId": "62113AA293414DB9",
        "name": "Bandage Patch",
        "version": "1.0.4"
    },
    {
        "modId": "5F1EE615E7AE3106",
        "name": "BGONE",
        "version": "1.1.25"
    },
    {
        "modId": "597C0CF3A7AA8A99",
        "name": "BetterSounds 3.6",
        "version": "3.6.0"
    },
    {
        "modId": "5B0D1E4380971EBD",
        "name": "COALITION Squad Interface",
        "version": "1.6.11"
    },
    {
        "modId": "5EE969D5E6047BC4",
        "name": "CTI_ScoringSystem",
        "version": "1.0.9"
    },
    {
        "modId": "5C8AD2767D87626B",
        "name": "Disable Friendly Fire",
        "version": "1.0.3"
    },
    {
        "modId": "605E3A755084A345",
        "name": "HumveeVariants4Conflict",
        "version": "1.0.5"
    },
    {
        "modId": "5D9ECAD071E9ECBC",
        "name": "HMMWV  VARIANTS PACK",
        "version": "1.0.37"
    },
    {
        "modId": "6088A3044B7ECBFD",
        "name": "Keep Gun When Uncon",
        "version": "1.0.1"
    },
    {
        "modId": "628729E87E79DA7F",
        "name": "LinearConflictPVE",
        "version": "1.0.6"
    },
    {
        "modId": "5AF6E0F075D79473",
        "name": "M249 Scope Rails",
        "version": "1.0.10"
    },
    {
        "modId": "5AB890B71D748750",
        "name": "M4 Block II and URG-I",
        "version": "1.2.7"
    },
    {
        "modId": "59A30ACC02650E71",
        "name": "Night Vision System",
        "version": "1.1.26"
    },
    {
        "modId": "613629A17AFFEBFE",
        "name": "NoAILivingQuarters",
        "version": "1.0.1"
    },
    {
        "modId": "5E92F5A4A1B75A75",
        "name": "Player Map Markers",
        "version": "1.1.1"
    },
    {
        "modId": "5AAAC70D754245DD",
        "name": "Server Admin Tools",
        "version": "1.0.61"
    },
    {
        "modId": "5E389BB9F58B79A6",
        "name": "SpaceCore",
        "version": "1.2.15"
    },
    {
        "modId": "62651AA564157FE5",
        "name": "SlowerXPGain4Conflict",
        "version": "0.9.1"
    },
    {
        "modId": "61661E2AF558E398",
        "name": "Springfield M1A Pack",
        "version": "1.0.6"
    },
    {
        "modId": "5CF0C3158AB2337E",
        "name": "Task Force Mattock Uniforms",
        "version": "1.0.2"
    },
    {
        "modId": "5B3ED33ADA805340",
        "name": "Task Force Mattock Weapons",
        "version": "2.0.6"
    },
    {
        "modId": "5D550926D43F1409",
        "name": "Tactical Flava",
        "version": "0.1.57"
    },
    {
        "modId": "5CAB06A845A6DC18",
        "name": "Units Map Markers",
        "version": "1.0.14"
    },
    {
        "modId": "5E8E12AF1EF94EE2",
        "name": "US Armed Forces",
        "version": "1.0.8"
    },
    {
        "modId": "5D0551624969C92E",
        "name": "Zeliks Character",
        "version": "1.1.13"
    }
]
 
	}
	
	
}


```
 
# 
