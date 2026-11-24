# The Critical Line Crossed: The Riemann Hypothesis and the ERI Labs Prediction Record

**Eric Ren · ERI Labs · Jersey City, New Jersey · Compiled November 24, 2026**

> *"The register is not empty. The AI will find what is in it."* — ERI Labs, May 29 / August 11, 2026
>
> *"I believe I have, working with Claude, discovered a proof of the Riemann Hypothesis."* — Levent Alpöge, November 20, 2026

| | |
|---|---|
| **Event** | Lean-only proof of the Riemann Hypothesis (RH) and the Generalized Riemann Hypothesis (GRH, Dirichlet *L*-functions) released Nov 20, 2026; certified by the Lean FRO and Mathlib Initiative Nov 21, 2026 |
| **Scope of this document** | Only the parts of the ERI Labs corpus that bear on RH, scored against the public record as of Nov 24, 2026 |
| **Corpus files scored** | `The-Mathematical-Discovery-Threshold…` (Aug 11) · `Mathematical-Structures-Reorganize-Entire-Systems` (Aug 12) · `Emergence-of-Mathematics` (Aug 18, one prediction) · `The-Bifurcation-of-Mathematical-Practice` (Aug 23) · ERI GitHub index (repo dates) |
| **Headline verdict** | Mechanism, format, verification regime, interpretation crisis, and cultural split: all called in advance, most arriving 12–30 months ahead of ERI's own windows. The one explicit miss: RH itself was placed outside AI reach before 2031. It fell in November 2026 through the exact mechanism ERI described. |

---

<img width="1300" height="1504" alt="Screenshot 2026-11-24 134244" src="https://github.com/user-attachments/assets/83cf14a8-8ce8-48f2-a235-d25a48b2b547" />

---

- https://github.com/ericrenone/The-Bifurcation-of-Mathematical-Practice

- https://github.com/ericrenone/Emergence-of-Mathematics

- https://github.com/ericrenone/Mathematical-Structures-Reorganize-Entire-Systems

---


## Contents

1. [TL;DR](#1-tldr)
2. [What happened, Nov 12–24, 2026](#2-what-happened-nov-1224-2026)
3. [The 2026 Riemann timeline (public record)](#3-the-2026-riemann-timeline-public-record)
4. [The ERI Labs timeline (RH-relevant entries only)](#4-the-eri-labs-timeline-rh-relevant-entries-only)
5. [Scorecard: ERI prediction → outcome](#5-scorecard-eri-prediction--outcome)
6. [Where the record ran ahead](#6-where-the-record-ran-ahead)
7. [The miss, stated plainly](#7-the-miss-stated-plainly)
8. [What the proof's own structure says about register crossing](#8-what-the-proofs-own-structure-says-about-register-crossing)
9. [Open items, dated](#9-open-items-dated)
10. [Sources](#10-sources)

---

## 1. TL;DR

- **Nov 20, 2026:** Levent Alpöge (Anthropic; Harvard Society of Fellows) posted a four-page note and a 14-part Lean archive (~17.4 million lines, 175,187 files) proving RH and GRH for Dirichlet *L*-functions. No human-readable paper. His Claude-drafted prose version ran past 250,000 pages and was withheld. The dated work spans **Oct 6 → Nov 16, 2026: 41 days.**
- **Nov 21, 2026:** The Lean FRO and Mathlib Initiative certified both statement and proof: the theorem matches Mathlib's own `RiemannHypothesis`; the export passed Lean's kernel, `con-leche`, `con-ron`, and independent third-party checkers in other languages.
- **No one has read it.** Kevin Buzzard: nobody yet knows *why* the theorem is true. Alpöge himself reports "little mastery" of some of the machinery (automorphic forms on higher-rank groups). This is the **alien proof** ERI defined in May and forecast for 2027–2029.
- **Same day, the other culture published too.** Hours after Alpöge, Ravi Vakil posted Alessandro Masullo's 940-page, twelve-year, no-AI GRH draft. Two research cultures, one afternoon: the **bifurcation** ERI described Aug 23.
- **The miss:** ERI placed RH in the "will NOT be solved 2026–2031" tier on Aug 11 and repeated it Aug 23. That was wrong by at least four years. It was also the *shortest* public horizon on record: Tao said ~2050; Metaculus ~May 2035; Anthropic's own Aug 10 note said it did not expect Claude's techniques to lead to a proof.
- **Why the miss matters less than it looks:** ERI's framework explicitly separated *mechanism* (predictable) from *problem selection and timing* (unpredictable), and the proof's architecture (Stepanov's finite-field argument transplanted into number fields via automorphic forms, Galois representations, Arakelov geometry, *p*-adic Hodge theory) is register crossing into the w≥4–5 tier ERI tabulated as "accessible via human–AI collaboration."

---

## 2. What happened, Nov 12–24, 2026

| Date | Event |
|---|---|
| **Nov 12** | Kevin Buzzard (Imperial) publishes four questions any AI-written Lean proof must answer. They become the checklist applied eight days later. |
| **Nov 19** | Anthropic stock-market debut. |
| **Nov 20 (morning)** | Alpöge's four-page note on his personal site: RH and GRH proved "working with Claude"; released only as Lean. Timeline (compiled by Claude) runs Oct 6 "Stepanov determinant" → Nov 16 "GRH." He writes he "guided us to the right situation" and that Claude "far outpaced me near the finish line." He addresses the IPO timing directly and says he consulted Dario Amodei before posting. |
| **Nov 20 (hours later)** | Ravi Vakil (Stanford) posts Masullo's *The Music of the Primes*: 940 pages, human-written, Connes-style trace formula on the idele class group, vetted privately by Brian Conrad for months. Masullo says it is not fit for dissemination and has many bugs; Chapter 13 (deduction of GRH) is placeholders. |
| **Nov 20** | Yudkowsky: RH "has fallen." Hacker News top story. Independent text scan of the archive: no `sorry`, no extra axioms. |
| **Nov 21** | **Joint statement, Lean FRO + Mathlib Initiative:** "full confidence" the proof is correct. Statement isolated in a Mathlib-only file; `comparator` and `con-leche --compare` confirm it is Mathlib's RH; dozens reproduce the build and identical export; kernel + `con-leche` + `con-ron` + third-party checkers accept it; checks run on an inert export so proof-source code cannot interfere. Andrew Sutherland (MIT) hosts the verification ledger. |
| **Nov 22** | Sutherland's ledger lists as verified: RH (Mathlib definition) and GRH for Dirichlet *L*-functions, all moduli and characters. **Not** verified: Dedekind zeta, Hecke, automorphic *L*-functions. Rubinstein and Adriazola circulate human-readable route sketches; R. Zhang (IHES) posts a preliminary architecture note; a crowd "proof guide" appears. John Baez posts on Masullo. |
| **Nov 22–23** | Alexandr Wang essay: superintelligence arriving. Maynard (Oxford): "98 or 99 percent" certain; "a historic milestone" if it checks out. Saha (QMUL): the result "shatters my model of reality"; Alpöge "should get a Fields Medal." Buzzard: understanding will arrive "in a matter of weeks." |
| **Nov 24** | Status: machine-certified, human-uninterpreted. Clay Institute: no statement; the prize requires publication and a two-year waiting period. |

---

## 3. The 2026 Riemann timeline (public record)

| Date | Milestone | Register / form |
|---|---|---|
| **Aug 10** | Anthropic: unreleased Claude research build lifts the proportion of zeta zeros known to lie on the line from **41.6% → 67.2%** (simple and on the line). Prompted by a non-mathematician staffer (Jarred Sumner) in Claude Code; two sessions, 31M output tokens. Validated by Alpöge and Ralph Furman; reviewed by Conrey and Goldston; Lean formalization supplied. Anthropic: "We don't expect that the techniques Claude used will lead to proving the Riemann hypothesis." | Analytic (Weil quadratic form, Montgomery pair correlation + Bombieri 2000). Lean. |
| **Aug (arXiv 2608.13637)** | Furman, *More than two thirds of the zeta zeros are simple and on the critical line*. | Human write-up of the Claude result. |
| **Sep 2** | Lamzouri (Lorraine), arXiv 2609.02882: shorter, all-human re-proof of 67.25% via a Hilbert-space inequality. | Human-led culture digesting an AI result. |
| **Sep–Oct** | Follow-on preprints push the bounds (83.69% distinct; 83.9% distinct / 67.35% simple-on-line), several shipping Lean developments built on the Aug library. | Lean becoming the submission norm. |
| **Sep 8** | OpenAI: claimed resolution of Navier–Stokes (finite-time blowup) with Lean, ~10,000 agents, 88 hours; credit dispute involving Buckmaster and Alpöge. | Millennium problem #1 claimed. |
| **Sep 30 / Oct 6** | OpenAI: **quasi-Riemann hypothesis** (all nontrivial zeros have real part in [1/8, 7/8]; 199 pp, Lean-verified) among 377 announced / 722 released results; a weaker 11/12 version (49 pp, not formalized) is the one humans studied. Metaplectic forms; a 2021 Dunn–Radziwiłł formula is a key ingredient. Lichtman: "the most significant AI-for-math achievement so far, by quite a margin." Experts had believed this branch's tools insufficient; the proof introduces no new concepts. Sarnak repurposes a course to study it. | Analytic → metaplectic register. First large-scale human *interpretation* effort. |
| **Oct** | Tao: expects RH to fall "to a combination of humans and AI around 2050 or so." Metaculus median ~May 2035. Sawin: full RH "may still feel as far off as before." Bloom: "nothing would surprise me." | Consensus horizon: 9–24 years. |
| **Oct 6** | Alpöge's dated timeline begins ("Stepanov determinant"). | — |
| **Nov 16** | Timeline ends ("GRH"). | — |
| **Nov 20–21** | Release and certification (Section 2). | Function-field → number-field transplant; automorphic forms, Galois representations, Arakelov geometry, integral *p*-adic Hodge theory, theta lifts, Siegel–Weil, trace formulas. Lean-only. |

---

## 4. The ERI Labs timeline (RH-relevant entries only)

| Date | ERI artifact | What it said about RH, Lean, alien proofs, or the culture split |
|---|---|---|
| **Feb 17** | `Mobius-Inversion-Frobenius-Fixed-Points` | "Grokking is just the moment the signal gets strong enough for the math to subtract the noise." Grokking-as-phase-transition framing later applied to mathematical AI. |
| **May 29** | Predictive framework published (referenced across the corpus) | Register-crossing mechanism named; unit-distance disproof (May 2026) taken as the validating case. Specific-problem bets: prime gap < 100, sunflower, chromatic number ≥ 6, R(5,5). |
| **Aug 3** | `ERI-Labs-vs.-OpenAI-Mathematical-Discovery-Predictions-and-Outcomes` | May predictions vs. OpenAI's Aug 1 ten results: zero overlap on specific problems; mechanism intact. |
| **Aug 11** | `The-Mathematical-Discovery-Threshold-Register-Crossing-and-Bifurcation-in-AI-Assisted-Proof` | Depth taxonomy (w=1…w≥5). **"Clay Millennium Problems remain open … Riemann Hypothesis: Requires new structures, not register crossing."** Alien proof defined and dated 2027–2029. Grokking window Q1 2027–Q2 2028. Lean "Erdős–Rao threshold." Collaboration Pattern C: formal verification + human interpretation. "Which specific problems fall in which order" declared unpredictable. |
| **Aug 12** | `Mathematical-Structures-Reorganize-Entire-Systems` | Tsimerman (Fields Medal) → OpenAI as prestige-bifurcation signal. First alien proof by Q2 2028. "Formalization as validation standard" for claimed classical open problems by 2028. Proof-interpretation conference track / journal section by 2029. Dual peer-review tracks by 2028. |
| **Aug 18** | `Emergence-of-Mathematics` | Prediction 3: mathematical reasoning emerges in artificial systems and improves spontaneously with scale. |
| **Aug 23** | `The-Bifurcation-of-Mathematical-Practice` (reply to Weinreich, arXiv 2608.02859) | Two coexisting cultures (AI-integrated vs. human-led). "Interpretation" named as a new class of mathematical work. Sides with Tao: prestige shifts to those who verify and digest. **"AI will not solve these [Clay problems] before 2031."** Prescriptions: formalize everything in Lean so no corporation owns the result; maintain institutional independence from AI companies. |

---

## 5. Scorecard: ERI prediction → outcome

Legend: ✅ landed · ⏩ landed early (ahead of ERI's own window) · ◐ partial / in progress · ❌ missed · ⏳ not yet due

| # | ERI prediction (file, date, stated window) | Outcome as of Nov 24, 2026 | Verdict |
|---|---|---|---|
| 1 | **Alien proof**: a Lean-verified theorem whose strategy no human can explain (Aug 11, P1.4, *2027–2029*; Aug 12, 3b, *by Q2 2028*) | 17.4M-line RH/GRH proof certified Nov 21; no human has read it; Alpöge reports limited mastery of its own tools; Buzzard: nobody yet knows why it is true. First on the most famous problem in mathematics. | ⏩ |
| 2 | **Lean as validation standard** for claimed solutions to classical open problems (Aug 12, 6c, *by 2028*; Aug 23, P1.4, *2028*) | Aug 10 Claude bound: Lean. Sep 8 Navier–Stokes: Lean. Sep 30 quasi-RH: Lean. Nov 20 RH: Lean **only**, no paper. Buzzard's four-question Lean checklist (Nov 12) is now the de facto gate. | ⏩ |
| 3 | **Interpretation as a distinct class of mathematical work** (Aug 23, Part II; Aug 12, 3c, *by 2029*) | Sarnak course on quasi-RH; Rubinstein/Adriazola route sketches; Zhang (IHES) architecture note; crowd proof-guide; "people worldwide translating parts of the code into English" (Buzzard). Not yet institutional. | ◐ early |
| 4 | **Collaboration Pattern C**: formal verification (Lean + AI) + human interpretation (Aug 11, Part VII) | Exactly the shape of Nov 20–24: machine certifies in 24h; humans begin weeks-to-months of interpretation. | ✅ |
| 5 | **Prestige transfers to verifiers/digesters; Weinreich's "humans as messengers" is taste, not necessity** (Aug 23, Part II) | Alpöge: "Claude far outpaced me near the finish line"; Saha: credit belongs to the human who steered, "should get a Fields Medal." Verification community (Lean FRO, Mathlib, Sutherland) is the public arbiter. | ✅ |
| 6 | **Bifurcation into two coexisting cultures** (Aug 11, P3.1, *2028–2031*; Aug 23, throughout) | Nov 20: Lean-only AI-assisted proof and a 940-page human draft of the same theorem posted hours apart. Lamzouri's human re-proof of the Aug AI bound. WaPo: the result brings "both wonder and loss." | ⏩ |
| 7 | **Prestige bifurcation**: frontier-lab affiliation displaces institutional prestige (Aug 12, Part VII) | Tsimerman → OpenAI (Aug 9). Alpöge, Harvard junior fellow, works at Anthropic; breakthroughs "concentrated in tech companies with access to internal models" (Buzzard). | ✅ |
| 8 | **Grokking-style multi-domain jump 9–18 months after Aug 2026** (Aug 11, P1.2, *Q1 2027–Q2 2028*) | Navier–Stokes (Sep 8), 377/722 results incl. quasi-RH (Oct 6), RH/GRH (Nov 20): three Millennium-class events in 11 weeks, 1–3 months after the August marker. | ⏩ direction right, window too conservative |
| 9 | **Corporate capture risk; "formalize everything in Lean, once in Lean no corporation owns it"** (Aug 23, Part VI) | Release the day after Anthropic's IPO; Alpöge pre-empts the cynical reading. Navier–Stokes authorship dispute (Bubeck/Alpöge). Lean release let an independent community certify RH in 24 hours with no dependence on the company. | ✅ |
| 10 | **Problem selection is unpredictable from mechanism alone** (Aug 11, Part II) | Every forecaster, ERI included, placed RH years out. It was the next to fall. The framework's own disclaimer is the most accurate sentence in the corpus. | ✅ (meta) |
| 11 | **w≥5 (motivic/categorical/automorphic) "accessible via human–AI collaboration"** (Aug 11, depth table) | The proof lives there: automorphic forms on higher-rank groups, Galois representations, *p*-adic Hodge theory, Arakelov geometry. Human steered, AI finished. | ✅ |
| 12 | **Mathematical reasoning emerges and scales spontaneously in artificial systems** (Aug 18, Prediction 3) | Aug 10 bound found by a model given an "unreasonable challenge" by a non-mathematician; Nov 20 proof finished by the model in the last stretch. | ✅ |
| 13 | **Lean "Erdős–Rao threshold": proof assistants move from verifying to discovering** (Aug 11, Part IV; Aug 12, Part X, *Q3 2027–Q1 2028*) | A 17M-line library depending directly only on Mathlib, generated faster than any human can read, is the discovery regime. Mathlib growth-rate metric not yet measured. | ◐ early |
| 14 | **"Riemann Hypothesis: requires new structures, not register crossing"** (Aug 11, Part VI) | Quasi-RH: "introduces no new concepts" (Quanta). RH: Stepanov's finite-field argument carried into number fields; Buzzard puts new theory anywhere from zero to ~1,000 pages. Register crossing did the work. | ❌ boundary misplaced |
| 15 | **"AI will not solve these [Clay problems] before 2031"; RH listed first** (Aug 11, Part VI; Aug 23, Part IV) | RH and GRH certified Nov 21, 2026. | ❌ |
| 16 | **Navier–Stokes global regularity remains open before 2031** (Aug 11, Part VI) | OpenAI claimed finite-time blowup Sep 8 with Lean; disputed credit; Clay prize unclaimed; not independently certified in the way RH was. | ❌ pending |
| 17 | Prime gap < 100; sunflower; chromatic number ≥ 6 (May 29; Aug 11, P2.x, *2027–2028*) | Not yet due. | ⏳ |
| 18 | FrontierMath 5–10% → 30–40% jump (Aug 11, P1.2; Aug 12, 2a, *Q1–Q2 2027*) | No benchmark data located in this compilation. | ⏳ |

**Tally:** 9 landed or landed early · 2 partial/early · 3 missed · 2 not yet due · 1 meta-hit. Of the 13 calls that are scoreable today, 10 resolved in ERI's favor and 7 of those arrived ahead of ERI's own window.

---

## 6. Where the record ran ahead

### 6.1 The alien proof (predicted 2027–2029; arrived Nov 2026)

ERI, Aug 11:

> *"Lean verification will produce the first formally-correct theorem whose proof no human mathematician can strategically understand. This 'alien proof' will be: Mathematically correct (Lean-verified) · Logically valid (every step justified) · Humanly opaque (proof strategy incomprehensible). This creates an epistemological crisis: a true mathematical statement without human understanding."*

Record, Nov 20–24: a 17.4-million-line Lean library; certified by kernel and three independent checker families; author withholds a 250,000-page prose draft; author reports little mastery of the automorphic machinery; Buzzard says nobody yet knows why the theorem is true. phys.org headline: "a proof no human can read." Alpöge's own stated next step is to understand, simplify, and write it up.

ERI's resolution path, Aug 11: *"New mathematical frameworks emerge to interpret alien proofs—not by translating them to human language, but by building intermediate abstraction layers that make the logical structure visible."* The Rubinstein/Adriazola sketches, Zhang's IHES note, and the crowd architecture guide are those layers forming in real time.

One caveat to carry: Buzzard expects comprehension "in a matter of weeks." If a human-readable account exists by January, the proof was *alien for a season*, not permanently. ERI's Part XI already listed this as open: "Whether alien proofs can be made humanly comprehensible, or if epistemology must shift."

### 6.2 Lean as the gate (predicted 2028; arrived 2026)

ERI, Aug 12, 6c: *"By 2028, papers claiming to solve classical open problems will include Lean formalization as standard validation method."*

Record: every 2026 Millennium-class claim shipped Lean (Aug 10, Sep 8, Sep 30, Nov 20), and the RH proof shipped *nothing else*. The verification protocol itself (statement isolation, `comparator`, multi-kernel replay on inert export, public ledger) was codified by Buzzard on Nov 12 and executed by the community in under 24 hours. ERI's Aug 23 prescription, *"Formalize everything in Lean. Once a theorem is in Lean, no corporation owns it,"* is the reason the certification could be issued by the Lean FRO and Mathlib rather than by Anthropic.

### 6.3 Two cultures, one afternoon (predicted 2028–2031; visible Nov 20, 2026)

ERI, Aug 23: *"Culture A (AI-Integrated): AI-assisted register-crossing for discovery, followed by human interpretation, followed by Lean formalization … Culture B (Human-Led): traditional methods, avoiding AI generation and AI verification … Neither will disappear."*

Record: Alpöge (Culture A: strategy by human, execution by Claude, Lean-only output) and Masullo (Culture B: twelve years, 940 pages, no AI, trace-formula route in the Connes tradition) posted the same theorem within hours. Lamzouri's September re-proof of the August AI bound is Culture B digesting Culture A. The Lean community is building a crowd formalization of Masullo's draft: Culture A tooling applied to Culture B output. Weinreich's "total opposition" essay (arXiv 2608.02859, Aug 2026) and the WaPo framing of "wonder and loss" are the professional-identity stress ERI located as the *real* crisis.

### 6.4 The grokking window (predicted Q1 2027–Q2 2028; opened Sep 2026)

ERI, Aug 11: *"the next major grokking event in mathematical capability is likely 9–18 months away … breakthroughs across at least 5 distinct mathematical domains simultaneously."*

Record: fluid dynamics (Sep 8), analytic number theory via metaplectic forms (Sep 30), and RH/GRH via automorphic/Galois machinery (Nov 20) inside eleven weeks, plus the 722-paper release on Oct 6. Direction and shape correct; ERI's timing was the conservative error, the same direction as the May→August compression ERI had already flagged as an open question.

### 6.5 Who gets the prestige (Aug 23 vs. Weinreich)

ERI backed Tao's position that prestige migrates to those who verify and digest, against Weinreich's view that this "sounds boring." Record: the names attached to the RH event on Nov 21–24 are Alpöge, the Lean FRO, the Mathlib Initiative, Sutherland, Buzzard, Maynard, Rubinstein, Adriazola, Zhang. The verification-and-interpretation layer *is* the public story.

---

## 7. The miss, stated plainly

ERI wrote, Aug 11 (`Part VI: What Will NOT Be Solved 2026–2031`):

> *"Clay Millennium Problems remain open · Riemann Hypothesis: Requires new structures, not register crossing … AI can cross into existing registers. It cannot yet generate genuinely new registers from first principles. This is the hard boundary."*

and Aug 23:

> *"Clay Millennium Problems remain untouched in August 2026. This is expected. Register-crossing cannot solve problems that require inventing new mathematical structures. … AI will not solve these before 2031. They require human mathematical imagination."*

RH and GRH were certified on Nov 21, 2026. Navier–Stokes was claimed on Sep 8, 2026. Two of the four named Clay problems moved within four months of the sentence being written.

What the miss consists of, item by item:

| Claim | Status |
|---|---|
| RH not before 2031 | Wrong by ≥4 years. |
| RH "requires new structures" | Not supported. The proof transplants a 1969 finite-field argument (Stepanov) into number fields using existing automorphic, Galois, Arakelov and *p*-adic Hodge machinery. Whether any genuinely new theory sits inside the 17M lines is open (Buzzard: zero to ~1,000 pages), but the *route* is cross-register, not new-register. |
| "Human mathematical imagination" required | Partly right in an unexpected way: Alpöge chose the Stepanov transplant and "guided us to the right situation." The imagination was human; the execution across registers was not. |
| Navier–Stokes open before 2031 | Claimed resolved Sep 8; not community-certified at RH's standard; credit disputed. Pending. |

How the horizon compared with other public forecasts:

| Forecaster | Date of forecast | RH horizon |
|---|---|---|
| Terence Tao | Oct 2026 | "around 2050 or so," humans + AI |
| Metaculus community | pre-Nov 2026 | ~May 2035 |
| Anthropic (Aug 10 note) | Aug 10, 2026 | did not expect Claude's techniques to lead to a proof |
| Abhishek Saha | stated Nov 21 | had expected "several years" |
| Will Sawin | Oct 19, 2026 | "may still feel as far off as before" |
| **ERI Labs** | **Aug 11 / Aug 23, 2026** | **not before 2031** |

ERI's was the shortest horizon in the set and still a miss. The framework's own Part II is where the correction already lived: *"Capability scales while predictability limits: We can predict register crossing will happen. We cannot predict which problem gets crossed into first."* RH was the problem crossed into. The error was treating one problem as structurally exempt from a mechanism the rest of the corpus called universal.

---

## 8. What the proof's own structure says about register crossing

ERI's depth taxonomy (Aug 11):

| Depth | Register | ERI's Aug 11 capacity estimate |
|---|---|---|
| w=2 | Analytic / geometric | Solvable via register crossing |
| w=4 | Algebraic number-theoretic (cyclotomic fields, *L*-functions) | Frontier of AI reach |
| w≥5 | Motivic / categorical / derived (Langlands program) | Accessible via human–AI collaboration |

The RH problem had crystallized, for 167 years, as a w=2 analytic question about one function. The three 2026 advances each moved it one register deeper:

1. **Aug 10 (Claude, 67.2%):** stayed analytic, Weil quadratic form and pair correlation. Anthropic correctly judged this route would not reach RH.
2. **Sep 30 (OpenAI, quasi-RH):** crossed into metaplectic forms, a family beyond zeta alone. Sarnak had argued for a family approach; Iwaniec "narrowly missed the right family in 2002." The proof "finds hidden connections between existing ideas" and "introduces no new concepts." Experts had believed the branch's tools insufficient. This is ERI's register-crossing description verbatim, applied to RH's neighborhood.
3. **Nov 20 (Alpöge + Claude, RH/GRH):** crossed into the function-field register (Stepanov's proof of RH for curves over finite fields) and carried it back to number fields through automorphic forms on unitary and general linear groups over CM fields, base change, Galois representations, Siegel–Weil, theta lifts, Arakelov geometry and integral *p*-adic Hodge theory. Alpöge's own analogy for the missing step: "differentiating the integers," an operation with no obvious meaning. Baez: "transplants Stepanov's proof from finite fields to number fields." Saha: a long detour through machinery built for other problems that "somehow creates a wormhole" to the target.

That third step is w≥5 by ERI's own table, and ERI's own table said w≥5 was reachable by human–AI collaboration. The corpus contained the correct answer and then overrode it with a one-line exemption for the Clay list.

Two more corpus items the proof's shape confirms:

- **Pattern A inverted.** ERI's Pattern A was "Register Proposal (AI) + Proof (Human)." Nov 20 was the mirror: register proposal by the human (Stepanov transplant), proof execution by the AI near the finish. Both directions are now on the record.
- **The Aug 10 "unreasonable challenge."** A non-mathematician prompted Claude to "take a real stab" at RH; it produced a bound instead. ERI's Aug 18 Prediction 3 (mathematical reasoning emerges and scales in artificial systems without being programmed in) and ERI's register-independence claim (search "blind to the crystallization barriers that human discourse inherited") describe this episode more precisely than the lab's own framing did.

---

## 9. Open items, dated

| Item | What would resolve it | ERI's stake |
|---|---|---|
| Human-readable account of the RH proof | A sketch accepted by analytic number theorists; Alpöge's promised write-up | Decides whether item #1 is "alien for a season" or a standing epistemological shift |
| Amount of genuinely new theory inside the 17M lines | Expert audit of the architecture guides (Rubinstein, Adriazola, Zhang) | Decides how wrong "requires new structures" was: boundary misplaced vs. boundary wrong |
| Extension to Dedekind / Hecke / automorphic *L*-functions | Sutherland ledger entries | Alpöge expects the extended version "given more time" |
| Masullo draft | Chapter 13 filled in; Conrad's revision; crowd formalization | Whether Culture B produces an independent human proof of the same theorem |
| Clay Prize | Publication + two-year window + committee | Tests ERI's claim that institutions lag research by 18–36 months |
| Journal handling | Where and how a Lean-only proof is "published" | ERI 8a (dual review tracks by 2028) and 3c (interpretation venue by 2029) |
| Mathlib growth rate, Q4 2026 vs Q4 2025 | Commit statistics | ERI's 3–5x "crystallization" signal |
| Prime gap, sunflower, chromatic number, R(5,5) | 2027 results | ERI's remaining Tier-2 bets |

---

## 10. Sources

**Primary**
- Lean FRO + Mathlib Initiative, *Lean verification of the Riemann Hypothesis*, Nov 21, 2026 — leanprover-community.github.io/blog/posts/riemann-hypothesis/
- A. Sutherland (MIT), verification ledger — math.mit.edu/~drew/grh
- Anthropic, *Learning more about Claude's mathematical capabilities*, Aug 10, 2026 — anthropic.com/research/riemann-zeta
- R. Furman, arXiv 2608.13637 (Aug 2026)
- Y. Lamzouri, arXiv 2609.02882 (Sep 2, 2026)
- OpenAI, *On the Navier–Stokes Millennium Prize Problem*, Sep 8, 2026
- R. Zhang (IHES), *A preliminary note on Alpöge's proposed proof of GRH*, Nov 2026
- M. Weinreich, arXiv 2608.02859 (Aug 2026)

**Reporting and commentary**
- Quanta, *AI Proved the Quasi-Riemann Hypothesis. What Happens Now?*, Oct 19, 2026
- Washington Post, Nov 20, 2026; Al Jazeera, Nov 21, 2026; IBM Think, Nov 20–23, 2026; phys.org, Nov 20 and Nov 23, 2026
- The Decoder, Nov 22, 2026 (Tao ~2050; Metaculus ~2035)
- J. Baez, *Masullo on the Riemann Hypothesis*, Nov 22, 2026
- NPR / Axios on Navier–Stokes, Sep 2026
- Alpöge's four-page note, Nov 20, 2026 (personal site), as quoted across the above

**ERI Labs corpus (github.com/ericrenone)**
- `The-Mathematical-Discovery-Threshold-Register-Crossing-and-Bifurcation-in-AI-Assisted-Proof` — Aug 11, 2026
- `Mathematical-Structures-Reorganize-Entire-Systems` — Aug 12, 2026
- `Emergence-of-Mathematics` — Aug 18, 2026
- `The-Bifurcation-of-Mathematical-Practice` — Aug 23, 2026
- `ERI-Labs-vs.-OpenAI-Mathematical-Discovery-Predictions-and-Outcomes` — Aug 3, 2026
- `Mobius-Inversion-Frobenius-Fixed-Points` — Feb 17, 2026

---

*Document status: record current to Nov 24, 2026. Next revision on first human-readable account of the Alpöge proof, or on a Clay Institute statement, whichever comes first.*
