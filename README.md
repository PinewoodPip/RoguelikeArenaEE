## Roguelike Arena EE2 Patch

This is a patch for the [Roguelike Arena](https://steamcommunity.com/sharedfiles/filedetails/?id=3254033921) mod that adds the minimum elements necessary for Epic Encounters 2 to function in it:

- Meditate & Source Infusion are available from the start for player characters and companions
- Leveling up gives 1 Ascension Point

The original mod seems to use treasure tables that allow Artifacts to drop, but the rates are untested.

[Latest version](https://drive.google.com/file/d/1_UQid9NsKlB20PWR2JA3K42-cp2V_UZd/view?usp=sharing).

Requires the original mod to be loaded before the patch.

Special thanks to Ameranth for instructions on EE-fying other campaigns, and the basic integration script from EE Origins.

## Contributing

Feel free to make PRs to adjust the campaign's gameplay for EE (ex. modifying Artifact sources).

### Project setup

After cloning the repository, symlink all 3 mod folders (`Mods/RogueLikeArenaEE...`, `Projects/RogueLikeArenaEE...`, and `Public/RogueLikeArenaEE...`) into their corresponding path in `DefEd/Data`. To be able to load the mod in the editor you will also need all dependencies (EE Core & Roguelike Arena) unpacked and loadable as projects - this involves get their `Editor` folders if you want levels to be loadable.

Roguelike Arena's `Editor` folder for the version from 15/06 can be found [here](https://drive.google.com/file/d/145CStO2Ks89KRqPD49jgfDWiu8w6A9Ko/view?usp=sharing). **Before using it, check if Bonesnake has posted an updated version anywhere**.

### Scripting

`Z_PIP_EEConsiderations` goal contains the Meditate & Source Infusions unlocks, largely copied from EE Origins.

### Mapping

The only change to the main level (`RoguelikeArena_Level`) is adding the EE UI level template, north of the lobby template. This would have to be moved if any additional arenas are added in that spot, though Bonesnake says any further ones are likely to be added to the east of existing ones instead.
