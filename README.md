## This mod requires Cloth Config API.
# Lifesteal Mod (Fabric)
This Lifesteal mod is identical by the Lifesteal SMP. In this mod, if you kill a player, you steal one of their hearts, and if you die, you lose one. Just like the Lifesteal SMP except for one change: if you lose all of your hearts, you enter **spectator mode** instead of getting banned. You can be revived if you lose all of your hearts.

## Features
- When a player kills another player, they steal one heart from the defeated player.
- Players lose a heart every time they die.
- If a player loses all their hearts, they are put into spectator mode.
- Players can withdraw hearts using the `/lifesteal withdraw [number]` command.
- --- **UPDATE 1.1.0** ---
- Netherite armor/tools (excluding pickaxe/shovel/hoe) are disabled.
- Disabled totem of undying.
- --- **UPDATE 1.2.0** ---
- Added config.
- --- **UPDATE 1.3.1** ---
- The mod is now only required on the server side.
- --- **UPDATE 2.0** ---
- Players can use a revive beacon to revive other players.
- Riptide trident cooldown (cooldown is configurable in config).
- Protection enchantment is now capped at level 3 and sharpness enchantment is capped at level 4.
- No dragon egg in enderchest.
- Disabled enderpearl (you can't use them by right clicking).
- Players can use `/lifesteal viewRecipes` to view the recipes of heart and the revive beacon.
- End crystals deal no damage to the player nor the environment.
- Respawn anchors works in the nether but not in the overworld and the end dimensions.
- --- **UPDATE 2.1** ---
- Changed /recipes screen to gray stained glass (looks better)
- Added /lifesteal set <player> <amount>
- Added /lifesteal take <player> <amount>
- Added a config option for healing on withdraw

### Next update:
- Add mod menu support.
- Add config for everything that doesn't have it right now.

More features will be added. (Possibly maybe idk for sure)

## Commands

- **/lifesteal oprevive [player_name]:** Revives the specified player (only works if you are an operator, use the revive beacon to revive if you are not an operator).
- **/lifesteal withdraw [number]:** Withdraws the specified number of hearts from your total hearts.
- **/lifesteal viewRecipes:** Opens a GUI with both the heart and the revive beacon recipes.
- **/lifesteal give [player_name] [amount]:** Adds the specified amount of hearts to the other players health bar (only works if you are a operator and bypasses heart cap).
- **/lifesteal set [player_name] [amount]:** Sets the other players health bat to the specified amount of hearts (only works if you are a operator and bypasses heart cap).
- **/lifesteal take [player_name] [amount]:** Takes the specified amount of hearts from the other players health bar (only works if you are a operator and bypasses heart cap). 

## Config
You can edit the mod config by going into the `config` directory and then opening the lifestealmod.json in any text editor.

```json
{
  "maxHeartCap": 40,
  "disableEnderPearl": true,
  "disableCPVP": true,
  "disableTotem": true,
  "disableNetherite": true,
  "noDragonEggEnderChest": true,
  "riptideCooldown": 200,
  "riptideCooldownEnabled": true
  "healPlayerOnWithdraw": false"
}
```

#### Config explained:
- **maxHeartCap**: Sets the maximum number of health points (HP) a player can have. Default is 40 HP (20 hearts).
- **disableEnderPearl**: Disables the use of ender pearls when set to `true`.~~~~
- **disableCPVP**: Disables crystal pvp when set to `true`.
- **disableTotem**: Prevents the use of Totems of Undying when set to `true`.
- **disableNetherite**: Disables the use of netherite tools(excluding pickaxe/shovel) and armor when set to `true`.
- **noDragonEggEnderChest**: Prevents players from placing dragon egg in ender chests when set to `true`.
- **riptideCooldown**: Configurable cooldown for the trident (in ticks).
- **riptideCooldownEnabled**: Enables riptide cooldown when set to `true`.
- **healPlayerOnWithdraw**: Heals the player when running the command /lifesteal withdraw when set to `true`.

## License

This mod is licensed under the MIT License. For more details, please refer to the [LICENSE]([https://github.com/sdphantomz3/LifestealMod/blob/main/LICENSE](https://github.com/sdphantomz3/LifestealMod/blob/main/LICENSE)) file in the repository.
