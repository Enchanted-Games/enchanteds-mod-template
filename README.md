# Enchanted's Mod Template

Multi-version, multi-loader mod template for Minecraft using Stonecutter. This template is set up for Minecraft 1.21.11 (fabric and neoforge), and 26.1-snapshot-1 (fabric).

This template was primarily made with my specific needs in mine, however you are free to expand upon and use this as a base for your own mods

## Setup

1. Find and replace all instances of `eg_template_mod` with your mod id. Do the same for `Enchanted's Template Mod` with your mod name
2. Update `mod.group` in gradle.properties, then rename `src/main/java/games/enchanted/eg_template_mod/` to `src/main/java/{group}/{mod id}`
3. Rename `src/main/resources/eg_template_mod.mixins.json` to your mod id
4. Make sure the project and gradle is configured to use Java 25 your IDE
5. Let gradle sync and you should be good to go!

## More info
- Change Minecraft versions in settings.gradle.kts
   - By default there are buildscripts for Fabric (remap, >=1.14), Fabric (>=26.1), and NeoForge (>1.20.2), if you need other versions you may make your own buildscripts for them
- Use the stonecutter gradle tasks to switch between versions, run configurations should be generated automatically
