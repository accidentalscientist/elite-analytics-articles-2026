> Three different season engines leave Arsenal and Man City separated by only 0.5%. The uncertainty is not a flaw in the analysis. It is the central finding.

## The thesis

The most misleading football forecast is the cleanest one: twenty clubs, one expected-points column, and no visible uncertainty. It turns small differences in inputs into a false claim that August already knows May.

Our approach starts from the opposite proposition: **a league forecast should expose its disagreements**. We first build a player and club evidence layer. We then ask three genuinely different season engines to interpret it. Model 1 assumes structural quality persists. Model 2 says stadium, manager, transfers and European workload change the path. Model 3 learns nonlinear match relationships and lets form update after every simulated game.

> **The thesis:** The question is not “who finishes first in the spreadsheet?” It is “which routes to the title remain plausible, and which assumptions create them?”

[[image1]]

*Figure 1. Arsenal, Manchester City and Liverpool dominate the merit places. Amber segments show where the three-per-club rule changes the published list.*

## The Premier League 100

The score is 65% EA FC overall percentile, 20% position-adjusted FPL price percentile and 15% five-season, position-adjusted FPL production. Each club's top three is protected before the remaining places are filled by league-wide score. Raw rank is unconstrained; route labels the club-floor additions.

| Rank | Player | Club | Pos | EA | FPL £m | 5y pts/90 | Score | Raw rank | Route |
|---:|---|---|:---:|---:|---:|---:|---:|---:|---|
| 1 | Gabriel dos Santos Magalhães | Arsenal | DEF | 88 | 8.0 | 5.01 | 97.9 | 1 | Merit |
| 2 | Bukayo Saka | Arsenal | MID | 88 | 9.5 | 6.31 | 97.7 | 2 | Merit |
| 3 | Erling Haaland | Man City | FWD | 90 | 15.5 | 7.25 | 97.7 | 3 | Merit |
| 4 | David Raya Martín | Arsenal | GKP | 87 | 6.0 | 4.15 | 97.2 | 4 | Merit |
| 5 | Cole Palmer | Chelsea | MID | 87 | 9.5 | 6.40 | 97.0 | 5 | Merit |
| 6 | Bruno Borges Fernandes | Man Utd | MID | 87 | 12.0 | 5.47 | 96.0 | 6 | Merit |
| 7 | Gianluigi Donnarumma | Man City | GKP | 89 | 5.5 | 3.97 | 95.9 | 7 | Merit |
| 8 | Alexander Isak | Liverpool | FWD | 88 | 9.0 | 6.53 | 95.4 | 8 | Merit |
| 9 | Virgil van Dijk | Liverpool | DEF | 90 | 6.5 | 4.16 | 94.7 | 9 | Merit |
| 10 | Phil Foden | Man City | MID | 85 | 7.0 | 6.21 | 93.6 | 10 | Merit |
| 11 | Florian Wirtz | Liverpool | MID | 89 | 7.5 | 4.74 | 93.5 | 11 | Merit |
| 12 | Bryan Mbeumo | Man Utd | MID | 85 | 8.0 | 5.33 | 92.8 | 12 | Merit |
| 13 | William Saliba | Arsenal | DEF | 87 | 6.0 | 4.31 | 92.4 | 13 | Merit |
| 14 | Martin Ødegaard | Arsenal | MID | 87 | 6.5 | 5.09 | 91.8 | 14 | Merit |
| 15 | James Maddison | Spurs | MID | 84 | 6.5 | 5.74 | 90.9 | 15 | Merit |
| 16 | Cody Gakpo | Liverpool | MID | 84 | 7.0 | 5.16 | 90.2 | 16 | Merit |
| 17 | Matheus Santos Carneiro da Cunha | Man Utd | MID | 83 | 8.0 | 5.33 | 89.8 | 17 | Merit |
| 18 | Declan Rice | Arsenal | MID | 87 | 7.5 | 4.28 | 89.1 | 18 | Merit |
| 19 | Jordan Pickford | Everton | GKP | 84 | 5.5 | 3.75 | 88.7 | 19 | Merit |
| 20 | Rodrigo 'Rodri' Hernandez Cascante | Man City | MID | 90 | 6.5 | 4.15 | 88.6 | 20 | Merit |
| 21 | Tijjani Reijnders | Man City | MID | 86 | 6.0 | 5.10 | 88.6 | 21 | Merit |
| 22 | Eberechi Eze | Arsenal | MID | 83 | 6.5 | 5.42 | 88.0 | 22 | Merit |
| 23 | Jeremie Frimpong | Liverpool | DEF | 83 | 5.5 | 5.49 | 88.0 | 23 | Merit |
| 24 | Omar Marmoush | Man City | FWD | 84 | 7.0 | 6.30 | 88.0 | 24 | Merit |
| 25 | Jurriën Timber | Arsenal | DEF | 82 | 6.5 | 4.87 | 87.6 | 25 | Merit |
| 26 | Ollie Watkins | Aston Villa | FWD | 84 | 8.0 | 5.62 | 87.2 | 26 | Merit |
| 27 | Joško Gvardiol | Man City | DEF | 84 | 5.5 | 4.59 | 87.2 | 27 | Merit |
| 28 | Rúben dos Santos Gato Alves Dias | Man City | DEF | 86 | 5.5 | 3.99 | 86.7 | 28 | Merit |
| 29 | Hugo Ekitiké | Liverpool | FWD | 83 | 7.5 | 6.26 | 86.5 | 29 | Merit |
| 30 | Mikel Merino Zazón | Arsenal | MID | 83 | 6.0 | 5.53 | 86.3 | 30 | Merit |
| 31 | Viktor Gyökeres | Arsenal | FWD | 87 | 7.5 | 5.20 | 86.2 | 31 | Merit |
| 32 | Dominik Szoboszlai | Liverpool | MID | 83 | 7.0 | 4.63 | 86.1 | 32 | Merit |
| 33 | Benjamin White | Arsenal | DEF | 83 | 5.5 | 4.69 | 85.7 | 33 | Merit |
| 34 | Rayan Cherki | Man City | MID | 81 | 7.5 | 6.86 | 85.7 | 34 | Merit |
| 35 | Morgan Gibbs-White | Nott'm Forest | MID | 82 | 8.0 | 4.77 | 84.7 | 35 | Merit |
| 36 | Piero Hincapié | Arsenal | DEF | 83 | 5.5 | 4.38 | 84.5 | 36 | Merit |
| 37 | Sávio Moreira de Oliveira | Man City | MID | 82 | 6.5 | 5.18 | 84.4 | 37 | Merit |
| 38 | Dejan Kulusevski | Spurs | MID | 83 | 6.5 | 4.52 | 84.1 | 38 | Merit |
| 39 | Morgan Rogers | Chelsea | MID | 82 | 7.5 | 4.66 | 83.9 | 39 | Merit |
| 40 | Enzo Fernández | Chelsea | MID | 84 | 7.0 | 3.94 | 83.5 | 40 | Merit |
| 41 | Emiliano Martínez Romero | Aston Villa | GKP | 85 | 5.0 | 3.54 | 83.1 | 41 | Merit |
| 42 | Alysson Edward Franco da Rocha dos Santos | Aston Villa | MID | 89 | 5.0 | 5.74 | 82.7 | 42 | Merit |
| 43 | Gabriel Martinelli Silva | Arsenal | MID | 81 | 6.5 | 5.35 | 82.0 | 43 | Merit |
| 44 | Marc Guéhi | Man City | DEF | 82 | 6.0 | 3.75 | 81.5 | 44 | Merit |
| 45 | Xavi Simons | Spurs | MID | 84 | 6.0 | 4.12 | 81.1 | 45 | Merit |
| 46 | Reece James | Chelsea | DEF | 81 | 5.5 | 4.88 | 81.1 | 46 | Merit |
| 47 | Jérémy Doku | Man City | MID | 80 | 7.5 | 5.70 | 80.7 | 47 | Merit |
| 48 | Ronald Araujo | Liverpool | DEF | 83 | 5.5 | — | 80.5 | 48 | Merit |
| 49 | Giorgi Mamardashvili | Liverpool | GKP | 84 | 5.0 | 3.53 | 80.3 | 49 | Merit |
| 50 | Jacob Murphy | Newcastle | MID | 81 | 6.0 | 5.42 | 80.0 | 50 | Merit |
| 51 | Youri Tielemans | Man Utd | MID | 85 | 6.0 | 3.64 | 79.9 | 51 | Merit |
| 52 | Marcus Rashford | Man Utd | MID | 80 | 7.0 | 5.45 | 79.7 | 52 | Merit |
| 53 | Nikola Milenković | Nott'm Forest | DEF | 83 | 5.5 | 3.51 | 79.7 | 53 | Merit |
| 54 | Ryan Gravenberch | Liverpool | MID | 85 | 6.0 | 3.54 | 79.5 | 54 | Merit |
| 55 | Antoine Semenyo | Man City | MID | 80 | 8.5 | 5.11 | 79.4 | 55 | Merit |
| 56 | Alexis Mac Allister | Liverpool | MID | 87 | 5.5 | 3.97 | 79.2 | 56 | Merit |
| 57 | Pedro Porro Sauceda | Spurs | DEF | 82 | 5.5 | 3.78 | 78.6 | 57 | Merit |
| 58 | Daniel Muñoz Mejía | Crystal Palace | DEF | 81 | 5.5 | 4.34 | 78.5 | 58 | Merit |
| 59 | Noni Madueke | Arsenal | MID | 80 | 6.5 | 5.42 | 78.3 | 59 | Merit |
| 60 | Federico Chiesa | Liverpool | MID | 81 | 5.5 | 9.57 | 78.0 | 60 | Merit |
| 61 | Kai Havertz | Arsenal | FWD | 82 | 7.5 | 5.07 | 77.8 | 61 | Merit |
| 62 | Matz Sels | Nott'm Forest | GKP | 83 | 5.0 | 3.51 | 77.3 | 62 | Merit |
| 63 | Jean-Philippe Mateta | Crystal Palace | FWD | 82 | 6.5 | 5.25 | 77.1 | 63 | Merit |
| 64 | Harvey Barnes | Newcastle | MID | 80 | 6.0 | 5.59 | 76.4 | 64 | Merit |
| 65 | Granit Xhaka | Sunderland | MID | 85 | 5.5 | 3.84 | 76.4 | 65 | Merit |
| 66 | Anthony Elanga | Newcastle | MID | 81 | 6.0 | 4.59 | 76.3 | 66 | Merit |
| 67 | Yoane Wissa | Newcastle | FWD | 82 | 6.0 | 5.48 | 76.3 | 67 | Merit |
| 68 | Nick Pope | Newcastle | GKP | 81 | 5.0 | 3.78 | 76.1 | 68 | Merit |
| 69 | Rayan Aït-Nouri | Man City | DEF | 81 | 5.5 | 3.81 | 75.8 | 69 | Merit |
| 70 | Murillo Costa dos Santos | Nott'm Forest | DEF | 83 | 5.5 | 3.11 | 75.2 | 70 | Merit |
| 71 | Chris Wood | Nott'm Forest | FWD | 82 | 6.0 | 5.40 | 75.0 | 71 | Merit |
| 72 | Dean Henderson | Crystal Palace | GKP | 81 | 5.0 | 3.53 | 73.5 | 78 | Merit |
| 73 | James Tarkowski | Everton | DEF | 80 | 6.0 | 3.47 | 72.9 | 81 | Merit |
| 74 | Nordi Mukiele | Sunderland | DEF | 79 | 5.5 | 4.88 | 70.7 | 86 | Merit |
| 75 | Anton Stach | Leeds | MID | 79 | 6.0 | 5.20 | 69.0 | 91 | Merit |
| 76 | Justin Kluivert | Bournemouth | MID | 79 | 6.0 | 5.17 | 68.9 | 93 | Merit |
| 77 | Caoimhín Kelleher | Brentford | GKP | 79 | 5.0 | 3.89 | 67.3 | 99 | Merit |
| 78 | Mikkel Damsgaard | Brentford | MID | 80 | 5.5 | 4.39 | 66.9 | 101 | Club floor |
| 79 | Pascal Groß | Brighton | MID | 80 | 5.5 | 4.33 | 66.7 | 103 | Club floor |
| 80 | Brennan Johnson | Everton | MID | 79 | 6.0 | 4.51 | 65.6 | 107 | Club floor |
| 81 | Alex Iwobi | Fulham | MID | 80 | 5.5 | 3.98 | 64.5 | 112 | Club floor |
| 82 | Francisco Evanilson de Lima Barbosa | Bournemouth | FWD | 80 | 6.0 | 4.27 | 62.5 | 121 | Club floor |
| 83 | Kevin Schade | Brentford | MID | 78 | 6.0 | 4.92 | 62.5 | 122 | Club floor |
| 84 | Daizen Maeda | Ipswich Town | MID | 79 | 5.5 | — | 60.5 | 130 | Club floor |
| 85 | Lucas Estella Perri | Leeds | GKP | 81 | 4.5 | 2.69 | 60.4 | 131 | Club floor |
| 86 | Rayan Vitor Simplício Rocha | Bournemouth | MID | — | 6.5 | 5.43 | 59.7 | 136 | Club floor |
| 87 | Matt O'Riley | Brighton | MID | 78 | 5.5 | 5.32 | 59.3 | 137 | Club floor |
| 88 | Antonee Robinson | Fulham | DEF | 82 | 4.5 | 3.09 | 58.7 | 140 | Club floor |
| 89 | Carlos Baleba | Brighton | MID | 81 | 5.0 | 2.87 | 57.6 | 146 | Club floor |
| 90 | Bernd Leno | Fulham | GKP | 80 | 4.5 | 3.33 | 57.0 | 151 | Club floor |
| 91 | Harry Wilson | Leeds | MID | 76 | 6.5 | 5.66 | 56.8 | 153 | Club floor |
| 92 | Florentino Ibrain Morris Luís | Ipswich Town | MID | 80 | 5.0 | 3.60 | 56.1 | 159 | Club floor |
| 93 | Omar Alderete | Sunderland | DEF | 78 | 5.0 | 4.02 | 54.2 | 170 | Club floor |
| 94 | Hidemasa Morita | Hull City | MID | 79 | 5.0 | — | 54.0 | 173 | Club floor |
| 95 | Konstantinos Tzolakis | Hull City | GKP | 79 | 4.5 | — | 53.9 | 175 | Club floor |
| 96 | Gustavo Hamer | Coventry City | MID | 77 | 5.5 | 3.34 | 44.3 | 226 | Club floor |
| 97 | Abdul Fatawu | Ipswich Town | MID | 76 | 5.5 | 4.06 | 42.6 | 235 | Club floor |
| 98 | Taiwo Awoniyi | Coventry City | FWD | 75 | 5.5 | 6.72 | 41.8 | 241 | Club floor |
| 99 | Jack Butland | Hull City | GKP | 75 | 4.5 | 3.53 | 33.8 | 289 | Club floor |
| 100 | Matt Grimes | Coventry City | MID | 74 | 5.0 | — | 30.1 | 315 | Club floor |

## History and squad strength

[[image2]]

*Figure 2. Five-season history and current squad strength agree at the top, but several clubs sit far from the diagonal—the space where model disagreement begins.*

## Model 1: structural mixture plus K

[[image3]]

*Figure 3. Model 1's complete structural forecast. Points are shown as a mean and 10–90% interval; title probability is printed at the right.*

[[image4]]

*Figure 4. K is a persistent season-level uncertainty control. Increasing it does not change the evidence; it changes how confidently the engine translates evidence into a title claim.*

## Models 2 and 3: adaptation versus feedback

Model 2 refuses to hide every unknown inside one K. It decomposes the season into club-specific stadium strength, zero-centred new-coach effects, transfer churn, promotion uncertainty, European workload and match-level availability. Its argument is that context does not affect every club equally. A new coach can be an improvement or a disruption; European competition creates fatigue in some weeks rather than subtracting an arbitrary number of points from August.

Model 3 takes a different route. A regularised gradient-boosted classifier learns nonlinear relationships from five chronological seasons of pre-match Elo, rolling points, goal difference, venue form, rest and season progress. Elo and form update after every simulated fixture, while heavy-tailed regime shocks permit the rare breakout or collapse seasons that Gaussian forecasts routinely suppress. On the 2025/26 holdout, its multiclass log loss is 1.058 against 1.082 for an unconditional baseline. That is useful improvement, not permission to call the algorithm an oracle.

The case for Model 2 is that 2026/27 contains enough manager, squad and workload change for adaptation to matter. The case for Model 3 is that early results create feedback: form, confidence and changing match probabilities alter the path after August. Their disagreement with Model 1 is a feature, because each can be wrong for a different reason.

## Where the models disagree

[[image5]]

*Figure 5. Each club's three model estimates, connected by their full spread. The black diamond is the declared consensus and the right label is the final expected-points rank.*

## Three models, one final probability distribution

[[image6]]

*Figure 6. Three engines, one probability distribution. Agreement is strongest on the leading group; the exact Arsenal–Manchester City order remains model-dependent.*

| Rank | Club | M1 pts | M1 title | M2 pts | M2 title | M3 pts | M3 title | Final pts | Final title | Top four | Relegated |
|---:|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 1 | Arsenal | 78.2 | 37.9% | 78.1 | 36.0% | 76.3 | 38.0% | 77.7 | 37.2% | 91.2% | 0.0% |
| 2 | Man City | 78.2 | 37.5% | 78.6 | 39.0% | 75.2 | 31.9% | 77.6 | 36.7% | 90.8% | 0.0% |
| 3 | Liverpool | 72.8 | 17.2% | 73.9 | 19.3% | 70.1 | 16.8% | 72.6 | 17.9% | 77.8% | 0.0% |
| 4 | Man Utd | 60.4 | 1.7% | 61.1 | 1.6% | 62.3 | 5.4% | 61.2 | 2.6% | 31.7% | 0.7% |
| 5 | Chelsea | 60.6 | 1.9% | 60.5 | 1.5% | 54.3 | 1.0% | 59.0 | 1.5% | 24.5% | 1.6% |
| 6 | Aston Villa | 58.5 | 1.2% | 59.7 | 1.1% | 57.5 | 2.6% | 58.8 | 1.5% | 22.8% | 1.3% |
| 7 | Newcastle | 58.2 | 1.2% | 60.5 | 1.2% | 54.2 | 0.8% | 58.1 | 1.1% | 21.1% | 1.7% |
| 8 | Spurs | 55.6 | 0.7% | 54.6 | 0.2% | 47.9 | 0.2% | 53.3 | 0.4% | 10.7% | 5.1% |
| 9 | Nott&#x27;m Forest | 51.0 | 0.2% | 49.8 | 0.0% | 52.4 | 0.8% | 50.9 | 0.3% | 6.6% | 5.9% |
| 10 | Bournemouth | 48.1 | 0.1% | 46.4 | 0.0% | 53.8 | 0.8% | 48.8 | 0.2% | 5.5% | 9.3% |
| 11 | Brighton | 47.5 | 0.1% | 46.9 | 0.0% | 51.1 | 0.4% | 48.2 | 0.2% | 4.0% | 9.8% |
| 12 | Brentford | 46.1 | 0.1% | 46.8 | 0.0% | 47.9 | 0.3% | 46.9 | 0.1% | 3.0% | 12.1% |
| 13 | Crystal Palace | 47.4 | 0.1% | 45.2 | 0.0% | 47.2 | 0.1% | 46.5 | 0.1% | 2.5% | 13.2% |
| 14 | Everton | 45.4 | 0.1% | 44.1 | 0.0% | 47.2 | 0.2% | 45.3 | 0.1% | 2.0% | 15.0% |
| 15 | Fulham | 44.9 | 0.0% | 45.2 | 0.0% | 45.9 | 0.1% | 45.3 | 0.0% | 1.9% | 15.9% |
| 16 | Leeds | 41.6 | 0.0% | 44.1 | 0.0% | 47.5 | 0.2% | 44.1 | 0.1% | 1.9% | 19.4% |
| 17 | Sunderland | 40.9 | 0.0% | 40.2 | 0.0% | 41.8 | 0.0% | 40.9 | 0.0% | 0.7% | 29.6% |
| 18 | Ipswich Town | 39.7 | 0.0% | 39.3 | 0.0% | 40.7 | 0.1% | 39.8 | 0.0% | 0.6% | 34.4% |
| 19 | Coventry City | 34.1 | 0.0% | 35.7 | 0.0% | 43.4 | 0.1% | 37.1 | 0.0% | 0.7% | 47.2% |
| 20 | Hull City | 29.6 | 0.0% | 28.2 | 0.0% | 32.4 | 0.0% | 29.8 | 0.0% | 0.0% | 77.7% |

## Complete evidence board

[[image7]]

*Figure 7. The complete evidence board: player representation, historical and squad evidence, uncertainty, all three simulations, their theses and the final weighted call.*

## The verdict

**Arsenal, by the smallest defensible margin.** The weighted view gives Arsenal 37.2%, Man City 36.7% and Liverpool 17.9%. The model's job is not to remove that ambiguity. Its job is to measure it.

## Full analysis and original sources

- [Full Elite analysis notebook](https://github.com/accidentalscientist/elite-analytics-articles-2026/blob/main/notebooks/13_premier_league_2026_27_forecast.ipynb)

Sources: [EA SPORTS FC 26](https://www.ea.com/games/ea-sports-fc/ratings?gender=0&orderBy=rank&page=1), [Fantasy Premier League](https://fantasy.premierleague.com/api/bootstrap-static/), [football-data.co.uk](https://www.football-data.co.uk/englandm.php), [Premier League manager guide](https://www.premierleague.com/en/news/4679012/meet-the-202627-premier-league-clubs-managers), and [2026/27 qualification summary](https://www.premierleague.com/en/news/4671514/summer-2026-key-football-dates-for-your-calendar).
