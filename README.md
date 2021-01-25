# TorchLight - A FoundryVTT Module

This is a slightly enhanced Torch and Light Module for Foundry VTT, based on the excellent work of RealDeuce on the Torch Module.

Instead of managing one light source, the Torchlight module recognises three different types of light sources, torches, lanterns and light spells, each with its own characteristics.

From the original module, I have dropped the management of Dancing Lights, as this should really just be its own module. I also have not yet implemented back the management of resources, in particular the availability of the Light spell, and the consumption of torches (and now flasks of oil for a lantern), as I feel that not every group manages that to that level of detail, and often the character bearing the light is not necessarily the one providing the resources. But I might put it back in as a future request.

I must also confess that I am a complete noob at Foundry VTT, Javascript, JQuery and GitHub, so developping this was really a good way for me to learn things and discoved Foundry VTT, so every bit of advice that can be provided would really be appreciated.

## Installation
### Method 1 (Not yet available)
- Start up Foundry and click "Install Module" in the "Add-On Modules" tab.
- Search for "Torchlight" in the pop up window.
- Click "Install" and it should appear in your modules list.

### Method 2
- Start up Foundry and click "Install Module" in the "Add-On Modules" tab.
- Paste the link: `https://raw.githubusercontent.com/PhilippeKr/TorchLight/main/module.json`
- Click "Install" and it should appear in your modules list.

### Method 3
- Download the [.zip file](https://github.com/PhilippeKr/TorchLight/raw/main/torchlight.zip) in this repository.
- Extract the contents of the zip in `\resources\app\public\modules\`
- Restart Foundry.

## Implemented Features
Torchlight provides 3 potential sources of light:
- Light Spell of varying aspects, with White Light (possibly for good characters), Red Light (probably not so good) and Green Light (for nature lovers out there, druids and rangers, I'm pointing at you)...
- Lantern, with hooded lanterns in both open and closed position, and bullseye lantern with enhanced range but only in a cone.
- Torch, with various colours and intensity

These are toggled on and off from the HUD of tokens, form three icons that can be positioned either to the left or to the right of the standard HUD. Only one type of light source can be active at a given time, if you change your light source, simply deactivate the current one and activate the new one.

The DM can keep the activation/deactivation to himself (in which case the HUD of the players will just show whether there is a light source active) or he can delegate the management of the light to his player through an option of the module.

In addition, the options allow the independent configuration of the light sources:
- Range for bright and dim light
- Type of light emitted

## Planned Features
- Verification of the availability of resources (ability to cast Light, flask of oil or torches in inventory).
- Actual consumption of resources like flask of oil or torches from the inventory
- Cleaning up the code from the original (all the code used is brand new, but there are remaining unused functions)

## Known Issues
None yet, but I'm sure some will be found very quickly... :)

## Acknowledgements
- Big thanks to Atropos for making a wonderful VTT that's worth making modules for!
- Many thanks to RealDeuce as well for making the original Torch module and giving me all these ideas!
- RedReign for providing the template for this Read me.

## License
The source code is licensed under GPL-3.0.
