# Rise of the Reich - Rule Mechanics 
A mod that implements rules from the scenario Rise of the Reich (https://docs.google.com/spreadsheets/d/17s7Zuz-TFOdlr2j4wlsbmydyqkxg9f0XNYB7IclYdu4/edit#gid=254942968)

## Download instructions
Download the repository as a zip-file and move it into the Paradox Interactive\Europa Universalis IV\mod folder. Extract **only** the .mod file from the zip-file.


## Changes in the mod files
- common/defines.lua
	- Changed peace cost for Return Core, Revoke Core, Release Nation to base 100 from 1
	- Changed ALLY_PEACE_COST_MULT to base 100 from 2
	- Changed PEACE_COST_DEMAND_PROVINCE to base 1000 from 1
	- Changed number of Great Powers to 9 from 8

- common/cb_types/00_cb_types.txt
	- Disabled Return Core, Revoke Core, Release Nation to all CB for attackers

- common/wargoal_types/00_wargoal_types.txt
	- take_claim - Changed demand_province_factor for claims or cores to 0.001, meaning base 1 cost
	- take_core - Changed demand_province_factor for cores to 0.001, meaning base 1 cost


- events/HolyRomanEmpire.txt
	- Added event if the emperor is not a GP, the capitol gets 50 dev in all three areas respectively but gets a province modifier that nulls the effects of this increase
	- Added event if the emperor was removed from power the buffs from previous event is removed along with the modifier

- localisation/generic_events_l_english.yml
	- Added text for events in HolyRomanEmpire.txt




## TODO
Change events about the emperor and GP to actually make them a GP, clear flags and such.
Change take_core to allow defender to take claims? Otherwise attackers could just wage uncostly wars against enemies that do not have cores on it
Change take_claim to allow for different AE based on if its claim or core

## Defunct changes
- common/triggered_modifiers/00_triggered_modifiers.txt
	- Added a triggered modifier if the emperor is not a GP, it will be seen as such

