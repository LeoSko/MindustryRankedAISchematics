# MindustryRankedAISchematics
Schematics that AI uses - all of them

# How to contribute
- Make your schematic.
- If you intend to place drills, AI can only find 1 type of ore OR 1 type of liquid. Specify this ore/liquid via placing and configuring `Item source`/`Liquid source` anywhere in the scheme.
- Bot's containers and vaults have spawning resources, use them + unloaders to make something more complex.
- Place walls to your liking. In case your don't, bot will try to place walls itself. Walls are not guaranteed to be placed and can be ignored by bot.
- Give it a simple name, reflecting:
  - First number in the name MUST reflect intended difficilty of the AI to use this schematic, ranging `from [00 to 99]`, **keep leading zeros**
    - Format can be either a single number `43`, or a period `43-52`
      - In case of period, it will be adjusted to match current schematic formula. You may expect your schematic to be chosen by bot at a certain level of difficulty.
    - To understand the scale, download some schematics and compare your to others. Also, see the table of difficulties below.
  - The rest of the name is freestyle, but try to write
    - units it produces
    - if no units, turrets it has
    - it no turrets, whatever important it has
    - if nothing important, this is probably schematic for Noob-Easy AI - specify at least some meaningful name
  - Good name example: `16-25 Shard Core flares.msch`
  - Bad name example: `dsafasdf 99.msch`
- Filename MUST match the name of schematic and have **msch** extension.

Name | Difficulty range | Schematics range | Growth rate (time/difficulty)
---- | ---------------- | ---------------- | -----------------------------
Noob | 0-16 | 00-22 | 04 at 60 minutes
Easy | 5-20 | 00-27 | 12 at 45 minutes
Normal | 10-40 | 04-49 | 22 at 30 minutes
Hard | 16-65 | 10-71 | 35 at 20 minutes
Extreme | 20-85 | 13-98 | 52 at 18 minutes

* `Difficulty` growth rate is similar to function `- 1 / (x + 1) + 1`, where `x` is time.
* `Schematics` are chosen using normal distribution with `mean=Difficulty`, `sigma=4` with hard cap range of `Difficulty / 10 + 5`.
