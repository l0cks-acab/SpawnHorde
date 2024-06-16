# SpawnHorde Plugin

The SpawnHorde plugin allows admins to spawn a horde of specified animals that chase a specific or random player on the map with custom size and health. Admins can also remove all spawned entities using a command.

##Author
This plugin was made by: herbs.acab

## Installation

1. Download the `SpawnHorde.cs` file.
2. Place the `SpawnHorde.cs` file in your `oxide/plugins` directory.
3. Reload the plugin using the console command: `oxide.reload SpawnHorde`.

## Commands

`/spawnhorde` - This command spawns a horde of specified animals that chase a specific or random player.
`/spawnhorde` <player> <horde_size> <horde_health> animal:bear,chicken,wolf,boar,stag
`/killhorde` - removes all entities from the last /spawnhorde command

## Parameters

- `<player>`: The target player's name or Steam64ID. If the player is not found, the command will return an error.
- `<horde_size>`: The number of animals to spawn. Must be a positive integer.
- `<horde_health>`: The health of each animal in the horde. Must be a positive number.
- `<animal>`: The type of animal to spawn. Valid options are: `bear`, `chicken`, `wolf`, `boar`, `stag`.

## Example

/spawnhorde PlayerName 10 50 bear

This will spawn a horde of 10 bears, each with 50 health, to chase `PlayerName`.

## Permissions

Only admins can use the `/spawnhorde` and `/killhorde` commands.

## Changelog

### Version 1.1.2
- Added the `/killhorde` command to remove all spawned entities.
- Improved message formatting.
- Added `stag` as a valid animal type.

### Version 1.1.1
- Changed the horde spawn message to include red-colored "HORDE".

### Version 1.1.0
- Removed custom AI behavior and added `stag` to the spawnable types.

### Version 1.0.9
- Ensured the spawned horde ignores their standard AI and exclusively follows the player.

### Version 1.0.8
- Added additional command parameters to specify player, horde size, horde health, and animal type.

### Version 1.0.7
- Set the health of spawned bears to 10 HP each.
- Removed the size scaling.

