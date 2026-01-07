# Monster Hunter Armory - Data Exporter

Export your decorations and talismans from **Monster Hunter Wilds** for use with the Monster Hunter Armory build optimizer.

## Requirements

- Monster Hunter Wilds (PC/Steam)
- [REFramework](https://www.nexusmods.com/monsterhunterwilds/mods/93)

## Installation

### Step 1: Install REFramework

1. Download REFramework from [Nexus Mods](https://www.nexusmods.com/monsterhunterwilds/mods/93)
2. Extract `dinput8.dll` into your game folder:
   ```
   Steam\steamapps\common\MonsterHunterWilds
   ```

### Step 2: Install the Export Script

1. Download `game_export.lua` from this repository ([Direct Download](https://raw.githubusercontent.com/Az3rate/Monster-Hunter-Armory-Public/master/game_export.lua))
2. Place it in the REFramework autorun folder:
   ```
   MonsterHunterWilds\reframework\autorun
   ```
   > Create the `autorun` folder if it doesn't exist

## Usage

1. Launch Monster Hunter Wilds
2. Load into any save file
3. Press `Insert` to open REFramework menu
4. Navigate to **Script Generated UI** → **MH Armory Exporter**
5. Click **Export All** (or export individual categories)

### Export Files

Your data will be saved to:
```
MonsterHunterWilds\reframework\data\mhwb_exports
```

Files created:
- `decorations.mhwb` - Your owned decorations
- `talismans.mhwb` - Your talismans with skills and slots
- `unified_export.mhwb` - Combined export (recommended)

## Import to Monster Hunter Armory

1. Open the Monster Hunter Armory app
2. Click **Select Export Folder**
3. Navigate to `mhwb_exports` folder
4. Your decorations and talismans will be imported automatically

## Troubleshooting

### Script not appearing in REFramework
- Ensure the file is named exactly `game_export.lua`
- Check that it's in the correct folder: `reframework\autorun`
- Restart the game after adding the script

### Export fails or no files created
- Make sure you're loaded into a save file (not title screen)
- Check the `reframework\data` folder for error logs

## Privacy & Safety

This script:
- Only reads your inventory data (decorations, talismans)
- Does not modify any game files
- Does not send data anywhere - all exports are local files
- Is safe to use online

## Version

Current version: **1.0.0**

## License

MIT License - Free to use and modify
