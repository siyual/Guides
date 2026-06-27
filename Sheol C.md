# Sheol C - Cruel Joke
The following is a video guide for doing a solo run of Sheol C on BLU/RDM using **Cruel Joke**:

https://youtu.be/3YzRNMHqPLk

## Gear Requirements
There are three extremely important sets you need to have to pull this off effectively:
1. **SIRD** 102% set for `Dream Flower` and `Sheep Song`
2. At least 700+ `Blue Magic Skill` for `Occulation` shadows
3. A good DT set.

These are the sets I use for each:

**SIRD**:
```lua
sets.midcast['Blue Magic']['Dream Flower'] = 
{
    main	= "Tizona",
    sub		= "Sakpata's Sword",
    ammo	= "Staunch Tathlum +1",
    head	= "Null Masque",
    body	= BLU_Empy_Body,
    hands	= "Amalric Gages +1",
    legs	= BLU_AF_Legs,
    feet	= "Amalric Nails +1",
    neck	= "Loricate Torque +1",
    waist	= "Emphatikos Rope",
    ear1	= "Halasz Earring",
    ear2	= "Magnetic Earring",
    ring1	= StikiniRing_Ring1,
    ring2	= "Murky Ring",
    back	= AmbuCape_MD,
}
```

**Blue Magic Skill**:
```lua
-- Blue Magic Skill: 757
sets.midcast['Blue Magic'].SkillBasedBuff = 
{
    main	= Iris_Main,
    sub		= Iris_Sub,
    ammo	= "Mavi Tathlum",
    head	= BLU_Relic_Head,
    body	= BLU_AF_Body,
    hands	= "Rawhide Gloves",
    legs	= BLU_Empy_Legs,
    feet	= BLU_Relic_Feet,
    neck	= "Mirage Stole +2",
    waist	= "Witful Belt",
    ear1	= "Njordr Earring",
    ear2	= BLU_Empy_Ear2,
    ring1	= StikiniRing_Ring1,
    ring2	= StikiniRing_Ring2,
    back	= "Cornflower Cape",
}
```

**DT**:
```lua
sets.idle = 
{
    ammo	= "Staunch Tathlum +1",
    head	= "Null Masque",
    body	= BLU_Empy_Body,
    hands	= Nyame_Hand,
    legs	= Nyame_Legs,
    feet	= Nyame_Feet,
    neck	= "Bathy Choker +1",
    waist	= "Null Belt",
    ear1	= "Alabaster Earring",
    ear2	= BLU_Empy_Ear2,
    ring1	= StikiniRing_Ring1,
    ring2	= StikiniRing_Ring2,
    back	= AmbuCape_TP
}
```

## Spells
This is my spell list:
```xml
<cleaveosmosis>
    <slot01>delta thrust</slot01>
    <slot02>dream flower</slot02>
    <slot03>cocoon</slot03>
    <slot04>sheep song</slot04>
    <slot05>rending deluge</slot05>
    <slot06>erratic flutter</slot06>
    <slot07>magic hammer</slot07>
    <slot08>entomb</slot08>
    <slot09>occultation</slot09>
    <slot10>subduction</slot10>
    <slot11>spectral floe</slot11>
    <slot12>sudden lunge</slot12>
    <slot13>osmosis</slot13>
    <slot14>barbed crescent</slot14>
    <slot15>sound blast</slot15>
    <slot16>battery charge</slot16>
    <slot17>magic fruit</slot17>
    <slot18>diamondhide</slot18>
    <slot19>tenebral crush</slot19>
    <slot20>cursed sphere</slot20>
</cleaveosmosis>
```

## Enemy List
You'll pick up on which mobs can and can't be afflicted with `Doom` over time, but this is a full list:

| Mob | Cruel Joke | Magic Hammer | Entomb | Dream Flower | Sheep Song |
| ----- | ----- | ----- | ----- | ----- | ----- |
Crab | ✅ | ✅| ✅ | ✅ | ✅
Pugil | ✅ | ❌ | ✅ | ✅ | ✅
Skeleton | ❌ | ❌ | ✅ | ❌ | ✅
Ghost | ❌ | ❌ | ✅ | ❌ | ✅
Qutrub | ❌ | ❌ | ✅ | ❌ | ❌
Raptor | ✅ | ❌ | ✅ | ✅ | ✅
Bugard | ✅ | ❌ | ✅ | ✅ | ✅
Bird | ✅ | ❌ | ✅ | ✅ | ✅
Bat | ❌ | ❌ | ✅ | ⚠️ | ✅
Cockatrice | ✅ | ❌ | ❌ | ✅ | ✅
Bigbird | ❌ | ❌ | ❌ | ❌ | ❌
Colibri | ✅ | ✅| ✅ | ✅ | ✅
Apkallu | ✅ | ❌ | ✅ | ⚠️ | ✅
Dahak | ❌ | ❌ | ✅ | ✅ | ✅
Wyvern | ✅ | ❌ | ✅ | ✅ | ✅
Puk | ✅ | ❌ | ✅ | ✅ | ✅
Rabbit | ✅ | ❌ | ✅ | ✅ | ✅
Sheep | ✅ | ❌ | ✅ | ✅ | ✅
Ram | ❌ | ❌ | ❌ | ❌ | ❌
Tiger | ❌ | ❌ | ✅ | ✅ | ✅
Coeurl | ✅ | ❌ | ✅ | ✅ | ✅
Manticore | ❌ | ❌ | ✅ | ✅ | ✅
Marid | ✅ | ❌ | ✅ | ✅ | ✅
Bombs | ❌ | ❌ | ✅ | ✅ | ✅
Weapons | ❌ | ✅ | ✅ | ✅ | ✅
Imp | ❌ | ✅ | ✅ | ⚠️ | ✅
Soulflayer | ❌ | ✅ | ✅ | ⚠️ | ✅
Worm | ❌ | ✅ | ✅ | ⚠️ | ✅
Leech | ❌ | ❌ | ✅ | ✅ | ✅
Slime | ❌ | ❌ | ✅ | ✅ | ✅
Flan | ❌ | ✅ | ✅ | ✅ | ✅
Funguar | ❌ | ❌ | ✅ | ✅ | ✅
Treant | ✅ | ❌ | ✅ | ✅ | ✅
Sapling | ✅ | ❌ | ✅ | ✅ | ✅
Mandragora | ✅ | ❌ | ✅ | ✅ | ✅
Goobbue | ✅ | ❌ | ✅ | ✅ | ✅
Morbol | ❌ | ❌ | ✅ | ✅ | ✅
Flytrap | ✅ | ❌ | ✅ | ✅ | ✅
Bee | ✅ | ❌ | ✅ | ✅ | ✅
Chigoe | ❌ | ❌ | ✅ | ⚠️ | ✅
Crawler | ✅ | ❌ | ✅ | ✅ | ✅
Fly | ✅ | ❌ | ✅ | ✅ | ✅
Scorpion | ❌ | ❌ | ✅ | ✅ | ✅
Spider | ❌ | ❌ | ✅ | ✅ | ✅
Diremite | ❌ | ❌ | ✅ | ✅ | ✅
Wamouras | ✅ | ✅ | ✅ | ✅ | ✅

With the exception of the `Cockatrices`, you can juggle `Entomb` and `Dream Flower` to keep all mobs locked in place while `Doom` ticks down.

You **must** stay in range of the mob for the entire duration of `Doom`, or it will wear off.

## Trusts
I used the following trusts mainly for buffs.  And only engaged when I had an add I needed to kill (or a resist), or when I needed trusts to apply buffs.

1. Yoran-oran
2. Monberaux
3. King of Hearts
4. Joachim
5. Ulmia