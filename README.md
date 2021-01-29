# MindustryRankedAISchematics
Schematics that AI uses - all of them

# How to contribute
- Make your schematic
- If you intend to place drills, AI can only find 1 type of ore. Specify this ore via placing and configuring `Item source` anywhere in the scheme
- Bot's containers and vaults have spawning resources, use them + unloaders to make something more complex
- Place walls to your liking. In case your don't, bot will try to place walls itself
- Give it a simple name, reflecting
  - First number in the name MUST reflect intended difficilty of the AI to use this schematic, ranging `from [00 to 99]`, **keep leading zeros**
    - To understand the scale, download some schematics and compare your to others
    - Example 1: Noob AI starts from difficulty 0 with maximum of 10
    - Example 2: Normal AI starts from difficulty 10 with maximum of 43
    - Example 3: Extreme AI starts from difficulty 20 with maximum of 85
  - The rest of the name is freestyle, but try to write
    - units it produces
    - if no units, turrets it has
    - it no turrets, whatever important it has
  - Good name example: `16 Shard Core flares.msch`
  - Bad name example: `dsafasdf 99.msch`
- Filename MUST match the name of schematic and have **msch** extension
