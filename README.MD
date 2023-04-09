# Installation
After downloading the module using the manifest (at bottom of README),

go to ```/data/modules/lancer-token-wildcard```.

Extract "token_wildcard.zip" to ```/Data/```. This archive is just empty folders configured with the correct paths for the tokens to recognize.

In your world, import the compendiums marked "tw-strikers", "tw-defenders", "tw-controllers", etc. They will be blank, unconfigured actors for legal reasons, as the NPC data and LCPs are property of Massif Press. Add the classes yourself! I would recommend "[Quick Insert](https://foundryvtt.com/packages/quick-insert)" to speed up the process.

done!

## What this module does
Ever want to just drag and drop NPC actors onto canvas without fiddling around with custom artwork? ~~And you don't mind them being randomly chosen?~~ Well here's the module for you!

LANCER for foundry doesn't come with any of the CRB NPCs made as actors because the NPC data is protected and must be purchased from Massif Press (which you should do!). This module also has to side benefit of already creating empty actor sheets for every category, all you need to do is drag and drop the NPC classes onto the corresponding actors.

## How it works
it takes advantage of Foundry's in-built "Randomize wildcard images" feature, which randomizes the token art of actors when placed, sourcing the artwork from a given directory. All I've done is preconfigure the actors and directories for you, so you can start building your encounters instead of fiddling with NPC tokens. 

You can always add your own directories and follow Foundry's guide [here] https://foundryvtt.com/article/tokens/ to configure them. 

## Some nice modules to have
- [Token Variant Art](https://foundryvtt.com/packages/token-variants)
- [Quick Insert](https://foundryvtt.com/packages/quick-insert)

## Extras
- If you want to create a character sheet for a token with no linked character sheet, use the following macro:
```js
Actor.create({...token.actor.toObject(), folder: null, name: `NEW ${token.actor.name}`})
```

## Sourcing Token Art:
Now you need to add art. They must be .png files. I would recommend "[Retrograde Minis](https://retrogrademinis.com/)" and their Discord!

Alternatively you can go to "https://mega.nz/file/UGcEDDQC#5hxWnFXlLurmcZwJdxdDxF4KQNWFbcX2yF_61JR1tlg" for my folder, which uses art by the wonderful folks over at the Retrograde Minis Discord Server. Their artwork is in turn derived from the style and assets created by Retrograde! Support their patreon. This file is configured with the correct paths and names, so you can Just extract this file to ```/Data/``` instead of the included empty "token_wildcard.zip" archive. 

Edit: updated MEGA file. now includes some factions and more art variety for non-Ronin NPCs.

### Manifest
manifest: "https://github.com/Cakeisgreater/Lancer-Token-Wildcard/releases/download/latest/module.json"

### Special Thanks to the folks at PILOT NET, Foundry, and Retrograde Minis Discord Servers.
![wildcard demo](https://user-images.githubusercontent.com/129597129/230131296-2c2ddec6-26f9-4f5f-8fa7-a3626fadc043.gif)
