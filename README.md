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
    "bindAddress": "xxx.xxx.xxx.xxx",
    "bindPort": 2427,
    "publicAddress": "xxx.xxx.xxx.xxx",
    "publicPort": 2427,
    "a2s": {
      "address": "xxx.xxx.xxx.xxx",
      "port": 3427
    },
    "game": {
      "name": "[ENG-EU] WillowSaysWhat | Test Server",
      "password": "xxxxx",
      "passwordAdmin": "admin123",
      "admins": [
        "c95e89f2-1aa9-4f72-927a-12363819fe56",
        "48666091-2220-47cf-a6a6-b1b08828174e",
        "3bc98c13-a402-4b04-8a73-5a73cb0ac170"
        
      ],
      "scenarioId": "{6DD58790690E9D29}Missions/ConflictPVERemixedVanilla2_US.conf",
      "maxPlayers": 10,
      "visible": true,
      "crossPlatform": true,
      "supportedPlatforms": [
        "PLATFORM_PC",
        "PLATFORM_XBL",
        "PLATFORM_PSN"
      ],
      "gameProperties": {
        "serverMaxViewDistance": 1600,
        "serverMinGrassDistance": 50,
        "networkViewDistance": 1500,
        "disableThirdPerson": false,
        "fastValidation": true,
        "battlEye": true,
        "VONDisableUI": false,
        "VONDisableDirectSpeechUI": false,
        "VONCanTransmitCrossFaction": false,
        "missionHeader": {
          "m_sName": "Test PVE",
          "m_eEditableGameFlags": 6,
          "m_eDefaultGameFlags": 6,
          "other": "values"
        }
      },
      "modsRequiredByDefault": true,
      "mods": [
        {
            "modId": "6303360DA719E832",
            "name": "WCS_AH-64D"
        },
        {
            "modId": "64610AFB74AA9842",
            "name": "WCS_Core"
        },
        {
            "modId": "644B042109700804",
            "name": "Enhanced Maps"
        },
        {
            "modId": "606B100247F5C709",
            "name": "Bacon Loadout Editor"
        },
        {
            "modId": "5B0D1E4380971EBD",
            "name": "COALITION Squad Interface"
        },
        {
            "modId": "5964E0B3BB7410CE",
            "name": "Game Master Enhanced"
        },
        {
            "modId": "628729E87E79DA7F",
            "name": "LinearConflictPVE"
        },
        {
            "modId": "595F2BF2F44836FB",
            "name": "RHS - Status Quo",
            "version": "0.12.4487"
        },
        {
            "modId": "64900A5A31F5DCB5",
            "name": "MRZR",
            "version": "1.0.5"
        },
        {
            "modId": "64D0C6A0FA2FD412",
            "name": "WillowBoard",
            "version": "1.0.9"
        },
        {
            "modId": "6518C209A48D4991",
            "name": "Medevac Huey",
            "version": "0.5.4"
        },
        {
            "modId": "647CB65DADE9ECF6",
            "name": "Conflict Domination PVE",
            "version": "1.0.24"
        },
        {
            "modId": "6214CEA5DA92BFF3",
            "name": "ACE Medical Prototypes",
            "version": "0.1.19"
        },
        {
            "modId": "6556DAA535FB5BEE",
            "name": "WCS AH64 Helipad Edit",
            "version": "1.0.2"
        },
        {
            "modId": "629543EC64631D3D",
            "name": "Modern RUS",
            "version": "0.0.3"
        },
        {
            "modId": "61B514B96692C049",
            "name": "ConflictPVERemixedVanilla2.0",
            "version": "2.3.11"
        },
        {
            "modId": "6152CB0BD0684837",
            "name": "WCS_Clothing",
            "version": "3.0.0"
        }
      ]
    },
    "rcon": {
      "address": "xxx.xxx.xxx.xxx",
      "port": 4427,
      "password": "xxxxx",
      "maxClients": 10,
      "permission": "admin",
      "blacklist": [],
      "whitelist": []
    },
    "operating": {
      "slotReservationTimeout": 60,
      "disableServerShutdown": false,
      "playerSaveTime": 120,
      "lobbyPlayerSynchronise": true,
      "joinQueue": {
        "maxSize":50
      },
      "disableNavmeshStreaming": [
        "Soldiers",
        "BTRlike"
      ]
    }
  }


```
 
# 
