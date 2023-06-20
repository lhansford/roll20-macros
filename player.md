# Macros

- Replace `CHARACTER_NAME` with your character name.
- These all assume the character sheet is [the default D&D 5E sheet from Roll20](https://wiki.roll20.net/D%26D_5E_by_Roll20).

## Initiative

```rmacro
&{template:simple}
  {{rname=Initiative}}
  {{mod=Dex}}
  {{normal=1}}
  {{r1=[[d20+@{CHARACTER_NAME|initiative_bonus}[DEX] &{CHARACTER_NAME|tracker}]]}}
  {{charname=Mara}}
```

```rmacro
&{template:simple} {{rname=Initiative}} {{mod=Dex}} {{normal=1}} {{r1=[[d20+@{CHARACTER_NAME|initiative_bonus}[DEX] &{CHARACTER_NAME|tracker}]]}} {{charname=Mara}}
```

## Skill check

- Suggested that you turn on always roll twice
- Would be nice to add positive sybmols in front of mods

```rmacro
/w @{CHARACTER_NAME|character_name}
  &{template:default}
  {{name=Skill check}}
  {{Acrobatics=[@{CHARACTER_NAME|acrobatics_bonus}](~CHARACTER_NAME|acrobatics)}}
  {{Animal Handling=[@{CHARACTER_NAME|animal_handling_bonus}](~CHARACTER_NAME|animal_handling)}}
  {{Arcana=[@{CHARACTER_NAME|arcana_bonus}](~CHARACTER_NAME|arcana)}}
  {{Athletics=[@{CHARACTER_NAME|athletics_bonus}](~CHARACTER_NAME|athletics)}}
  {{Deception=[@{CHARACTER_NAME|deception_bonus}](~CHARACTER_NAME|deception)}}
  {{History=[@{CHARACTER_NAME|history_bonus}](~CHARACTER_NAME|history)}}
  {{Insight=[@{CHARACTER_NAME|insight_bonus}](~CHARACTER_NAME|insight)}}
  {{Intimidation=[@{CHARACTER_NAME|intimidation_bonus}](~CHARACTER_NAME|intimidation)}}
  {{Investigation=[@{CHARACTER_NAME|investigation_bonus}](~CHARACTER_NAME|investigation)}}
  {{Medicine=[@{CHARACTER_NAME|medicine_bonus}](~CHARACTER_NAME|medicine)}}
  {{Nature=[@{CHARACTER_NAME|nature_bonus}](~CHARACTER_NAME|nature)}}
  {{Perception=[@{CHARACTER_NAME|perception_bonus}](~CHARACTER_NAME|perception)}}
  {{Performance=[@{CHARACTER_NAME|performance_bonus}](~CHARACTER_NAME|performance)}}
  {{Persuasion=[@{CHARACTER_NAME|persuasion_bonus}](~CHARACTER_NAME|persuasion)}}
  {{Religion=[@{CHARACTER_NAME|religion_bonus}](~CHARACTER_NAME|religion)}}
  {{Sleight of hand=[@{CHARACTER_NAME|sleight_of_hand_bonus}](~CHARACTER_NAME|sleight_of_hand)}}
  {{Stealth=[@{CHARACTER_NAME|stealth_bonus}](~CHARACTER_NAME|stealth)}}
  {{Survival=[@{CHARACTER_NAME|survival_bonus}](~CHARACTER_NAME|survival)}}
```

```rmacro
/w @{CHARACTER_NAME|character_name} &{template:default} {{name=Skill check}} {{Acrobatics=[@{CHARACTER_NAME|acrobatics_bonus}](~CHARACTER_NAME|acrobatics)}} {{Animal Handling=[@{CHARACTER_NAME|animal_handling_bonus}](~CHARACTER_NAME|animal_handling)}} {{Arcana=[@{CHARACTER_NAME|arcana_bonus}](~CHARACTER_NAME|arcana)}} {{Athletics=[@{CHARACTER_NAME|athletics_bonus}](~CHARACTER_NAME|athletics)}} {{Deception=[@{CHARACTER_NAME|deception_bonus}](~CHARACTER_NAME|deception)}} {{History=[@{CHARACTER_NAME|history_bonus}](~CHARACTER_NAME|history)}} {{Insight=[@{CHARACTER_NAME|insight_bonus}](~CHARACTER_NAME|insight)}} {{Intimidation=[@{CHARACTER_NAME|intimidation_bonus}](~CHARACTER_NAME|intimidation)}} {{Investigation=[@{CHARACTER_NAME|investigation_bonus}](~CHARACTER_NAME|investigation)}} {{Medicine=[@{CHARACTER_NAME|medicine_bonus}](~CHARACTER_NAME|medicine)}} {{Nature=[@{CHARACTER_NAME|nature_bonus}](~CHARACTER_NAME|nature)}} {{Perception=[@{CHARACTER_NAME|perception_bonus}](~CHARACTER_NAME|perception)}} {{Performance=[@{CHARACTER_NAME|performance_bonus}](~CHARACTER_NAME|performance)}} {{Persuasion=[@{CHARACTER_NAME|persuasion_bonus}](~CHARACTER_NAME|persuasion)}} {{Religion=[@{CHARACTER_NAME|religion_bonus}](~CHARACTER_NAME|religion)}} {{Sleight of hand=[@{CHARACTER_NAME|sleight_of_hand_bonus}](~CHARACTER_NAME|sleight_of_hand)}} {{Stealth=[@{CHARACTER_NAME|stealth_bonus}](~CHARACTER_NAME|stealth)}} {{Survival=[@{CHARACTER_NAME|survival_bonus}](~CHARACTER_NAME|survival)}}
```

## Saving throw

- Suggested that you turn on always roll twice
- Would be nice to add positive symbols in front of mods

```rmacro
/w @{CHARACTER_NAME|character_name}
  &{template:default}
  {{name=Saving throw}}
  {{Strength=[@{CHARACTER_NAME|strength_save_bonus}](~CHARACTER_NAME|strength_save)}}
  {{Dexterity=[@{CHARACTER_NAME|dexterity_save_bonus}](~CHARACTER_NAME|dexterity_save)}}
  {{Constitution=[@{CHARACTER_NAME|constitution_save_bonus}](~CHARACTER_NAME|constitution_save)}}
  {{Intelligence=[@{CHARACTER_NAME|intelligence_save_bonus}](~CHARACTER_NAME|intelligence_save)}}
  {{Wisdom=[@{CHARACTER_NAME|wisdom_save_bonus}](~CHARACTER_NAME|wisdom_save)}}
  {{Charisma=[@{CHARACTER_NAME|charisma_save_bonus}](~CHARACTER_NAME|charisma_save)}}
```

```rmacro
/w @{CHARACTER_NAME|character_name} &{template:default} {{name=Saving throw}} {{Strength=[@{CHARACTER_NAME|strength_save_bonus}](~CHARACTER_NAME|strength_save)}} {{Dexterity=[@{CHARACTER_NAME|dexterity_save_bonus}](~CHARACTER_NAME|dexterity_save)}} {{Constitution=[@{CHARACTER_NAME|constitution_save_bonus}](~CHARACTER_NAME|constitution_save)}} {{Intelligence=[@{CHARACTER_NAME|intelligence_save_bonus}](~CHARACTER_NAME|intelligence_save)}} {{Wisdom=[@{CHARACTER_NAME|wisdom_save_bonus}](~CHARACTER_NAME|wisdom_save)}} {{Charisma=[@{CHARACTER_NAME|charisma_save_bonus}](~CHARACTER_NAME|charisma_save)}}
```

## Cantrip

```rmacro
/w @{CHARACTER_NAME|character_name}
  &{template:default}
  {{name=Cantrip select}}
  {{Cast=
    [@{CHARACTER_NAME|repeating_spell-cantrip_$0_spellname}](~CHARACTER_NAME|repeating_spell-cantrip_$0_spell)
    [@{CHARACTER_NAME|repeating_spell-cantrip_$1_spellname}](~CHARACTER_NAME|repeating_spell-cantrip_$1_spell)
    [@{CHARACTER_NAME|repeating_spell-cantrip_$2_spellname}](~CHARACTER_NAME|repeating_spell-cantrip_$2_spell)
    [@{CHARACTER_NAME|repeating_spell-cantrip_$3_spellname}](~CHARACTER_NAME|repeating_spell-cantrip_$3_spell)
    [@{CHARACTER_NAME|repeating_spell-cantrip_$4_spellname}](~CHARACTER_NAME|repeating_spell-cantrip_$4_spell)
  }}
```

```rmacro
/w @{CHARACTER_NAME|character_name} &{template:default} {{name=Cantrip Select}} {{Cast= [@{CHARACTER_NAME|repeating_spell-cantrip_$0_spellname}](~CHARACTER_NAME|repeating_spell-cantrip_$0_spell) [@{CHARACTER_NAME|repeating_spell-cantrip_$1_spellname}](~CHARACTER_NAME|repeating_spell-cantrip_$1_spell) [@{CHARACTER_NAME|repeating_spell-cantrip_$2_spellname}](~CHARACTER_NAME|repeating_spell-cantrip_$2_spell) [@{CHARACTER_NAME|repeating_spell-cantrip_$3_spellname}](~CHARACTER_NAME|repeating_spell-cantrip_$3_spell) [@{CHARACTER_NAME|repeating_spell-cantrip_$4_spellname}](~CHARACTER_NAME|repeating_spell-cantrip_$4_spell) }}
```

## Level 1 spells

```rmacro
/w @{CHARACTER_NAME|character_name}
  &{template:default}
  {{title=Level 1 spell select}}
  {{Cast=
    [@{CHARACTER_NAME|repeating_spell-1_$0_spellname}](~CHARACTER_NAME|repeating_spell-1_$0_spell)
    [@{CHARACTER_NAME|repeating_spell-1_$1_spellname}](~CHARACTER_NAME|repeating_spell-1_$1_spell)
    [@{CHARACTER_NAME|repeating_spell-1_$2_spellname}](~CHARACTER_NAME|repeating_spell-1_$2_spell)
    [@{CHARACTER_NAME|repeating_spell-1_$3_spellname}](~CHARACTER_NAME|repeating_spell-1_$3_spell)
    [@{CHARACTER_NAME|repeating_spell-1_$4_spellname}](~CHARACTER_NAME|repeating_spell-1_$4_spell)
    [@{CHARACTER_NAME|repeating_spell-1_$5_spellname}](~CHARACTER_NAME|repeating_spell-1_$5_spell)
    [@{CHARACTER_NAME|repeating_spell-1_$6_spellname}](~CHARACTER_NAME|repeating_spell-1_$6_spell)
    [@{CHARACTER_NAME|repeating_spell-1_$7_spellname}](~CHARACTER_NAME|repeating_spell-1_$7_spell)
  }}
```

```rmacro
/w @{CHARACTER_NAME|character_name}&{template:default}{{title=Level 1 spell select}}{{Cast=[@{CHARACTER_NAME|repeating_spell-1_$0_spellname}](~CHARACTER_NAME|repeating_spell-1_$0_spell)[@{CHARACTER_NAME|repeating_spell-1_$1_spellname}](~CHARACTER_NAME|repeating_spell-1_$1_spell)[@{CHARACTER_NAME|repeating_spell-1_$2_spellname}](~CHARACTER_NAME|repeating_spell-1_$2_spell)[@{CHARACTER_NAME|repeating_spell-1_$3_spellname}](~CHARACTER_NAME|repeating_spell-1_$3_spell)[@{CHARACTER_NAME|repeating_spell-1_$4_spellname}](~CHARACTER_NAME|repeating_spell-1_$4_spell)[@{CHARACTER_NAME|repeating_spell-1_$5_spellname}](~CHARACTER_NAME|repeating_spell-1_$5_spell)[@{CHARACTER_NAME|repeating_spell-1_$6_spellname}](~CHARACTER_NAME|repeating_spell-1_$6_spell)[@{CHARACTER_NAME|repeating_spell-1_$7_spellname}](~CHARACTER_NAME|repeating_spell-1_$7_spell)}}
```

## Rebuke Death (whisper)

- Assumes a macro with ID `RebukeDeathPublic`

```rmacro
/w @{CHARACTER_NAME|character_name}
  &{template:traits}
  @{CHARACTER_NAME|charname_output}
  {{name=Rebuke Death}}
  {{source=Class: White Necromancer}}
  {{description=Also starting at 2nd level, you can use an action to heal a creature you can touch. The creature regains hit points equal to your Intelligence modifier + your wizard level (minimum of 1). This feature can restore a creature to no more than half its hit point maximum. Once a creature has regained hit points from this feature, it can’t do so again until it finishes a long rest. [Send to chat](!&#13;#RebukeDeathPublic) }}
```

## Rebuke Death

```rmacro
@{CHARACTER_NAME|wtype}&{template:traits} @{CHARACTER_NAME|charname_output} {{name=Rebuke Death}} {{source=Class: White Necromancer}} {{description=Also starting at 2nd level, you can use an action to heal a creature you can touch. The creature regains hit points equal to your Intelligence modifier + your wizard level (minimum of 1). This feature can restore a creature to no more than half its hit point maximum. Once a creature has regained hit points from this feature, it can’t do so again until it finishes a long rest. }}
```

## Telekinetic shove

```rmacro
&{template:dmg}
  {{savedesc=Telekinetic Shove}}
  {{desc=As a bonus action, you can try to telekinetically shove one creature you can see within 30 feet of you. When you do so, the target must succeed on a Strength saving throw (DC 8 + your proficiency bonus + the ability modifier of the score increased by this feat) or be moved 5 feet toward you or away from you. A creature can willingly fail this save.}}
  {{save=1}}
  {{saveattr=STR}}
  {{savedc=[[8+@{CHARACTER_NAME|pb}[Proficiency]+@{CHARACTER_NAME|wisdom_mod}[Wisdom]]]}}
```

```rmacro
&{template:dmg}{{savedesc=Telekinetic Shove}}{{desc=As a bonus action, you can try to telekinetically shove one creature you can see within 30 feet of you. When you do so, the target must succeed on a Strength saving throw (DC 8 + your proficiency bonus + the ability modifier of the score increased by this feat) or be moved 5 feet toward you or away from you. A creature can willingly fail this save.}}{{save=1}}{{saveattr=STR}}{{savedc=[[8+@{CHARACTER_NAME|pb}[Proficiency]+@{CHARACTER_NAME|wisdom_mod}[Wisdom]]]}}
```

## Spell slots

```rmacro
/w @{CHARACTER_NAME|character_name}
  &{template:default}
  {{name=Spell slots}}
  {{Level 1=[[@{CHARACTER_NAME|lvl1_slots_total}[Total slots] - @{CHARACTER_NAME|lvl1_slots_expended}[Used slots]]]}}
  {{Level 2=[[@{CHARACTER_NAME|lvl2_slots_total}[Total slots] - @{CHARACTER_NAME|lvl2_slots_expended}[Used slots]]]}}
  {{Level 3=[[@{CHARACTER_NAME|lvl3_slots_total}[Total slots] - @{CHARACTER_NAME|lvl3_slots_expended}[Used slots]]]}}
  {{Level 4=[[@{CHARACTER_NAME|lvl4_slots_total}[Total slots] - @{CHARACTER_NAME|lvl4_slots_expended}[Used slots]]]}}
  {{Level 5=[[@{CHARACTER_NAME|lvl5_slots_total}[Total slots] - @{CHARACTER_NAME|lvl5_slots_expended}[Used slots]]]}}
  {{Level 6=[[@{CHARACTER_NAME|lvl6_slots_total}[Total slots] - @{CHARACTER_NAME|lvl6_slots_expended}[Used slots]]]}}
  {{Level 7=[[@{CHARACTER_NAME|lvl7_slots_total}[Total slots] - @{CHARACTER_NAME|lvl7_slots_expended}[Used slots]]]}}
  {{Level 8=[[@{CHARACTER_NAME|lvl8_slots_total}[Total slots] - @{CHARACTER_NAME|lvl8_slots_expended}[Used slots]]]}}
  {{Level 9=[[@{CHARACTER_NAME|lvl9_slots_total}[Total slots] - @{CHARACTER_NAME|lvl9_slots_expended}[Used slots]]]}}
```

```rmacro
/w @{CHARACTER_NAME|character_name}&{template:default}{{name=Spell slots}}{{Level 1=[[@{CHARACTER_NAME|lvl1_slots_total}[Total slots] - @{CHARACTER_NAME|lvl1_slots_expended}[Used slots]]]}}{{Level 2=[[@{CHARACTER_NAME|lvl2_slots_total}[Total slots] - @{CHARACTER_NAME|lvl2_slots_expended}[Used slots]]]}}{{Level 3=[[@{CHARACTER_NAME|lvl3_slots_total}[Total slots] - @{CHARACTER_NAME|lvl3_slots_expended}[Used slots]]]}}{{Level 4=[[@{CHARACTER_NAME|lvl4_slots_total}[Total slots] - @{CHARACTER_NAME|lvl4_slots_expended}[Used slots]]]}}{{Level 5=[[@{CHARACTER_NAME|lvl5_slots_total}[Total slots] - @{CHARACTER_NAME|lvl5_slots_expended}[Used slots]]]}}{{Level 6=[[@{CHARACTER_NAME|lvl6_slots_total}[Total slots] - @{CHARACTER_NAME|lvl6_slots_expended}[Used slots]]]}}{{Level 7=[[@{CHARACTER_NAME|lvl7_slots_total}[Total slots] - @{CHARACTER_NAME|lvl7_slots_expended}[Used slots]]]}}{{Level 8=[[@{CHARACTER_NAME|lvl8_slots_total}[Total slots] - @{CHARACTER_NAME|lvl8_slots_expended}[Used slots]]]}}{{Level 9=[[@{CHARACTER_NAME|lvl9_slots_total}[Total slots] - @{CHARACTER_NAME|lvl9_slots_expended}[Used slots]]]}}
```

## Resistances

```rmacro
/w @{CHARACTER_NAME|character_name}
  &{template:default}
  {{name=Resistances & Advantages}}
  {{Resistances="Necrotic damage"}}
  {{Saving throw advantage="Poison, disease"}}
  {{Skill advantage="Religion checks to recall lore about deities of death, burial practices, and the afterlife."}}
```

```rmacro
/w @{CHARACTER_NAME|character_name} &{template:default} {{name=Resistances & Advantages}} {{Resistances="Necrotic damage"}} {{Saving throw advantage="Poison, disease"}} {{Skill advantage="Religion checks to recall lore about deities of death, burial practices, and the afterlife."}}
```

## Other skills

```rmacro
/w @{CHARACTER_NAME|character_name}
  &{template:default}
  {{name=Other skills}}
  {{Languages=Common, Dwarvish, Elven, Umbral}}
  {{Tools=Calligrapher's tools}}
  {{Weapons=Simple}}
```

```rmacro
/w @{CHARACTER_NAME|character_name}&{template:default}{{name=Other skills}}{{Languages=Common, Dwarvish, Elven, Umbral}}{{Tools=Calligrapher's tools}}{{Weapons=Simple}}
```

## Emote

```rmacro
/em *?{Mara...|sighs.}*
```
