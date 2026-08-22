> A forecast is most useful where it refuses to collapse uncertainty. Three independently constructed engines put Manchester City first in the consensus, but their distances for individual clubs reveal where the evidence is stable and where it is conditional.

A league table is the end of a season, not an honest description of one before it begins. Turning changing squads, new managers, European workload and 380 unplayed matches into a single points column creates precision the evidence cannot support. The snapshot is 22 August 2026; everything that follows is a model of what was knowable then, not a claim to know May in advance.

Persistent club quality, summer disruption and match-by-match momentum each tell a different story about the season. The **Foundations Engine** asks what happens if established quality dominates. The **Disruption Engine** gives transfers, coaches, promotion, Europe and data uncertainty room to move a season. The **Momentum Engine** learns match probabilities from rolling form and Elo-like state. Each simulates the complete 380-match schedule **10,000 times**. The consensus is a weighted mixture of those simulations, not a fourth model.

## Four views of player value

The player layer now has four equally weighted, position-normalised components: the current official EA overall rating; Transfermarkt's estimated market value in euros; a recency-weighted five-season Fantasy Premier League points-per-90 measure; and FotMob's 2025/26 match rating. FPL price has been removed. Transfermarkt contributes a market estimate rather than a fantasy-game budget, while FotMob adds a performance-derived rating independent of EA's game-rating process. Equal 25% weights prevent one source's scale from dominating merely because it is measured in millions, points or rating units.

Names are reconciled to the current FPL player registry using normalised exact matching followed by conservative fuzzy matching. The direct-observation counts are 519 of 600 for EA, 524 for Transfermarkt, 474 for five-year production and 237 for FotMob. FotMob's lower coverage is expected because its published leaderboard applies a participation threshold. Missing values are never left blank: EA, points-per-90 and FotMob gaps receive the arithmetic mean for the player's position; Transfermarkt first uses the position-by-age-band mean, then falls back to position and league means. Every imputed table value is marked with a dagger, and the imputation share is carried into club-level uncertainty rather than silently treated as observed truth.

[[image1]]

*Figure 1. The raw top 100 is preserved in rank order, after which 15 players are added to give every club at least three representatives.*

This is a constrained selection problem, not a re-ranking. The algorithm first freezes the 100 highest composite scores league-wide, counts club membership, and then appends each under-represented club's best unselected players until its count reaches three. The stacked bars distinguish selection by raw score from selection through the coverage constraint; the dashed line marks the floor rather than a performance target. Opacity keeps the two routes visible where the bars overlap.

The resulting list contains 115 players. Manchester City, Arsenal and Chelsea remain dominant because the raw evidence puts many of their players in the first hundred. The floor does not dilute that signal or take places away from them; it adds enough information for Ipswich Town, Hull City, Coventry City and the other thinly represented clubs to have a usable squad core.

That ordering matters. In the earlier construction, floor places were interleaved into a table labelled as a top 100, which made raw rank and publication rank answer different questions. Here the first hundred rows are genuinely the raw top 100. The rows after them are explicitly labelled “Three-club floor”, retain their original raw rank and make the modelling safeguard auditable.

| Raw rank | Player | Club | Pos | EA | Transfermarkt €m | 5y pts/90 | FotMob | Score | Route |
|---:|---|---|:---:|---:|---:|---:|---:|---:|---|
| 1 | Bukayo Saka | Arsenal | MID | 87 | 110.0 | 6.31 | 7.52 | 96.9 | Raw top 100 |
| 2 | Rayan Cherki | Man City | MID | 86 | 90.0 | 6.86 | 7.35 | 96.0 | Raw top 100 |
| 3 | Jérémy Doku | Man City | MID | 84 | 75.0 | 5.70 | 7.33 | 92.3 | Raw top 100 |
| 4 | Phil Foden | Man City | MID | 84 | 70.0 | 6.21 | 7.32 | 92.3 | Raw top 100 |
| 5 | Cole Palmer | Chelsea | MID | 85 | 100.0 | 6.40 | 7.04 | 92.1 | Raw top 100 |
| 6 | Gabriel dos Santos Magalhães | Arsenal | DEF | 89 | 75.0 | 5.01 | 7.32 | 92.0 | Raw top 100 |
| 7 | Erling Haaland | Man City | FWD | 91 | 220.0 | 7.25 | 7.68 | 90.6 | Raw top 100 |
| 8 | Nico O'Reilly | Man City | DEF | 83 | 70.0 | 5.43 | 7.17 | 90.0 | Raw top 100 |
| 9 | Jurriën Timber | Arsenal | DEF | 84 | 70.0 | 4.87 | 7.26 | 90.0 | Raw top 100 |
| 10 | Reece James | Chelsea | DEF | 84 | 60.0 | 4.88 | 7.23 | 89.8 | Raw top 100 |
| 11 | William Saliba | Arsenal | DEF | 88 | 100.0 | 4.31 | 7.16 | 88.3 | Raw top 100 |
| 12 | Gianluigi Donnarumma | Man City | GK | 89 | 45.0 | 3.97 | 7.25 | 88.1 | Raw top 100 |
| 13 | Riccardo Calafiori | Arsenal | DEF | 82 | 55.0 | 5.07 | 7.15 | 87.2 | Raw top 100 |
| 14 | Antoine Semenyo | Man City | MID | 85 | 80.0 | 5.11 | 7.34 | 87.2 | Raw top 100 |
| 15 | David Raya Martín | Arsenal | GK | 88 | 30.0 | 4.15 | 7.21 | 86.8 | Raw top 100 |
| 16 | Matheus Santos Carneiro da Cunha | Man Utd | MID | 84 | 75.0 | 5.33 | 7.29 | 86.5 | Raw top 100 |
| 17 | Marc Guéhi | Man City | DEF | 85 | 70.0 | 3.75 | 7.37 | 86.4 | Raw top 100 |
| 18 | Dominik Szoboszlai | Liverpool | MID | 86 | 100.0 | 4.63 | 7.50 | 86.1 | Raw top 100 |
| 19 | Bruno Borges Fernandes | Man Utd | MID | 89 | 35.0 | 5.47 | 8.03 | 86.1 | Raw top 100 |
| 20 | Matheus Nunes | Man City | DEF | 83 | 50.0 | 4.21 | 7.45 | 86.0 | Raw top 100 |
| 21 | Rúben dos Santos Gato Alves Dias | Man City | DEF | 87 | 55.0 | 3.99 | 7.18 | 86.0 | Raw top 100 |
| 22 | Bryan Mbeumo | Man Utd | MID | 84 | 75.0 | 5.33 | 7.19 | 85.3 | Raw top 100 |
| 23 | Hugo Ekitiké | Liverpool | FWD | 85 | 80.0 | 6.26 | 7.08 | 84.9 | Raw top 100 |
| 24 | Declan Rice | Arsenal | MID | 88 | 120.0 | 4.28 | 7.56 | 84.5 | Raw top 100 |
| 25 | Piero Hincapié | Arsenal | DEF | 84 | 50.0 | 4.38 | 7.07 | 84.5 | Raw top 100 |
| 26 | Florian Wirtz | Liverpool | MID | 86 | 100.0 | 4.74 | 7.16 | 84.4 | Raw top 100 |
| 27 | Martin Ødegaard | Arsenal | MID | 86 | 70.0 | 5.09 | 7.00 | 83.0 | Raw top 100 |
| 28 | Elliot Anderson | Man City | MID | 84 | 110.0 | 4.34 | 7.51 | 82.9 | Raw top 100 |
| 29 | Eberechi Eze | Arsenal | MID | 84 | 65.0 | 5.42 | 6.97 | 82.2 | Raw top 100 |
| 30 | Cody Gakpo | Liverpool | MID | 82 | 60.0 | 5.16 | 7.17 | 82.1 | Raw top 100 |
| 31 | Pedro Porro Sauceda | Spurs | DEF | 83 | 45.0 | 3.78 | 7.14 | 81.6 | Raw top 100 |
| 32 | Abdukodir Khusanov | Man City | DEF | 82 | 50.0 | 3.83 | 7.12 | 81.4 | Raw top 100 |
| 33 | Morgan Rogers | Chelsea | MID | 84 | 110.0 | 4.66 | 7.00 | 81.3 | Raw top 100 |
| 34 | Morgan Gibbs-White | Nott'm Forest | MID | 83 | 70.0 | 4.77 | 7.15 | 80.8 | Raw top 100 |
| 35 | Maxence Lacroix | Chelsea | DEF | 82 | 50.0 | 3.94 | 7.04 | 80.7 | Raw top 100 |
| 36 | João Pedro Junqueira de Jesus | Chelsea | FWD | 83 | 80.0 | 5.41 | 7.18 | 80.6 | Raw top 100 |
| 37 | Benjamin Sesko | Man Utd | FWD | 82 | 75.0 | 6.13 | 6.80 | 80.2 | Raw top 100 |
| 38 | Enzo Fernández | Chelsea | MID | 86 | 100.0 | 3.94 | 7.30 | 79.8 | Raw top 100 |
| 39 | Senne Lammens | Man Utd | GK | 82 | 35.0 | 3.41 | 7.11 | 79.7 | Raw top 100 |
| 40 | Luka Vušković | Brighton | DEF | 81 | 60.0 | 5.68† | 6.96† | 79.2 | Raw top 100 |
| 41 | Harry Wilson | Leeds | MID | 81 | 25.0 | 5.66 | 7.14 | 78.3 | Raw top 100 |
| 42 | Dean Henderson | Crystal Palace | GK | 82 | 28.0 | 3.53 | 7.01 | 78.0 | Raw top 100 |
| 43 | Adrien Truffert | Bournemouth | DEF | 80 | 30.0 | 4.40 | 7.18 | 78.0 | Raw top 100 |
| 44 | Lewis Hall | Newcastle | DEF | 83 | 40.0 | 3.70 | 6.99 | 77.8 | Raw top 100 |
| 45 | Malick Thiaw | Newcastle | DEF | 81 | 45.0 | 3.83 | 7.03 | 77.6 | Raw top 100 |
| 46 | Joško Gvardiol | Man City | DEF | 85 | 70.0 | 4.59 | 6.96† | 77.5 | Raw top 100 |
| 47 | Viktor Gyökeres | Arsenal | FWD | 86 | 65.0 | 5.20 | 6.82 | 77.3 | Raw top 100 |
| 48 | Martín Zubimendi Ibáñez | Arsenal | MID | 84 | 75.0 | 4.00 | 7.20 | 77.2 | Raw top 100 |
| 49 | Marcos Senesi Barón | Spurs | DEF | 82 | 25.0 | 3.93 | 7.19 | 76.6 | Raw top 100 |
| 50 | Alexander Isak | Liverpool | FWD | 86 | 85.0 | 6.53 | 6.68† | 76.6 | Raw top 100 |
| 51 | Iliman Ndiaye | Everton | MID | 82 | 55.0 | 4.18 | 7.22 | 76.3 | Raw top 100 |
| 52 | Ryan Gravenberch | Liverpool | MID | 85 | 80.0 | 3.54 | 7.25 | 76.0 | Raw top 100 |
| 53 | Sven Botman | Newcastle | DEF | 81 | 35.0 | 3.91 | 7.00 | 75.7 | Raw top 100 |
| 54 | Robert Lynch Sánchez | Chelsea | GK | 80 | 22.0 | 3.59 | 7.07 | 75.6 | Raw top 100 |
| 55 | Anton Stach | Leeds | MID | 80 | 28.0 | 5.20 | 7.31 | 75.4 | Raw top 100 |
| 56 | Daniel Muñoz Mejía | Crystal Palace | DEF | 82 | 22.0 | 4.34 | 7.15 | 74.8 | Raw top 100 |
| 57 | Yankuba Minteh | Brighton | MID | 80 | 45.0 | 4.64 | 7.07 | 74.6 | Raw top 100 |
| 58 | Pedro Lomba Neto | Chelsea | MID | 81 | 60.0 | 4.31 | 7.04 | 74.4 | Raw top 100 |
| 59 | Jan Paul van Hecke | Spurs | DEF | 81 | 60.0 | 3.21 | 7.10 | 74.1 | Raw top 100 |
| 60 | Emiliano Martínez Romero | Aston Villa | GK | 85 | 12.0 | 3.54 | 7.07 | 73.7 | Raw top 100 |
| 61 | Johan Manzambi | Aston Villa | MID | 80 | 65.0 | 5.60† | 6.94† | 73.5 | Raw top 100 |
| 62 | Amad Diallo | Man Utd | MID | 79 | 45.0 | 4.61 | 7.19 | 73.4 | Raw top 100 |
| 63 | Kiernan Dewsbury-Hall | Everton | MID | 81 | 35.0 | 4.41 | 7.17 | 73.1 | Raw top 100 |
| 64 | Alex Scott | Bournemouth | MID | 81 | 50.0 | 4.02 | 7.17 | 73.0 | Raw top 100 |
| 65 | Tijjani Reijnders | Man City | MID | 84 | 27.0† | 5.10 | 6.95 | 73.0 | Raw top 100 |
| 66 | Mamadou Sangaré | Brentford | MID | 81 | 40.0 | 5.60† | 6.94† | 72.9 | Raw top 100 |
| 67 | Virgil van Dijk | Liverpool | DEF | 88 | 15.0 | 4.16 | 7.26 | 72.8 | Raw top 100 |
| 68 | Mohammed Kudus | Spurs | MID | 81 | 50.0 | 4.28 | 6.99 | 72.8 | Raw top 100 |
| 69 | Jeremie Frimpong | Liverpool | DEF | 81 | 35.0 | 5.49 | 6.96† | 72.7 | Raw top 100 |
| 70 | Mike Penders | Chelsea | GK | 78 | 25.0 | 6.04† | 6.96† | 71.6 | Raw top 100 |
| 71 | Marcus Rashford | Man Utd | MID | 82 | 40.0 | 5.45 | 6.94† | 71.5 | Raw top 100 |
| 72 | Sandro Tonali | Spurs | MID | 85 | 80.0 | 3.23 | 7.04 | 71.5 | Raw top 100 |
| 73 | Moisés Caicedo Corozo | Chelsea | MID | 86 | 100.0 | 2.87 | 7.10 | 71.5 | Raw top 100 |
| 74 | Ollie Watkins | Aston Villa | FWD | 83 | 25.0 | 5.62 | 6.97 | 71.4 | Raw top 100 |
| 75 | Youri Tielemans | Man Utd | MID | 85 | 40.0 | 3.64 | 7.15 | 71.3 | Raw top 100 |
| 76 | Omar Marmoush | Man City | FWD | 82 | 50.0 | 6.30 | 6.68† | 71.2 | Raw top 100 |
| 77 | Jeremy Jacquet | Liverpool | DEF | 77 | 55.0 | 5.68† | 6.96† | 71.1 | Raw top 100 |
| 78 | Nordi Mukiele | Sunderland | DEF | 81 | 16.0 | 4.88 | 7.13 | 71.0 | Raw top 100 |
| 79 | Michael Kayode | Brentford | DEF | 81 | 40.0 | 3.30 | 7.01 | 70.8 | Raw top 100 |
| 80 | James Garner | Everton | MID | 82 | 45.0 | 3.34 | 7.40 | 70.7 | Raw top 100 |
| 81 | Dango Ouattara | Brentford | MID | 79 | 35.0 | 4.87 | 6.97 | 70.5 | Raw top 100 |
| 82 | Adam Wharton | Crystal Palace | MID | 82 | 70.0 | 3.60 | 7.01 | 70.4 | Raw top 100 |
| 83 | Mats Wieffer | Brighton | DEF | 79 | 25.0 | 4.52 | 7.02 | 70.1 | Raw top 100 |
| 84 | James Hill | Bournemouth | DEF | 78 | 23.0 | 4.55 | 7.18 | 70.1 | Raw top 100 |
| 85 | Junior Kroupi | Bournemouth | MID | 80 | 70.0 | 6.12 | 6.93 | 69.9 | Raw top 100 |
| 86 | Marco Palestra | Chelsea | DEF | 78 | 35.0 | 5.68† | 6.96† | 69.8 | Raw top 100 |
| 87 | Benjamin White | Arsenal | DEF | 81 | 30.0 | 4.69 | 6.96† | 69.4 | Raw top 100 |
| 88 | Enzo Le Fée | Sunderland | MID | 80 | 28.0 | 4.52 | 7.14 | 69.2 | Raw top 100 |
| 89 | Noah Okafor | Leeds | MID | 77 | 25.0 | 6.32 | 6.94 | 69.0 | Raw top 100 |
| 90 | Jack Grealish | Man City | MID | 82 | 20.0 | 4.62 | 7.21 | 69.0 | Raw top 100 |
| 91 | Patrick Dorgu | Man Utd | MID | 78 | 35.0 | 4.63 | 7.16 | 68.9 | Raw top 100 |
| 92 | Mateus Fernandes | Spurs | MID | 80 | 50.0 | 3.54 | 7.24 | 68.9 | Raw top 100 |
| 93 | Lukás Hornícek | Newcastle | GK | 77 | 18.0 | 6.04† | 6.96† | 68.8 | Raw top 100 |
| 94 | Rayan Vitor Simplício Rocha | Bournemouth | MID | 79 | 60.0 | 5.43 | 6.94† | 68.8 | Raw top 100 |
| 95 | Bazoumana Touré | Newcastle | MID | 78 | 50.0 | 5.60† | 6.94† | 68.7 | Raw top 100 |
| 96 | Giorgi Mamardashvili | Liverpool | GK | 83 | 28.0 | 3.53 | 6.96† | 68.5 | Raw top 100 |
| 97 | Shumaira Mheuka | Chelsea | FWD | 76† | 28.2† | 90.00 | 6.68† | 68.2 | Raw top 100 |
| 98 | Rayan Aït-Nouri | Man City | DEF | 81 | 40.0 | 3.81 | 6.96† | 68.0 | Raw top 100 |
| 99 | Nico González Iglesias | Man City | MID | 81 | 40.0 | 3.64 | 7.13 | 68.0 | Raw top 100 |
| 100 | Kobbie Mainoo | Man Utd | MID | 81 | 70.0 | 3.33 | 7.01 | 67.7 | Raw top 100 |
| 105 | Neco Williams | Nott'm Forest | DEF | 80 | 28.0 | 3.33 | 7.08 | 67.5 | Three-player club floor |
| 110 | Ousmane Diomande | Nott'm Forest | DEF | 77† | 42.0 | 5.68† | 6.96† | 66.7 | Three-player club floor |
| 118 | Carl Rushworth | Coventry City | GK | 76 | 16.0 | 6.04† | 6.96† | 65.7 | Three-player club floor |
| 128 | Konstantinos Tzolakis | Hull City | GK | 75† | 18.0 | 6.04† | 6.96† | 63.8 | Three-player club floor |
| 140 | Harvey Cartwright | Hull City | GK | 75† | 17.0† | 6.04† | 6.96† | 62.9 | Three-player club floor |
| 142 | Norman Bassette | Coventry City | FWD | 76† | 28.2† | 9.55† | 6.68† | 62.7 | Three-player club floor |
| 146 | Mason Burstow | Hull City | FWD | 76† | 23.5† | 22.50 | 6.68† | 62.2 | Three-player club floor |
| 147 | Antonee Robinson | Fulham | DEF | 80 | 22.0 | 3.09 | 7.16 | 61.7 | Three-player club floor |
| 161 | Robin Roefs | Sunderland | GK | 81 | 28.0 | 3.89 | 6.95 | 60.4 | Three-player club floor |
| 168 | Gonzalo García | Fulham | FWD | 75 | 30.0 | 9.55† | 6.68† | 59.4 | Three-player club floor |
| 169 | Alex Iwobi | Fulham | MID | 80 | 20.0 | 3.98 | 7.04 | 59.4 | Three-player club floor |
| 177 | George Shepherd | Coventry City | MID | 77† | 27.6† | 5.60† | 6.94† | 57.9 | Three-player club floor |
| 178 | Kjell Scherpen | Ipswich Town | GK | 75† | 8.0 | 6.04† | 6.96† | 57.8 | Three-player club floor |
| 206 | George Hirst | Ipswich Town | FWD | 76† | 25.8† | 6.42 | 6.68† | 55.0 | Three-player club floor |
| 219 | Abdoul Ouattara | Ipswich Town | DEF | 77† | 15.0 | 5.68† | 6.96† | 54.0 | Three-player club floor |

† Arithmetic peer-mean imputation: position mean for EA, five-year points per 90 and FotMob; position-by-age-band mean, then position/league fallback, for Transfermarkt. Imputed inputs remain in the ranking but increase the uncertainty assigned to the relevant squad.

## From players to clubs

The player score is an input rather than the team forecast itself. For each club, the squad component builds a valid 1-4-4-2 core, adds four depth players and retains an elite-tail term from its top three players. The blend is 70% core, 20% depth and 10% elite quality. That construction prevents a club with several highly rated attackers but an incomplete defence from receiving the same squad score as a balanced team.

The historical component uses five seasons of points per game and goal difference per game, standardised within season and division, with recent years weighted more heavily. Championship seasons are standardised within the Championship and shifted before entering the Premier League scale, rather than comparing raw second-tier points with top-flight points. The club base is then a 50:50 blend of historical and current-squad strength, so a transfer-heavy summer can move a club without erasing what repeated league performance says about it.

[[image2]]

*Figure 2. Five-season historical strength against the four-metric current-squad score; bubble size is published-list representation and colour is the share of core inputs imputed.*

Both axes are standard scores, so a one-unit movement means one league standard deviation rather than one point or one million euros. Standardisation puts player composites and historical performance onto a common scale. Bubble area represents the count of selected players, while colour shows data completeness. Clubs above the 45-degree line are rated more strongly by current personnel than by recent results; clubs below it are being supported more by history than by the present squad layer.

The upper-right group is strong by both definitions and is consequently robust to modest changes in weighting. The more interesting clubs are those away from the diagonal. They tell us where a forecast is relying on a proposition: that a newly assembled squad will outperform its club history, or that an established structure will extract more than the apparent individual talent suggests.

This graph is also why imputation is not just a table-cleaning detail. A market-value estimate inserted from positional peers is suitable for maintaining a complete feature matrix, but it does not contain the same information as an observed valuation. The Disruption Engine therefore turns higher imputation shares into wider shocks rather than awarding false certainty to tidy data.

## The Foundations Engine

The Foundations Engine starts from the 50:50 historical/squad club standard score. Before each simulated season, every club receives a persistent Gaussian season shock with base magnitude `K = 0.42`. “Persistent” matters: the same latent good or bad season affects all 38 fixtures, producing correlated results instead of pretending every surprise is an isolated coin flip. A sensitivity pass at `K = 0.20`, `0.42` and `0.70` tests how much the table depends on that volatility judgement.

For each home-away fixture, the engine converts the two shocked strengths and a home term into win, draw and loss probabilities using a three-outcome softmax. If the latent scores are `z_H`, `z_D` and `z_A`, the probability of outcome `j` is `p(j) = exp(z_j) / Σ_k exp(z_k)`. Softmax is used because the three probabilities must be positive and sum to one, while strength differences can still have a nonlinear effect. A calibrated coefficient of 0.45 controls how sharply a quality gap becomes a match advantage.

The model plays every ordered fixture in each of 10,000 seasons, awards three points for a win and one for a draw, and stores the entire points distribution. It is intentionally sparse: it asks how far stable structural quality can take us before adding narrative variables. Its intervals therefore capture match randomness and a correlated season state, but not named transfer, coaching or workload mechanisms.

[[image3]]

*Figure 3. Foundations Engine expected points and 10–90% simulation intervals, with the K sensitivity result alongside.*

The dots are Monte Carlo means and the horizontal whiskers are the 10th and 90th percentiles of the simulated seasons. The sensitivity panel changes one structural hyperparameter while holding the evidence layer and match mechanism fixed. If rankings or gaps reverse as K moves through the range, the conclusion depends heavily on that volatility choice even when its base-run interval looks narrow.

The model's leading pair is stable because their underlying squad and historical scores are both high. Increasing K does not simply add identical noise to the final points column; it creates season-long states in which challengers can repeatedly perform above expectation. That is why volatility affects the chance of an upset season more strongly than it affects the mean order.

The Foundations Engine should be read as the clean base case. It is valuable precisely because its assumptions are limited and inspectable. Where it disagrees sharply with the richer engines, the question becomes which additional mechanism (form, transfers, management or workload) is doing the work.

## The Disruption Engine

The Disruption Engine begins from the same structural base and then decomposes uncertainty into independent latent shocks. It includes a base season term, a larger coach term for changed managers, a transfer term scaled by squad churn, a heavy-tailed promotion or second-year term and a data-quality term scaled by imputation. These shocks are sampled once per club-season so their effects persist, reflecting the fact that an unsuccessful tactical change or unusually effective recruitment window tends to influence many fixtures.

Promotion uncertainty uses a Student-t draw rather than a normal draw. The heavier tails allow rare but plausible outcomes (an unexpectedly competitive promoted side or a collapse) to occur more often than a Gaussian assumption would permit. European participation adds both a season-level workload effect and intermittent match-level fatigue. Stadium-specific home bonuses preserve the possibility that home advantage is heterogeneous rather than one league-wide constant.

After those contextual states are drawn, the engine uses the same calibrated three-outcome match mechanism and simulates the full schedule 10,000 times. Sharing the match link with Foundations isolates the effect of contextual assumptions: differences between the two engines arise from their uncertainty structures, not from an unrelated scoring rule. This makes the comparison closer to a controlled model experiment.

[[image4]]

*Figure 4. Disruption Engine points distributions and the relative scale of its coach, transfer, promotion, workload and data-quality shocks.*

The interval plot comes directly from the simulated seasons, while the component panel shows the standard deviation assigned to each mechanism. A transfer window can improve or weaken a season, so the model samples direction while the chart displays magnitude. Independent components add in variance space, allowing several modest shocks to create a materially wider season distribution without any single factor dominating.

The contextual engine remains close to Foundations at the top because Manchester City and Arsenal are supported by deep player layers and recent performance. Further down, its intervals widen where promotion status, churn or missing observations make the baseline less secure. Wider ranges are the model's answer to seasons with more ways to go right or wrong.

The factorisation keeps coach, transfer, promotion, workload and data quality from disappearing into one residual standard deviation. Their magnitudes are scenario choices informed by football structure, giving the simulation distinct ways for a season to depart from its baseline.

## The Momentum Engine

The Momentum Engine is a chronological supervised-learning model built at match level. A histogram gradient-boosting classifier estimates home-win, draw and away-win probabilities from pre-match Elo difference, rolling points-per-game difference, rolling goal-difference difference, venue-specific performance, rest-day difference, division and season progress. Gradient boosting fits a sequence of shallow decision trees to residual error, which allows nonlinear thresholds and interactions without requiring a manually specified formula for every relationship.

Every feature is computed only from information available before the match. The 2025/26 season is held out chronologically rather than sampled randomly, avoiding leakage from later matches into earlier predictions. On that holdout, multiclass log loss is 1.058 compared with 1.082 for the unconditional outcome-frequency baseline. Log loss is preferred to accuracy because it rewards calibrated probability assignments and heavily penalises confident errors; a 0.40/0.30/0.30 forecast and a 0.90/0.05/0.05 forecast should not receive the same credit when both select the same outcome.

For season simulation, the model is refitted on all five training seasons, the league is played in chronological rounds, and Elo and rolling-form state are updated after every simulated result. A heavy-tailed regime shock allows team trajectories to move beyond ordinary match noise. Probability temperature is calibrated at 0.65 so the distribution of simulated champion totals matches the historical scoring environment; lower temperature sharpens the largest class probabilities without changing their ordering. This complete dynamic season is run 10,000 times.

[[image5]]

*Figure 5. Momentum Engine points distributions and its chronological holdout comparison against a frequency baseline.*

Histogram gradient boosting bins continuous features before searching tree splits, reducing computational cost and regularising noisy thresholds. The holdout bars compare multiclass log loss and Brier score rather than in-sample fit. The simulation then predicts recursively: a sampled match changes future Elo and form features, so hot and cold runs propagate through the schedule. This feedback is why the Momentum Engine can differ materially from a static strength model even when both begin with similar teams.

The largest disagreements are informative. Momentum is notably higher on Bournemouth and lower on Spurs and Chelsea than the two structural engines. Those gaps say the recent match-state patterns and nonlinear interactions learned by the classifier are telling a different story from squad/history strength. That conflict is more useful than the average alone.

The modest holdout improvement earns Momentum 25% of the consensus rather than a majority share. Its role is to challenge the base case with a genuinely different mechanism, capturing relationships the structural engines miss without allowing the most flexible model to dominate the result.

## Where the engines disagree

[[image6]]

*Figure 6. Three model means for every club; the connecting line is the distance from the lowest to the highest engine. No consensus marker is shown.*

For club `i`, the displayed distance is `max_m(P_im) − min_m(P_im)`, where `m` indexes the three engines and `P` is mean simulated points. It is simply the range from the lowest model mean to the highest. Near-identical estimates remain visible as layered shapes, while the consensus point is omitted because an average would sit inside every line by construction and disguise the distance the chart is meant to reveal.

Manchester City's three means are separated by only 0.3 points. Arsenal's are separated by 3.0. At the other extreme, Bournemouth spans 10.8 points, Spurs 9.8 and Coventry City 8.0. Those are not rounding errors. They identify clubs whose outlook depends strongly on whether one believes structural strength, contextual shocks or recursively updated form is the better description of 2026/27.

The names make the disagreement readable. “Foundations” means persistent club quality, “Disruption” means explicit season context, and “Momentum” means learned dynamic match state. The labels do not imply that one engine is conservative and another optimistic for every club; each is a compact description of the causal story encoded by its features and simulation process.

## Historical calibration and confidence

The last ten champions scored 93, 100, 98, 99, 86, 93, 89, 91, 84 and 85 points. All ten exceeded 80 and the mean was 91.8. The earlier model scale under-produced elite totals, so the match-strength coefficient and Momentum probability temperature are now selected against the distribution of the **highest realised points total in each simulated season**. This is important: calibration does not force Manchester City, Arsenal or any named favourite above 80 expected points. It makes the simulated league capable of producing champion totals on the scale the competition has actually required.

The consensus uses a mixture of season draws: 35% Foundations, 40% Disruption and 25% Momentum, for 10,000 mixture draws. The expected points are the mean of that mixture. Confidence combines two quantities: the standard deviation within the mixed simulations and the distance among the three model means. The uncertainty index is `sqrt(s_i² + d_i²)`, where `s_i` is the consensus simulation standard deviation and `d_i` is model distance. League terciles translate the index into High, Medium and Low labels, while the numeric 10–90% interval remains visible.

[[image7]]

*Figure 7. Historical champion calibration on the left; consensus 10–90% intervals and confidence classes on the right.*

Calibration matches the mean of the highest points total in each simulated season rather than fitting one club's forecast. The intervals are quantiles of the weighted mixture, so they carry both the spread within each engine and the differences between them. The coloured class is inverse uncertainty: “High” means a smaller combined uncertainty index, not a greater expected points total or a greater probability of finishing in a particular position.

The distinction is clearest in the examples raised by the graph. Arsenal is high-confidence because all three engines place it in a narrow elite band, even though individual simulated seasons still vary. Bournemouth is low-confidence because the Momentum Engine is roughly eleven points above the Disruption Engine. A single standard error around an averaged forecast would miss that structural uncertainty.

The final table stays with expected points from each engine, consensus expected points and confidence. Title, top-four and relegation percentages are omitted because small modelling changes near those cut-offs can move the headline more than the underlying season outlook.

| Rank | Club | Foundations | Disruption | Momentum | Consensus | Confidence |
|---:|---|---:|---:|---:|---:|---|
| 1 | Man City | 87.6 | 87.9 | 87.5 | 87.7 | High (80%: 78–97) |
| 2 | Arsenal | 84.9 | 84.6 | 87.7 | 85.5 | High (80%: 75–96) |
| 3 | Liverpool | 74.5 | 75.6 | 78.5 | 75.9 | High (80%: 64–88) |
| 4 | Chelsea | 67.2 | 67.2 | 60.3 | 65.3 | Low (80%: 52–78) |
| 5 | Man Utd | 63.5 | 64.1 | 69.9 | 65.3 | Low (80%: 52–78) |
| 6 | Newcastle | 56.5 | 58.9 | 54.0 | 56.8 | Medium (80%: 43–70) |
| 7 | Aston Villa | 53.9 | 54.9 | 56.6 | 55.0 | Medium (80%: 42–68) |
| 8 | Brighton | 51.5 | 50.9 | 56.7 | 52.5 | Low (80%: 40–66) |
| 9 | Bournemouth | 50.9 | 49.1 | 59.9 | 52.5 | Low (80%: 39–67) |
| 10 | Spurs | 53.9 | 53.0 | 44.0 | 51.0 | Low (80%: 36–65) |
| 11 | Brentford | 46.6 | 47.3 | 47.7 | 47.2 | High (80%: 35–60) |
| 12 | Crystal Palace | 48.3 | 46.0 | 46.3 | 46.8 | Medium (80%: 34–60) |
| 13 | Leeds | 44.0 | 46.4 | 49.6 | 46.3 | Medium (80%: 34–59) |
| 14 | Nott'm Forest | 42.7 | 41.4 | 47.9 | 43.6 | Low (80%: 31–57) |
| 15 | Everton | 40.4 | 39.5 | 42.2 | 40.5 | High (80%: 29–53) |
| 16 | Fulham | 38.7 | 39.4 | 39.9 | 39.5 | High (80%: 27–52) |
| 17 | Coventry City | 35.8 | 37.4 | 43.8 | 38.3 | Low (80%: 26–52) |
| 18 | Sunderland | 35.9 | 35.0 | 35.2 | 35.5 | High (80%: 24–48) |
| 19 | Ipswich Town | 35.4 | 35.1 | 34.4 | 35.1 | Medium (80%: 22–49) |
| 20 | Hull City | 30.6 | 28.9 | 25.5 | 28.6 | Medium (80%: 17–40) |

## What the forecast says now

[[image8]]

*Figure 8. Synthesis board: the three engines, their distance, consensus points, confidence and the historical scoring scale.*

All three engine panels use the same points scale and percentile convention, so their positions can be compared directly. The distance panel removes consensus to expose disagreement, while the final bars use colour for confidence rather than adding another probability axis. The statistical meaning of each mark stays consistent as the board moves from individual engines to disagreement and consensus.

Manchester City leads the calibrated consensus on 87.7 expected points, with Arsenal on 85.5 and Liverpool on 75.9. The gap between the first two is meaningful but not decisive: expected points average across title-winning, ordinary and disappointing seasons. A recent champion benchmark averaging 91.8 can coexist with a favourite below 90 because the identity of the champion varies across simulations and the season maximum is higher than any one club's unconditional mean.

The middle of the table is less orderly. Chelsea and Manchester United are virtually tied in consensus but arrive there differently; Newcastle has a higher consensus than Aston Villa but broader confidence; Bournemouth and Spurs sit near one another while their model distances are among the league's largest. These are precisely the cases where reporting one decimal place without an uncertainty label would be most misleading.

At the bottom, the consensus places Coventry City, Sunderland, Ipswich Town and Hull City in the most difficult band, but their intervals overlap several established clubs and the models do not agree equally about all of them. The call is comparative vulnerability: August has not resolved three discrete relegation places.

## What I would change next time

If I rebuilt this forecast tomorrow, I would spend less time adding another engine and more time strengthening the evidence the three already consume. I would refresh every source at the same snapshot, replace as many imputed player values as possible, model likely minutes and availability, and make the promoted-team adjustment respond to the strength of each Championship season.

The working recipe would remain transparent. The source notebook records the snapshot files, matching rules, feature construction, chronological holdout, calibration grids, random seeds and simulation counts. The inputs came from the official [Fantasy Premier League player registry](https://fantasy.premierleague.com/api/bootstrap-static/), [EA Sports FC ratings](https://www.ea.com/en/games/ea-sports-fc/ratings/leagues-ratings/premier-league/13?page=1), [Transfermarkt Premier League valuations](https://www.transfermarkt.com/premier-league/marktwerte/wettbewerb/GB1), [FotMob Premier League player ratings](https://www.fotmob.com/leagues/47/stats/season/27110/players/rating), the [Vaastav FPL historical archive](https://github.com/vaastav/Fantasy-Premier-League) and [football-data.co.uk match results](https://www.football-data.co.uk/englandm.php).

What I would keep is the disagreement. A fourth model would only earn its place by bringing a genuinely different view of the season. The next forecast should improve the evidence, not conceal the distances.
