## Initiative

```rmacro
&{template:simple}
  {{rname=Initiative}}
  {{mod=Dex}}
  {{normal=1}}
  {{r1=[[d20+@{Mara Nawojka|initiative_bonus}[DEX] &{Mara Nawojka|tracker}]]}}
  {{charname=Mara}}
```

```rmacro
&{template:simple} {{rname=Initiative}} {{mod=Dex}} {{normal=1}} {{r1=[[d20+@{Mara Nawojka|initiative_bonus}[DEX] &{Mara Nawojka|tracker}]]}} {{charname=Mara}}
```

## Skill check

- Suggested that you turn on always roll twice
- Would be nice to add positive sybmols in front of mods

```rmacro
/w @{Mara Nawojka|character_name}
  &{template:default}
  {{name=Skill check}}
  {{Acrobatics=[@{Mara Nawojka|acrobatics_bonus}](~Mara Nawojka|acrobatics)}}
  {{Animal Handling=[@{Mara Nawojka|animal_handling_bonus}](~Mara Nawojka|animal_handling)}}
  {{Arcana=[@{Mara Nawojka|arcana_bonus}](~Mara Nawojka|arcana)}}
  {{Athletics=[@{Mara Nawojka|athletics_bonus}](~Mara Nawojka|athletics)}}
  {{Deception=[@{Mara Nawojka|deception_bonus}](~Mara Nawojka|deception)}}
  {{History=[@{Mara Nawojka|history_bonus}](~Mara Nawojka|history)}}
  {{Insight=[@{Mara Nawojka|insight_bonus}](~Mara Nawojka|insight)}}
  {{Intimidation=[@{Mara Nawojka|intimidation_bonus}](~Mara Nawojka|intimidation)}}
  {{Investigation=[@{Mara Nawojka|investigation_bonus}](~Mara Nawojka|investigation)}}
  {{Medicine=[@{Mara Nawojka|medicine_bonus}](~Mara Nawojka|medicine)}}
  {{Nature=[@{Mara Nawojka|nature_bonus}](~Mara Nawojka|nature)}}
  {{Perception=[@{Mara Nawojka|perception_bonus}](~Mara Nawojka|perception)}}
  {{Performance=[@{Mara Nawojka|performance_bonus}](~Mara Nawojka|performance)}}
  {{Persuasion=[@{Mara Nawojka|persuasion_bonus}](~Mara Nawojka|persuasion)}}
  {{Religion=[@{Mara Nawojka|religion_bonus}](~Mara Nawojka|religion)}}
  {{Sleight of hand=[@{Mara Nawojka|sleight_of_hand_bonus}](~Mara Nawojka|sleight_of_hand)}}
  {{Stealth=[@{Mara Nawojka|stealth_bonus}](~Mara Nawojka|stealth)}}
  {{Survival=[@{Mara Nawojka|survival_bonus}](~Mara Nawojka|survival)}}
```

```rmacro
/w @{Mara Nawojka|character_name} &{template:default} {{name=Skill check}} {{Acrobatics=[@{Mara Nawojka|acrobatics_bonus}](~Mara Nawojka|acrobatics)}} {{Animal Handling=[@{Mara Nawojka|animal_handling_bonus}](~Mara Nawojka|animal_handling)}} {{Arcana=[@{Mara Nawojka|arcana_bonus}](~Mara Nawojka|arcana)}} {{Athletics=[@{Mara Nawojka|athletics_bonus}](~Mara Nawojka|athletics)}} {{Deception=[@{Mara Nawojka|deception_bonus}](~Mara Nawojka|deception)}} {{History=[@{Mara Nawojka|history_bonus}](~Mara Nawojka|history)}} {{Insight=[@{Mara Nawojka|insight_bonus}](~Mara Nawojka|insight)}} {{Intimidation=[@{Mara Nawojka|intimidation_bonus}](~Mara Nawojka|intimidation)}} {{Investigation=[@{Mara Nawojka|investigation_bonus}](~Mara Nawojka|investigation)}} {{Medicine=[@{Mara Nawojka|medicine_bonus}](~Mara Nawojka|medicine)}} {{Nature=[@{Mara Nawojka|nature_bonus}](~Mara Nawojka|nature)}} {{Perception=[@{Mara Nawojka|perception_bonus}](~Mara Nawojka|perception)}} {{Performance=[@{Mara Nawojka|performance_bonus}](~Mara Nawojka|performance)}} {{Persuasion=[@{Mara Nawojka|persuasion_bonus}](~Mara Nawojka|persuasion)}} {{Religion=[@{Mara Nawojka|religion_bonus}](~Mara Nawojka|religion)}} {{Sleight of hand=[@{Mara Nawojka|sleight_of_hand_bonus}](~Mara Nawojka|sleight_of_hand)}} {{Stealth=[@{Mara Nawojka|stealth_bonus}](~Mara Nawojka|stealth)}} {{Survival=[@{Mara Nawojka|survival_bonus}](~Mara Nawojka|survival)}}
```

## Saving throw

- Suggested that you turn on always roll twice
- Would be nice to add positive symbols in front of mods

```rmacro
/w @{Mara Nawojka|character_name}
  &{template:default}
  {{name=Saving throw}}
  {{Strength=[@{Mara Nawojka|strength_save_bonus}](~Mara Nawojka|strength_save)}}
  {{Dexterity=[@{Mara Nawojka|dexterity_save_bonus}](~Mara Nawojka|dexterity_save)}}
  {{Constitution=[@{Mara Nawojka|constitution_save_bonus}](~Mara Nawojka|constitution_save)}}
  {{Intelligence=[@{Mara Nawojka|intelligence_save_bonus}](~Mara Nawojka|intelligence_save)}}
  {{Wisdom=[@{Mara Nawojka|wisdom_save_bonus}](~Mara Nawojka|wisdom_save)}}
  {{Charisma=[@{Mara Nawojka|charisma_save_bonus}](~Mara Nawojka|charisma_save)}}
```

```rmacro
/w @{Mara Nawojka|character_name} &{template:default} {{name=Saving throw}} {{Strength=[@{Mara Nawojka|strength_save_bonus}](~Mara Nawojka|strength_save)}} {{Dexterity=[@{Mara Nawojka|dexterity_save_bonus}](~Mara Nawojka|dexterity_save)}} {{Constitution=[@{Mara Nawojka|constitution_save_bonus}](~Mara Nawojka|constitution_save)}} {{Intelligence=[@{Mara Nawojka|intelligence_save_bonus}](~Mara Nawojka|intelligence_save)}} {{Wisdom=[@{Mara Nawojka|wisdom_save_bonus}](~Mara Nawojka|wisdom_save)}} {{Charisma=[@{Mara Nawojka|charisma_save_bonus}](~Mara Nawojka|charisma_save)}}
```

## Cantrip

```rmacro
/w @{Mara Nawojka|character_name}
  &{template:default}
  {{name=Cantrip select}}
  {{Cast=
    [@{Mara Nawojka|repeating_spell-cantrip_$0_spellname}](~Mara Nawojka|repeating_spell-cantrip_$0_spell)
    [@{Mara Nawojka|repeating_spell-cantrip_$1_spellname}](~Mara Nawojka|repeating_spell-cantrip_$1_spell)
    [@{Mara Nawojka|repeating_spell-cantrip_$2_spellname}](~Mara Nawojka|repeating_spell-cantrip_$2_spell)
    [@{Mara Nawojka|repeating_spell-cantrip_$3_spellname}](~Mara Nawojka|repeating_spell-cantrip_$3_spell)
    [@{Mara Nawojka|repeating_spell-cantrip_$4_spellname}](~Mara Nawojka|repeating_spell-cantrip_$4_spell)
  }}
```

```rmacro
/w @{Mara Nawojka|character_name} &{template:default} {{name=Cantrip Select}} {{Cast= [@{Mara Nawojka|repeating_spell-cantrip_$0_spellname}](~Mara Nawojka|repeating_spell-cantrip_$0_spell) [@{Mara Nawojka|repeating_spell-cantrip_$1_spellname}](~Mara Nawojka|repeating_spell-cantrip_$1_spell) [@{Mara Nawojka|repeating_spell-cantrip_$2_spellname}](~Mara Nawojka|repeating_spell-cantrip_$2_spell) [@{Mara Nawojka|repeating_spell-cantrip_$3_spellname}](~Mara Nawojka|repeating_spell-cantrip_$3_spell) [@{Mara Nawojka|repeating_spell-cantrip_$4_spellname}](~Mara Nawojka|repeating_spell-cantrip_$4_spell) }}
```

## Level 1 spells

```rmacro
/w @{Mara Nawojka|character_name}
  &{template:default}
  {{title=Level 1 spell select}}
  {{Cast=
    [@{Mara Nawojka|repeating_spell-1_$0_spellname}](~Mara Nawojka|repeating_spell-1_$0_spell)
    [@{Mara Nawojka|repeating_spell-1_$1_spellname}](~Mara Nawojka|repeating_spell-1_$1_spell)
    [@{Mara Nawojka|repeating_spell-1_$2_spellname}](~Mara Nawojka|repeating_spell-1_$2_spell)
    [@{Mara Nawojka|repeating_spell-1_$3_spellname}](~Mara Nawojka|repeating_spell-1_$3_spell)
    [@{Mara Nawojka|repeating_spell-1_$4_spellname}](~Mara Nawojka|repeating_spell-1_$4_spell)
    [@{Mara Nawojka|repeating_spell-1_$5_spellname}](~Mara Nawojka|repeating_spell-1_$5_spell)
    [@{Mara Nawojka|repeating_spell-1_$6_spellname}](~Mara Nawojka|repeating_spell-1_$6_spell)
    [@{Mara Nawojka|repeating_spell-1_$7_spellname}](~Mara Nawojka|repeating_spell-1_$7_spell)
  }}
```

```rmacro
/w @{Mara Nawojka|character_name}&{template:default}{{title=Level 1 spell select}}{{Cast=[@{Mara Nawojka|repeating_spell-1_$0_spellname}](~Mara Nawojka|repeating_spell-1_$0_spell)[@{Mara Nawojka|repeating_spell-1_$1_spellname}](~Mara Nawojka|repeating_spell-1_$1_spell)[@{Mara Nawojka|repeating_spell-1_$2_spellname}](~Mara Nawojka|repeating_spell-1_$2_spell)[@{Mara Nawojka|repeating_spell-1_$3_spellname}](~Mara Nawojka|repeating_spell-1_$3_spell)[@{Mara Nawojka|repeating_spell-1_$4_spellname}](~Mara Nawojka|repeating_spell-1_$4_spell)[@{Mara Nawojka|repeating_spell-1_$5_spellname}](~Mara Nawojka|repeating_spell-1_$5_spell)[@{Mara Nawojka|repeating_spell-1_$6_spellname}](~Mara Nawojka|repeating_spell-1_$6_spell)[@{Mara Nawojka|repeating_spell-1_$7_spellname}](~Mara Nawojka|repeating_spell-1_$7_spell)}}
```

## Rebuke Death (whisper)

- Assumes a macro with ID `RebukeDeathPublic`

```rmacro
/w @{Mara Nawojka|character_name}
  &{template:traits}
  @{Mara Nawojka|charname_output}
  {{name=Rebuke Death}}
  {{source=Class: White Necromancer}}
  {{description=Also starting at 2nd level, you can use an action to heal a creature you can touch. The creature regains hit points equal to your Intelligence modifier + your wizard level (minimum of 1). This feature can restore a creature to no more than half its hit point maximum. Once a creature has regained hit points from this feature, it can’t do so again until it finishes a long rest. [Send to chat](!&#13;#RebukeDeathPublic) }}
```

## Rebuke Death

```rmacro
@{Mara Nawojka|wtype}&{template:traits} @{Mara Nawojka|charname_output} {{name=Rebuke Death}} {{source=Class: White Necromancer}} {{description=Also starting at 2nd level, you can use an action to heal a creature you can touch. The creature regains hit points equal to your Intelligence modifier + your wizard level (minimum of 1). This feature can restore a creature to no more than half its hit point maximum. Once a creature has regained hit points from this feature, it can’t do so again until it finishes a long rest. }}
```

## Telekinetic shove

```rmacro
&{template:dmg}
  {{savedesc=Telekinetic Shove}}
  {{desc=As a bonus action, you can try to telekinetically shove one creature you can see within 30 feet of you. When you do so, the target must succeed on a Strength saving throw (DC 8 + your proficiency bonus + the ability modifier of the score increased by this feat) or be moved 5 feet toward you or away from you. A creature can willingly fail this save.}}
  {{save=1}}
  {{saveattr=STR}}
  {{savedc=[[8+@{Mara Nawojka|pb}[Proficiency]+@{Mara Nawojka|wisdom_mod}[Wisdom]]]}}
```

```rmacro
&{template:dmg}{{savedesc=Telekinetic Shove}}{{desc=As a bonus action, you can try to telekinetically shove one creature you can see within 30 feet of you. When you do so, the target must succeed on a Strength saving throw (DC 8 + your proficiency bonus + the ability modifier of the score increased by this feat) or be moved 5 feet toward you or away from you. A creature can willingly fail this save.}}{{save=1}}{{saveattr=STR}}{{savedc=[[8+@{Mara Nawojka|pb}[Proficiency]+@{Mara Nawojka|wisdom_mod}[Wisdom]]]}}
```

## Spell slots

```rmacro
/w @{Mara Nawojka|character_name}
  &{template:default}
  {{name=Spell slots}}
  {{Level 1=[[@{Mara Nawojka|lvl1_slots_total}[Total slots] - @{Mara Nawojka|lvl1_slots_expended}[Used slots]]]}}
  {{Level 2=[[@{Mara Nawojka|lvl2_slots_total}[Total slots] - @{Mara Nawojka|lvl2_slots_expended}[Used slots]]]}}
  {{Level 3=[[@{Mara Nawojka|lvl3_slots_total}[Total slots] - @{Mara Nawojka|lvl3_slots_expended}[Used slots]]]}}
  {{Level 4=[[@{Mara Nawojka|lvl4_slots_total}[Total slots] - @{Mara Nawojka|lvl4_slots_expended}[Used slots]]]}}
  {{Level 5=[[@{Mara Nawojka|lvl5_slots_total}[Total slots] - @{Mara Nawojka|lvl5_slots_expended}[Used slots]]]}}
  {{Level 6=[[@{Mara Nawojka|lvl6_slots_total}[Total slots] - @{Mara Nawojka|lvl6_slots_expended}[Used slots]]]}}
  {{Level 7=[[@{Mara Nawojka|lvl7_slots_total}[Total slots] - @{Mara Nawojka|lvl7_slots_expended}[Used slots]]]}}
  {{Level 8=[[@{Mara Nawojka|lvl8_slots_total}[Total slots] - @{Mara Nawojka|lvl8_slots_expended}[Used slots]]]}}
  {{Level 9=[[@{Mara Nawojka|lvl9_slots_total}[Total slots] - @{Mara Nawojka|lvl9_slots_expended}[Used slots]]]}}
```

```rmacro
/w @{Mara Nawojka|character_name}&{template:default}{{name=Spell slots}}{{Level 1=[[@{Mara Nawojka|lvl1_slots_total}[Total slots] - @{Mara Nawojka|lvl1_slots_expended}[Used slots]]]}}{{Level 2=[[@{Mara Nawojka|lvl2_slots_total}[Total slots] - @{Mara Nawojka|lvl2_slots_expended}[Used slots]]]}}{{Level 3=[[@{Mara Nawojka|lvl3_slots_total}[Total slots] - @{Mara Nawojka|lvl3_slots_expended}[Used slots]]]}}{{Level 4=[[@{Mara Nawojka|lvl4_slots_total}[Total slots] - @{Mara Nawojka|lvl4_slots_expended}[Used slots]]]}}{{Level 5=[[@{Mara Nawojka|lvl5_slots_total}[Total slots] - @{Mara Nawojka|lvl5_slots_expended}[Used slots]]]}}{{Level 6=[[@{Mara Nawojka|lvl6_slots_total}[Total slots] - @{Mara Nawojka|lvl6_slots_expended}[Used slots]]]}}{{Level 7=[[@{Mara Nawojka|lvl7_slots_total}[Total slots] - @{Mara Nawojka|lvl7_slots_expended}[Used slots]]]}}{{Level 8=[[@{Mara Nawojka|lvl8_slots_total}[Total slots] - @{Mara Nawojka|lvl8_slots_expended}[Used slots]]]}}{{Level 9=[[@{Mara Nawojka|lvl9_slots_total}[Total slots] - @{Mara Nawojka|lvl9_slots_expended}[Used slots]]]}}
```

## Resistances

```rmacro
/w @{Mara Nawojka|character_name}
  &{template:default}
  {{name=Resistances & Advantages}}
  {{Resistances="Necrotic damage"}}
  {{Saving throw advantage="Poison, disease"}}
  {{Skill advantage="Religion checks to recall lore about deities of death, burial practices, and the afterlife."}}
```

```rmacro
/w @{Mara Nawojka|character_name} &{template:default} {{name=Resistances & Advantages}} {{Resistances="Necrotic damage"}} {{Saving throw advantage="Poison, disease"}} {{Skill advantage="Religion checks to recall lore about deities of death, burial practices, and the afterlife."}}
```

## Other skills

```rmacro
/w @{Mara Nawojka|character_name}
  &{template:default}
  {{name=Other skills}}
  {{Languages=Common, Dwarvish, Elven, Umbral}}
  {{Tools=Calligrapher's tools}}
  {{Weapons=Simple}}
```

```rmacro
/w @{Mara Nawojka|character_name}&{template:default}{{name=Other skills}}{{Languages=Common, Dwarvish, Elven, Umbral}}{{Tools=Calligrapher's tools}}{{Weapons=Simple}}
```

## Emote

```rmacro
/em *?{Mara...|sighs.}*
```
