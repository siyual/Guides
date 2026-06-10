# Ongo V25

This used to be the most frustrating NM in the land of Gaol, but V25 is actually surprisingly one of the easiest.  This isn't due to a reduction in difficulty, but rather an increase in difficulty that begged for a multi Key Item approach.  Splitting this into multiple Key Items for previous Veng levels didn't really make the fight too much easier to warrant taking the extra time, but for V25, it's begging for it, and honestly, it makes it so much easier.

This fight is going to be a **three** Key Item approach.  The following is the party composition we used, (vertically stacked to match each player):

```
KI-1 : BST NIN PLD BLU RDM SMN
KI-2 : PUP WHM DRG DNC WAR GEO
KI-3 : BRD SCH RUN COR BLM THF
```

**SP Usage**:

| Entry | Player 1 | Player 2 | Player 3 | Player 4 | Player 5 | Player 6 | 
| ----------- | ----------- | ----------- | ----------- | ----------- | ----------- | ----------- |
| #1 | BST | NIN | PLD | BLU | RDM | SMN |
| #1 | | | | | SP2 | |
| #2 | PUP | WHM | DRG | DNC | WAR | GEO |
| #2 | | | | | | SP1 |
| #3 | BRD | SCH | RUN | COR | BLM | THF |
| #3 | SP1, SP2 | SP1, SP2 | | SP1 | SP1, SP2 | SP2 |

In our party composition, Player 3 and Player 4 never need to use their SP2, so after the first Key Item, they both used **Cutting Cards** on Player 5, so that they would have access to their SP2 on the 3rd entry.

There's a lot of wiggle room here; the only SP that's really required before the last Key Item is **Stymie**.  

## Key Item #1

The goal of this entry is to get Ongo down to at least 74%.  Getting it lower is nice, but not required here.  This is honestly the hardest part of the entire fight.

Everyone needs to have an idle TP Regain set.  **NIN** has a *massive* amount of natural TP Regain, so they will be part of every skillchain.  Everyone else needs to have a ton of **[Frontier Sodas](https://www.bg-wiki.com/ffxi/Frontier_Soda)** to give TP.  The **SMN** and **BST** need to be constaintly draining Ongo's TP.  Everyone else needs to coordinate doing **Scission**, **Gravitation**, or **Darkness** skillchains, however they need to with the **NIN**.

The **BLU** will need to use **Burst Affinity** every time it's available and Magic Burst `Entomb`.  **RDM** needs to use `Enstone` and go ham on Ongo.  The only source of damage is going to be Magic Bursts and En-spell damage.  It's fine for everyone to melee Ongo, since he takes 0 damage from physical attacks.

The **PLD** is the main tank and healer.  The **NIN** is going to be focused on skillchains and magic bursts.

At the start, the **RDM** needs to get a **Stymie** `Frazzle III` on Ongo.  **This is critical.**

The **SMN** needs to primarily focus on wiping TP, but being part of skillchains and/or magic bursts when it can be afforded.  

**BST** needs to focus primarily on wiping TP, but also closing `Darkness` when they have TP.  **Cloudsplitter** was my WS of choice here, since it cannot miss.  Even though it's thunder-based, it does not heal Ongo unless it has fetters out.  And if it has fetters out, you've already lost.  The leech is good for `Killer Instinct` as well against Ongo.

That's basically it.  This will be the largest hurdle to clear.  Get the add to come out and you have accomplished your goal here.  Fail to do so, and there's no point in continuing.

## Key Item #2

This entry has a very simple goal, and surprisingly it has nothing to do with Ongo.  The goal on this entry is just to kill the add.  That's it.

The main tank for Ongo is going to be the **PUP**.  Below are the attachments used and gear equipped:

**Automaton** :
```xml
<ongo>
    <frame>valoredge frame</frame>
    <head>soulsoother head</head>
    <slot01>armor plate iii</slot01>
    <slot02>strobe ii</slot02>
    <slot03>shock absorber ii</slot03>
    <slot04>mana jammer iv</slot04>
    <slot05>mana jammer iii</slot05>
    <slot06>steam jacket</slot06>
    <slot07>shock absorber</slot07>
    <slot08>shock absorber iii</slot08>
    <slot09>auto-repair kit iv</slot09>
    <slot10>optic fiber</slot10>
    <slot11>optic fiber ii</slot11>
    <slot12>eraser</slot12>
</ongo>
```

**Master** :
```lua
OngoIdle = 
{
    main	= "Ohrmazd",
    range	= Animator_Melee,
    head	= "Anwig Salade",
    body	= TaeonBody_DT,
    hands	= TaeonHand_DT,
    legs	= TaeonLegs_DT,
    feet	= TaeonFeet_DT,
    neck	= "Shepherd's Chain",
    waist	= "Isa Belt",
    ear1	= "Enmerkar Earring",
    ear2	= "Rimeice Earring",
    ring1	= "Cath Palug Ring",
    ring2	= "Murky Ring",
    back	= AmbuCape_TP,
}

Augments:
TaeonBody_DT    = { name="Taeon Tabard", augments={'Pet: Mag. Evasion+24','Pet: "Regen"+3','Pet: Damage taken -4%',}}
TaeonHand_DT	= { name="Taeon Gloves", augments={'Pet: Mag. Evasion+25','Pet: "Regen"+3','Pet: Damage taken -4%',}}
TaeonLegs_DT	= { name="Taeon Tights", augments={'Pet: Mag. Evasion+22','Pet: "Regen"+3','Pet: Damage taken -4%',}}
TaeonFeet_DT	= { name="Taeon Boots", augments={'Pet: Mag. Evasion+23','Pet: "Regen"+3','Pet: Damage taken -4%',}}
```

**Maneuvers** :
```
Earth → Light → Fire
```

You may need to adjust the Maneuvers a bit.  `Fire` will be needed for `Provoke`, but if you start taking large amounts of fetter damage, you may need to sub out `Earth` for `Water`.

**[PUP Ongo Tank Sample Video](https://youtu.be/mvBKtFaUShQ)**

The **PUP** will need to stay out of range, but close enough to read the WS usage.  Every time Ongo uses `Crashing Thunder`, the add will have all debuffs wiped.  You will need to maintain `Fire Maneuvers` to keep the puppet using `Provoke` on Ongo to prevent it from running downstairs.

As for everyone else, when the fight starts, the puppet will get hate and the add will spawn (if you only got Ongo to 74% in the first Key Item, have the **WHM** cast `Holy` or something to coax it out).  Pull the add to the bottom of the stairs, and everyone else kill it with piercing while the **PUP** holds Ongo up top.  Use `Bolster` if you have to, but try to avoid using SPs on this one.  It should be fairly straight-forward.

Once the add is dead, just let the puppet tank Ongo until the timeout.  It's fine if he regenerates to full, the third entry will be unaffected.

## Key Item #3

At this point, Ongo already has a chunk of health missing, and the first add is dead.  From this point forward, this is just a standard V20 Ongo strategy.  He will still SP at 39%, and will still summon another add at that point, but it should be dealt with the exact same way you have prior to this point.  There are many strategies, but this is the one we used:

### Buffs

**BRD** : **Soul Voice** → **Clarion Call** (*Do not use **NiTro** yet*):
1. `Victory March`
2. `Mage's Ballad III`
3. `Mage's Ballad II`
4. `Sage Etude`
5. `Learned Etude`
6. `Foe Sirvente` → **RUN**

**SCH** : `Protect`, `Shell`, `Regen`, `Sandstorm II`, `Klimaform`\
**COR** : `Wizard`, `Warlock`

**RUN** goes in and gets hate.  While the rest get positioned.  

**SCH** needs to do `Gravitation` first and the **BLM** magic bursts `Impact`, and the **COR** extends to `Darkness` where the **SCH** magic bursts `Geohelix II`.

After the initial burst setup, start the standard magic burst rotation.  **BLM** needs to apply `Stoneja` as often as possible to maintain the 25% Earth Damage boost.  **COR** should use `Earth Shot` strategically to enhance the magic bursts.

Our preferred skillchain was:
```
Aero → Noctohelix → Rudra's Storm → Wildfire
```

When there is 1 minute remaining on **Soul Voice**, the **BRD** needs to pop **NiTro** and resing:
1. `Victory March`
2. `Mage's Ballad III`
3. `Mage's Ballad II`
4. `Sage Etude`
5. `Learned Etude`

Sing the following on Ongo:

6. `Earth Threnody II` → Ongo
7. `Pining Nocturne` → Ongo
8. `Carnage Elegy` → Ongo

Run over to the **RUN** and continue singing:

9. `Honor March`
10. `Mage's Ballad III`
11. `Knight's Minne V`
12. `Lightning Carol`
13. `Foe Sirvente`

After the last song, move out of AoE range, and continue singing on Ongo to build hate using `Lullaby` and `Virelai`.

When Ongo is nearing the 40% mark, the **SCH** should SP2 and put all hate on the **RUN**, and let the **BLM** push him over the edge to get the add out.  The **BLM** should use **Mana Wall** before the add comes out as a safety measure, and **Enmity Douse** after it's popped to ensure the hate goes to the **BRD**.  

The **BRD** should claim the add with `Virelai` and take the add down the stairs to kite in circles in the open space below until the battle has concluded.

Meanwhile, upstairs, after the add has been removed, the **THF** should **Larceny** the SP off Ongo, and continue the volleys of magic bursts.

**Important**: Throughout the run, the **BLM** and **RUN** must coordinate usage of **Rayke**, **Gambit**, and **Subtle Sorcery**.  Maximize the time you have these up, and don't overlap usage.  When then **BLM** has **Subtle Sorcery** up, they should get a fresh `Burn` and `Impact` on when they can, but focus on just spamming spells.

**COR** needs to **Random Deal** and **Wild Card** where appropriate.

Overall, this should be a pretty smooth fight.  There are other strategies for clearing in 1 Key Item, but this will be consistent with previous strategies, and has a *lot* of wiggle room in regards to time management.  

Our clear had over 10 minutes left on the clock.