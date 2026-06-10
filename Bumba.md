# Bumba V25

This is probably the most removed fight as far as strategy is concerned.  The gimmick of this fight is that Bumba will Denouce based on the amount of time that has passed since it was first engaged.  And at V+25, you are alloted an extremely unforgiving **60 seconds** before he uses Denounce and spawns fetters.  Denounce is 100% a death sentence.  Anyone in range is just straight up dead, and even if they SOMEHOW survive it, the fetters will surely finish you off.  

So the strategy for V+25 is *completely* different.  The winning composition that we used took advantage of a two KI method.

The composition below is vertically stacked to match each player:
```
KI-1: WHM BRD WAR SMN DRK DRG 
KI-2: SCH RUN BLU COR RDM GEO
```

**SP Usage**:

| Entry | Player 1 | Player 2 | Player 3 | Player 4 | Player 5 | Player 6 | 
| ----------- | ----------- | ----------- | ----------- | ----------- | ----------- | ----------- |
| #1 | WHM | BRD | WAR | DRK | SMN | DRG |
| #1 | SP2 | SP1, SP2 | SP1 |  | SP1 |  |
| #2 | SCH | RUN | BLU | COR | RDM | GEO |
| #2 | SP1 |  | SP2 | SP1 | SP2 | SP1 |

**Lobby**: In the above example, there are two players that have not used SP2, so Cutting Cards could be used by both of them in the Lobby if you need to.

## Key Item #1

### Buffs

**WHM** :  `Protect`, `Shell`, `Baraera`, `Barsilencra`, `Regen`, `Auspice`\
**BRD** : `Honor March`, `Valor Minuet V`, `Valor Minuet IV`, `Valor Minuet III`, `Aria of Passion` *(or `Herculean Etude`)*\
**SMN** : `Ecliptic Howl`, `Wind's Blessing`, `Crystal Blessing`, `Hastega II`\
**ALL** : Use `Poison Potion`

### Pull

When ready, the **WHM** needs to use `Asylum` *right before* the pull. \
**DRK** pulls with `Impact`.

**Important:** Keep track of the time remaining when `Impact` lands.  You have exactly **60 seconds** until Bumba will **Denounce** and summon fetters.  This is a death sentence, and you need to be prepared for this.

### Fight

This is a straight zerg.  The goal for this Key Item is to get it as low as possible.  You want to get it to at least 69%.  74% is doable, but you will need to do some damage to coax the add out at the start of the second entry.  If it is at 69% or lower, just agroing Bumba will ensure the add is present from the start.

The **SMN** needs to `Astral Flow` and time Alexander's `Perfect Defense` *right before* the 60 second mark.  This will prevent a full wipe from **Denounce** and allow you to continue pumping as much damage as you can.

Keep pushing through until you can't anymore, die in a safe spot, reraise and wait out the timer.

[Recording of the KI-1 (WHM Perspective)](https://youtu.be/yaIEFV5DE-g)

**Important** There is a bug with Sheol - Gaol where using BST's Ooze to lower the boss's HP during the fight will cause issues with the second KI.  If you got it to 69% while using a BST's Ooze ability, when you go back in, it would be at 72% HP.  This *can* be a serious issue if you only got it to 74%, where going back in it will be at 77%, and you will need to do another 3% damage to get the adds to come out.  Workable if you are expecting this issue, but a run ender if you don't do enough damage.

## Key Item #2

### Buffs

**SCH** : Buff order below.  **Bold** are strategems.
1. **Addendum: White**
2. **Accession** `Protect`
3. **Accession** `Shell`
4. **Accession** `Regen V`
5. **Accession** `Voidstorm II`
6. **Accession** `Adloquium`
7. `Animus Minuo` → **SCH**
8. `Animus Augeo` → **BLU**
9. `Reraise III`
10. *Dark Arts*
11. **Addendum: Black**
12. `Klimaform` → **SCH**

**GEO** : `Geo-INT`, `Indi-Acumen`, entrust `Indi-Focus`\
**COR** : `Wizard's Roll`, `Monk's Roll`\
**RDM** : `Haste II`, `Phalanx II`, `Refresh III`

### Pull

**BLU** will be the tank for Bumba this fight.  Use `Saline Coat` and enmity generating spells.  The **BLU** needs to ensure that Bumba's TP is constantly being wiped.  It cannot get any TP moves off.

**BLU** will pull Bumba, and **RUN** will grab the add and pull it away from the others.

**RDM** *needs* to land `Silence`.  After `Silence` is on, apply `Paralyze II` and `Slow II`.

### Fight

When everyone is ready, it's time for the **SCH** to shine.  Pop **Tabula Rasa** and let's get to work.  

The skillchain to use is the following:

```
Stone → Aero → Geohelix → Anemohelix → Noctohelix → Quad. Continuum
```

After **Noctohelix** lands, the **SCH** needs to *immediately* use **Enlightenment** and **Ebullience** and start casting `Kaustra` to burst.  You will have *very* little time for this.

If done correctly, `Kaustra` will land right after the **BLU** closes the `Darkness` skillchain.

**Important:** The **RUN** needs to run in and use **Gambit** and **Rayke** during this time.  The **RDM** also needs to land `Impact` *before* the `Gravitation` skillchain.  It is very important that this is **not** magic bursted.  It is also very important that this does not do much damage at all.  It needs to be under 10,000 damage.

**Important:** The **SCH** *must* cast all spells in the skillchain is as little gear as possible.  You need all steps in the skillchain to do virtually no damage.  The more damage a spell does, the more he builds resistance to magic.  You need to limit ALL spell damage to *only* be the important magic bursts.

The following gear sets are what I used for **Immanence**, **Kaustra**, and **Helicies**:

```lua
Immanence = 
{
    main	= empty,
    sub		= empty,
    ammo	= empty,
    head	= empty,
    body	= empty,
    hands	= SCH_Empy_Hand,
    legs	= empty,
    feet	= empty,
    neck	= "Bathy Choker +1",
    waist	= empty,
    ear1	= "Dignitary's Earring",
    ear2	= empty,
    ring1	= ChirichRing_Ring1,
    ring2	= ChirichRing_Ring2,
    back	= AmbuCape_FC,
}

Kaustra = 
{
    main	= "Bunzi's Rod",
    sub		= "Ammurapi Shield",
    ammo	= "Ghastly Tathlum +1",
    head	= SCH_Empy_Head,
    body	= Agwu_Body,
    hands	= Agwu_Hand,
    legs	= Agwu_Legs,
    feet	= SCH_Empy_Feet,
    neck	= "Argute Stole +2",
    waist	= "Refoccilation Stone",
    ear1	= Malignance_Ear,
    ear2	= "Barkarole Earring",
    ring1	= "Freke Ring",
    ring2	= "Metamorph Ring +1",
    back	= AmbuCape_MD,
}

Helix = 
{
    main	= "Bunzi's Rod",
    sub		= "Ammurapi Shield",
    ammo	= "Ghastly Tathlum +1",
    head	= SCH_Relic_Head,
    body	= Agwu_Body,
    hands	= Agwu_Hand,
    legs	= Agwu_Legs,
    feet	= SCH_Empy_Feet,
    neck	= "Argute Stole +2",
    waist	= "Refoccilation Stone",
    ear1	= Malignance_Ear,
    ear2	= "Friomisi Earring",
    ring1	= "Freke Ring",
    ring2	= "Shiva Ring +1",
    back	= AdouCape_Helix
}
```

After the first `Kaustra`, swap to `Light Arts` and give out:
1. **Perpetuance**, **Accession** `Regen V`
2. **Perpetuance**, **Accession** `Embrava`
3. **Perpetuance** `Animus Augeo` → **BLU**
4. **Perpetuance** `Animus Minuo` → **SCH**
5. **Perpetuance**, **Accession** `Voidstorm II`
6. `Dark Arts` → **Addendum: Black**
7. **Manifestation** `Klimaform`

**COR** needs to **Random Deal** during this time.

When **Tabula Rasa** has 60 seconds remaining on the timer, repeat the skillchain and `Kaustra` magic burst.

After the second `Kaustra`, do another skillchian aligning with the current day, and apply a `Helix` magic burst.

### RNGesus

Now I'm not going to sugar coat this.  If you've made it this far, sadly, this is the moment that decides whether your fight will be successful, or if you're just doing a fancy RP farm.  You **need** to get a **Wild Card** of `5` or `6` here.  

If the **Wild Card** is successful, wait for the current `Kaustra` to get closer to wearing off.  You don't want to immediately start a new `Kaustra` skillchain before giving the current one time to cook.  `Kaustra` lasts for exactly **150 seconds** (2½ minutes).  Time the 3rd `Kaustra` accordingly.

When you are ready, pop **Tabula Rasa** and do it rinse-repeat.

### Issues

There are certainly some things to be aware of here:
1. Never do more than 10,000 magic damage unless you're applying `Kaustra` or a `Helix`.  Bumba builds resistance to magic damage each time a spell does more than 10,000 damage.  All non-serious magic bursts should be done virtually naked.
2. **RUN** needs to be on alert and ready to claim the second add at 39%.
3. The absolute worst aura to get is **Magic Accuracy Down**.  Not only is this a massive Magic Accuracy debuff, but it *also* prevents `Klimaform` from being applied.  This is a double-whammy for **SCH** as that's a big Magic Accuracy hit **and** it prevents the 25% damage boost from `Klimaform`.
4. **BLU** absolutely must be on their game wiping TP and preventing Bumba from otherwise getting TP.  They also need to be on top of closing the `Darkness` skillchain with **Chain Affinity**.  Failure here is an end to the run.

This is a recording of a failed run, but used the correct mechanics described.  The only reason this run was a failure was because we got **two** Magic Accuracy Down auras.  But een despite that, we got it to 5%.	

[KI-2 (SCH perspective)](https://youtu.be/P1UdqGQ62_w)