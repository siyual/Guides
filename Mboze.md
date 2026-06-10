# Mboze V25

This is arguably the most difficult fight of all V25 NMs.  One can make a solid case for Arebati being harder, but this is certainly the most infuriating.  This requires a two Key Item approach, and your success is never guaranteed.  The sheer difficulty of this fight is that you can never let Mboze ever get a WS off.  He has six different TP moves that he can use, and only **two** of them do not result in a full wipe.

**<ins>If you let him get TP, there is only a 33.33% (repeating, of course) chance of survival.</ins>**

That said, let's go into the strategy.

This is a two Key Item approach, and our winning composition used the following (vertically stacked to match each player):

```
KI-1 : WAR SMN BST RUN GEO SCH
KI-2 : BRD WHM COR DRK RDM BLU
```

**SP Usage**:

| Entry | Player 1 | Player 2 | Player 3 | Player 4 | Player 5 | Player 6 | 
| ----------- | ----------- | ----------- | ----------- | ----------- | ----------- | ----------- |
| #1 | WAR | SMN | BST | RUN | GEO | SCH |
| #1 | |  | |  | SP1 | SP1 |
| #2 | BRD | WHM | COR | DRK | RDM | BLU |
| #2 | SP1, SP2 | As needed | SP1 | SP2 | SP2 | SP2 |

**Note:** You have some wiggle room here for which SPs can and can't be used.  You could potentially have the **WAR** and **DRK** be the same player, and doing so would allow for **Mighty Strikes** to be used in the first Key Item.  We did not have that option when we did the fight.

## Key Item #1

The goal of the first Key Item is to get it to 69% or lower.  74% is the absolute max his health can be - if you do not get him to 74%, don't bother continuing.  You have to get the Add out, and ideally it needs to come out on pull.

The strategy for this is pretty straight-forward: the **WAR** will be the only one engaged doing damage, and the **SMN** and **BST** coordinate TP wipes between `Cait Sith` and `Fatso Fargann`.

### Lobby (Before Entry)
Have someone change to **COR** and give a **Tactician's Roll** to let the **WAR** build up to 3000 TP.  They need this TP on a <span style="color:cyan">**Great Sword**</span>.

The **BST** needs to call a beetle pet (`Hurler Percival`) in the lobby, and have the **COR** use **Random Deal** to reset the timers.

Have a **GEO** **Entrust** the following spells:
- `Indi-STR` → **WAR**
- `Indi-Frailty` → **RUN**
- `Indi-Haste` → **SCH**
- `Indi-Refresh` → **SMN**
- `Indi-AGI` → **BST**

The **GEO** will need to change subjobs with the moogle between each **Entrust** to reset the timer.  When the buff is applied to a player, they need to click on the entry pole, but don't enter.  Being in the menu will pause the **Entrust** timer and allow the full duration upon entry.  When the battlefield is entered, each player will need to cancel out of the menu to be warped to the arena.

### Buffs

**SMN** : `Ecliptic Howl`, `Hastega II`, `Crystal Blessing`, `Crimson Howl`\
**SCH** : `Protect`, `Shell`, `Regen`, `Windstorm II` → **WAR**, `Animus Minuo` → **WAR**, `Adloquium` → **WAR**\
**GEO** : `Indi-Barrier`, `Geo-Fury`

### Fight

The **RUN** will pull Mboze and establish hate.  Use **Gambit** and **Rayke**, and the **WAR** should use **Tomahawk**, then open with **Armor Break**.

The **BST** should use **Killer Instict** with a Beetle pet, then dismiss it and summon the Leech.

Now, here's the fun.  At V25, Mboze builds resistances to successive weapon skills, so you need to get creative here.  What I found worked best was to use both <span style="color:cyan">**Sword**</span> and <span style="color:salmon">**Axe**</span>.  You will need to alternate between both <span style="color:cyan">**Savage Blade**</span> and <span style="color:salmon">**Calamity**</span>.

I did this by defining a `Sword` and `Axe` weapon set in gearswap, and my macros were set up like this:

<span style="color:cyan">**Savage Blade**</span>

```
/ws "Savage Blade" <t>
/con gs c set weapons Axe
```

<span style="color:salmon">**Calamity**</span>

```
/ws "Calamity" <t>
/con gs c set weapons Sword
```

I also use **[Selindrile's Gearswap](https://github.com/Selindrile/GearSwap)**, and define macro pages per weapon type via:

```lua
weapons_pagelist = 
{
    ['Sword']	= {6, 13},
    ['Axe']		= {10, 13},
}
```

This will automatically change your macro page based on the selected weapon set.  And finally, keeping both <span style="color:cyan">**Savage Blade**</span> and <span style="color:salmon">**Calamity**</span> on the same macro chord (e.g. `ALT 1` for both) takes all of the guesswork out.

**Important:** You *need* to be capped `Subtle Blow` on **WAR**.  Period, full stop.  Farm a `Dagon Breastplate` if you have to.

The following are the TP and WS sets I used:

```lua
Armor Break = 
{
    ammo	= "Pemphredo Tathlum",
    head	= WAR_Empy_Head,
    body	= WAR_Empy_Body,
    hands	= WAR_Empy_Hand,
    legs	= WAR_Empy_Legs,
    feet	= WAR_Empy_Feet,
    neck	= "Fotia Gorget",
    waist	= "Fotia Belt",
    ear1	= "Crepuscular Earring",
    ear2	= "Dignitary's Earring",
    ring1	= "Metamorph Ring +1",
    ring2	= "Cornelia's Ring",
    back	= AmbuCape_MD,
}

Savage Blade = 
{
    ammo	= "Knobkierrie",
    head	= WAR_Relic_Head,
    body	= Nyame_Body,
    hands	= WAR_Empy_Hand,
    legs	= Nyame_Legs,
    feet	= Nyame_Feet,
    neck	= "War. Beads +2",
    waist	= "Sailfi Belt +1",
    ear1	= "Hoxne Earring",
    ear2	= "Moonshade Earring",
    ring1	= "Regal Ring",
    ring2	= "Cornelia's Ring",
    back	= AmbuCape_WS,	
}

Calamity = 
{
    ammo	= "Knobkierrie",
    head	= WAR_Relic_Head,
    body	= Nyame_Body,
    hands	= WAR_Empy_Hand,
    legs	= Nyame_Legs,
    feet	= Nyame_Feet,
    neck	= "War. Beads +2",
    waist	= "Sailfi Belt +1",
    ear1	= "Hoxne Earring",
    ear2	= "Thrud Earring",
    ring1	= "Regal Ring",
    ring2	= "Cornelia's Ring",
    back	= AmbuCape_WS,	
}

TP = 
{
    ammo	= "Coiste Bodhar",
    head	= Sakpata_Head,
    body	= "Dagon Breastplate",
    hands	= Sakpata_Hand,
    legs	= WAR_Empy_Legs,
    feet	= Sakpata_Feet,
    neck	= "Bathy Choker +1",
    waist	= "Ioskeha Belt +1",
    ear1	= "Schere Earring",
    ear2	= WAR_Empy_Ear2,
    ring1	= "Niqmaddu Ring",
    ring2	= ChirichRing_Ring2,
    back	= AmbuCape_TP,
}
```

Alternate <span style="color:cyan">**Savage Blade**</span> and <span style="color:salmon">**Calamity**</span> on Mboze and focus on pushing him as low as you can.  Be in communication with the **SMN** and **BST**.  If they start reporting very high TP drains, turn for a bit to get the TP under control.  Use **Warcry** and **Blood Rage** only once in the higher percents.  You don't want it to be on cooldown when you push it to 74%.

As you near 74%, turn a bit and let the **SMN** reapply buffs.  When they're done and back on TP wiping duties, push it to 74% and let it invicible.  Use **Provoke** on the add - the **WAR** should already be second on the hate list, so it should firmly be on the **WAR**, but just in case.

Don't bother switching to TP on the add here.  Just keep doing what you're doing.  Once **Invincible** wears off, pop **Berserk**, **Warcry**, **Bolster**, and tear Mboze a new asshole.  If you can use **Mighty Strikes** with your party composition, use it here.  Your goal is to push it to at least 69%, but as low as possible.

Our record on KI 1 was 49%.  The more you push, the easier the next round will be.  It's OK if it gets off a WS at this point.  You've accomplished your mission of getting it to at least 69%.  Staying alive is ideal, but it's not a run ender if he decides to put your party on a T-Shirt.

## Key Item #2

You've made it through the free trial.  Now, the real game begins.

In this Key Item, **everyone** will need to engage on the add, but WS on Mboze.  This is absolutely critical.  The easiest way I've found to do this is with the following macros:

**Setting Target to Mboze**:
```
/aim <stnpc>
```

Hitting this macro,tabbing over, and selecting Mboze will set your `<lastst>` target to be Mboze.

Your WS macro should then just be:
```
/ws "Savage Blade" <lastst>
```

Everyone should configure their macros this way.  It lets you stay engaged on the Snapweed while also correctly targeting Mboze for whatever you need to do.

### Buffs

**BRD** : Get dummy songs up first.  Hold off on **NiTro** until the **COR** finishes the second roll.\
**WHM** : `Protect`, `Shell`, `Regen`, `Auspice`\
**RDM** : `Haste`, `Refresh`, `Phalanx`\
**COR** : `Gallant's Roll` → **Crooked** `Chaos Roll`

After the **COR** finishes the second roll, the **BRD** needs to pop **NiTro** and sing songs in the following order:
1. `Mage's Ballad III`
2. `Mage's Ballad II`
3. `Knight's Minne V`
4. `Knight's Minne IV`
5. `Honor March`

Pause here and let the **WHM** run out of range, then continue:

6. `Valor Minuet V`
7. `Valor Minuet IV`
8. `Valor Minuet III`
9. `Aria` or `Herculean Etude`

After the **WHM** runs out of range, the **COR** needs to do the last roll: **Samurai Roll**.

Once the songs are done, the **BRD** runs upstairs and pulls with `Wind Threnody II`.  When downstairs, put `Elegy` on the Snapweed.

**RDM** needs to `Silence` Mboze, and enfeeble the shit out of the add.\
The **DRK** needs to get `Armor Break` on Mboze.

After that, engage the Snapweed, set your `<st>` target to Mboze, and go to work.  

The **BLU** is going to be extremely busy spamming TP reset moves on Mboze while also buffing and doing damage.  

**WHM** needs to focus on keeping everyone alive and keeping `Auspice` up.

The second add will come out at 39%, along with Mboze using `Invincible` again.

When the second add comes out, the **RDM** needs to SP2 and `Sleep II` the second add.  Stay focused and wait for invicible to wear off.  Once it's off, continue pushing.

When you get down to about 10%, this is a critical HP moment.  You can't afford Mboze getting 1000 TP, as it will **always** use a TP move when it gets 1000 at this point.  The **DRK** should SP2 here and engage directly on Mboze.  **Soul Enslavement** will keep his TP at bay while the rest continue pouring in the gasoline.

When **Soul Enslavement** wears off, the **DRK** needs to be back on the add.  At this point, I would advise the **BRD** and **RDM** disengage to avoid feeding Mboze too much TP while its HP is critical.

With a little luck and perseverance, he'll go down.

The following is a video recording of a heartbreaking 1% loss:\
[Recording of Mboze V25 (WAR & BRD Perspective)](https://www.youtube.com/watch?v=D_xm3N01ZJE)