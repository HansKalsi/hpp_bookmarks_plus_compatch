# CK3 Mod Template
This is a template for the basic setup of a CK3 mod with base files.
It can be used to start a new project with ease so base files are generated and all required placeholder information is present for quick kickoff

## Quick Setup Instructions
- Update name of folder from ck3_mod_template to something relevant to the new mod
- Setup 'descriptor.mod' file
    - Remember to increment version as the mod is updated (not in this initial setup)
    - Setup initially known 'tags' (this helps discovery), e.g: 
        - "Decisions"
        - "Events"
        - "Warfare"
        - "Gameplay"
    - Set mod display 'name' (which is how it will display in the mod list)
    - Set 'supported_version' to the current game version, e.g: 1.14.* (always use a star at the end since patches won't break things)
- Replace 'thumbnail.png' image (keep thumbnail.png as the name)
- Update this readme for your purposes
- REMEMBER TO SETUP A NEW GIT, DON'T PUSH TO THE TEMPLATE

## Folder Structure Information
The structure of your folders should align precisely with the base game folder structure, as the mod files get merged based on this structure.
An empty common folder and localization with a placeholder english file has been setup by default, although you may not needs these based on the mods goal.

## Correct Localization Structure
Localization folder structure is:
- localization
    - english
    - spanish
    - etc

At the top of the each file with in the correspective folder should start with a declaritive line
- e.g:
    - l_english:
    - l_spanish:
    - etc

The naming convention for these files is X_l_LOCALIZATION.yml, e.g: example_l_english.yml