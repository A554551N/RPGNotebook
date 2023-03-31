*A S&W pointcrawl rebuilt for 13th Age, covering chapters 1-3*
# Intro
The **Zephyr** was tasked with departing New Port fully laden and making a fairly standard trading voyage with ports of call in Drakkenhall, Concord, and Glitterhagen.  Instead, her captain diverted her on a dangerous journey beyond the Midland Sea to an island supposedly covered in easy gold.  Instead the crew was murdered and she was captured by vicious Stormsea Suahagin.
# NPCs
## Jaxon Brand
Head of Zephyr Assimilated (ZA), his daughter is missing.
## ZA *Zephyr*
Flagship of the ZA fleet, captained by Elisa Brand
## DEN *Discovery*
A Dragon-Navy warship, possibly the last to see the *Zephyr*
## Joshua Cree
A sailor from the Dragon-Navy ship *Discovery*, recently assigned to patrol of the Koru Strait
## ZA *Bounty*
Captained by Jaxon's son **Timothy Brand**, conscripted to the mission to allow the party a way of journeying out onto the Midland
## Captain Timothy Brand
A loudmouth and a braggart, always in the shadow of his sister Elisa.  He'll tell you he's slain a dozen men and sailed straight into the teeth of the Kraken itself, these are all lies.  In truth, he's insecure in his position and covers for it with a mountain of blather.
## First Mate Jace
A competent and skilled leader, does her best to rein in the Captain's excesses.
## Gar, a Stowaway
Gar has hidden out aboard the ZA *Bounty* in the hopes of finding adventure (he might be a Doppelganger?  He was in the original module but we'll see how it feels)

# Encounters
## Kobold Pirates & Lacedons
*A smashed up raft appears off the starboard bow with a number of small figures leaping up and down, clearly clamoring for rescue.  Upon closer inspection, it appears to be a group of stranded kobolds dressed up as pirates.

*Unbeknownst to the crew, the bottom of the raft is swarming with Lacedons (aquatic ghouls) that the kobolds feed in exchange for their help with taking ships.  Once the **Bounty** pulls up alongside, the Lacedons will sneak aboard while the Kobolds distract them.*

**Contents**
1x Kobold Pirate Captatin
1x Lacedon Pusbuster
3x Lacedon Fleshrippers
3x Kobold Mateys

```13a
name: Kobold Pirate Captain
blurb: Flourishes a broken cutlasss and a very impressive hat
level: 5
role: leader
tag: HUMANOID
initiative: 10

ac: 21
pd: 19
md: 15
hp: 72

attacks:
- name: 'A Broken Blade'
  attack: +10 vs AC
  hit: 18 damage
  extras:
  - name: Natural 16+
    description: The Captain's Crew gains a +2 attack bonus against this target until the start of the Captain's next turn
- name: 'R: Explosive Grog'
  attack: +5 vs PD
  hit: The target is vulnerable to non-magical attacks (6+ save ends)

traits:
- name: Evasive
  description: Kobolds take no damage from missed attacks
```

```13a
name: Kobold Matey
blurb: Wears clothes that are too big for it, brandishes what appear to be kitchen implements
level: 7
role: mook
tag: HUMANOID
initiative: 12

ac: 23
pd: 21
md: 17
hp: 27 (mook)

attacks:
- name: 'Random Bullshit Go!'
  attack: +12 vs AC
  hit: 18 damage
  extras:
  - name: Natural 16+
    description: The Crew steals a real weapon from someone on the ship, their next attack deals +5 (23) damage

traits:
- name: Evasive
  description: Kobolds take no damage from missed attacks
```

```13a
name: Lacedon Fleshrippers
blurb: Hungry and soaked to the exposed bone
level: 7
role: mook
tag: UNDEAD
initiative: 10
vulnerability: holy

ac: 20
pd: 18
md: 14
hp: 27 (mook)

attacks:
- name: 'Rip and Tear'
  attack: +15 vs AC (2 attacks)
  hit: 9 damage and the target is Vulnerable (Save ends)

traits:
- name: Undead
  description: The Lacedon is vulnerable to Holy damage.
```

```13a
name: Lacedon Pusbuster
blurb: It looks sick...
level: 7
role: spoiler
vulnerability: holy
tag: UNDEAD
initiative: 11

ac: 23
pd: 21
md: 15
hp: 120

attacks:
- name: 'Feeble Claws'
  attack: +11 vs AC
  hit: 21 damage
- name: 'C: Vomit Comet'
  attack: +11 vs PD (1d3 nearby enemies)
  hit: 10 ongoing damage and the target is vulnerable (Save ends both)
  extras:
  - name: Natural even hit
    description: The target is hampered (Save ends)
  - name: Natural odd hit
    description: The target is dazed (save ends)
  - name: Self-diminishing
    description: The Pusbuster takes 2d6 damage for each creature targeted with this attack.
```
