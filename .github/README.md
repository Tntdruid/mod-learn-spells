# ![logo](https://raw.githubusercontent.com/azerothcore/azerothcore.github.io/master/images/logo-github.png) AzerothCore

## mod-learn-spells
### This is a module for [AzerothCore](http://www.azerothcore.org)

- Latest build status with azerothcore:

[![Build Status](https://github.com/azerothcore/mod-learn-spells/workflows/core-build/badge.svg?branch=master&event=push)](https://github.com/azerothcore/mod-learn-spells)

#### Features:

LearnAllSpells teaches new class spells on level-up, like in Mists of Pandaria and later, so players don't need to visit a class trainer.

- Class spells from the trainers, learned at the level they become available
- Spells from class quests (Warrior stances, Warlock demons, Druid forms, ...)
- Extra spells such as Paladin and Warlock mounts, Mage teleports and Shaman totems
- Optional catch-up on login for characters that existed before the module was installed

#### Configuration

See `conf/mod_learnspells.conf.dist`:

| Option | Default | Description |
|---|---|---|
| `LearnSpells.Enable` | 1 | Enable the module |
| `LearnSpells.Announce` | 1 | Announce the module on login |
| `LearnSpells.OnFirstLogin` | 0 | Learn all spells up to the current level on the first login |
| `LearnSpells.OnLogin` | 0 | Learn all missing spells up to the current level on every login |
| `LearnSpells.QuestSpells` | 1 | Learn spells rewarded by class quests |
| `LearnSpells.IgnoreSpells` | "" | Comma separated spell ids that are never learned |
| `LearnSpells.MaxLevel` | 80 | Highest level spells are learned for |

### This module currently requires:

- AzerothCore v1.0.1+

### How to install

1. Simply place the module under the `modules` folder of your AzerothCore source folder.
2. Re-run cmake and launch a clean build of AzerothCore
3. Ready.

