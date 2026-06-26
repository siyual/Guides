# Ngai V25
The name of the game here is survival.  **MNK** is going to be the star of the show.  This is really not too difficult of a fight, you just need to keep your HP above 50% and be on top add maintenance and fetter dismissals.

Our composition was:
> MNK WHM WAR BRD COR RDM

## Buffs
**WHM**: `Protect`, `Shell`, `Barwater`, `Barpoison`, `Auspice`, `Boost-STR`, `Regen`

**RDM**: `Phalanx`, `Haste`

**COR**: Crooked `Chaos`, `Samurai`

**BRD**: `Scherzo`, `Water Carol`, `Water Carol 2`, `Minuet 5`, `Minuet 4`

**MNK**: `Boost` up to 3000 TP while buffing.

**WAR**: Get 3000 TP in the lobby on **Great Axe** to apply **Armor Break**, then switch to **Club**.

## Fight
Pull **Ngai** to a corner somewhere and have the **MNK** engage.  Coordinate with the **COR** to keep `Impetus` up fulltime.  The engaged set I used on **MNK** was the following:

```lua
sets.engaged.Ngai = 
{
    ammo	= "Coiste Bodhar",
    head	= Nyame_Head,
    body	= Nyame_Body,
    hands	= Nyame_Hand,
    legs	= MNK_Empy_Legs,
    feet	= Nyame_Feet,
    neck	= "Mnk. Nodowa +2",
    waist	= "Moonbow Belt +1",
    ear1	= "Sherida Earring",
    ear2	= "Schere Earring",
    ring1	= "Niqmaddu Ring",
    ring2	= "Shadow Ring",
    back	= AmbuCape_TP_STR,
}
```

The biggest problem you're going to have with **Ngai** is his instant-death moves.  The **MNK**'s HP needs to be kept above 50% at all times to avoid this!

The **WAR** should engage with `Club` (**Judgment**), and the **RDM** should also engage with `Club` (**Black Halo**).

When **Ngai** gets to 75%, the **WHM** should `Divine Seal` → `Full Cure` on the **MNK** and **Mystic Boon** to get MP back.  This will give the **MNK** a massive cureskin, and essentially negate **Mighty Strikes**.

If the **WHM** cannot do this again at 40%, the **MNK** should pop **Inner Strength** to stay alive.

When **Ngai** uses **Carcharian Verve**, this will proc a red <span style="color:red">**!!**</span> and spawn fetters.  The fetters **must** be cleared as quickly as possible.  The **Drown** effect is a massive DoT, but it also afflicts a staggering **STR -999**, effectively killing all of your damage output.

To remove the fetter and proc a blue <span style="color:blue">**!!**</span>, you need to time weaponskills among all party members.  The **MNK** should have a macro with a timer in party chat to coordinate this.  For example:

```
(Siyual) === GET READY TO WEAPONSKILL === <call3>
(Siyual) ■□□□ 3...
(Siyual) ■■□□ 2...
(Siyual) ■■■□ 1...
(Siyual) ■■■■ GO!!! <call17>
```

At the time specified, everyone should use a WS.  If done correctly, this will proc a blue <span style="color:blue">**!!**</span> and remove the fetters.

The **COR** needs to coordinate `Random Deal` and `Wild Card` to maximize `Impetus` and `Warcry` times.

Stay focused on heals and damage, and you'll get the win!