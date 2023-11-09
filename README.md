# Police Helicopter Spawn Script for FiveM

This script enables police officers in your FiveM server to spawn a police helicopter at a designated location. Players with the police job can utilize this feature within a specified range of the spawn point.

## Installation

1. Ensure you have the [FiveM](https://fivem.net/) client installed on your system.
2. Copy the `PoliceHelicopterSpawn` file into your FiveM resources folder.
3. Add `start PoliceHelicopterSpawn` to your `server.cfg` file to ensure the script is started when your server launches.

## Usage

- Police officers will see a marker indicating the spawn location.
- To spawn the helicopter, police officers need to approach the marker and press the 'E' key (default control, configurable in the script).
- If the player is not a police officer or is not within the designated range, an error notification will be displayed.

## Frequently Asked Questions (FAQ)

### Q: How do I change the keybind for spawning the helicopter?
**A:** You can modify the control key by editing the script. Look for the line `IsControlJustPressed(0, 38)` and change `38` to the [control code](https://docs.fivem.net/docs/game-references/controls/) corresponding to the desired key.

### Q: Can I change the spawn location of the helicopter?
**A:** Yes, you can change the spawn location by modifying the `spawnLocation` variable in the script. Adjust the `vector3` values (X, Y, Z) to specify the new coordinates.

### Q: How can I customize the helicopter model?
**A:** The script currently spawns a helicopter with the model "polmav". If you want to use a different helicopter model, change both occurrences of `GetHashKey("polmav")` in the script to the desired vehicle model name.

Feel free to reach out if you have any further questions or issues.
