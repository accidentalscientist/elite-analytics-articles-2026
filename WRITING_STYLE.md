# Field Notes: structure and writing style

A working analysis of the house style across the 13 published articles, written for future reference and eventual folding into the Field Notes section of the site design doc. Grounded in what the pieces actually do, not in aspiration.

## 1. The seven-part skeleton

Every data-journalism piece (all but Bluewater Ascendancy, which is a personal essay and deliberately exempt) now follows the same load-bearing shape:

1. **Unnamed executive summary**, no heading, minimum two paragraphs. Paragraph one states the thesis in plain declarative sentences. Paragraph two tells the reader how many views are coming and, increasingly, gestures at the cover image directly ("the chart above," "summarised in the chart opening this piece").
2. **Background**, one `##` section, no image. Supplies the context a reader needs before the evidence starts: history, definitions, why the topic matters. In several pieces (Premier League 15 Years, Article 13) this doubles as a methodological cold open — a data-hygiene failure, a modelling caveat — which does double duty as both context and credibility.
3. **Five graphic sections**, each `##` heading naming the *finding*, not the chart type ("Annual totals conceal the operating problem," never "Chart 2: Seasonal boxplot"). Each follows a fixed three-paragraph internal order:
   - **Paragraph 1 (technical, unlabelled):** how the chart was built. Not narrated as a caption ("this chart shows..."), but as method: what was grouped, weighted, fitted, or compared, and why that construction was chosen over an obvious alternative.
   - **Paragraph 2 (discussion):** what the chart actually shows, described in specific, checkable terms.
   - **Paragraph 3 (discussion):** what it means, and what it argues against.
4. **The sixth, synthesis graphic.** A large-format composite board recapping the five preceding figures plus the restated thesis, always positioned as its own section immediately before the closing prose, always described the same way ("brings the article's five principal pieces of evidence into one readable argument").
5. **Expanded thesis close.** A `##` section that walks back through each of the five findings in one sentence apiece, states the deeper conclusion explicitly, and ends on a short, quotable line that echoes (never repeats verbatim) the opening thesis.
6. **Personal takeaway**, folded into the last paragraph of the close rather than given its own heading. First-person, specific to that article's evidence, never generic ("what I find myself watching," "the number I'd want updated first," "I'd rather publish a model that honestly found nothing"). This is the one place the voice drops the analytical third person on purpose.
7. **Methods and original sources.** States the actual tools (pandas, matplotlib, scikit-learn, statsmodels — named specifically, not "data science techniques"), then lists the source notebooks as a plain bullet list. Never repeats what the graphic-section technical paragraphs already said; adds the tooling layer they leave implicit.

The structure is never labelled. No section is called "Technical Note" or "Discussion" or "Personal Takeaway." A reader infers the register shift from content alone, which is the whole point — declaring the seams would flatten exactly the texture the structure is built to create.

## 2. Sentence-level habits

- **No em dashes, anywhere, on principle.** Parenthetical asides use actual parentheses or a colon; a break that would reach for a dash instead becomes two sentences. This is a hard site-wide rule, not a per-article style choice.
- **En dashes survive** in genuinely numeric or compound contexts (`2010–2017`, `attack–defence`), which is a different mark doing a different job and isn't covered by the em-dash ban.
- **Numbers are exact, never rounded to a vague adjective.** "China's total rises to more than double the US level," not "China's emissions are much higher." A chart caption states a percentage or a unit; the interpreting sentence around it never restates the number in softer language.
- **The "X is not Y, it is Z" construction** recurs constantly as a thesis-sharpening device: "Meeting demand is a quantity problem; lowering emissions is a composition problem." "It is not a smaller version of national data. It answers different questions." This is the single most identifiable sentence pattern in the whole corpus.
- **Rhetorical negation before affirmation.** A claim is frequently stated by first ruling out the easy misreading, then landing on the real one: "This is not a correction that makes the first chart wrong. It measures a different capability." The reader is walked past the wrong interpretation on the way to the right one, rather than being told the right one cold.
- **Section headings are findings, never labels.** "Cleaner does not automatically mean cheaper," not "Price Analysis." A heading should be quotable on its own, ideally arguable, never a table of contents entry.
- **Caveats are load-bearing, not defensive.** "The chart cannot identify the cause. It contains no training load, sleep, injury, weather or course-condition variables. It can still reject one interpretation" — the caveat states exactly what the evidence *can't* claim, then immediately re-anchors what it *can*. Never a vague "of course, correlation isn't causation" thrown in without follow-through.

## 3. Structural devices used across the corpus

- **Five findings, walked twice.** Once individually (the five graphic sections) and once as a compressed recap in the close ("The generation chart shows a changing mix. Seasonality shows why timing matters..."). The second pass is always a single sentence per finding, in the same order they appeared.
- **The synthesis board mirrors the text, on purpose.** Its title and subtitle are drawn from the opening thesis; its closing "argument" box is drawn from the closing thesis. The visual structure and the prose structure are the same argument told twice, not two different summaries.
- **A named methodological failure, told straight, is a recurring credibility move.** Premier League 15 Years opens on a season-calculation bug that wrongly crowned Arsenal twice. Article 13 documents a migration-adjacent bug in its own construction (`StringDataRightTruncation`), a discipline model that found no signal, and states plainly when a modest engine beats a fancy one only "modestly." The house instinct is to report a negative or embarrassing result as the finding, not bury it.
- **Numbers earn their place by being specific and comparable, not just large.** "91% of the deepest longitudinal sample" lands harder than "most of the data," because it's falsifiable and because the piece already told you what it's 91% *of*.

## 4. What doesn't vary by topic

The same skeleton, sentence habits and devices show up whether the subject is NEM generation data, global GDP composites, Premier League tables, or a personal parkrun record. The house style is topic-agnostic; only the vocabulary changes (megawatt-hours vs. expected points vs. Gini coefficients). That consistency is itself a design decision worth naming explicitly if this becomes a formal style guide: a reader who's finished one Field Notes piece already knows the shape of the next one before opening it.

## 5. The one deliberate exception

Bluewater Ascendancy (the Total War modding piece) does not follow this skeleton, and per the current editorial decision, it stays that way rather than being forced into it. It's personal essay, not data journalism: no numbered graphics, no synthesis board, no explicit thesis-then-echo structure. If the site ever wants every Field Notes piece to share one skeleton regardless of genre, this is the piece that would need the most rework to fit it, and the most honest test of whether the skeleton actually generalises beyond data-driven writing.
