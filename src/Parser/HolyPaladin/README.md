## Features
| Feature | Note | Accuracy |
| --- | --- | --- |
| [Mastery Effectiveness](https://github.com/MartijnHols/WoWAnalyzer/blob/master/src/Main/Parser/Modules/Features/MasteryEffectiveness.js) | Tracks your distance to other players and the healing done to determine the effectiveness of your healing weighted by the amount of healing done. | >90% |
| [Always Be Casting](https://github.com/MartijnHols/WoWAnalyzer/blob/master/src/Main/Parser/Modules/Features/AlwaysBeCasting.js) | Tracks your casting and healing time to determine your non healing and dead GCD time. May get slightly inaccurate with unaccounted for Haste buffs. | 80%-100% |
| [Beacon Targets](https://github.com/MartijnHols/WoWAnalyzer/blob/master/src/Main/Parser/Modules/PaladinCore/BeaconTargets.js) | Used by other features: tracks who have beacons active for all beacon types. | 100% |
| [Ability Tracker](https://github.com/MartijnHols/WoWAnalyzer/blob/master/src/Main/Parser/Modules/Core/AbilityTracker.js) | Tracks ability casts and healing done (damage tracking NYI)w. | 100% |
| [Paladin Ability Tracker](https://github.com/MartijnHols/WoWAnalyzer/blob/master/src/Main/Parser/Modules/PaladinCore/PaladinAbilityTracker.js) | Tracks healing done on beacons and with IoL. | 100% |
| [Cast Efficiency](https://github.com/MartijnHols/WoWAnalyzer/blob/master/src/Main/CastEfficiency.js) | Displays the amount of casts and estimates the max amount of casts possible to determine your skill at keeping important spells (close to) on cooldown. The estimated max amount of casts is slightly inaccurate due to not considering Haste increasers like Holy Avenger, Bloodlust and from boss abilities. | >90% |
| [Chain of Thrayn](https://github.com/MartijnHols/WoWAnalyzer/blob/master/src/Main/Parser/Modules/Legendaries/ChainOfThrayn.js) |  | 100% |
| [Drape of Shame](https://github.com/MartijnHols/WoWAnalyzer/blob/master/src/Main/Parser/Modules/Legendaries/DrapeOfShame.js) |  | 100% |
| [Ilterendi, Crown Jewel of Silvermoon](https://github.com/MartijnHols/WoWAnalyzer/blob/master/src/Main/Parser/Modules/Legendaries/Ilterendi.js) |  | 100% |
| [Maraad's Dying Breath](https://github.com/MartijnHols/WoWAnalyzer/blob/master/src/Main/Parser/Modules/Legendaries/MaraadsDyingBreath.js) | The healing gain is calculated by comparing boosted LotMs with unbuffed LotMs. Since most people wouldn't ever cast unbuffed LotMs as fillers but a FoL/HL instead, this can be somewhat inaccurate. | ≈70% |
| [Obsidian Stone Spaulders](https://github.com/MartijnHols/WoWAnalyzer/blob/master/src/Main/Parser/Modules/Legendaries/ObsidianStoneSpaulders.js) | | 100% |
| [Prydaz, Xavaric's Magnum Opus](https://github.com/MartijnHols/WoWAnalyzer/blob/master/src/Main/Parser/Modules/Legendaries/Prydaz.js) | | 100% |
| [Velen's Future Sight](https://github.com/MartijnHols/WoWAnalyzer/blob/master/src/Main/Parser/Modules/Legendaries/Velens.js) | | 100% |
| [Sacred Dawn](https://github.com/MartijnHols/WoWAnalyzer/blob/master/src/Main/Parser/Modules/Features/SacredDawn.js) | | 100% |
| [Tyr's Deliverance](https://github.com/MartijnHols/WoWAnalyzer/blob/master/src/Main/Parser/Modules/Features/TyrsDeliverance.js) | Includes the healing gained from casting a FoL/HL on a target affected with the buff. | 100% |

The accuracy percentages assume there are no bugs in the implementation, the accuracy of all features was verified extensively. All interactions with Aura of Sacrifice are ignored.

## Suggestions

This may be outdated.

| Suggestion | Minor | Average | Major |
| --- | --- | --- | --- |
| Non healing time | >20% | >40% | >45% |
| Dead GCD time | >20% | >35% | >40% |
| Total heals on beacon | >20% | >25% | >35% |
| Mastery Effectiveness | <75% | <70% | <60% |
| Rule of Law uptime | <25% | <20% | <10% |
| IoL FoL to HL cast ratio | <70% | <60% | <40% |
| Unused IoL ratio (no 4PT19) | >0% | >5% | >20% |
| Unused IoL ratio (no 4PT19 +CM) | >5% | >10% | >25% |
| Unused IoL ratio (no 4PT19 +CM +DP) | >10% | >15% | >30% |
| Unused IoL ratio (4PT19) | >20% | >25% | >40% |
| Unused IoL ratio (4PT19 +CM) | >30% | >35% | >50% |
| Unused IoL ratio (4PT19 +CM +DP) | >40% | >45% | >60% |
| Ilterendi Healing | <4.5% | <4% | <3% |
| Velen's Healing | <4.5% | <4% | <3% |
| Filler Light of the Martyr CPM | >1 CPM | >1.5 CPM | >2 CPM |
| Aura of Sacrifice healing done | <30k HPS | <25k HPS | <20k HPS |
| Light of Dawn overhealing | >40% | >50% | >60% |
| Light of Dawn overhealing (with DP) | >45% | >55% | >65% |
| Holy Shock overhealing | >40% | >50% | >60% |
| Holy Shock overhealing (with DP) | >45% | >55% | >65% |
| Flash of Light overhealing | >25% | >40% | >50% |
| Bestow Faith overhealing | >40% | >50% | >60% |
| Cast Efficiency (see spells) | <80% | <75% | <65% |
| Crusader Strike Cast Efficiency | <30% | <25% | <15% |
| Divine Protection Cast Efficiency | <60% | <55% | <45% |
| Blessing of Sacrifice Cast Efficiency | - | - | - |
