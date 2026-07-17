---
title: "Bluewater Ascendancy: Teaching Empire: Total War to Care About the Sea"
description: "A personal rebalance of Empire: Total War built on a single wager — that the game is really a trade-and-colony game wearing a war game's coat, and plays better once you admit it."
date: 2026-07-08
tags:
  - Empire Total War
  - Total War
  - modding
  - strategy games
  - Bluewater Ascendancy
---

# Bluewater Ascendancy: Teaching Empire: Total War to Care About the Sea

Empire: Total War has always held an awkward place in my gaming life. It is not the cleanest game the series has made, and it is nowhere near the most polished. It is full of quirks, brittle systems, hesitant diplomacy, and campaign behaviours that feel held together with sealing wax and optimism. And yet I keep returning to it, because no other Total War game captures the same sense of scale — not scale of armies, but scale of *consequence*. A decision made in Paris can matter in Bengal. A fleet leaving the Caribbean can tip a European war. A single fragile colony can become the hinge on which an empire turns.

That is the promise of Empire, and it remains one of the most exciting the series has ever made. Bluewater Ascendancy grew out of a stubborn wish to see that promise show up more often than the base game allows.

## The wager behind the mod

Most rebalance mods begin with a complaint. Mine began with a suspicion: that Empire is secretly a trade-and-colony game wearing the coat of a war game, and that it plays better the moment you stop apologising for it.

Vanilla Empire gestures at this. It has trade nodes, ports, commodities, plantations, chartered companies, and sea lanes. But it prices them timidly, as though embarrassed by its own eighteenth century. The century itself was not embarrassed. It was an era of sugar islands and slaving routes, of monopolies defended by cannon, of governments financed less by conquest than by commerce carried across water. The sea was not decoration. It was infrastructure. Empire knows this in its bones and forgets it in its numbers.

> **The core idea:** Empire is at its best when sea lanes, colonial footholds, and fragile frontier states create pressure across the whole map. Bluewater Ascendancy does not add new systems. It re-prices the ones already there until the campaign's incentives point back toward what makes the game special.

Everything else in the mod follows from that wager. I did not want to replace Empire with a different game. I wanted to make the campaign breathe — to let more of Empire actually happen.

## First principle: unstick the map

Before I could make the sea matter, I had to stop the land from strangling everything.

Empire has a habit of turning the campaign map into a defensive tangle. Forts are interesting in moderation, but in practice they slow the game in ways that do not produce better strategy. They block movement, interrupt wars, reward passive play, and make an already timid AI even more hesitant. Instead of dynamic eighteenth-century campaigning, you end up with a map of small obstacles, each one making every theatre feel sticky. Wars freeze around little works of earth and stone rather than spilling across regions the way they should.

So the first design principle was narrow and deliberate: keep the campaign's flavour, but remove the things that make it stagnate. Bluewater Ascendancy disables new fort construction and fort upgrades while leaving the broader structure intact. Existing forts remain where the start position places them; the map simply stops metastasising into a fortress maze. The change sounds minor and reads minor in a changelog. In play it is anything but. Armies move. Campaigns develop. Colonial wars travel. The map recovers its capacity to surprise.

[[image1]]

*Disabling new fort construction and upgrades stops the campaign map from calcifying into a fortress maze.*

This is the least glamorous change in the mod and, I suspect, the one that does the most quiet work.

## Second principle: make the sea pay

With the land unstuck, the trade economy could finally carry weight.

Bluewater Ascendancy pushes hard here, and it is not subtle by design. Commodity base prices are tripled. Trade-node commodity quantities are tripled. Sea trade-route values from trading ports, commercial ports, commercial basins, and trading companies are all tripled. Plantation output is doubled. Coffee, cotton, furs, ivory, spices, sugar, tea, tobacco — each becomes something worth building a strategy around rather than a rounding error in your treasury.

[[image2]]

*Commodity base prices tripled in RPFM — coffee, cotton, sugar and the rest stop being a rounding error in the treasury.*

The point is to change what a player *wants*. When a Caribbean possession is worth genuine money, fleets stop being mere ferries and become the thing that protects your income. When a trade port is more than a small income bump, contesting one becomes a real campaign decision. When plantation output doubles, an overseas colony can reshape a national economy instead of decorating a coastline. The Atlantic and the Indian Ocean stop being scenery you sail past on the way to a European war and start being the war.

[[image3]]

*Sea trade-route values and plantation output raised across trading ports, commercial ports and colonial plantations.*

A maritime empire should *feel* materially different from a landlocked one. Under vanilla numbers it rarely does. Under these numbers, it finally must. Suddenly it is easy to understand why states of this period took such enormous risks for islands, coasts, and trading posts. The mod does not explain that logic to you. It lets you feel it in your ledger.

## Third principle: a France that acts like France

France is one of the great powers of the century, but in Empire it can feel oddly constrained — dominant enough in Europe, yet strangely weightless on the global stage. I wanted a France that behaves like a true blue-water contender: wealthy enough to act, stretched enough to be interesting, connected enough to make hard choices across theatres at once.

So the version I have been testing gives France a substantial opening advantage, including a significant money boost at campaign start. This is partly balance, but mostly it is about story. A stronger France is not a gift to the player who picks France; it is a gift to everyone else on the map. It hands Britain, Spain, the Dutch, and the smaller powers a more dangerous world to react to. It forces the interesting questions to be asked early. Does France contest Britain at sea, or lean into the sugar economy of the Caribbean, or gamble on India, or try to hold a sprawling colonial system together while Europe burns? France should have those choices from turn one. In vanilla it too often has only the European ones.

## Fourth principle: oxygen for the small powers

Some of my favourite campaigns in any strategy game are not the clean, obvious ones. They are the awkward starts — the fragile states that should probably be doomed and somehow survive. Empire is rich in these: Louisiana, New Spain, Portugal, Saxony, Hannover, Georgia, Denmark. They sit at the edges of larger systems with thin money, exposed borders, and little strategic depth. That fragility is the appeal. But a faction too weak to participate is not a story; it is a footnote.

Bluewater Ascendancy does not try to make every minor state a great power — that would flatten the very campaign it wants to enrich. It gives selected struggling factions more room to breathe. Some receive extra starting money — Louisiana, New Spain, Portugal, Saxony, and Hannover each begin with more in the coffers than vanilla allows. The richer trade economy raises the ceiling for any colonial or maritime position. The absence of fort spam lets wars move in ways that create openings. The aim is not equality. The aim is possibility.

[[image4]]

*Extra starting treasuries for Louisiana, New Spain, Portugal, Saxony and Hannover in the campaign start position.*

Louisiana is the campaign I most want to support properly in future versions. It is historically fascinating precisely because it sits at the seam of empire: French in identity, American in geography, dependent on wider imperial systems, and permanently exposed to stronger neighbours. I do not want it to become France by another name. I want it to survive as its own problem. The same holds for New Spain and New France, both of which are on the roadmap for careful playable-faction work.

## The unglamorous part: modding as archaeology

None of this was clean to build. Modding Empire is half design and half archaeology. You start with a frustration, follow it down through old files and half-documented systems, test something, break something, fix it, and slowly arrive at a version of the game closer to the one you always imagined.

The biggest lesson was learning what does *not* belong in `startpos.esf`. The start position is seductive because it holds so much of the opening world — factions, money, regions, ownership, diplomacy, campaign setup — so it tempts you to treat it as the answer to every problem. It is also fragile, and easy to break in ways that crash a campaign before it becomes interesting. Faction playability alone, I learned the hard way, is controlled in more than one place: a faction can be marked selectable in the campaign-setup layer while its underlying record still reads as AI. Miss one and the whole thing quietly refuses to work.

So the release is split by responsibility rather than crammed into one magic file. The pack files carry the broad rules — trade values, plantation output, fort construction, fort upgrades. The campaign files hold the current start position. The script file governs which packs load. It is less elegant than a single hammer, but it is much closer to how Empire actually thinks.

[[image5]]

*The release split by responsibility — pack files for rules, campaign files for the start position, script file for load order.*

The mod also borrows selectively from the wider ecosystem — Empire Enhanced, Empire Extended, Empire Total Flags, and dedicated no-siege work — for visuals and faction flavour, while refusing to drift into a total conversion. I wanted a cleaner campaign, not a different battle game.

## What I hoped to receive from it

I did not build Bluewater Ascendancy to make Empire harder in a blunt way or easier in a lazy one. I built it to make the campaign's incentives point toward the things that make Empire special: ships, trade, colonies, fragile powers, global rivalry, and the long reach of money across water.

What I hoped to receive was a particular *feeling* — the one Empire promises on its box and delivers only in flashes. The feeling that a campaign might begin in Europe and suddenly become about Caribbean islands or Indian ports. That a navy is worth building because it guards something real. That France might do something ambitious and force the whole map to answer. That a doomed little colony might, against the odds, write a strange and memorable story instead of dying quietly in the second act.

That is the heart of it. Bluewater Ascendancy is not a rejection of vanilla Empire. In many ways it comes from affection for it — for the huge map, the many theatres, the awkward but compelling global politics, the invitation to think in oceans rather than borders. I simply wanted more of that, more often: more movement, more value in colonies, more reason to build a fleet, more reason for France to behave like France, more oxygen for the small states to become stories rather than scenery.

The roadmap from here is clear enough. The next real goal is making New France and New Spain cleanly playable without destabilising the campaign — careful start-position work, faction checks, diplomacy and menu testing, first-turn stability. One good change at a time is worth more than a pile of unstable ideas in a campaign that crashes before it becomes interesting.

For now, the foundation holds. The map is less strangled by forts. The trade game is richer. France has genuine global weight. The smaller powers have a little more air. And Empire: Total War feels, at least to me, closer to the sweeping oceanic strategy game I always wanted it to be. That is why I made Bluewater Ascendancy — not to replace Empire, but to let more of Empire happen.
