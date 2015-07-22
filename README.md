# CavemansWAI2.2.0Missions
Caveman's custom missions for WAI 2.2.0 Arma 2 Epoch/Overpoch

Requires that you already have WAI 2.2.0 installed  http://epochmod.com/forum/index.php?/topic/15671-release-wicked-ai-220/
For bugs and updates, follow the dev thread http://epochmod.com/forum/index.php?/topic/36089-release-new-missions-for-wai-220/
#INSTRUCTIONS
1: Edit the mission list inside the config.sqf in your WAI folder to include the new missions.
##ADD
```
["gem_tower",5],
["cannibal_cave",5],
["crop_raider",5],
["drone_pilot",5], 
["slaughter_house",5],
["drugbust",5],
["armybase",5],
["abandoned_trader",5],
["lumberjack",5],
["tankcolumn",5],
["macdonald",5],
["radioshack",5],
["junkyard",5]
```
to each hero and bandit list.

##example ( without [Bandit] Junk Yard )
```
wai_hero_missions = [ // ["mission filename",% chance of picking this mission],Make sure the chances add up to 100,or it will not be accurate percentages
["patrol",4],
["black_hawk_crash",4],
["armed_vehicle",4],
["bandit_base",4],
["captured_mv22",4],
["ikea_convoy",4],
["destroyed_ural",4],
["disabled_milchopper",4],
["mayors_mansion",4],
["weapon_cache",4],
["bandit_patrol",4],
["gem_tower",4],
["cannibal_cave",4],
["crop_raider",4],
["drone_pilot",4], 
["slaughter_house",4],
["drugbust",4],
["armybase",4],
["abandoned_trader",4],
["lumberjack",4],
["tankcolumn",5],
["macdonald",5],
["radioshack",5],
["junkyard",5]
]; 
wai_bandit_missions = [
["patrol",4], 
["armed_vehicle",4], 
["black_hawk_crash",4], 
["captured_mv22",4], 
["broken_down_ural",4], 
["hero_base",4], 
["ikea_convoy",4], 
["medi_camp",4], 
["presidents_mansion",4], 
["sniper_extraction",4], 
["weapon_cache",4],
["gem_tower",4],
["cannibal_cave",4],
["crop_raider",4],
["drone_pilot",4], 
["slaughter_house",5],
["drugbust",5],
["armybase",5],
["abandoned_trader",5],
["lumberjack",5],
["tankcolumn",5],
["macdonald",5],
["radioshack",5]
];
```

##WITH [Bandit] Junk Yard (This mission could still be broken)
```
wai_hero_missions = [ // ["mission filename",% chance of picking this mission],Make sure the chances add up to 100,or it will not be accurate percentages
["patrol",4],
["black_hawk_crash",4],
["armed_vehicle",4],
["bandit_base",4],
["captured_mv22",4],
["ikea_convoy",4],
["destroyed_ural",4],
["disabled_milchopper",4],
["mayors_mansion",4],
["weapon_cache",4],
["bandit_patrol",4],
["gem_tower",4],
["cannibal_cave",4],
["crop_raider",4],
["drone_pilot",4], 
["slaughter_house",4],
["drugbust",4],
["armybase",4],
["abandoned_trader",4],
["lumberjack",4],
["tankcolumn",5],
["macdonald",5],
["radioshack",5],
["junkyard",5]
]; 
wai_bandit_missions = [
["patrol",4], 
["armed_vehicle",4], 
["black_hawk_crash",4], 
["captured_mv22",4], 
["broken_down_ural",4], 
["hero_base",4], 
["ikea_convoy",4], 
["medi_camp",4], 
["presidents_mansion",4], 
["sniper_extraction",4], 
["weapon_cache",4],
["gem_tower",4],
["cannibal_cave",4],
["crop_raider",4],
["drone_pilot",4], 
["slaughter_house",4],
["drugbust",4],
["armybase",4],
["abandoned_trader",4],
["lumberjack",4],
["tankcolumn",5],
["macdonald",5],
["radioshack",5],
["junkyard",5]
];
```

2: Edit the crate_items list in the config.sqf of your WAI folder and add the new crates.

##ADD
```
crate_items_crop_raider = ["ItemKiloHemp"];
crate_items_gem_tower = ["ItemRuby","ItemEmerald","ItemSapphire"];
```

example
```
crate_items = ["FoodNutmix","FoodPistachio","FoodMRE","ItemSodaOrangeSherbet","ItemSodaRbull","ItemSodaR4z0r","ItemSodaMdew","ItemSodaPepsi","ItemBandage","ItemSodaCoke","FoodbaconCooked","FoodCanBakedBeans","FoodCanFrankBeans","FoodCanPasta","FoodCanSardines","FoodchickenCooked","FoodmuttonCooked","FoodrabbitCooked","ItemTroutCooked","ItemTunaCooked","ItemSeaBassCooked","ItemAntibiotic","ItemBloodbag","ItemEpinephrine","ItemHeatPack","ItemMorphine","ItemGoldBar","ItemGoldBar10oz","CinderBlocks","ItemCanvas","ItemComboLock","ItemLightBulb","ItemLockbox","ItemSandbag","ItemTankTrap","ItemWire","MortarBucket","PartEngine","PartFueltank","PartGeneric","PartGlass","PartPlankPack","PartVRotor","PartWheel","PartWoodPile"];
crate_items_high_value = ["ItemBriefcase100oz","ItemVault","30m_plot_kit","ItemHotwireKit"];
crate_items_food = ["ItemWaterbottle","FoodNutmix","FoodPistachio","FoodMRE","ItemSodaOrangeSherbet","ItemSodaRbull","ItemSodaR4z0r","ItemSodaMdew","ItemSodaPepsi","ItemSodaCoke","FoodbaconCooked","FoodCanBakedBeans","FoodCanFrankBeans","FoodCanPasta","FoodCanSardines","FoodchickenCooked","FoodmuttonCooked","FoodrabbitCooked","ItemTroutCooked","ItemTunaCooked","ItemSeaBassCooked"];
crate_items_buildables = ["forest_large_net_kit","cinder_garage_kit",["PartPlywoodPack",5],"ItemSandbagExLarge5X","park_bench_kit","ItemComboLock",["CinderBlocks",10],"ItemCanvas","ItemComboLock",["ItemLightBulb",5],"ItemLockbox",["ItemSandbag",10],["ItemTankTrap",10],["ItemWire",10],["MortarBucket",10],["PartPlankPack",5],"PartWoodPile"];
crate_items_vehicle_repair = ["PartEngine","PartFueltank","PartGeneric","PartGlass","PartVRotor","PartWheel"];
crate_items_medical = ["ItemWaterbottle","ItemAntibiotic","ItemBloodbag","ItemEpinephrine","ItemHeatPack","ItemMorphine","ItemBandage","FoodCanFrankBeans","FoodCanPasta"];
crate_items_chainbullets = ["2000Rnd_762x51_M134","200Rnd_762x51_M240","100Rnd_127x99_M2","150Rnd_127x107_DSHKM"];
crate_items_sniper = [["ItemPainkiller",5],"Skin_Sniper1_DZ","Skin_CZ_Soldier_Sniper_EP1_DZ","Skin_GUE_Soldier_Sniper_DZ"];
crate_items_president = ["ItemDocument","ItemGoldBar10oz"];
crate_items_crop_raider  = ["ItemKiloHemp"];
crate_items_gem_tower  = ["ItemRuby","ItemEmerald","ItemSapphire"];
```

You can edit the amount of loot in the custom crates at gem tower and weed missions by adjusting the number highlighted below inside each mission.
example: 
```
if(_complete) then {
  [_crate,0,0,[3,crate_items_gem_tower],0] call dynamic_crate;
};
 ```
**********************************************************************************************************
To make your own custom loot crates go to this forum link:
http://epochmod.com/...ai-220/page-103
post#2045
**********************************************************************************************************

3. Download, unzip and copy the new missions into the hero and bandit folders of your WAI.

#CHANGELOG
```
(July 18th 2015) 	[FIXED] Removed Bandit Junk yard
(July 18th 2015)  	[FIXED] -Error in Junkyard Mission (Thank you Megaz & Satlzman)
(July 14th 2015)  	[FIXED] RADIOSHACK & JUNKYARD MISSION - MISSING "   (Thank You MEGAZ)
(July 12th 2015)  	[FIXED] CROP RAIDER Missions - Ai HAD TRADER SKIN (Thank You Donnovan)
(July 6th 2015)    	[FIXED] ALL Bandit Missions  (thank you Saltzman)
(July 5th 2015)    	[FIXED] Crop Raider & drone pilot - WRONG TYPE OF Ai (thank you ElDubya)
(July 5th 2015)    	[FIXED] Crop Raider - WRONG TYPE OF Ai (thank you casual_Jeff) 
(July 3rd 2015)  	[FIXED] [HERO] Army Base Mission - invisible Ai 
(July 1st 2015)  	[FIXED] Army Base - LOOT BOX NOT SPAWNING EVERYTHING (thank you ElDubya)
(June 30th 2015) 	[FIXED] Drug Bust - DELETED MOUNTED GUNNERS
(June 30th 2015) 	[FIXED] Gem Tower - CASTLE TOWER BLOCKING LADDER (thank you cen)
(June 27th 2015) 	[FIXED] Slaughter House  - MISSION NOT COMPLETING (thank you cen)
(June 27th 2015) 	[FIXED] Gem Tower - GAP IN TOWERS (thank you Bob_the_K)
```
