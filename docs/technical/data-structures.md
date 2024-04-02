# Datenstrukturen

Auf dieser Seite werden die Datenstrukturen zur Nutzung in Datenbanken/Programmlogik.

## Characterbogen Datenstruktur

Zur Dartellung von Charakteren wird diese Struktur verwendet. Die Struktur beinhaltet nicht alles, was auf einem Characterbogen

``` 
    CharId: guid
CharName: string
Race: guid
Class: guid
Level: int
Alignment: string
Background: string

GameStats
    Base
        Str: int
        Dex: int
        Con: int
        Int: int
        Wis: int
        Chr: int
    ProficiencyBonus: int
    Skills
        Acrobatics: bool
        Animal Handling: bool
        Arcana: bool
        Athletics: bool
        Deception: bool
        History: bool
        Insight: bool
        Intimidation: bool
        Investigation: bool
        Medicine: bool
        Nature: bool
        ...
    CombatStats
        ArmorClass: int
        HitPoints: int
        Speed: int
    Languages: guid[]
    Wallet
        Copper: int
        Silver: int
        Gold: int

AppearanceStats
    Age: int
    Height: int
    Weight: int
    Eyes: string
    Skin: string
    Hair: string

Equipment:
    Item0
        Id: guid
        Name: string
        Description: string
        Effects
            Effect0
                Stat: string
                Modifier: int
            Effect1
                Stat: string
                Modifier: int
            ...

Spells
    Lvl0
        Slots: int
        Spells
            Spell0
                ID: guid
                Name: string
                Description: string
            Spell1
                ID: guid
                Name: string
                Description: string
    Lvl1
        Slots: int
        Spells
            Spell0
                ID: guid
                Name: string
                Description: string
            Spell1
                ID: guid
                Name: string
                Description: string
    Lvl2
        Slots: int
        Spells
            Spell0
                ID: guid
                Name: string
                Description: string
            Spell1
                ID: guid
                Name: string
                Description: string
    Lvl3
        Slots: int
        Spells
            Spell0
                ID: guid
                Name: string
                Description: string
            Spell1
                ID: guid
                Name: string
                Description: string
            ...  
    ...

Traits
    Trait0
        ID: guid
        Name: string
        Description: string
    Trait1
        ID: guid
        Name: string
        Description: string
    ...
    
Inventory
    Item0
        ID: guid
        Name: string
        Description: string
        Weight: string
        Worth: string
    Item1
        ID: guid
        Name: string
        Description: string
        Weight: string
        Worth: string
        ...
```
