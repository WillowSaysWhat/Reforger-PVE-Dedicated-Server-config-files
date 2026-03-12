# Reforger PVE Dedicated Server config files

Congratulations, you are about to make your own dedicated Arma Reforger PVE server.

This README hold the different code you will need to fill out the different .json files.

* [Blank Server.json](#blank-serverjson)
* [ConflictPVEvanilla.json](#conflictpvevanillajson)
* [Official Game mode IDs](#official-gamemode-ids)

## Blank Server.json

```json
{
	"bindAddress": "",
	"bindPort": 0,
	"publicAddress": "",
	"publicPort": 0,
	"a2s": {
		"address": "",
		"port": 0
	},
	"rcon": {
		"address": "",
		"port": 0,
		"password": "",
		"permission": "monitor",
		"blacklist": [],
		"whitelist": []
	},
	"game": {
		"name": "",
		"password": "",
		"passwordAdmin": "",
		"admins" : [],
		"scenarioId": "",
		"maxPlayers": 0,
		"visible": true,
		"gameProperties": {
			"serverMaxViewDistance": 1600,
			"serverMinGrassDistance": 0,
			"networkViewDistance": 1500,
			"disableThirdPerson": false,
			"fastValidation": true,
			"battlEye": true,
			"VONDisableUI": false,
			"VONDisableDirectSpeechUI": false,
			"VONCanTransmitCrossFaction": false
		},
		"mods": []
	}
}

```

## conflictPVEvanilla.json

## NOTE

This is Gramps Conflict PVER emixed Vanilla 2.0 gamemode. it is a mod found in the workshop. The mode id number and mod location is `{6DD58790690E9D29}Missions/ConflictPVERemixedVanilla2_US.conf`
This is important for the scenarioId section in the json. 

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
      "xxxxxxxx-xxxx-xxxx-xxxx-xxxxx",
      "xxxx-xxxx-xxxx-xxx-xxxxxxxxx",
      "xxxx-xxxx-xxxx-xxxx-xxxxxxxx"
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
        "m_sName": "Conflict PVE",
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
        "name": "RHS - Status Quo"
      },
      {
        "modId": "64900A5A31F5DCB5",
        "name": "MRZR"
      },
      {
        "modId": "6518C209A48D4991",
        "name": "Medevac Huey"
      },
      {
        "modId": "6214CEA5DA92BFF3",
        "name": "ACE Medical Prototypes"
      },
      {
        "modId": "6556DAA535FB5BEE",
        "name": "WCS AH64 Helipad Edit"
      },
      {
        "modId": "629543EC64631D3D",
        "name": "Modern RUS"
      },
      {
        "modId": "61B514B96692C049",
        "name": "ConflictPVERemixedVanilla2.0"
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
      "maxSize": 50
    },
    "disableNavmeshStreaming": [
      "Soldiers",
      "BTRlike"
    ]
  }
}

```
 
# Official Gamemode IDs

Official scenarios (31 entries)
### Conflict PVP - Everon
{ECC61978EDCC2B5A}Missions/23_Campaign.conf (Conflict - Everon)

### Training/Tutorial
{002AF7323E0129AF}Missions/Tutorial.conf (Training)

### Game Master Everon
{59AD59368755F41A}Missions/21_GM_Eden.conf (Game Master - Everon)

### Game Master Arland
{2BBBE828037C6F4B}Missions/22_GM_Arland.conf (Game Master - Arland)

### Game Master Kolguyev
{F45C6C15D31252E6}Missions/27_GM_Cain.conf (Game Master - Kolguyev)

### Conflict - Northern Everon
{C700DB41F0C546E1}Missions/23_Campaign_NorthCentral.conf (Conflict - Northern Everon)

### Conflict - Southern Everon
{28802845ADA64D52}Missions/23_Campaign_SWCoast.conf (Conflict - Southern Everon)

### Conflict - Western Everon
{94992A3D7CE4FF8A}Missions/23_Campaign_Western.conf (Conflict - Western Everon)

### Conflict - Montignac
{FDE33AFE2ED7875B}Missions/23_Campaign_Montignac.conf (Conflict - Montignac)

### Combat Ops - Arland
{DAA03C6E6099D50F}Missions/24_CombatOps.conf (Combat Ops - Arland)

### Conflict - Arland
{C41618FD18E9D714}Missions/23_Campaign_Arland.conf (Conflict - Arland)

### Combat Ops - Everon
{DFAC5FABD11F2390}Missions/26_CombatOpsEveron.conf (Combat Ops - Everon)

### Capture & Hold - Briars
{3F2E005F43DBD2F8}Missions/CAH_Briars_Coast.conf (Capture & Hold - Briars)

### Capture & Hold - Montfort Castle
{F1A1BEA67132113E}Missions/CAH_Castle.conf (Capture & Hold - Montfort Castle)

### Capture & Hold - Concrete Plant
{589945FB9FA7B97D}Missions/CAH_Concrete_Plant.conf (Capture & Hold - Concrete Plant)

### Capture & Hold - Almara Factory
{9405201CBD22A30C}Missions/CAH_Factory.conf (Capture & Hold - Almara Factory)

### Capture & Hold - Simon's Wood
{1CD06B409C6FAE56}Missions/CAH_Forest.conf (Capture & Hold - Simon's Wood)

### Capture & Hold - Le Moule
{7C491B1FCC0FF0E1}Missions/CAH_LeMoule.conf (Capture & Hold - Le Moule)

### Capture & Hold - Camp Blake
{6EA2E454519E5869}Missions/CAH_Military_Base.conf (Capture & Hold - Camp Blake)

### Capture & Hold - Morton
{2B4183DF23E88249}Missions/CAH_Morton.conf (Capture & Hold - Morton)

### Elimination
{C47A1A6245A13B26}Missions/SP01_ReginaV2.conf (Elimination)

### Air Support
{0648CDB32D6B02B3}Missions/SP02_AirSupport.conf (Air Support)

### Conflict: HQ Commander - Everon
{0220741028718E7F}Missions/23_Campaign_HQC_Everon.conf (Conflict: HQ Commander - Everon)

### Conflict: HQ Commander - Arland
{68D1240A11492545}Missions/23_Campaign_HQC_Arland.conf (Conflict: HQ Commander - Arland)

### Conflict: HQ Commander - Kolguyev
{BB5345C22DD2B655}Missions/23_Campaign_HQC_Cain.conf (Conflict: HQ Commander - Kolguyev)

### Operation Omega 01: Over The Hills And Far Away
{10B8582BAD9F7040}Missions/Scenario01_Intro.conf (Operation Omega 01: Over The Hills And Far Away)

### Operation Omega 02: Radio Check
{1D76AF6DC4DF0577}Missions/Scenario02_Steal.conf (Operation Omega 02: Radio Check)

### Operation Omega 03: Light In The Dark
{D1647575BCEA5A05}Missions/Scenario03_Villa.conf (Operation Omega 03: Light In The Dark)

### Operation Omega 04: Red Silence
{6D224A109B973DD8}Missions/Scenario04_Sabotage.conf (Operation Omega 04: Red Silence)

### Operation Omega 05: Cliffhanger
{FA2AB0181129CB16}Missions/Scenario05_Hill.conf (Operation Omega 05: Cliffhanger)

### Combat Ops - Kolguyev
{CB347F2F10065C9C}Missions/CombatOpsCain.conf (Combat Ops - Kolguyev)
