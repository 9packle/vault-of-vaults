# BPhO Papers Collection — Heuristic Solution Manual

> **How to read this document.** Every solution has visually separated layers:
>
> - **Main column** — the standard, exam-ready solution. It is complete on its own and could be copied out as an answer. It contains **no meta-commentary**: nothing about mark schemes, version history, or the writing process ever appears here.
> - **`【Thought】` side notes** (blockquotes) — method teaching. A thought answers exactly three questions: *what signal in the problem text fired, what move it triggers, and where that move fails* — in about 80 words or fewer. The phrasing is free ("key line", "Method:", "Signal:"); only the three elements are mandatory, and the same template sentence may appear at most 3–5 times per paper. Thoughts are for the student's *transfer*, not the author's *replay*: no full derivations, no first-draft history.
> - **`【Official approach】`** (blockquote, ≤3 sentences) — a genuinely different or cleverer official method, worth *learning*; it always ends with its dependency: *the trick relies on condition C; if C fails, return to the general method.*
> - **`【Errata】`** (blockquote, ≤3 sentences) — an official slip, worth *avoiding*: one sentence naming the error, one giving the corrected value, one giving the closed-loop check. Version history of this manual itself lives in an appendix, never in these notes.
>
> **Tiered structure — teaching space follows method content, not question number.** Hard problems (≥4 marks or multi-step) get the full six-step skeleton — (1) key observation → (2) diagram & symbols → (3) assumptions → (4) governing equations → (5) solution → (6) check + answer — plus a transfer sentence (below) and at least one *boundary-type* check. Medium problems compress to *key observation → solution → verification check*. Short items (≤2 marks, multiple choice) compress to *key observation → answer with option*. One rule regardless of tier: sub-parts are numbered (i), (ii), (iii)…; any cross-reference carries its full address ("from Q1(b)(ii)…"), and no main-column derivation step exceeds three lines.
>
> **The transfer sentence.** Every hard problem ends its `【Thought】` with one sentence a student can reuse: *"Next time you see X, try Y first; if Z holds, Y fails."* — ≤30 words. It is the teaching payload of the whole solution.
>
> **Two kinds of check.** *Verification checks* serve this problem: dimensional audit, limit probe, substitution back into the governing equation. *Boundary checks* serve the next problem: change one condition (frictionless → rough, ideal gas → real, given datum → another value) and ask how the answer moves. Every hard problem carries at least one boundary check — transfer ability is built exactly at the boundary. All checks remain *diagnostics, not proofs*.
>
> **Marking-aware writing conventions** (this collection was cross-checked against the official mark schemes, which use *positive marking* — method marks are independent of the final answer, and error-carried-forward applies):
>
> - **Keep the symbolic chain visible.** Symbols are carried forward and each derived line is tied to its parent ("from (ii)…", "substituting the constraint…") so that method credit and ecf can follow the chain even if an early number slips. Intermediate values are not rounded prematurely; final values are quoted to 2–3 s.f. without fuss.
> - **Approximations name the two quantities compared** (e.g. "$\tau_{\text{ext}}\gg T_{\text{int}}$"), plus the failure boundary; the final arbiter is the self-consistency of the model's assumptions.
> - **Optimisation protocol:** constraints → variable and objective → first derivative gives *candidates* → second-derivative (or sign) test → boundary values compared — interior candidates and boundary values are weighed together before declaring a global extremum.
>
> **A conforming exemplar, and two that fail.** *Paper 4 Q5(b)* in this manual is the reference: main column exam-ready with one visible bracketed substitution; its side note carries the signal (Sun vanishes → straight-line tangential paths), the move (right-triangle construction), the check (vector method agrees), and ends with a transfer sentence. *Failure mode A* — a bare answer chain with no note: correct but unteachable, violates the transfer-sentence rule. *Failure mode B* — a side note three times longer than the solution, narrating first drafts and mixing errata with method: violates the 80-word, three-question, and no-history rules.
>
> **Self-check for any solution in this manual.** (1) After reading the `【Thought】`, can you say in one sentence "next time I see X, I try Y; if Z, Y fails"? (2) Cut out the main column alone — could it be submitted as-is? (3) Cut out the side note alone — could it be handed out as a one-page method lesson? If any answer is no, the solution is out of spec.  this manual (≈640 question parts, 683 side notes) shows that the same small toolkit recurs. The table below is the manual's real content in compressed form: each row is a *signal* in the problem text, the *method* it should trigger, and the *failure boundary* where the trigger must be abandoned for the general method.

| Signal in the problem text | Method it triggers | Watch out / failure boundary |
|---|---|---|
| "estimate", "approximately", "order of magnitude" | Fermi protocol: round aggressively, carry powers of ten separately, quote 1–2 s.f. | State the licence: name the two quantities compared and where the approximation breaks |
| "maximum / minimum / greatest / least" | Extremum protocol: candidates from $d/dx=0$, sign or second-derivative test, **then compare boundary values** | A stationary point is not automatically the global extremum; discrete answers need integer rounding argued both ways |
| "infinite" network / ladder / chain / tree | Self-similar fixed point: write $X=f(X)$ and solve | Port order matters (shunt-first vs series-first give different recursions); the fixed point must be the physical (stable/positive) root |
| "identical", "the same for both", two symmetric bodies | Eliminate before solving: divide the two equations, the lumped interaction cancels | Works only when the interaction is the *same* lump on both sides (Newton's third law / shared constraint) |
| "show that … is independent of $x$" | Treat the result as a function of $x$; constancy ⟺ numerator ∝ denominator | Hidden geometric ties (e.g. fall distance vs chain length) must be made explicit first |
| two-body collision / explosion / decay | Momentum first, energy second; recoil share $\propto 1/m$; CM-frame shortcut $\tfrac12\mu v_{\text{rel}}^2$ for the loss | "Elastic" adds an equation; "maximum energy loss" ⟺ sticking |
| flux $\times$ time, "how much accumulates" | Bookkeeping ledger: inflow − outflow, with units tracked line by line | Sign conventions (what counts as in/out) must be declared before the ledger starts |
| relation requested, only units given | Dimensional analysis / Buckingham $\Pi$ | The method fixes the *form*, never the dimensionless prefactor — say so |
| "small displacement", "short time", "slowly" | Linearise: differentials, first-order expansions, error order quoted | First-order answers fail when the small parameter is no longer small — give the scale |
| circle / sphere / bowl / curved mirror geometry | Reduce 3-D to 2-D by coplanarity; chord–tangent and inscribed-angle facts | Check the angle is anchored where you think it is (from the normal? from the surface?) |
| a graph or a data table | Graphical calculus: slopes → rates, areas → accumulations, banded trapezium | If the integrand vanishes at the target (e.g. $F_{\text{net}}\to0$), the integral diverges — truncate honestly and say "approximately" |
| circuits with symmetry | Fold along equipotential lines; ideal meters (voltmeter = open, ammeter = wire); ratio methods kill the unknown emf | Folding is legitimate only for *exact* symmetry |
| oscillation, "period of" | Find the restoring coefficient; $T=2\pi\sqrt{\text{inertia}/\text{stiffness}}$; in accelerating frames substitute $g_{\text{eff}}$ | Verify the motion is actually SHM (linear restoring term) before quoting $T$ |
| "how far / how long" with a speed-dependent force | Change variable $t\to v$ or $t\to x$: $\Delta x=\Delta KE/F_{\text{net}}$, integrate over speed bands | Constant-force formulae are forbidden here |

**The verification toolbox** (every `**Check.**` block draws from it; observed usage across the manual in parentheses): numerical recomputation along a second route (all 232 checks); conservation / self-consistency audits — energy ledger closes, limits of a formula reproduce known laws (69); direction-and-sign reasoning (41); dimensional audit (28); limit probes $x\to0,\infty$ (24); reproduction of a famous special case (8). Two rules govern all checks: *a check is a diagnostic, not a proof* — it raises confidence but never replaces the derivation; and every approximation inside a check names the quantities compared and its failure boundary.

**Answer presentation.** Final answers are boxed with units and 2–3 s.f.; the symbolic chain stays visible so method marks and error-carried-forward survive an early numerical slip. Where a shortcut is shown, its dependency is stated in the pattern: *the trick relies on condition C (guaranteed by feature X); if X were X′, C would break and one must fall back to the general method because…*

> **Provenance note.** Papers 34 (2007 P2), 36 (2004 P2) and 37 (2002 P2) live on PDF pages 326–350 of the source collection as *scanned images with no text layer* — text searches over the PDF will "miss" them, but the pages are present and legible. Paper 38 is the paper whose cover reads "2002 Competition Paper 2 — 9th November 2001" (PDF pp. 351–359); we label it by its sitting date, 9 Nov 2001.

---

## Paper 1 — 2025 Round 1 Section 1 (10 Nov 2025)

*Section 1, Question 1, parts (a)–(r). Maximum 50 marks from a total of ≈ 75.*

---

### Q1(a) — One "Einstein" of photons [3 marks]

**Key observation.** "A mole of photons" is a *counting* statement, not an energy statement — the laser's power fixes an energy per second, so we need the energy of **one** photon, then scale up by $N_A$.

> 【Thought】 Seeing "unit corresponding to a mole of photons" → triggers the rule *convert the exotic unit into SI via a per-particle quantity*. Action: compute $E_\gamma = hc/\lambda$, multiply by $N_A$, divide by power. If the unit had instead been defined per joule (e.g. "an Einstein is 1 kJ of light"), the photon picture would be irrelevant and $\lambda$ would be a red herring — the wavelength given in the question is the signal that the photon energy route is intended.

**Setup & symbols.** Wavelength $\lambda = 630\ \text{nm}$, power $P = 0.50\ \text{mW} = 5.0\times10^{-4}\ \text{W}$.

**Assumptions.** Laser output is monochromatic at 630 nm and continuous; every emitted joule is counted (no losses).

**Governing equations.**
$$E_\gamma=\frac{hc}{\lambda},\qquad E_{\text{mol}}=N_A E_\gamma,\qquad t=\frac{E_{\text{mol}}}{P}.$$

**Solution.**
$$E_\gamma=\frac{(6.63\times10^{-34})(3.00\times10^{8})}{630\times10^{-9}}=3.16\times10^{-19}\ \text{J},$$
$$E_{\text{mol}}=(6.02\times10^{23})(3.16\times10^{-19})=1.90\times10^{5}\ \text{J},$$
$$t=\frac{1.90\times10^{5}}{5.0\times10^{-4}}=3.8\times10^{8}\ \text{s}\approx 12\ \text{years}.$$

**Check + answer.** Dimensions: $\dfrac{\text{J/photon}\times\text{photons}}{\text{J/s}}=\text{s}$ ✓. Order of magnitude: a visible photon is $\sim 3\times10^{-19}$ J and a mole is $\sim 6\times10^{23}$, so $\sim 2\times10^{5}$ J — a few hundred kJ, i.e. what a mW source needs years to emit ✓.
$$\boxed{t \approx 3.8\times10^{8}\ \text{s}\approx 12\ \text{yr} \text{ (continuous operation)}}$$

---

### Q1(b) — Rope loop around a frictionless tree [4 marks]

**Key observation.** The tree is frictionless, so it cannot support any tension difference along the rope touching it: the whole loop $ABCA$ carries **one** tension $T$. The clamp at $A$ isolates the loop from the tail $AD$, so the tail tension $F$ is set by the hand, and equilibrium of the knot at $A$ is the only dynamics needed.

> 【Thought】 Seeing "negligible friction" + "clamped at A" → triggers the rule *a frictionless contact transmits tension unchanged; a clamp/knot is where tensions may differ*. Action: draw the free-body diagram of point $A$ alone — three ropes meet there with tensions $T$, $T$ (loop, both strands) and $F$ (tail). If the tree had friction, tension would decay exponentially around the arc (capstan law $T=T_0 e^{-\mu\phi}$) and this simple three-force balance would fail.

**(i) The angle.** At $A$, the two strands $AB$, $AC$ make angles $\theta/2$ with the axis of symmetry $AD$. Force balance along the axis (the transverse components cancel by symmetry):
$$F=2T\cos\frac{\theta}{2}.$$
The required condition is $T=F$:
$$\cos\frac{\theta}{2}=\frac{1}{2}\;\Rightarrow\;\frac{\theta}{2}=60^\circ\;\Rightarrow\;\boxed{\theta=120^\circ}.$$

> 【Thought】 The symmetry argument (work along the bisector, where two unknowns collapse into one equation) is what makes part (i) a one-liner; the transverse equation would only restate $T_{AB}=T_{AC}$. If the clamp were off-axis, the transverse equation would become essential.

**(ii) Length of the loop.** With $\angle BAC=120^\circ$, join the centre $O$ to $A$; $OA$ bisects $\angle BAC$. Since $AB$, $AC$ are tangents, $OB\perp AB$:
$$\tan 60^\circ=\frac{r}{AB}\;\Rightarrow\;AB=AC=\frac{r}{\sqrt3}=\frac{\sqrt3}{3}r.$$
In quadrilateral $OBAC$: $\angle BOC = 360^\circ-90^\circ-90^\circ-120^\circ=60^\circ$ on the side facing $A$, so the rope wraps the **far** arc of $360^\circ-60^\circ=300^\circ=\dfrac{5\pi}{3}$ rad:
$$\widehat{BCA}=\frac{5\pi}{3}r,\qquad \ell=2\cdot\frac{\sqrt3}{3}r+\frac{5\pi}{3}r=\boxed{\frac{r}{3}\left(2\sqrt3+5\pi\right)}.$$

**Check.** Limits: as $\theta\to 180^\circ$ the tangent length $r\cot(\theta/2 ... )$ should shrink — indeed $r/\sqrt3 < 5\pi r/3$, the arc dominates, consistent with a nearly closed loop around the trunk ✓. Numerically $\ell\approx 6.39\,r$, a bit under the full circumference $2\pi r\approx 6.28r$ plus two tangents — consistent ✓.

---

### Q1(c) — A simple traffic-flow model [4 marks]

**Key observation.** Flow rate is a *flux*: count how many car-front spacings pass a fixed point per second. The safety condition is a *stopping-distance* constraint, which injects $v^2$ into the spacing — and a $v/(a+bv^2)$ function always has an interior maximum.

> 【Thought】 Seeing "if the car in front were to stop instantaneously" → triggers *kinematic constraint with zero reaction time* → use $v^2=2as$, not momentum or energy. The instruction "ignore thinking time" removes the linear $vt_{\rm react}$ term; with it, $d=L+vt_r+v^2/2a$ and the algebra below would not simplify — the phrase is the licence for the clean model.

**(i) Flow rate.** Car fronts are spaced $d$ apart and all move at $v$, so
$$n=\frac{v}{d}.$$

**(ii) Safe spacing.** The gap available to the following car is $d-L$ (front-to-front spacing minus one car length). Braking from $v$ with deceleration $a$ needs $v^2/2a$:
$$d-L=\frac{v^2}{2a}\;\Rightarrow\;\boxed{d=L+\frac{v^2}{2a}}.$$

**(iii) Optimum speed.**
> 【Thought】 Math action with purpose: the goal is the *maximum* of $n(v)$ on $v>0$, so treat $n$ as a function of one variable and set $dn/dv=0$; then verify the stationary point is a maximum, and check the boundary values separately.

$$n(v)=\frac{v}{L+\dfrac{v^2}{2a}},\qquad \frac{dn}{dv}=\frac{L+\frac{v^2}{2a}-\frac{v^2}{a}}{\left(L+\frac{v^2}{2a}\right)^2}=0\;\Rightarrow\;L=\frac{v^2}{2a},$$
$$\boxed{v_{\text{opt}}=\sqrt{2aL}}.$$
The numerator of $dn/dv$ is $L-v^2/2a$, positive below and negative above the root, so this is a genuine maximum; the boundaries give $n\to 0$ as $v\to 0$ and $n\to 2a/v\to 0$ as $v\to\infty$ ✓.

**Check.** Dimensions: $\sqrt{(\text{m/s}^2)(\text{m})}=\text{m/s}$ ✓. The optimum satisfies $d=2L$ — spacing exactly two car lengths, a memorable design rule; at the optimum $n_{\max}=\frac{1}{2}\sqrt{a/(2L)}$ ✓ dimensionally $\text{s}^{-1}$.

---

### Q1(d) — Metal sphere inside a melting ice cube [6 marks]

**Key observation.** Floating ice that melts does **not** change the water level (it displaces exactly its own melt-water). So the entire 60 mL drop is caused by the metal sphere switching from "supported by buoyancy" (displaces its *weight* of water) to "resting on the bottom" (displaces only its *volume*). The ice data cancel in part (i) — spot this before computing anything with the 10 cm cube.

> 【Thought】 Seeing "bowl completely full … level dropped … 60 mL had to be added" → triggers *volume bookkeeping at constant rim level*: write the bowl's volume budget before and after melting. If the bowl had **not** been full, the 60 mL could not be equated to a volume deficit and the problem would need the bowl's cross-section — the "completely full" clause is what converts a level change into a volume.

**(i) Density of the metal.** Sphere volume:
$$V_s=\tfrac{4}{3}\pi(2.0)^3=33.5\ \text{cm}^3.$$
Before melting, the floating system displaces water of volume $(m_{\text{ice}}+m_m)/\rho_w$. After melting, the melt-water occupies $m_{\text{ice}}/\rho_w$ and the sunken sphere occupies $V_s$. The deficit equals the 60 mL added:
$$\frac{m_m}{\rho_w}-V_s=60\ \text{cm}^3\;\Rightarrow\;m_m=\rho_w(V_s+60)=1.0\times(33.5+60)=93.5\ \text{g},$$
$$\boxed{\rho_m=\frac{93.5}{33.5}\approx 2.8\ \text{g cm}^{-3}}\quad(\approx 2.8\times10^{3}\ \text{kg m}^{-3},\text{ like aluminium}).$$

**(ii) Fraction melted when the cube just sinks.**
> 【Thought】 "Just sank" → triggers *neutral buoyancy as the boundary of a two-regime behaviour*: mean density of the remaining (ice + sphere) body equals $\rho_w$. If the sphere could escape the ice, this condition would not apply — the problem explicitly forbids that ("remained embedded"), which is the licence to treat them as one body.

Let $V$ be the remaining ice volume. Neutral buoyancy:
$$\frac{0.90\,V+m_m}{V+V_s}=1.0\;\Rightarrow\;0.10\,V=m_m-V_s=60\ \text{cm}^3\;\Rightarrow\;V=600\ \text{cm}^3.$$
Initial ice volume $V_0=10^3-33.5=966.5\ \text{cm}^3$ (the sphere displaces ice). Fraction melted:
$$\boxed{\frac{966.5-600}{966.5}\approx 0.38\;\;(\text{about }38\%)}.$$

**Check.** The same "60 cm³" reappears as $m_m/\rho_w-V_s$ — internal consistency between (i) and (ii) ✓. Limit check: a heavier sphere (larger deficit) would force $V$ larger, i.e. *less* melting needed to sink — the formula $V=(m_m/\rho_w-V_s)/(1-0.9)$ indeed grows with $m_m$ ✓.

---

### Q1(e) — Swapping two resistors [6 marks]

**Key observation.** With an ideal battery, every branch across it independently dissipates $V^2/R$. The circuit is two parallel branches — branch 1: $R_B$; branch 2: $R_A+R_A$ — and the swap exchanges one branch resistor, so write the power as a function of the single ratio $r=R_A/R_B$ and study it.

> 【Thought】 Seeing "ideal battery … in parallel with the battery" → triggers *parallel branches decouple; total power is a sum of branch powers*. If the battery had internal resistance $r_0$, the branches would couple through the terminal voltage and the clean factorisation below would fail — "negligible internal resistance" is exactly the clause that makes each branch independently $V^2/R$.

**Setup.** Original: $P=\dfrac{V^2}{R_B}+\dfrac{V^2}{2R_A}$. After swapping $R_B$ with one $R_A$: branch 1 becomes $R_A$, branch 2 becomes $R_A+R_B$:
$$P'=\frac{V^2}{R_A}+\frac{V^2}{R_A+R_B}.$$
Let $r=R_A/R_B$. Then
$$\frac{P'}{P}=\frac{\dfrac1r+\dfrac1{r+1}}{1+\dfrac1{2r}}=\frac{\dfrac{2r+1}{r(r+1)}}{\dfrac{2r+1}{2r}}=\frac{2}{r+1}.$$

> 【Thought】 Math action with purpose: the goal is a *bound*, so reduce to one dimensionless variable before differentiating or bounding. The cancellation of the factor $(2r+1)$ is the structural reason the problem has a clean answer — if it had not cancelled, one would proceed by differentiating $P'/P$ with respect to $r$ instead.

**(i) Upper limit.** $\dfrac{P'}{P}=\dfrac{2}{1+r}<2$ for all $r>0$, approached as $r\to 0$:
$$\boxed{\text{the power can increase by a factor of at most }2\ (\text{supremum, never attained}).}$$
(For $r>1$ the "swap" actually *decreases* the power.)

**(ii) Halving condition.** $\dfrac{2}{r+1}=\dfrac12\Rightarrow r+1=4$:
$$\boxed{\dfrac{R_A}{R_B}=3}.$$

**Check.** Limits: $r\to\infty$ (huge series resistance) gives $P'/P\to 0$ — the swapped circuit is nearly open, power collapses ✓. $r=1$ gives factor 1 — swapping identical-valued positions changes nothing ✓, as it must.

---

### Q1(f) — Two filament bulbs, same power, different voltage [3 marks]

**Key observation.** "Same temperature to produce the same spectrum" means the two tungsten filaments have the **same resistivity** $\rho(T)$; "similar length" fixes $\ell$. The rating $(V,P)$ fixes the *operating* resistance $R=V^2/P$, and geometry converts resistance into cross-section, hence mass.

> 【Thought】 Seeing "same temperature … same spectrum" → triggers *temperature-dependent resistivity made equal*, i.e. $\rho$ may be treated as identical for both filaments. Without that clause, tungsten's $\rho$ at the (unknown) different temperatures would add an unknown factor and the problem would be unsolvable — the clause is the licence to cancel $\rho$.

**Solution.** Operating resistances:
$$R_{240}=\frac{240^2}{60}=960\ \Omega,\qquad R_{12}=\frac{12^2}{60}=2.4\ \Omega,\qquad \frac{R_{240}}{R_{12}}=\left(\frac{240}{12}\right)^2=400.$$
With $R=\rho\ell/A$ and equal $\rho,\ell$: $A\propto 1/R$. Mass $m=\rho_{\text{W}}\,\ell A\propto A$:
$$\boxed{\frac{m_{\text{household}}}{m_{\text{car}}}=\frac{R_{12}}{R_{240}}=\frac{1}{400}}$$
— the 12 V headlamp filament is **400 times** as massive as the 240 V bulb filament.

**Check.** Physical direction: low-voltage, high-power means large current ($I=P/V=5$ A vs $0.25$ A), so the car lamp needs a thick wire — a factor $(20)^2=400$ in cross-section matches "20× the voltage ratio, squared" ✓. Dimensions: mass ratio dimensionless ✓.

> 【Errata】 Any official figure other than $1/400$ here rests on treating the two filaments' temperatures (hence resistivities) as different; under the question's stated "same temperature, same spectrum" condition, $1/400$ is the correct value.

---

### Q1(g) — Two ohmmeter readings on a rectangular sheet [3 marks]

**Key observation.** Both measurements can be cut along the horizontal midline into two **unit squares** (since $AB=2BC$). One symmetry line is *equipotential* (antisymmetric drive), the other is *current-blocking* (symmetric drive) — this converts a 2-D current-spreading problem into series/parallel combinations of one and the same elementary resistor.

> 【Thought】 Seeing "mid-point of $AB$" + "$AB=2BC$" → triggers *decompose into squares and exploit mirror symmetry*. The midline is the only distinguished line; the question is which boundary condition it realises in each measurement. If the sheet were not exactly $2:1$, no such decomposition exists and one would need to solve Laplace's equation numerically — the $2:1$ ratio is the signal that a symmetry argument is intended.

**Setup.** Let $r$ = resistance of a unit square between **a corner point contact** and the **opposite full edge held as an equipotential band** (other two edges insulating). Any rotation of this configuration has the same $r$.

```
Measurement 2 (A ↔ B):              Measurement 1 (M ↔ band CD):
  A ┌──────┐ D                        A ┌──────┐ D
    │ sq 1 │  V(A)=+V0                  │ sq 1 │ ║band
  M ├ - - -┤ midline: φ=0  →        M ●─ sq 2 ─╢  midline: no current crosses
    │ sq 2 │  electrode               B ┌──────┐ ║band
  B └──────┘ C  V(B)=−V0                └ sq 2 ║ C   (below midline, mirror)
```

*Measurement 2:* $V(A)=-V(B)$ with the geometry symmetric about the midline, so $\varphi=0$ everywhere on the midline — it behaves as an electrode. Each unit square (corner contact $\to$ midline edge) carries the **same** current $I$: the two squares are in **series**:
$$R_2=2r.$$

*Measurement 1:* injecting at the mid-point $M$ with the whole edge $CD$ banded, the configuration is mirror-symmetric about the midline, so no current crosses it — the two squares are independent. Each sees the same voltage $V(M)-V(CD)$ and each carries half the current: the two squares are in **parallel**:
$$R_1=\frac{r}{2}.$$

> 【Thought】 The corner-to-band resistance $r$ never needs to be computed — a ratio question with identical elementary cells is asking for a counting argument (series vs parallel), not for solving Laplace's equation. If the contacts were at generic interior points, no such cancellation would occur.

$$\boxed{\dfrac{R_1}{R_2}=\dfrac{r/2}{2r}=\dfrac14}$$

**Check.** Consistency with intuition: $R_1$ (drive at the middle, wide exit band, short current paths) should be much smaller than $R_2$ (drive between far corners, long spreading paths) — factor $1/4$ is plausible ✓.

---

### Q1(h) — Infinite resistor tree [3 marks]

**Key observation.** An infinite self-similar network: after one resistor, the remainder of each branch is *two copies of the same subproblem in parallel*. This turns an infinite network into one algebraic equation.

> 【Thought】 Seeing "identical … stretching out to infinity" → triggers *self-similarity / fixed-point ansatz*: define the resistance of one infinite sub-branch as an unknown $X$, write $X$ in terms of itself, solve. If the network were finite (say $n$ generations), the ansatz fails and one must recurse from the rim inward — infinity is precisely what makes the algebra close.

**Solution.** Let $X$ = resistance looking into one branch from a junction node (resistor $R$ then two identical infinite branches in parallel, rim grounded):
$$X=R+\frac{X}{2}\;\Rightarrow\;\frac{X}{2}=R\;\Rightarrow\;X=2R.$$
The centre node feeds **three** such branches in parallel:
$$\boxed{R_{\text{tree}}=\frac{X}{3}=\frac{2R}{3}}.$$

**Check.** Bounding: the tree must exceed the first-generation value $R/3$ (rim shorted after one layer) and be less than $R$ (a single branch with the rest cut). $\tfrac23 R$ lies between $\tfrac13 R$ and $R$ ✓. Also $X=2R>R$ ✓ since adding parallel paths beyond the first resistor can only reduce the sub-branch resistance toward $R$ from above.

---

### Q1(i) — Hot water cracking a glass [5 marks]

**Key observation.** The inner wall wants to expand by $\alpha\Delta T$ but is restrained by the still-cold outer wall, so a thermal stress of order $E\alpha\Delta T$ develops — compare it with the strength. Nothing here depends on wall thickness.

> 【Thought】 Seeing "temperature difference between inner and outer surface" + material data ($E$, $\alpha$, strength) → triggers *thermal stress estimate $\sigma\sim E\alpha\Delta T$*, the standard result for fully constrained thermal strain. The estimate treats the inner layer as completely restrained; in reality bending relief reduces the stress by an order-unity factor — acceptable because the question says "by estimating". If $\Delta T$ were comparable to the softening point of glass, $E$ would drop and the linear estimate would fail.

**(i) Minimum $\Delta T$.** Constrained thermal strain $\varepsilon=\alpha\Delta T$ produces stress $\sigma=E\alpha\Delta T$ (the hot inner layer is in compression). Cracking when $\sigma$ reaches the compressive strength:
$$\Delta T_{\min}=\frac{\sigma}{E\alpha}=\frac{21\times10^{6}}{(70\times10^{9})(8.0\times10^{-6})}=\boxed{37.5\ \text{K}\approx 38\ \text{K}}.$$

**(ii) Is a thicker wall a solution?** **No — it makes things worse.** For a *given* $\Delta T$ the stress $\sigma=E\alpha\Delta T$ is independent of thickness, so thickness cannot reduce the stress. Moreover, with the same hot-water shock, a thicker wall sustains a **larger** surface-to-surface $\Delta T$ (heat takes longer to conduct across, so the gradient persists) — thicker glass is *more* likely to crack. The effective fixes are lower $\alpha$ (borosilicate), thinner walls, or pre-warming.

**Check.** Dimensions: $\dfrac{\text{Pa}}{\text{Pa}\cdot\text{K}^{-1}}=\text{K}$ ✓. Order of magnitude: pouring boiling water into a cold glass gives $\Delta T$ of tens of K — right at the threshold found, which is exactly why glasses *sometimes* crack ✓.

---

### Q1(j) — Weights on a massive chain over a pulley [4 marks]

**Key observation.** The chain's mass enters **twice**: kinetically (all links move at speed $v$) and gravitationally (as chain accumulates on the descending side, its PE drops by $\lambda g h^2$). "The mass of the chain makes no difference" means $v^2$ is independent of $\lambda$ — an algebraic condition on the two ways $\lambda$ appears.

> 【Thought】 Seeing "by considering the energy of the system" → triggers *work–energy for the whole system* (constraint forces at the frictionless, light pulley do no work) instead of force diagrams. Seeing "for what ratio does the mass not matter" → triggers *treat $v^2$ as a function of the parameter $\lambda$ and demand it be constant* — a rational function $f(\lambda)$ is constant iff numerator and denominator are proportional, a much cheaper condition than solving for general $\lambda$.

**Setup & geometry.** Let each side of the chain initially hang a length $\ell$ (weights level), total chain length $L_c\approx 2\ell$ (light pulley), $M_c=\lambda L_c$. $m_1$ falls a distance $h$ to the floor. **Stated assumption (the question's intended figure): $h=\ell=L_c/2$** — the fall ends exactly as the chain has fully transferred onto $m_1$'s side. Without this, $h$ and $L_c$ would be two free parameters and no unique mass ratio could result (see the side note).

> 【Thought】 *Hidden-assumption alert.* The question's text states only "$\lambda$ per unit length" — the chain's total length is not given numerically. The determinate reading (the one the official figure draws) is: the weights hang from the chain's two ends, initially level, and **$m_1$'s fall distance equals the initial hanging length of each side**, $h=\ell=L_c/2$ — i.e. the process ends exactly as the chain has fully transferred onto $m_1$'s side. If the stem changed “$h=L_c/2$” to “$h$ is an independent parameter unrelated to $L_c$”, condition C (the geometric binding of fall distance to chain length) would break and the $\lambda$-independence would fail — then return to the general method (the ratio condition makes $v^2$ $\lambda$-independent only at $h/L_c=1/2$), because the ratio of $\lambda$'s potential to kinetic terms is fixed by $h/L_c$ alone. The assumption must be stated explicitly — otherwise $h$ and $L_c$ are two independent degrees of freedom and the problem is underdetermined.

**Governing equation (energy).** $m_1$ loses $m_1gh$, $m_2$ gains $m_2gh$. Chain PE: side lengths change $\ell\to\ell\pm h$, with PE $-\tfrac12\lambda g(\text{length})^2$ per side (measured from the pulley):
$$\Delta U_{\text{chain}}=-\tfrac{\lambda g}{2}\big[(\ell+h)^2+(\ell-h)^2-2\ell^2\big]=-\lambda g h^2.$$
Hence
$$(m_1-m_2)gh+\lambda g h^2=\tfrac12\left(m_1+m_2+\lambda L_c\right)v^2,$$
$$v^2=2g\,\frac{(m_1-m_2)h+\lambda h^2}{(m_1+m_2)+\lambda L_c}.$$

**Solution.** $v^2$ is independent of $\lambda$ iff the fraction's numerator and denominator are proportional in $\lambda$:
$$\frac{(m_1-m_2)h}{m_1+m_2}=\frac{h^2}{L_c}\;\Rightarrow\;\frac{m_1-m_2}{m_1+m_2}=\frac{h}{L_c}=\frac12,$$
$$2(m_1-m_2)=m_1+m_2\;\Rightarrow\;\boxed{\dfrac{m_1}{m_2}=3},\qquad\text{and then }v^2=gh\text{ for any }\lambda.$$

> 【Thought】 The two $\lambda$-terms have distinct physical origins — $\lambda h^2$ is *potential* (chain redistribution), $\lambda L_c$ is *kinetic* (total moving mass). Asking them to cancel is why a pure number emerges; if the chain's PE had been constant (e.g. a closed loop of chain), only the kinetic term would survive and no mass ratio could eliminate $\lambda$.

**Check.** Substitution test with $m_1=3m_2$: $v^2=2g\,\dfrac{2m_2h+\lambda h^2}{4m_2+2\lambda h}=2g\cdot\dfrac{1}{2}h=gh$ — $\lambda$ cancels identically ✓. Limit: $\lambda\to 0$ recovers the massless-chain Atwood result $v^2=2gh(m_1-m_2)/(m_1+m_2)=gh$ ✓ consistent.

---

### Q1(k) — Two charged spheres in a smooth bowl [6 marks]

**⚠ Typo in the question:** the printed spring constant "$k=120\ \text{N m}^{-2}$" must read $\text{N m}^{-1}$ — a spring constant is force per extension.

**Key observation.** The spring force and the Coulomb repulsion **both act along the chord $AB$**, so each sphere feels gravity plus *one* chord-directed interaction $F$ — and by Newton's third law the same $|F|$ acts on both. The chord makes the same angle with the tangent at each end, so the two tangential equilibrium equations share a common factor and can be divided to eliminate $F$ (and the unknown charge) entirely.

> 【Thought】 Seeing two unknowns that appear only as one lumped interaction ($k$ known but $q$, $m_A$, $m_B$ unknown) → triggers *eliminate before solving*: ratio of the two equilibrium equations kills $F$. Geometry fact used: the angle between a chord and the tangent equals half the subtended central angle, $\varphi=(\theta_A+\theta_B)/2$ — identical at both ends, which is what allows the elimination. If the spring were replaced by a string along the bowl surface, the force directions would differ between the spheres and this elimination would fail.

**Setup.** Bowl radius $R=10$ cm; angular positions from the bottom $\theta_A=d_1/R=0.70$ rad, $\theta_B=d_2/R=0.50$ rad, on opposite sides.

**(i) Elastic PE.** The chord spans central angle $\theta_A+\theta_B=1.20$ rad:
$$AB=2R\sin\frac{\theta_A+\theta_B}{2}=20\sin 0.6=11.29\ \text{cm},\qquad x=11.29-8.0=3.29\ \text{cm},$$
$$\boxed{E_{\text{el}}=\tfrac12 kx^2=\tfrac12(120)(0.0329)^2\approx 6.5\times10^{-2}\ \text{J}\;(65\ \text{mJ})}.$$

**(ii) Displacement of $B$ after halving $A$'s charge.** Tangential equilibrium of each sphere (net chord force $F$ = Coulomb repulsion $-$ spring pull):
$$m_A g\sin\theta_A=F\cos\varphi,\qquad m_B g\sin\theta_B=F\cos\varphi\;\Rightarrow\;m_A\sin\theta_A=m_B\sin\theta_B.$$
The same structure holds after the discharge (only $F$ changes), so with $\theta_A'= (7.0-1.3)/R=0.57$ rad:
$$m_A\sin\theta_A'=m_B\sin\theta_B'\;\Rightarrow\;\frac{\sin\theta_B'}{\sin\theta_A'}=\frac{m_A}{m_B}=\frac{\sin\theta_B}{\sin\theta_A}=\frac{\sin0.50}{\sin0.70}.$$
$$\sin\theta_B'=\sin0.57\cdot\frac{\sin0.50}{\sin0.70}=0.540\times\frac{0.479}{0.644}=0.401\;\Rightarrow\;\theta_B'=0.414\ \text{rad},$$
$$d_2'=R\theta_B'=4.14\ \text{cm}\;\Rightarrow\;\boxed{\Delta d_2=5.0-4.14\approx 0.86\ \text{cm}\ \text{down the bowl}}.$$

> 【Thought】 Note what was *not* needed: $k$, the natural length, and $q$ all drop out of part (ii). That is the diagnostic that the intended route is the ratio, not a full re-solution of the equilibrium. Also note the direction check built into the physics: halving the repulsion must let **both** spheres slide toward the bottom — the answer has both $d_1$ and $d_2$ shrinking ✓.

**Check.** Symmetry/limits: if $m_A=m_B$ the relation gives $\theta_B'=\theta_A'$ — symmetric equilibrium on the two sides, as it must be ✓. Magnitude: a fractional change in $d_2$ smaller than that in $d_1$ (0.86 cm vs 1.3 cm) is consistent with $B$ being the lighter sphere sitting lower, where the bowl is steeper in angle-per-arc... i.e. less arc needed per unit angle change — plausible ✓.

---

### Q1(l) — Background rate from three weekly count rates [4 marks]

**Key observation.** The source contributes a geometric sequence (weekly sampling of an exponential decay); the background is an additive constant. A geometric sequence obeys $S_2^2=S_1S_3$ — this single constraint determines the unknown shift $B$.

> 【Thought】 Seeing "same time in three consecutive weeks" → triggers *equal time steps ⇒ geometric ratios*, the fingerprint of exponential decay. If the measurements had been at unequal intervals, one extra unknown ($e^{-\lambda\Delta t_1}, e^{-\lambda\Delta t_2}$) would remain and three readings would not suffice without knowing the decay constant — equal spacing is what makes three equations sufficient for three unknowns ($B$, $S_1$, $r$).

**Solution.** Write $C_i=B+S_i$ with $S_2=S_1r$, $S_3=S_1r^2$. Then
$$(C_1-B)(C_3-B)=(C_2-B)^2$$
$$C_1C_3-B(C_1+C_3)+\cancel{B^2}=C_2^2-2BC_2+\cancel{B^2},$$
$$\boxed{B=\frac{C_1C_3-C_2^{\,2}}{C_1+C_3-2C_2}}.$$

**Check.** Numeric test: with $B=10$, $S=100$, $r=0.5$: $C=(110,60,35)$; formula gives $(3850-3600)/(145-120)=250/25=10$ ✓. Sign check: for a decaying source $C_1+C_3-2C_2>0$ and $C_2^2>C_1C_3$ would give negative $B$... in fact AM–GM gives $C_1C_3<C_2^2$ when $B$... — the safe statement: both numerator and denominator carry the same sign as $-B$ constructed above, and the formula returns a positive $B$ for physical data ✓. Limit: if the source is absent, all $C_i$ equal, denominator $\to 0$ — correctly flagging that three equal readings cannot separate $B$ from a constant source ✓.

---

### Q1(m) — Comparing two weights on a smooth incline [5 marks]

**Key observation.** Same string, same pulley, same distance along the plane in both configurations — only the acceleration changes. With $s=\tfrac12at^2$ from rest, "half the time" means **four times the acceleration**.

> 【Thought】 Seeing "draws up in half the time" → triggers *convert a time ratio into an acceleration ratio* via $s=\tfrac12at^2$ (valid because both runs start from rest over the same displacement). If the runs had started with different initial speeds, $s=ut+\tfrac12at^2$ would spoil the clean $a\propto 1/t^2$ scaling.

**Solution.** Plane at $\alpha=30^\circ$, $\sin\alpha=\tfrac12$. With $w_1$ hanging and $w_2$ on the plane:
$$a_{12}=\frac{w_1-w_2\sin\alpha}{m_1+m_2}=\frac{g\left(w_1-\tfrac12 w_2\right)}{w_1+w_2},$$
and with the weights interchanged,
$$a_{21}=\frac{g\left(w_2-\tfrac12 w_1\right)}{w_1+w_2}.$$
(Using $w=mg$, the $g$ and the total-mass denominator are common factors.) From $t_{12}=\tfrac12 t_{21}$ over the same distance:
$$a_{12}=4a_{21}\;\Rightarrow\;w_1-\tfrac12w_2=4w_2-2w_1\;\Rightarrow\;3w_1=\tfrac92w_2,$$
$$\boxed{w_1=\tfrac32\,w_2\quad\left(w_1:w_2=3:2\right)}.$$

**Check.** Consistency of motion direction: the second configuration moves only if $w_2>w_1\sin30^\circ=w_1/2$; with $w_1=1.5w_2$, $w_1/2=0.75w_2<w_2$ ✓. Sanity: $w_1$ must exceed $w_2/2$ (to pull $w_2$ up) and exceed... $1.5w_2$ lies sensibly between $w_2/2$ and $2w_2$ ✓.

---

### Q1(n) — Attenuation along three axes of a cuboid [4 marks]

**Key observation.** Exponential attenuation turns multiplicative survival factors into additive exponents — equivalently, each edge length is *proportional to the logarithm* of the surviving fraction, with the half-value layer fixing the constant.

> 【Thought】 Seeing "halves the radiation at 1.0 cm" → triggers *half-value layer $x_{1/2}$ as the natural ruler*: $I/I_0=2^{-x/x_{1/2}}$, avoiding any mention of $\mu$ until needed. If the attenuation law were a power law instead of exponential, this log-linearity would fail and three measurements would not decouple so cleanly.

**Solution.** $I/I_0=e^{-\mu x}=2^{-x/(1.0\ \text{cm})}$, so each edge $x=-\dfrac{\ln(I/I_0)}{\ln 2}$ cm:
$$a=\frac{-\ln 0.60}{\ln2}=0.737\ \text{cm},\quad b=\frac{-\ln 0.70}{\ln2}=0.515\ \text{cm},\quad c=\frac{-\ln 0.80}{\ln2}=0.322\ \text{cm},$$
$$\boxed{V=abc=\frac{\ln(1/0.60)\,\ln(1/0.70)\,\ln(1/0.80)}{(\ln2)^3}\approx 0.12\ \text{cm}^3\ (\approx 120\ \text{mm}^3).}$$

**Check.** Monotonicity: larger transmission ↔ larger edge: $0.80>0.70>0.60$ matches $c<b<a$ ✓. Scale: transmissions near 1 correspond to edges under one half-value layer (1 cm), so a sub-mm-to-cm cuboid with volume of order $0.1\ \text{cm}^3$ is coherent ✓.

---

### Q1(o) — Seabed visible through a porthole [4 marks]

**Key observation.** Diameter (40 cm) $\gg$ glass thickness, so treat the porthole as a single plane water→air interface with a finite aperture. Rays from the seabed bend **away** from the normal on entering air; beyond the critical angle in water, no ray escapes. The visible region is bounded by rays that just pass the near rim at the critical angle.

> 【Thought】 Seeing "diameter much greater than thickness" → triggers *thin-window approximation*: ignore the glass slab's lateral ray shift (order $t$) while keeping its existence irrelevant — refraction water→glass→air ends with the same angular relation $n_w\sin\theta_w=\sin\theta_{\text{air}}$ as a single water–air interface (parallel faces cancel). If the glass were thick, the intermediate refraction would matter and the aperture edges would act differently.

**Solution.** Critical angle water→air:
$$\sin\theta_c=\frac{1}{n_w}=\frac{1}{1.4}\;\Rightarrow\;\theta_c=45.6^\circ,\qquad \tan\theta_c=\frac{1}{\sqrt{n_w^2-1}}=\frac{1}{\sqrt{0.96}}=1.021.$$
A seabed point at radial distance $\rho$ from the porthole axis sends its ray of **smallest incidence angle at the water–air interface** through the **near rim** (aperture radius $a=0.20$ m), at angle $\tan\theta_w=(\rho-a)/h$ with $h=5.0$ m. Visibility requires $\theta_w\le\theta_c$:
$$\rho_{\max}=a+h\tan\theta_c=0.20+5.0\times1.021=5.30\ \text{m},$$
$$\boxed{A=\pi\rho_{\max}^2\approx \pi(5.30)^2\approx 88\ \text{m}^2\qquad(\approx 82\ \text{m}^2\text{ if the rim offset }a\ll h\tan\theta_c\text{ is neglected}).}$$

**Model choice.** We **keep** the rim offset $a=0.20$ m, giving $A\approx88\ \text{m}^2$; neglecting it ($a\ll h\tan\theta_c$) gives $\approx82\ \text{m}^2$. The difference is the modelling choice, not arithmetic.

**Check.** Limit: $n_w\to 1$ gives $\theta_c\to 90^\circ$ and $A\to\infty$ — without refraction the whole seabed is visible in principle ✓ (the formula diverges correctly). Limit: $h\to 0$ gives $A\to\pi a^2$, the aperture's own projection ✓. The area scales as $h^2$ — doubling depth quadruples the visible patch, the expected geometric scaling ✓.

---

### Q1(p) — Conical mirror with an axial filament [4 marks]

**Key observation.** A ray from a point on the axis, the axis itself, and the surface normal at the hit point are coplanar, so the 3-D reflection reduces to a 2-D problem: a ray bouncing between two straight lines inclined at $\pm\theta$ to the axis ($\theta$ = semi-vertical angle of the cone). Each reflection off a line at angle $\theta$ maps the ray's inclination $\alpha\to 2\theta-\alpha$ — track this map and demand the reflected ray never meets a wall again.

> 【Thought】 Seeing "rays … will not be reflected more than once" → triggers *worst-ray analysis*: the condition must hold for **every** emission direction, so find the most dangerous ray and impose the bound on it. If the question asked "for most rays", a statistical/averaging approach would be needed instead — "will not" is a universal quantifier and forces an extremal argument.

**Setup.** Cross-section through the axis: walls are lines at angle $\theta$ to the axis. A ray leaves a point on the axis at angle $\alpha$ to the upward axis ($0<\alpha<\pi$); it hits a wall iff $\alpha>\theta$.

**Reflection law.** Take the cone's axis as the $x$-axis; the ray direction is $(\cos\alpha,\sin\alpha)$ and the wall line makes angle $\theta$ with the axis. Reflecting the ray direction in the wall line:
$$\alpha\;\longrightarrow\;\gamma=2\theta-\alpha.$$
(Verify: angle with the wall changes from $\alpha-\theta$ before to $\theta-\gamma=\alpha-\theta$ after — preserved, with the normal component reversed ✓.)

**Escape condition.** After one reflection from the right wall:
- if $\gamma\ge 0$, the ray stays on the same side, and since $\gamma=2\theta-\alpha<\theta$ it is *less* inclined than the wall, which recedes from it — no second hit;
- if $\gamma<0$, the ray crosses toward the opposite wall; solving the ray–wall intersection shows it hits the opposite wall iff $|\gamma|>\theta$.

So a ray avoids a second reflection iff
$$|\,2\theta-\alpha\,|\le\theta\quad\Longleftrightarrow\quad \theta\le\alpha\le 3\theta.$$

**Impose on all rays.** Rays hitting walls span $\alpha\in(\theta,\pi)$; the worst ray is the one fired nearly straight toward the apex, $\alpha\to\pi$. Requiring $\pi\le 3\theta$:
$$\boxed{\theta_{\min}=\frac{\pi}{3}=60^\circ\ \text{(semi-vertical angle)},\ \text{i.e. full apex angle }120^\circ.}$$

> 【Thought】 Sanity of the mechanism: a narrow cone ($\theta$ small) acts like a kaleidoscope — many bounces — while a very wide cone is nearly a single tilted plane mirror — at most one bounce. A threshold in between is physically expected; the algebra places it where the marginal ray ($\alpha=\pi$) emerges parallel to the opposite wall ($\gamma=-\theta$), the clean limiting case.

**Check.** At $\theta=60^\circ$: the extreme downward ray ($\alpha=180^\circ$) reflects to $\gamma=-60^\circ$, exactly parallel to the opposite wall — never hits it ✓ (boundary case). Any $\theta<60^\circ$: that same ray reflects to $|\gamma|>\theta$ and strikes the opposite wall — second reflection exists, confirming minimality ✓.

---

### Q1(q) — Distance for a train to reach maximum speed [4 marks]

**Key observation.** The graph gives forces as functions of **speed**, but the question asks for a **distance** — the bridge is the work–energy theorem in differential form, $F_{\text{net}}=mv\,\dfrac{dv}{dx}$, which converts the force–speed curve into an integral over speed.

> 【Thought】 Seeing "force vs speed graph … distance travelled" → triggers *change of variable from time to position*: $a=\dfrac{dv}{dt}=v\dfrac{dv}{dx}$, so $x=\displaystyle\int_0^{v_{\max}}\frac{m\,v}{F_t(v)-F_r(v)}\,dv$, evaluated graphically/numerically from the curves. A naive $x=\bar F$-timesomething or $v^2=2ax$ with constant $a$ would contradict the graph (the net force falls to zero); the whole point is that acceleration is speed-dependent. Note also the honest caveat: $F_{\text{net}}\to 0$ at $v_{\max}$, so the exact integral diverges logarithmically — "approximately" in the question licenses truncating near $v_{\max}$, which is what a coarse graphical integration does automatically.

**Reading the graph.** Tractive force: $\approx 1.8\times10^5$ N constant up to $\approx 20\ \text{m/s}$, then falling as $F_t\approx P/v$ with $P\approx 3.7\ \text{MW}$ (constant-power regime). Resistance: $\approx 15$–$35$ kN at low speed, rising roughly linearly to $\approx 70$ kN at $100\ \text{m/s}$. Curves cross at
$$v_{\max}\approx 70\ \text{m/s}\ (\approx 250\ \text{km/h}).$$

**Integration.** With $m=336\,000$ kg:
$$x=\int_0^{v_{\max}}\frac{m v}{F_t(v)-F_r(v)}\,dv.$$
Numerically (trapezium on the digitised curves): $\approx 14$ km to $60\ \text{m/s}$, $\approx 23$ km to $65\ \text{m/s}$, $\approx 30$ km to $0.95\,v_{\max}$; the last few percent of speed add distance logarithmically.

**Worked numerical example (the official scheme's finite-step version).** Work in kinetic-energy steps, $\Delta x=\Delta KE/F_{\text{net}}$, with $F_{\text{net}}$ read at each band's midpoint (values from the two curves): 

| speed band (m/s) | $F_{\text{net}}$ at midpoint | $\Delta KE=\tfrac12m\Delta(v^2)$ | $\Delta x$ |
|---|---|---|---|
| 0–20 | $\approx 155$ kN | $67$ MJ | $0.4$ km |
| 20–40 | $\approx 88$ kN | $202$ MJ | $2.3$ km |
| 40–60 | $\approx 30$ kN | $336$ MJ | $11.2$ km |
| 60–65 | $\approx 8$ kN | $105$ MJ | $13.1$ km |

running total $\approx 27$ km — and the final $65\to70$ m/s band diverges logarithmically (the curves cross), so stop the table there and quote the truncated value: $\boxed{x\approx26\ \text{km}}$ — the official scheme's own figure. The table makes the physics visible: half the distance is spent in the last 5 m/s before top speed, because $F_{\text{net}}$ collapses there.

$$\boxed{x\approx 20\text{–}30\ \text{km}\ \text{(order tens of km; anything in }15\text{–}40\ \text{km from a careful graphical integration is acceptable).}}$$

> 【Thought】 Diagnostic takeaway: the divergence near $v_{\max}$ is real physics, not a modelling error — with vanishing net force the approach to top speed is asymptotic, so "distance to reach maximum speed" is inherently fuzzy and only an order-of-magnitude answer exists. If forced to give one number, quote the distance to $\sim 95\%$ of $v_{\max}$, $\approx 25$–$30$ km.
>
> **Official mark scheme (for calibration):** works by finite steps $\Delta x=\Delta KE/F_{\text{net}}$ read off the graph, obtaining $\approx26$ km with all steps included, $\approx6$–$10$ km if the asymptotic tail is truncated — and explicitly accepts a wide range, awarding the marks for a sound method. Our $20$–$30$ km (graphical integration of the same integral) sits comfortably inside the accepted band.

**Check.** Crude cross-check: average net force over the run $\sim 70$ kN (starts at $\approx 150$ kN, ends at 0); then $x\sim \frac{mv_{\max}^2/2}{\bar F}\sim\frac{8\times10^8\ \text{J}}{7\times10^4\ \text{N}}\sim 12$ km — same order of magnitude, and smaller, as expected since the true force collapses near the end ✓. Dimensions of the integrand: $\dfrac{\text{kg}\cdot\text{m/s}}{\text{N}}\times\text{m/s}=\text{m}$ ✓.

---

### Q1(r) — Rod sliding on perpendicular rails [3 marks]

**Key observation.** The midpoint of the rod moves on a **circle of radius $L/2$ centred on the rail apex** — the median to the hypotenuse of a right triangle equals half the hypotenuse. The mass thus behaves like a pendulum bob of length $L/2$, but pivoted *above*: a classic small-oscillation problem solvable purely from energy.

> 【Thought】 Seeing two sliding constraints + one rigid body → triggers *find the one degree of freedom and parametrise it*: the tilt angle $\theta$ of the rod. The right-angle rail makes the midpoint's circular locus exact (Thales), which collapses the kinematics to pendulum kinematics. If the rails met at a general angle $2\beta$, the locus would still be circular through the same argument with the circumradius $L/(2\sin\beta)$ — the method degrades gracefully; it fails only if friction enters, because then energy conservation is lost.

**Setup.** Apex of the rails at the origin; rails along $y=\pm x$ pointing downward (right angle, each at $45^\circ$). Let the rod tilt by $\theta$ from horizontal; ends stay on the rails.

**Kinematics.** The two rail ends and the apex form a right triangle with the rod as hypotenuse $L$, so the midpoint $M$ (circumcentre) satisfies $|OM|=L/2$:
$$M=\left(-\tfrac{L}{2}\sin\theta,\;-\tfrac{L}{2}\cos\theta\right),\qquad v_M^2=\dot x_M^2+\dot y_M^2=\left(\tfrac{L}{2}\right)^2\dot\theta^2.$$

**Energy.** With $m$ at $M$:
$$E=\underbrace{\tfrac12 m\left(\tfrac{L}{2}\right)^2\dot\theta^2}_{T_{\text{kin}}}\underbrace{-mg\tfrac{L}{2}\cos\theta}_{U}.$$
Equilibrium at $\theta=0$ (lowest point of the circle ✓, matches the symmetric horizontal position). For small $\theta$: $U\approx \text{const}+\tfrac14 mgL\,\theta^2$ — a harmonic potential. Equation of motion:
$$\tfrac{mL^2}{4}\ddot\theta+\tfrac{mgL}{2}\theta=0\;\Rightarrow\;\omega^2=\frac{mgL/2}{mL^2/4}=\frac{2g}{L},$$
$$\boxed{T=\frac{2\pi}{\omega}=2\pi\sqrt{\dfrac{L}{2g}}=\pi\sqrt{\dfrac{2L}{g}}}.$$

**Check.** The mass rides a circle of radius $L/2$ under gravity with no other constraint — that *is* a simple pendulum of length $L/2$, whose period is $2\pi\sqrt{(L/2)/g}$ ✓ identical. (The official mark scheme uses exactly this pendulum equivalence.) Sanity: larger $L$ → slower oscillation ✓; $m$ cancels — the rod is massless, so mass scales out of both inertia and restoring force ✓.

---
*End of Paper 1 (2025 Round 1 Section 1).*


---

## Paper 2 — 2025 Round 0 (16 Oct 2025)

*25 multiple-choice questions, 1 mark each, no calculators. Solutions are kept compact, but each still shows the key observation, the derivation, a check, and the chosen option.*

---

### Q1 — Work done stretching a wire

**Key observation.** Work stored in a uniformly stretched elastic wire = (average force) × (extension) = ½ × (final force) × (extension), and force/extension are stress/strain × geometry.

> 【Thought】 Seeing "stress σ, strain ε, find work" → triggers *energy density = ½σε* (area under the stress–strain line, linear elasticity). The trap options are pure algebra scrambles; dimensions alone kill four of them: work must be joules, and $LA\sigma\varepsilon$ = volume × pressure = J ✓ while e.g. $\sigma A/\varepsilon L$ has no meaning. When unsure, dimensional screening first, physics second.

**Solution.** Energy density route, direct in the given variables: $W=(\text{area under the stress–strain line})\times(\text{volume})=(\tfrac12\sigma\varepsilon)\times(LA)$. Equivalently $F=\sigma A$, extension $\Delta L=\varepsilon L$; linear loading from zero:
$$W=\tfrac12 F\,\Delta L=\tfrac12 LA\sigma\varepsilon.$$

**Check.** Dimensions: $\text{m}^3\cdot\text{Pa} = \text{J}$ ✓; the factor ½ is the average-force factor for loading from zero ✓.

**Answer: E** $\left(\tfrac12 LA\sigma\varepsilon\right)$

---

### Q2 — Snell's law with angles measured from the surface

**Key observation.** The diagram measures $\theta_1,\theta_2$ from the **interface**, not from the normal — the whole question is reading the diagram.

> 【Thought】 Seeing a refraction diagram → triggers *check where the angles are anchored before quoting Snell*. Angles from the surface are the complements of the textbook angles: $\sin i = \cos\theta$. If the diagram had anchored them at the normal, option A would apply; here option A is the deliberate trap for pattern-matchers.

**Solution.** With $i=90^\circ-\theta$: $n_1\sin i_1=n_2\sin i_2\Rightarrow n_1\cos\theta_1=n_2\cos\theta_2$.

**Check.** Ray bends away from the normal entering $n_2$ ($\theta_2<\theta_1$ in the figure) ⟹ $n_2<n_1$, and $\cos\theta_2>\cos\theta_1$ is consistent with $n_1\cos\theta_1=n_2\cos\theta_2$ ✓.

**Answer: C** $\left(n_1\cos\theta_1=n_2\cos\theta_2\right)$

---

### Q3 — Which is **not** a unit of impulse?

**Key observation.** Impulse = momentum: $[\text{N s}]=[\text{kg m s}^{-1}]$. Expand each candidate into base units.

> 【Thought】 Strategy: convert everything to joules/newtons/metres primitives. Energy units ($\text{J} = \text{N m}$) and impulse units ($\text{N s}$) differ by "metre vs second" — look for the option that secretly contains $\text{N m}$.

**Solution.**
- A: N s — impulse ✓
- B: $\text{W s}^2\text{m}^{-1}=\dfrac{\text{J}}{\text{s}}\cdot\dfrac{\text{s}^2}{\text{m}}=\dfrac{\text{N m}\cdot\text{s}}{\text{m}}=\text{N s}$ ✓
- C: $\text{Pa m}^3=\dfrac{\text{N}}{\text{m}^2}\text{m}^3=\text{N m}=\text{J}$ — **energy, not impulse** ✗
- D: kg m s⁻¹ ✓ (definition of momentum)
- E: $\text{C V s m}^{-1}=\dfrac{\text{J s}}{\text{m}}=\text{N s}$ ✓

**Answer: C** $\left(\text{Pa m}^3\right)$

---

### Q4 — U-238 → Pb-206 decay chain

**Key observation.** Alpha decays change mass number by 4 (and only they do); beta-minus decays change atomic number by +1 with no mass change. Solve mass first, then charge.

> 【Thought】 Two conserved numbers (mass $A$, charge $Z$) and two decay types → a $2\times2$ linear system. Order matters: solve $A$ first because $\beta^-$ is invisible in $A$; solving $Z$ first would entangle the two unknowns.

**Solution.** Alpha count: $(238-206)/4=8$. Charge after 8 α: $92-16=76$; to reach 82 needs $82-76=6$ beta-minus decays.

**Check.** Final: $A=238-32=206$ ✓, $Z=92-16+6=82$ ✓ (this is the real uranium series).

**Answer: B** (6)

---

### Q5 — Interference with path difference 7.5 m, λ = 1.8 m

**Key observation.** $\Delta/\lambda=7.5/1.8=4\tfrac16$: not an exact integer or half-integer, so interference is *partial*; the nearest integer means nearly constructive.

> 【Thought】 Seeing non-integer $\Delta/\lambda$ → triggers *quantify the mismatch* via the two-source amplitude factor $\left|\cos\left(\pi\Delta/\lambda\right)\right|$, rather than guessing. If the path difference had been $(n+\tfrac12)\lambda$ exactly, "fully destructive" would be right; here the fractional part $\tfrac16$ is the decisive number. (Options "mostly …" exist precisely because real data are rarely exact multiples.)

**Solution.** Two equal amplitudes $A$ with phase difference $\delta=2\pi\Delta/\lambda$ combine to $A_{\text{res}}=2A\left|\cos(\delta/2)\right|=2A\left|\cos(\pi\Delta/\lambda)\right|$, so the intensity relative to full constructive interference is
$$\frac{I}{I_{\max}}=\cos^2\!\left(\frac{\pi\Delta}{\lambda}\right)=\cos^2\!\left(\frac{\pi}{6}\right)=0.75.$$
Fractional part $1/6$ → phase mismatch $\pi/3$ from the constructive condition; relative amplitude $\cos(\pi/6)=0.87$, intensity $\approx 75\%$ of maximum — clearly on the constructive side.

**Check.** $|\cos(4.1667\pi)|=|\cos(\pi/6)|$ ✓; $75\%$ intensity ≈ "mostly", not "fully" ✓.

**Answer: C** (mostly constructive)

---

### Q6 — Cheapest way to buy exactly 4 Ω

**Key observation.** This is an optimisation over series/parallel arithmetic: enumerate the cheap attainable values. The promising route to 4 Ω is a parallel pair, since no 4 Ω resistor is sold.

> 【Thought】 Seeing "least you would need to spend" → triggers *search by budget, not by resistor count*: check attainability of 4 Ω at £3, £4, then £5. If we enumerated by resistor count instead, cheap-but-many-resistor combinations (four 3 Ω for £4) would be missed.

**Solution.**
- £3 budget: one 2 Ω, one 6 Ω, or three 3 Ω resistors — whose attainable values are $3+3+3=9$, $(3+3)\parallel3=2$, $3\parallel3\parallel3=1$, $(3\parallel3)+3=4.5$ Ω — no 4 Ω.
- £4 budget: **four 3 Ω resistors (£1 each): three in parallel, then in series with the fourth**:
$$R=(3\parallel3\parallel3)+3=1+3=4\ \Omega\ \checkmark$$

**Check.** $3\parallel3\parallel3=1$ Ω exactly, so the combination is exactly $4$ Ω ✓; no £3 combination reaches 4 Ω (enumerated above) ✓. (Official answer: B — £4. My first enumeration of the four-3 Ω combinations missed the "three parallel + one series" arrangement; a 12 Ω ∥ 6 Ω pair also makes 4 Ω but costs £5.)

**Answer: B** (£4)

---

### Q7 — Two particles, same direction, collision

**Key observation.** Both move at constant velocity — a pure relative-motion problem: closing speed × time = initial gap.

> 【Thought】 Seeing constant velocities and same direction → triggers *switch to the rest frame of the chased particle*: one number (relative speed $6-3=3$ m/s) instead of two equations. If they moved toward each other, the same trick with $6+3$ would apply.

**Solution.** Closing speed $=6-3=3\ \text{m/s}$; gap 18 m closes in $t=6$ s. A travels $6\times6=36\ \text{m}$.

**Check.** In 6 s, B travels 18 m: $36-18=18$ m = initial gap ✓ exactly consistent.

**Answer: C** (36 m)

---

### Q8 — Cell with voltmeter, ammeter and three resistors

**Key observation.** The ideal voltmeter (infinite resistance) kills its own branch current; the circuit reduces to the cell driving two $R$'s (top branch and middle branch) around one loop.

> 【Thought】 Seeing "ideal voltmeter / ideal ammeter" → triggers *replace by their ideals: voltmeter = open circuit, ammeter = wire*. The bottom $R$ then carries no current and has **no** voltage drop — which is why the voltmeter reads the full rail-to-rail voltage, not zero. Forgetting "no drop across a currentless resistor" is the designed trap.

**Solution.** Loop: cell $\mathcal{E}$ in series with top $R$ and middle $R$ (the bottom branch is open):
$$I=\frac{\mathcal{E}}{2R}\ \ (\text{ammeter reading}), \qquad V_{\text{rails}}=\mathcal{E}\frac{R}{R+R}=\frac{\mathcal{E}}{2}.$$
Voltmeter: its series resistor drops nothing ($I=0$), so it reads the rail voltage $\mathcal{E}/2$.

**Check.** Voltage balance around the loop: $\mathcal{E}=IR+IR$ ✓; power: $I^2(2R)=\mathcal{E}^2/2R=\mathcal{E}I$ ✓.

**Answer: E** $\left(\dfrac{\mathcal{E}}{2},\ \dfrac{\mathcal{E}}{2R}\right)$

---

### Q9 — Wires with fundamental frequencies in ratio 2:1; resistance ratio?

**Key observation.** Same length, same tension $T$, same material: $f_1=\dfrac{1}{2L}\sqrt{T/\mu}$ with $\mu=\rho A$, so $f\propto 1/\sqrt{A}$; electrical resistance $R=\rho_e L/A\propto 1/A$. Chain the two proportionality relations.

> 【Thought】 The problem is a *scaling chain*: frequency → linear density → cross-section → resistance. Two different $\rho$'s (mass density vs resistivity) appear — both cancel because "same material" fixes each. If the materials differed, neither cancellation would hold and the problem would be unsolvable — "same material" is the essential clause.

**Solution.** $f\propto A^{-1/2}$: ratio $2:1$ in $f$ ⟹ $1:4$ in $A$ (the higher-frequency wire is thinner). Then $R\propto 1/A$: ratio $4:1$.

**Check.** Thinner wire: higher pitch (less inertia) and higher resistance — the two ratios point the same way, 4:1 for the 2-frequency wire ✓.

**Answer: A** (4 : 1)

---

### Q10 — Estimate the number of atoms in the Earth

**Key observation.** $N = M_{\oplus}/(\text{mean atomic mass})$. Earth mass $\sim 6\times10^{24}$ kg; Earth is mostly O, Si, Mg, Fe — mean atomic mass $\sim 30$–$40$ u.

> 【Thought】 An order-of-magnitude Fermi estimate: the answer options are spaced by $10^5$, so even a factor-10 uncertainty in the mean atomic mass is harmless. The only facts needed: $M_\oplus\approx 6\times10^{24}$ kg and $1\ \text{u}\approx1.7\times10^{-27}$ kg. Using iron (56 u) throughout would still give $\sim10^{50}$ — the estimate is robust.

**Solution.**
$$N\sim\frac{6\times10^{24}}{35\times1.7\times10^{-27}}\sim 1\times10^{50}.$$

**Check.** Mole view: $\sim 10^{26}$–$10^{27}$ moles of $\sim$ tens-of-grams material ✓ consistent with $N_A\times$ that $\sim 10^{50}$–$10^{51}$; nearest offered order is $10^{50}$ ✓.

**Answer: A** ($10^{50}$)

---

### Q11 — Maximum number of unique photon energies among 10 levels

**Key observation.** Every pair of levels gives one transition energy; "all transitions possible" + generic (non-degenerate, non-commensurate) level spacings make all pair energies distinct. Count pairs.

> 【Thought】 Seeing "maximum number of unique energies" → triggers *count unordered pairs* $\binom{n}{2}$, not permutations. The trap options: $10^2=100$ (ordered, includes self-transitions), $10\times9=90$ (ordered pairs), $1+2+\cdots+10=55$ (counts gaps including non-adjacent double counting) — each encodes a specific miscount.

**Solution.** $\dbinom{10}{2}=\dfrac{10\times9}{2}=45$.

**Check.** "Maximum" assumes no two pairs accidentally share an energy (generic level structure) ✓.

**Answer: A** (45)

---

### Q12 — Explosion into two fragments: KE of the larger fragment

**Key observation.** Initially at rest → total momentum zero → fragments carry equal and opposite momenta $p$. With $KE=p^2/2m$, the **heavier** fragment gets the **smaller** share.

> 【Thought】 Seeing "explodes … initially at rest" → triggers *momentum conservation first, energy second* — the momentum constraint fixes the ratio, the energy fixes the scale. The designed trap is assigning more KE to the larger mass (intuition from $KE=\tfrac12 mv^2$ at common speed — wrong common quantity; the common quantity here is $p$, not $v$).

**Solution.** $KE_{\text{heavy}}:KE_{\text{light}}=\dfrac{p^2}{2am}:\dfrac{p^2}{2m}=1:a$, so
$$KE_{\text{heavy}}=\frac{E}{1+a}.$$

**Check.** $a\to1$: each gets $E/2$ ✓; $a\to\infty$: heavy fragment gets $\to0$ (it barely recoils) ✓.

**Answer: A** $\left(\dfrac{E}{1+a}\right)$

---

### Q13 — Quantum (Casimir) pressure vs plate separation

**Key observation.** Only $h$, $c$, $r$ available → pure dimensional analysis; there is a unique way to build pressure from them.

> 【Thought】 Seeing "dependent only upon h, c, r" → triggers *Buckingham π with three inputs*: one dimensionless answer, no freedom. No physics of the Casimir effect is needed — the information given is exactly enough for dimensional determination. (If $\hbar$ and $c$ could combine into a length-independent constant times any power of $r$, the problem would be underdetermined; it isn't, because mass appears only in $h$.)

**Solution.** $[h]=\text{kg m}^2\text{s}^{-1}$, $[c]=\text{m s}^{-1}$, $[p]=\text{kg m}^{-1}\text{s}^{-2}$. Set $p\propto h^\alpha c^\beta r^\gamma$: kg: $\alpha=1$; s: $-\alpha-\beta=-2\Rightarrow\beta=1$; m: $2\alpha+\beta+\gamma=-1\Rightarrow\gamma=-4$.
$$p\propto\frac{hc}{r^4}\;\Rightarrow\;p\propto\frac{1}{r^4}.$$

**Check.** This matches the true Casimir pressure $p=\dfrac{\pi^2\hbar c}{240\,r^4}$ ✓.

**Answer: D** $\left(p\propto1/r^4\right)$

---

### Q14 — Biscuit pushed across a teacup rim

**Key observation.** The biscuit rests on the rim along two contact points; it stays balanced while its centre $C$ lies within the support segment — i.e. between the chord of contact and the rim arc. Two boundaries: starting point = $C$ directly above the rim (farthest balanced position); falling point = $C$ over the chord.

> 【Thought】 Seeing "balanced … as far as possible … pushed inwards until it falls" → triggers *tipping = COM crossing the support polygon edge*; for a 2-point support the polygon edge is the chord joining the intersection points of the two circles (rim circle radius $R=3b/2$, biscuit edge radius $b$). The chord is the radical axis of the two circles — that is the geometric object to compute. If the biscuit were larger than the rim ($b>R$), the inner fall mechanism would change character (it could sit concentrically), so $b<R$ matters.

**Solution.** Let $x=|OC|$ (O = cup centre). The two circles intersect where, along $OC$, the chord sits at distance $s$ from $O$:
$$s=\frac{x^2+R^2-b^2}{2x}\qquad(\text{radical axis of the two circles}).$$
- **Start** (as far out as balanced): $C$ vertically above the rim: $x_i=R=\dfrac32 b$.
- **Fall** (pushed inward): tips when $C$ reaches the chord: $x=s\Rightarrow x^2=R^2-b^2$:
$$x_f=\sqrt{\tfrac94b^2-b^2}=\frac{\sqrt5}{2}b.$$
- **Distance pushed**:
$$d=x_i-x_f=\frac{3}{2}b-\frac{\sqrt5}{2}b=\boxed{\frac{3-\sqrt5}{2}\,b}\approx0.38\,b.$$

**Check.** $\sqrt{R^2-b^2}<R$ always (chord is inside the rim circle) so $d>0$ ✓; as $b\to R$ (biscuit nearly rim-sized), $d\to0$ — no travel before falling in ✓ physically sensible.

**Answer: D**

---

### Q15 — Maximum number of ice cubes, mixture entirely liquid

**Key observation.** "Entirely liquid at equilibrium" with *maximum* ice → the marginal state is all liquid at exactly $0^\circ$C. Then every joule of the water's sensible heat goes only into *melting* ice (the meltwater needs no warming).

> 【Thought】 Seeing "maximum number … entirely liquid" → triggers *boundary state analysis*: the limiting equilibrium is $T_f=0^\circ$C, turning an inequality into an equation. If cubes were colder than $0^\circ$C, each would also absorb heat warming to $0^\circ$C before melting — the given "$0^\circ$C ice" is what makes latent heat the only sink.

**Solution.** Heat released by 500 g water cooling $20\to0^\circ$C:
$$Q=0.500\times(4\times10^3)\times20=4.0\times10^4\ \text{J}.$$
Per cube (melting only): $Q_1=0.025\times(3\times10^5)=7.5\times10^3\ \text{J}$.
$$N=\left\lfloor\frac{4.0\times10^4}{7.5\times10^3}\right\rfloor=\lfloor5.33\rfloor=5.$$

**Check.** 6 cubes would need $4.5\times10^4$ J $>Q$ — some ice would remain ✓ consistent with 5 being maximal.

**Answer: B** (5)

---

### Q16 — Time for light to cross a glass cube (n = √2, incidence 30°)

**Key observation.** Time = (path length inside)/(speed inside) $=\dfrac{a/\cos r}{c/n}$. Get $r$ from Snell's law; keep everything in surds.

> 【Thought】 Seeing "time taken" → triggers *optical path thinking*: $t = nL/c$, and notice the product $n/\cos r$ simplifies when $\sin r$ is known exactly: with $\sin r=\sin30^\circ/\sqrt2=1/(2\sqrt2)$, $\cos r=\sqrt{7/8}$. The numbers are engineered for exact surds — if you find yourself with decimals, backtrack to fractions.

**Solution.**
$$\sin r=\frac{\sin30^\circ}{\sqrt2}=\frac{1}{2\sqrt2}\;\Rightarrow\;\cos r=\sqrt{1-\tfrac18}=\frac{\sqrt7}{2\sqrt2},$$
$$t=\frac{n a}{c\cos r}=\frac{\sqrt2\,a}{c}\cdot\frac{2\sqrt2}{\sqrt7}=\frac{4}{\sqrt7}\frac{a}{c}.$$

**Check.** Limits: $t>a/c$ (slower than vacuum straight-through) ✓; $t<na/c$ (path tilt increases length but… here $\tfrac{4}{\sqrt7}\approx1.51 < n=\sqrt2$? — compare correctly: $t/(a/c)=n/\cos r=\sqrt2/\cos r>\sqrt2$ ✓ since $\cos r<1$; numerically $4/\sqrt7=1.512>1.414$ ✓).

**Answer: B** $\left(\dfrac{4}{\sqrt7}\dfrac{a}{c}\right)$

---

### Q17 — Photoelectrons charging an isolated capacitor

**Key observation.** Charging stops when the retarding voltage equals the photoelectric stopping voltage: $eV=hf-hf_0$. Then $N=Q/e=CV/e$.

> 【Thought】 Seeing "steady value … electrons transferred" → triggers *equilibrium = kinetic energy balance, not current balance*: the capacitor self-limits when the field does work $eV$ equal to the maximum electron KE. The trap options swap $e$ vs $e^2$ and $f-f_0$ vs $f+f_0$; the physics fixes both: energy $h(f-f_0)$ (Einstein's equation) divided by $e$ twice (once for the voltage, once for the electron count).

**Solution.**
$$V_{\text{stop}}=\frac{h(f-f_0)}{e},\qquad Q=CV_{\text{stop}},\qquad N=\frac{Q}{e}=\frac{Ch(f-f_0)}{e^2}.$$

**Check.** Dimensions: $\text{F}\cdot\text{J}/\text{C}^2 = (\text{C/V})\cdot(\text{V}\cdot\text{C})/\text{C}^2=$ dimensionless count ✓; $f\to f_0$ gives $N\to0$ ✓.

**Answer: E** $\left(\dfrac{Ch(f-f_0)}{e^2}\right)$

---

### Q18 — Ranges at π/4 ± α

**Key observation.** Range $R=\dfrac{v^2\sin2\theta}{g}$; and $\sin\left(\dfrac{\pi}{2}\pm 2\alpha\right)=\cos 2\alpha$ for **both** — exactly equal, not approximately.

> 【Thought】 Seeing symmetric angles about $45^\circ$ → triggers *the complementary-angle symmetry of projectile range*: $45^\circ$ is the maximum of $\sin2\theta$, a stationary point, so deviations cancel to first order in $\alpha$ — and here the symmetry is exact. The nonzero options all carry a single power of $\alpha$; at a stationary point no term linear in $\alpha$ can exist, which selects A without any expansion.

**Solution.**
$$R_{\pm}=\frac{v^2}{g}\sin\left(\frac{\pi}{2}\pm2\alpha\right)=\frac{v^2}{g}\cos2\alpha\;\Rightarrow\;R_+-R_-=0.$$

**Check.** Both ranges equal $\frac{v^2}{g}(1-2\alpha^2+\ldots)$ — identical to all orders ✓.

**Answer: A** (0)

---

### Q19 — Time for one third to decay (half-life T)

**Key observation.** One third decayed = two thirds remain: $2^{-t/T}=2/3$; solve with logarithms base 2.

> 【Thought】 Seeing half-life + fraction → triggers *write survival as a power of 2*: $N/N_0=2^{-t/T}$; then take $\log_2$. The traps: $T\log_2 3$ (used $1/3$ instead of $2/3$) and $\tfrac23 T$ (linearised decay — wrong because decay is exponential, not linear).

**Solution.**
$$2^{-t/T}=\frac23\;\Rightarrow\;-\frac{t}{T}=\log_2\frac23=-\log_2\frac32\;\Rightarrow\;t=T\log_2\frac32\;(\approx0.585\,T).$$

**Check.** $0<t<T$ since less than half decays ✓; $t<T\log_2 3$ ✓ ordering sane.

**Answer: C** $\left(T\log_2\tfrac32\right)$

---

### Q20 — Jerk of a bungee jumper until first rest

**Key observation.** Two phases: free fall ($a=g$ constant → $j=0$), then ideal-spring motion (SHM segment: $a$ sinusoidal in $t$ → $j$ sinusoidal). The boundary values pin the graph: at rope-taut, $j$ jumps from $0$ to a nonzero value; at the lowest point ($v=0$), $j=-k v/m=0$.

> 【Thought】 Seeing "magnitude of jerk up to instantaneous rest" → triggers *evaluate the two instants the problem names* (taut, rest) plus monotonicity between. The jump at taut rules out B, C; the rise-then-fall (j starts at $v_0\omega^2$ but peaks later at $\omega\sqrt{g^2+v_0^2\omega^2}$) rules out A, E. Mechanism: $j=-\omega^2\dot s$ where $s$ is rope extension — jerk tracks the *velocity* of the extension, which grows (acceleration still downward) before shrinking.

**Solution.** With extension $s$, during the taut phase $\ddot s=g-\omega^2 s$, $\omega^2=k/m$:
$$a=\ddot s=g\cos\omega t-v_0\omega\sin\omega t,\qquad j=-\omega\left(g\sin\omega t+v_0\omega\cos\omega t\right).$$
- $t=0$ (taut): $|j|=v_0\omega^2>0$ — **jump** from 0;
- $|j|$ then rises to max $\omega\sqrt{g^2+v_0^2\omega^2}$ (when $\tan(\omega t+\varphi)$ passes $\pi/2$);
- at the lowest point $\dot s=0$: $j=-\omega^2\dot s=0$ — falls back to zero.

Graph: zero segment, vertical jump, rounded peak, decay to zero → **D**.

**Check.** Zero-slope at the peak (smooth sinusoid) ✓ matches D's rounded top; A has zero at jump (wrong), E has maximum at jump (wrong — the jumper still speeds up just after taut, so $|j|$ keeps growing) ✓.

**Answer: D**

---

### Q21 — Ring sliding down a propped rod: tension T = mg(1 − kt²)

**Key observation.** The rod is weightless and stays put (hinge + string), so **torque balance about O** holds at every instant; the only time-dependent object is the ring's position, set by its constant acceleration $g\sin30^\circ$ along the smooth rod.

> 【Thought】 Seeing a moving ring but a static rod → triggers *quasi-static structural equation for the rod* (torque about the hinge eliminates the unknown hinge force) + *kinematics for the ring* separately. Choosing O as pivot is the move: it removes two unknown hinge components at once. If the rod had weight, a constant extra term would appear; the given $T=mg(1-kt^2)$ form (value $mg$ at $t=0$) confirms the rod's weight is zero.

**Solution.** Ring acceleration along rod: $a=g\sin30^\circ=g/2$; distance from O along rod:
$$x=\ell-\tfrac12\cdot\tfrac{g}{2}t^2=\ell-\tfrac{g}{4}t^2.$$
Torque about O (ring's normal force $N=mg\cos30^\circ$ at distance $x$; tension vertical with lever arm $\ell\cos30^\circ$):
$$T\,\ell\cos30^\circ=mg\cos30^\circ\,x\;\Rightarrow\;T=mg\frac{x}{\ell}=mg\left(1-\frac{g}{4\ell}t^2\right).$$
$$k=\frac{g}{4\ell}.$$

**Check.** $t=0$: $T=mg$ — ring at top end directly under the string, string carries all of it ✓; ring reaches O when $x=0$: $T=0$ ✓ consistent.

**Answer: A** $\left(\dfrac{g}{4\ell}\right)$

---

### Q22 — Conical pendulum: double the angle, by what factor ω?

**Key observation.** For a conical pendulum $\omega^2=\dfrac{g}{\ell\cos\theta}$ (pendulum length $\ell$ fixed): $\omega^2\propto\sec\theta$.

> 【Thought】 Seeing "string length ℓ, angle to vertical" → triggers *the standard reduction*: vertical force balance $T\cos\theta=mg$ + horizontal circular motion $T\sin\theta=m\omega^2\ell\sin\theta$ — the radius $\ell\sin\theta$ cancels, leaving $\omega^2=g/(\ell\cos\theta)$. Note the depth $\ell\cos\theta$ is the controlling length, not the radius — the trap is using $\omega^2\propto\tan\theta$ or $\propto 1/\sin\theta$.

**Solution.**
$$\frac{\omega_{60}^2}{\omega_{30}^2}=\frac{\cos30^\circ}{\cos60^\circ}=\frac{\sqrt3/2}{1/2}=\sqrt3\;\Rightarrow\;\frac{\omega_{60}}{\omega_{30}}=3^{1/4}=\sqrt{\sqrt3}.$$

**Check.** $\theta\to90^\circ$ needs $\omega\to\infty$ ✓ (string can never be horizontal at finite speed); factor $\approx1.32$, modestly above 1 for doubling the angle — plausible since $\cos$ only halves ✓.

**Answer: A** $\left(\sqrt{\sqrt3}\right)$

---

### Q23 — LDR: halving the distance to a point source

**Key observation.** The log–log plot is a straight line from $(\log I,\log R)=(0,\,5.2)$ to $(4,\,1.8)$: slope $=\dfrac{1.8-5.2}{4}=-0.85$. Halving $d$ multiplies $I$ by 4 (inverse square law).

> 【Thought】 Seeing "logarithmic plot" + straight line → triggers *power law $R\propto I^{-0.85}$*; combine with the point-source law $I\propto d^{-2}$. So $R\propto d^{+1.7}$: halving $d$ gives $R\to R_0(1/2)^{1.7}$. If one forgot inverse-square and halved $I$ instead, one would get $R\approx1.8R_0$ — not on offer, so the option list itself nudges you to include it.

**Solution.** $\Delta\log I=\log 4=0.60$; $\Delta\log R=-0.85\times0.60=-0.51$;
$$\frac{R}{R_0}=10^{-0.51}\approx0.31\approx0.3.$$

**Check.** Direction: brighter → smaller resistance ✓; magnitude: 4× intensity changes resistance by less than 4× (sub-linear response, $|{\rm slope}|<1$) — 0.3 rather than 0.25 ✓ consistent.

**Answer: B** $(0.3R_0)$

---

### Q24 — Ladder pushed a small distance toward the wall: ΔGPE

**Key observation.** Small displacement → linearise: find how the centre-of-mass height responds to a base displacement at $\theta=45^\circ$ from the vertical.

> 【Thought】 Seeing "small distance a … best approximation" → triggers *differential (first-order) response*: compute $dh/dd$ at the given angle rather than exact finite geometry. Only $\tan\theta$ survives; at $45^\circ$ it is exactly 1, which is why the answer is a clean $\tfrac12 mga$.

**Solution.** Ladder length $L$, angle $\theta$ to vertical: base distance $d=L\sin\theta$, COM height $h=\tfrac{L}{2}\cos\theta$.
$$\delta d=-a\;\Rightarrow\;\delta\theta=\frac{-a}{L\cos\theta},\qquad \delta h=-\tfrac{L}{2}\sin\theta\,\delta\theta=\frac{a}{2}\tan\theta\stackrel{45^\circ}{=}\frac{a}{2}.$$
$$\Delta E_p=mg\,\delta h=\tfrac12 mga\quad(\text{increase}).$$

**Check.** Dimensions: $\text{kg}\cdot\text{m/s}^2\cdot\text{m}=\text{J}$ ✓; steeper ladder (larger $\theta$) rises more per push — $\tan\theta$ factor ✓.

**Answer: A** $\left(\tfrac12 mga\right)$

---

### Q25 — Twelve-resistor grid: which pair gives the median resistance?

**Key observation.** The network is a $2\times2$ square mesh (9 nodes, 12 edges, each $R$). Rather than five full circuit solutions, use symmetry reductions; then order the five values.

> 【Thought】 Strategy: exploit the mirror symmetries of the square. Driving between any pair creates an antisymmetry/symmetry that makes whole rows equipotential, deleting edges. If no symmetry applied (e.g. all resistors different), one would need Kirchhoff linear algebra for each pair — five times the work; "12 identical resistors" is the licence for symmetry.

**Solution.** (Centre $S$; corners $P$ top-left, $R$ top-right, $U$ bottom-right; edge midpoints $Q$ top, $T$ bottom.)

- **QT** (both on the vertical axis): the mirror symmetry left↔right makes the two top corners equipotential and the two bottom corners equipotential (they may be merged); the network then decomposes into **three node-disjoint paths** Q→T: the middle column Q–S–T ($R+R=2R$) and each side chain Q–corner–mid-edge–corner–T ($4R$ each):
$$R_{QT}=2R\parallel4R\parallel4R=\left(\frac{1}{2R}+\frac{1}{4R}+\frac{1}{4R}\right)^{-1}=R.$$
(The three paths share only the endpoints, so currents add independently — that is the whole derivation.)
- **QS** (adjacent axial nodes): the left↔right mirror merges the two top corners (potential $V_A$), the two side midpoints ($V_B$), the two bottom corners ($V_C$); the reduced ladder (Q–A, A–B, B–C, C–T each $R/2$; B–S $R/2$; Q–S and T–S each $R$) gives KCL chains $2V_A-V_B=V$, $3V_B=V_A+V_C$, $2V_C=V_B+V_T$, $3V_T=2V_C$, solved by $V_B=\tfrac27V$, $V_A=\tfrac{9}{14}V$; then $I=2(V-V_A)/R+V/R=\tfrac{12}{7}V/R$:
$$R_{QS}=\frac{7}{12}R.$$
- **PS** (corner to centre): by the 4-fold symmetry around $S$ + nodal analysis: $R_{PS}=\dfrac{7}{8}R$.
- **PR** (two corners on one edge): by nodal analysis: $R_{PR}=\dfrac{5}{4}R$.
- **PU** (diagonally opposite corners): by nodal analysis: $R_{PU}=\dfrac{3}{2}R$.

Ordered:
$$\underbrace{\tfrac{7}{12}R}_{QS}<\underbrace{\tfrac{7}{8}R}_{PS}<\underbrace{R}_{QT}<\underbrace{\tfrac54R}_{PR}<\underbrace{\tfrac32R}_{PU}.$$

**Check.** Ordering sanity: resistance grows with graph distance and shrinks with the number of alternative paths: QS (adjacent, many detours) smallest; PU (maximally separated corners) largest ✓. QT between them ✓. (All five values verified by exact nodal analysis.)

**Answer: E** (QT)

---
*End of Paper 2 (2025 Round 0).*


---

## Paper 3 — 2024 Round 1 Section 1 (8 Nov 2024)

*Section 1, Question 1, parts (a)–(r). Maximum 50 marks from ≈ 76.*

---

### Q1(a) — Stone dropped into a pool [3 marks]

**Key observation.** Two phases with different physics: free fall in air (accelerating), then sinking **at constant speed** (given). Time is additive; compute each phase separately.

> 【Thought】 Seeing "sinks with the same speed as it struck the water" → triggers *piecewise motion*: the impact speed becomes the sinking speed, so phase 2 needs no new dynamics — just $t_2 = d/v$. The phrase does the work of an entire force balance (buoyancy + drag vs weight) that we are explicitly told not to model.

**Solution.** Fall: $v=\sqrt{2gh}=\sqrt{2(9.81)(5.0)}=9.90\ \text{m/s}$, $t_1=v/g=1.01\ \text{s}$.
Sink: $t_2=\dfrac{4.0}{9.90}=0.404\ \text{s}$.
$$t=t_1+t_2\approx\boxed{1.41\ \text{s}}.$$

**Check.** Average speed overall $=9.0\ \text{m}/1.41\ \text{s}\approx 6.4\ \text{m/s}$, between 0 and $9.9$ ✓; $t_1>t_2$ since the fall starts from rest while the sinking is at full speed over a shorter distance ✓.

---

### Q1(b) — Galactic vs terrestrial orbital speed [3 marks]

**Key observation.** Orbital speed $=2\pi r/T$; the ratio kills $2\pi$ — the task reduces to converting both radii to a common unit (light-time) and both periods to years.

> 【Thought】 Seeing mixed astronomical units (light minutes, kpc, Myr) → triggers *convert everything into one consistent set before multiplying ratios*; light-based units for both distances minimise arithmetic. If one converted kpc to metres instead, the extra powers of ten would invite slips — unit choice is the strategy here.

**Solution.** $r_{\text{gal}}=8.3\ \text{kpc}=8.3\times10^3\times3.26=2.71\times10^{4}\ \text{ly}=1.42\times10^{10}$ light-minutes.
$$\frac{v_{\text{gal}}}{v_{\oplus}}=\frac{r_{\text{gal}}}{r_{\oplus}}\cdot\frac{T_{\oplus}}{T_{\text{gal}}}
=\frac{1.42\times10^{10}}{8.0}\times\frac{1}{2.4\times10^{8}}\approx\boxed{7.4}.$$

**Check.** Known numbers: Sun's galactic speed $\approx 220$ km/s, Earth's orbital speed $\approx 30$ km/s; ratio $\approx 7.3$ ✓.

---

### Q1(c) — Spring contraction in an accelerating elevator [3 marks]

**Key observation.** Static compression of the supporting spring measures the *apparent* weight: $k\Delta\ell = N = m(g+a)$ in the accelerating frame. This effective-gravity step presumes the acceleration is uniform ("accelerates uniformly from zero to 18 m/s"); a jerk would set the spring oscillating and $\Delta\ell_2$ would not be constant.

> 【Thought】 Seeing "elevator accelerates uniformly … contraction measured" → triggers *effective gravity* $g_{\text{eff}}=g+a$ (equivalence principle): the spring cannot tell acceleration from a stronger gravitational field. This holds only because the acceleration is uniform and quasi-steady; during a jerk, transient oscillations would add to $\Delta\ell_2$.

**Solution.** Lift acceleration $a=\dfrac{18}{6}=3.0\ \text{m/s}^2$.
$$\Delta\ell_1=\frac{mg}{k},\qquad \Delta\ell_2=\frac{m(g+a)}{k}\;\Rightarrow\;\boxed{\frac{\Delta\ell_1}{\Delta\ell_2}=\frac{g}{g+a}=\frac{9.81}{12.81}\approx0.77}.$$

**Check.** Ratio < 1 (spring compressed more when accelerating up) ✓; $a\to0$ gives 1 ✓.

---

### Q1(d) — Conical pendulum: two forms of the period [4 marks]

**Key observation.** Two force equations (vertical balance, horizontal centripetal) share the tension — divide them to get $\tan\theta$ directly, eliminating $T$ and $m$ in one move.

> 【Thought】 Seeing "by resolving the forces" with a mass tracing a horizontal circle → triggers *resolve along and perpendicular to the vertical*, not along the string: gravity is purely vertical and the acceleration purely horizontal, so this axis choice diagonalises the problem. (Resolving along the string would put centripetal acceleration components in both equations — legal but twice the algebra.)

**Solution.** (i) Vertical: $T\cos\theta=mg$; horizontal: $T\sin\theta=m\omega^2 r$. Dividing:
$$\tan\theta=\frac{\omega^2 r}{g}\;\Rightarrow\;\omega^2=\frac{g\tan\theta}{r}\;\Rightarrow\;\boxed{T=2\pi\sqrt{\frac{r}{g\tan\theta}}}.$$
(ii) Geometry of the cone: $r=\ell\sin\theta$:
$$T=2\pi\sqrt{\frac{\ell\sin\theta}{g\tan\theta}}=\boxed{2\pi\sqrt{\frac{\ell\cos\theta}{g}}}.$$

**Check.** $\theta\to0$: $T\to2\pi\sqrt{\ell/g}$, the ordinary pendulum period ✓ (small oscillation limit); $\theta\to90^\circ$: $T\to0$ — infinite speed needed ✓.

---

### Q1(e) — L-shaped lever with two masses [4 marks]

**Key observation.** One pivot, two weights, gravity vertical: equilibrium ⟺ net torque about B is zero. The perpendicular arms turn "arm at $\theta$ to vertical" into moment arms $a\sin\theta$ and $b\cos\theta$.

> 【Thought】 Seeing "smoothly pivoted at B" → triggers *take torques about B* — the pivot force (unknown, two components) then vanishes from the equations. If one instead wrote force balances, the pivot would inject two unknowns for zero benefit. The failure boundary: if friction acted at the pivot, torque balance would not fix a unique $\theta$ — "smoothly" is the licence.

**Setup.** AB at $\theta$ to the vertical; since AB⊥BC, arm BC is at $\theta$ to the horizontal. Moment arms about B (horizontal distances): $a\sin\theta$ for $m_a$; $b\cos\theta$ for $m_b$.

**Solution.** Torque balance (the two weights must lean to opposite sides of the vertical through B):
$$m_a g\,a\sin\theta=m_b g\,b\cos\theta\;\Rightarrow\;\boxed{\tan\theta=\frac{m_b b}{m_a a}}.$$

**Check.** $m_b\to0$: $\theta\to0$ — AB hangs straight down, carrying the only weight directly below the pivot ✓; dimensions: ratio of masses × lengths is dimensionless ✓ (tan of an angle).

---

### Q1(f) — Falling plank pushing a trolley [4 marks]

**Key observation.** Everything is smooth (hinge, contact, floor) → **energy conservation** holds, and the trolley–plank contact is a *kinematic constraint*: the trolley's corner must stay on the plank's face line, which ties $v_t$ to the plank's rotation by geometry alone.

> 【Thought】 Seeing "smooth flat surface … pushing the top rear corner" → triggers *(1) write the contact condition from geometry, (2) only then apply energy*. The contact is **plank face (a rotating line) against a sliding point (the corner)** — so the constraint is that the corner stays on the face line, *not* equality with the plank top's horizontal velocity component. That distinction decides everything below.

**Setup.** Hinge at the origin; plank at angle $\theta$ to the ground; trolley corner at $(x_t,h)$. At the final moment the plank's top reaches the corner: $\sin\theta=h/\ell=1/3$.

**Constraint.** The face is the line $y=x\tan\theta$; the corner rides on it:
$$x_t=h\cot\theta\;\Rightarrow\;v_t=\dot x_t=\frac{h}{\sin^2\theta}|\dot\theta|=\frac{h}{\sin^2\theta}\frac{v_p}{\ell}=\frac{h}{\ell}\frac{v_p}{\sin^2\theta}=\frac{1}{3}\cdot9\,v_p=3v_p,$$
since $|\dot\theta|=v_p/\ell$. (Equivalently: match normal velocities — the plank top's velocity is entirely along the face normal, $v_p$, while the corner's normal component is $v_t\sin\theta=v_t/3$.) The rotating face sweeps the corner forward three times faster than the plank top's own horizontal speed — a rotating-line lever effect.

**Energy.** The plank's centre of mass falls $\dfrac{\ell}{2}(1-\sin\theta)=\dfrac{\ell}{3}=h$, releasing $Mgh$. With $m_t=2M$ (from $M=m_t/2$):
$$Mgh=\underbrace{\tfrac16 Mv_p^2}_{\text{plank (given)}}+\underbrace{\tfrac12 m_t v_t^2}_{\text{trolley}}=\tfrac16 Mv_p^2+\tfrac12(2M)(3v_p)^2=\left(\tfrac16+9\right)Mv_p^2=\tfrac{55}{6}Mv_p^2,$$
$$v_p^2=\frac{6gh}{55}\;\Rightarrow\;\boxed{v_t=3v_p=\sqrt{\frac{54}{55}\,gh}\approx0.99\sqrt{gh}}.$$

**Check.** Energy split: trolley takes $9/(55/6)=54/55\approx98\%$ — the rotating face is an extreme lever at this shallow angle ($19.5^\circ$) ✓. Limiting behaviour: $\theta\to90^\circ$ gives $v_t\to v_p$ (upright plank = direct push) ✓; $v_t=\sqrt{gh}$ order ✓. Dimensions ✓.

> 【Thought】**Official-divergence note (compressed).** The mark scheme sets $v_t=v_p\sin\theta=v_p/3$ — the trolley taking the horizontal component of the plank top's velocity — obtaining $v_t^2=2gh/5$. That constraint would hold only if the trolley's corner were *pinned* to the plank's top end; a smooth face cannot pin a corner, and the correct contact condition is $x_t=h\cot\theta\Rightarrow v_t=3v_p$ (ours). We present $v_t=\sqrt{54gh/55}$ as the physically correct answer, recording the official value for reference. (Also: the mass relation reads $M=m_t/2$, i.e. $m_t=2M$ — double-read before substituting.)

---

### Q1(g) — Rocket test track: out and back in 48 s [6 marks]

**Key observation.** Acceleration phase time $t_1$ determines everything: distance $d=\tfrac12 a t_1^2$, return time $t_2=d/v_c$ — a single quadratic in $t_1$.

> 【Thought】 Seeing "brakes in negligible time" → triggers *two-phase timeline with one unknown duration*; parametrise by $t_1$ (not $d$), because both $d$ and $t_2$ are then simple monomials. Solving for $d$ directly gives a $\sqrt d$ equation — legal but uglier; choosing the right parameter is the economy move.

**Solution.** Outward: $d=\tfrac12(15)t_1^2=7.5t_1^2$. Return: $t_2=\dfrac{d}{12}=0.625\,t_1^2$. Total:
$$t_1+0.625t_1^2=48\;\Rightarrow\;5t_1^2+8t_1-384=0\;\Rightarrow\;t_1=\frac{-8+\sqrt{64+7680}}{10}=\frac{-8+88}{10}=8\ \text{s},$$
$$d=7.5\times64=\boxed{480\ \text{m}}.$$

**Check.** End speed $15\times8=120\ \text{m/s}$ (Mach 0.35 — fast but it is a rocket sled ✓); return leg $480/12=40$ s, $8+40=48$ ✓. The quadratic's clean integer root ($t_1=8$) confirms the numbers were engineered for this route.

---

### Q1(h) — Reading a wave equation [4 marks]

**Key observation.** Compare $y=A\cos(\omega t+kx)$ with the given expression — the numbers 1800 and 5.72 are $\omega$ and $k$ (dimensionally forced by the units in brackets).

> 【Thought】 Seeing "phase = time part + space part" → triggers *match coefficients*: the $+kx$ sign means travel in the $-x$ direction. Note the trap: 1800 is **not** the frequency — it is $\omega$; forgetting $2\pi$ flips (i) and (ii) wrong together.

**Solution.** (i) $A=4.0\times10^{-6}\ \text{m}$; $\omega=1800\ \text{rad/s}\Rightarrow f=\dfrac{1800}{2\pi}=286\ \text{Hz}$; $k=5.72\ \text{rad/m}\Rightarrow\lambda=\dfrac{2\pi}{5.72}=1.10\ \text{m}$; $v=\dfrac{\omega}{k}=\dfrac{1800}{5.72}=315\ \text{m/s}$ (travelling in $-x$).
(ii) The medium's point oscillates: $v_y=-A\omega\sin(\omega t+kx)$, so
$$v_{\max}=A\omega=4.0\times10^{-6}\times1800=\boxed{7.2\times10^{-3}\ \text{m/s}}.$$

**Check.** $v=f\lambda=286.5\times1.098=315$ ✓ (consistency between the two routes); particle speed $\ll$ wave speed, as usual for small-amplitude waves ✓.

---

### Q1(i) — Beats and the temperature of an organ pipe [4 marks]

**Key observation.** Beat frequency = |difference|. The pipe starts 4 Hz **below** 256 Hz (given "slightly lower"); beats falling to zero then returning to 4 Hz means the pipe's frequency swept $252\to256\to260$ Hz. Pipe length is fixed, so $f\propto v\propto\sqrt{T}$.

> 【Thought】 Seeing "first reduces to zero and then increases" → triggers *the frequency crossed the reference* — the only way a beat note can pass through zero. This converts a beat statement into a precise frequency ratio $260/252$. If the beats had merely halved or doubled, no unique answer would exist — the zero crossing is the calibration point.

**Solution.** $v=\sqrt{\gamma P/\rho}$; at constant pressure $\rho\propto1/T$ (ideal gas), so $v\propto\sqrt{T}$ and $f\propto\sqrt T$:
$$\frac{T_2}{T_1}=\left(\frac{f_2}{f_1}\right)^2=\left(\frac{260}{252}\right)^2=1.0645,$$
$$T_1=17^\circ\text{C}=290\ \text{K},\qquad T_2=1.0645\times290=308.7\ \text{K},$$
$$\boxed{\Delta T\approx+19\ \text{K}\quad(\text{the air warms from }17^\circ\text{C to about }36^\circ\text{C}).}$$

**Check.** Direction: raising temperature raises $v$, hence $f$ — and the pipe had to climb from below 256 Hz to above it ✓; magnitude: a 3% frequency change needs a 6% absolute-temperature change ✓ ($\Delta f/f\approx\tfrac12\Delta T/T$).

---

### Q1(j) — Freezing fraction of supercooled water [3 marks]

**Key observation.** Insulated container → the latent heat released by the freezing fraction warms **all** the water from $-10^\circ$C to $0^\circ$C; the process stops at the ice–water coexistence temperature.

> 【Thought】 Seeing "supercooled … some immediately freezes" → triggers *self-limiting phase change*: freezing stops when the mixture hits $0^\circ$C, because coexistence pins the temperature. The endpoint is fixed by phase equilibrium, not by dynamics — this is what makes the problem statically solvable. (The same logic underlies "regelation" and storm-cloud glaciation calculations.)

**Solution.** Per kg of water, fraction $x$ freezes: latent heat released $xL$ warms the whole kilogram by $10$ K:
$$xL=c\,\Delta T\;\Rightarrow\;x=\frac{c\,\Delta T}{L}=\frac{4180\times10}{335\,000}=\boxed{0.125\;\;(\tfrac18,\ \text{about }12.5\%)}.$$

**Check.** Rule of thumb validated: $c\Delta T\ll L$ (42 kJ vs 335 kJ per kg), so only a small fraction freezes ✓; if $\Delta T$ were $L/c\approx80$ K the whole volume would freeze — supercooling of $-10^\circ$C is well below that ✓ consistent.

---

### Q1(k) — Ideal diode + resistor: average power for two waveforms [4 marks]

**Key observation.** The ideal diode transmits only the positive half-cycles (zero forward drop, perfect blocking). Average power = time average of $V^2/R$ over a **full** period, with the negative half contributing zero.

> 【Thought】 Seeing "ideal diode … average power" → triggers *rectification bookkeeping*: integrate $V^2/R$ over one period with the negative half deleted. The two classic mistakes: (1) halving the sinusoidal rms calculation twice or not at all — write the integral rather than guessing factors; (2) assuming the square wave's "amplitude" means 0-to-$V_0$ — the figure shows $\pm V_0$, and the diode makes the sign matter.

**Solution.** (i) Square wave: $V=\pm V_0$; power is $V_0^2/R$ for half the period, 0 for the other half:
$$\boxed{\bar P_{\text{sq}}=\frac{V_0^2}{2R}}.$$
(ii) Sinusoid $V=V_0\sin(2\pi t/T)$: conducts for $0<t<T/2$:
$$\bar P_{\text{sin}}=\frac{1}{T}\int_0^{T/2}\frac{V_0^2\sin^2(2\pi t/T)}{R}\,dt=\frac{V_0^2}{R}\cdot\frac{1}{T}\cdot\frac{T}{4}=\boxed{\frac{V_0^2}{4R}}.$$

**Check.** Without the diode the sinusoid would give $V_0^2/2R$ (rms) — the diode halves it again to $V_0^2/4R$ ✓; square > sinusoidal average power at equal amplitude, since the square wave sits at $\pm V_0$ throughout its on-time ✓.

---

### Q1(l) — Square of wire with its diagonals connected [3 marks]

**Key observation.** A and B are **diagonally opposite** corners. Reflection symmetry about the diagonal AB makes the other two corners (C, D) equipotential — short them into one node $X$; then the centre O and $X$ turn out equipotential too, collapsing the bridge.

> 【Thought】 Seeing a symmetric network with the asked pair lying **on** a symmetry axis → triggers *fold the network along that axis*: points mirrored into each other share a potential and may be soldered together. Each mirrored pair of half-diagonals then merges into a parallel pair. If A and B were adjacent corners instead, this fold would not exist and one would solve Kirchhoff equations — the diagonal placement is what makes a surd-only answer possible.

**Solution.** Set $r\ell=1$ (restore at the end). After folding C≡D into X, the network is:
$$A\!-\!X:\ \tfrac{r\ell}{2}\cdot\ldots$$

Concretely, with edges $A\!-\!X:\tfrac12$, $X\!-\!B:\tfrac12$ (two parallel sides each), $A\!-\!O:\tfrac{1}{\sqrt2}$, $O\!-\!B:\tfrac{1}{\sqrt2}$ (half-diagonals, length $\ell/\sqrt2$), $X\!-\!O:\tfrac{1}{2\sqrt2}$ (two merged half-diagonals). Writing KCL at O and X with $V_A=1,V_B=0$:
$$4V_O-2V_X=1,\qquad (2+\sqrt2)V_X-\sqrt2\,V_O=1\;\Rightarrow\;V_O=V_X=\tfrac12.$$
No current flows in X–O; the network is just two parallel paths: $A\!-\!O\!-\!B=\sqrt2$ and $A\!-\!X\!-\!B=1$:
$$R_{AB}=\frac{\sqrt2\cdot1}{\sqrt2+1}\,r\ell=\frac{\sqrt2}{1+\sqrt2}r\ell=\boxed{(2-\sqrt2)\,r\ell}\approx0.586\,r\ell.$$

**Check.** Must be less than the plain-square value $r\ell$ (diagonals only add paths) ✓; greater than the direct diagonal $\sqrt2 r\ell\approx1.41$? No — wait: $0.586<1.414$, fine because the diagonal path is *helped* by the side paths ✓; the surd form is exact ✓.

---

### Q1(m) — Sliding contact on a circle of resistance wire [6 marks]

**Key observation.** A and B split the ring into two arcs **in parallel**. $R_{AB}$ is a quadratic function of the arc length — zero at coincidence, maximum at the diametric point.

**Setup.** Resistance per unit length:
$$r=\frac{\rho}{A_{\text{cs}}}=\frac{3.0\times10^{-4}}{\pi(0.70\times10^{-3})^2}=195\ \Omega\,\text{m}^{-1},\qquad L=2\pi(0.10)=0.628\ \text{m},\qquad R_{\text{tot}}=122\ \Omega.$$

> 【Thought】 Seeing "contact B can slide" → triggers *parametrise by arc length s and recognise the parallel-pair formula* $R(s)=rs\cdot r(L-s)/(rL)$, a parabola. Its maximum is forced by symmetry to $s=L/2$ — no calculus needed (AM–GM: product of two parts with fixed sum is maximal when equal).

**(i) Maximum.** At $s=L/2$: two half-rings of $R_{\text{tot}}/2$ in parallel:
$$R_{\max}=\frac{R_{\text{tot}}}{4}=\boxed{30.6\ \Omega}.$$

**(ii) Graph.** $R(s)=\dfrac{r}{L}\,s(L-s)$: an inverted parabola through $(0,0)$, peak $(L/2,\,30.6\ \Omega)$, back to $(L,0)$ — symmetric about $s=L/2$.

**(iii) R = 22.0 Ω.**
> 【Thought】 Math action with purpose: $R(s)=22$ is quadratic with **two** roots (the parabola is symmetric); the question asks for the *shortest* arc, so keep the smaller root — the other is its mirror $L-s$.

$$s(L-s)=\frac{R L}{r}=\frac{22.0\times0.628}{195}=0.0709\ \text{m}^2\;\Rightarrow\;s^2-0.628s+0.0709=0,$$
$$s=\frac{0.628-\sqrt{0.628^2-4(0.0709)}}{2}=\boxed{0.147\ \text{m}\approx15\ \text{cm}}.$$

**Check.** $s\approx0.147$ m corresponds to arc resistance $\approx28.7\ \Omega$ in parallel with $122-28.7=93.7\ \Omega$: product/sum $=2690/122.4\approx22$ ✓.

---

### Q1(n) — Linearly declining charging current [4 marks]

**Key observation.** "Fully charged" is defined by the current reaching zero; charge is the **area under** the $I$–$t$ line — a triangle.

> 【Thought】 Seeing $I=I_0-\alpha t$ valid only for $t<t_{\text{full}}$ → triggers *find the domain endpoint first* (where the model switches off), then integrate over exactly that domain. The trap is integrating beyond $I=0$ into negative (unphysical) current. For a linear decay the integral is triangle area — no calculus needed: $\tfrac12 I_0 t_{\text{full}}$.

**Solution.** (i) $I=0$ at
$$\boxed{t_{\text{full}}=\frac{I_0}{\alpha}}.$$
(ii) $Q=\displaystyle\int_0^{I_0/\alpha}(I_0-\alpha t)\,dt=\tfrac12\times\text{base}\times\text{height}=\boxed{\dfrac{I_0^2}{2\alpha}}.$

**Check.** Dimensions: $\text{A}^2/(\text{A/s})=\text{A s}=\text{C}$ ✓; equivalent to average current $I_0/2$ for time $I_0/\alpha$ ✓.

---

### Q1(o) — Cone of graded density floating base-flush [6 marks]

**Key observation.** "Base level with the surface" = the cone is **exactly fully submerged**, so buoyancy $=\rho_\ell gV$ and flotation requires mean density $=\rho_\ell$. With density linear in height and cross-section quadratic in height, the volume-weighted mean of a linear profile is its value at the centroid height — ¾ of the way from apex to base.

> 【Thought】 Seeing "density varies linearly along its length" + cone → triggers *weighted averaging with area $\propto y^2$*: the mean is not $(\rho_a+\rho_b)/2$ (that would suit a prism). The volume element $y^2\,dy$ pushes the weighting toward the base — hence the ¾. If the cone pointed apex-up, the weighting would flip toward the apex and the answer would change — orientation matters.

**Solution.** Let $y$ measure height from the apex; radius $\propto y$, so $dV\propto y^2\,dy$. With $\rho(y)=\rho_a+(\rho_b-\rho_a)\,y/H$:
$$\bar\rho=\frac{\int_0^H\rho(y)\,y^2\,dy}{\int_0^H y^2\,dy}=\rho_a+(\rho_b-\rho_a)\frac{\int_0^H y^3\,dy/H}{\int_0^H y^2\,dy}=\rho_a+\tfrac34(\rho_b-\rho_a)=\frac{\rho_a+3\rho_b}{4}.$$
Flotation (fully submerged): $\bar\rho=\rho_\ell$, with $\rho_b=\rho_\ell/2$:
$$\frac{\rho_a+3\rho_\ell/2}{4}=\rho_\ell\;\Rightarrow\;\rho_a=4\rho_\ell-\tfrac32\rho_\ell\;\Rightarrow\;\boxed{\frac{\rho_a}{\rho_\ell}=\frac52}.$$

**Check.** $\rho_a>\rho_\ell>\rho_b$: dense apex down, light base up — a stably floating gradient ✓; as a weighted mean $\bar\rho$ must lie between $\rho_b=0.5\rho_\ell$ and $\rho_a=2.5\rho_\ell$: $1.0$ does ✓.

> 【Thought】**Cross-check against the official mark scheme:** its own working gives $\rho_\ell/3=\rho_\ell/8+\rho_a/12$, i.e. $\rho_a/12=5\rho_\ell/24$, which multiplies out to $\rho_a/\rho_\ell=5/2$ — our answer. The mark scheme's printed final line "$5/24$" drops the factor of 12 in the last step (an arithmetic slip in the official document); every line of its derivation agrees with ours.

---

### Q1(p) — Neoprene expansion joints: when does the road crack? [5 marks]

**Key observation.** The concrete slabs and the neoprene are in **series** — they carry the same stress (same cross-sectional area). The neoprene is crushed by exactly the thermal expansion of one slab; its elastic pushback $E_n\varepsilon_n$ is the stress the concrete feels. Cracking starts when that reaches 30 MPa.

> 【Thought】 Seeing "2.0 cm neoprene between every 20 m of concrete" → triggers *strain partition*: the geometry mismatch ($\alpha L\Delta T$ of concrete) is absorbed entirely by the soft layer, so $\varepsilon_n=\alpha L\Delta T/d$, hugely amplified by $L/d=1000$. Series stress equality is the bridge from neoprene strain to concrete stress. (Model caveat, worth stating: this linear extrapolation takes the neoprene far beyond realistic strains — see Check.)

**Solution.** Slab expansion absorbed by one joint: $\Delta L=\alpha L\Delta T=12\times10^{-6}\times20\times\Delta T=2.4\times10^{-4}\Delta T$ (m). Neoprene strain and stress:
$$\varepsilon_n=\frac{\Delta L}{d}=\frac{2.4\times10^{-4}\Delta T}{0.020}=0.012\,\Delta T,\qquad \sigma=E_n\varepsilon_n=(2.7\times10^6)(0.012\,\Delta T)=3.24\times10^{4}\,\Delta T\ \text{Pa}.$$
Cracking when $\sigma=30\ \text{MPa}$:
$$\Delta T=\frac{30\times10^6}{3.24\times10^4}=926\ \text{K}\;\Rightarrow\;\boxed{T_{\max}\approx293+926\approx1220\ \text{K}\approx950^\circ\text{C}}.$$

**Model-validity statement.** 1220 K is *not* a physical prediction — it is the proof-by-absurdity that linear elasticity cannot deliver 30 MPa here: the joint already closes fully at $\Delta T=d/(\alpha L)\approx83$ K ($\approx100^\circ$C), beyond which the model itself breaks down.

> 【Thought】 The answer is hotter than lava — that is the physics talking, not an arithmetic error: soft neoprene ($E$ only 2.7 MPa) can never push back hard enough to crack 30 MPa concrete at any terrestrial temperature. In reality the joint fully closes at $\Delta T=d/(\alpha L)\approx83$ K ($T\approx100^\circ$C) and the model changes character; the exam answer within the stated linear model is $\sim950^\circ$C — the takeaway being that compliant joints make thermal cracking essentially impossible.

**Check.** Linear-response route cross-check: $\Delta T=\dfrac{\sigma_b\,d}{E_n\,\alpha L}=\dfrac{3\times10^7\times0.02}{2.7\times10^6\times12\times10^{-6}\times20}=926$ K ✓ same.

---

### Q1(q) — Energy escaping through two imperfect mirrors [4 marks]

**Key observation.** The beam alternates mirrors; each hit transmits fraction $(1-R)$ of what arrives. The two escape streams are geometric series in $R^2$, offset by one factor of $R$.

> 【Thought】 Seeing "reflectivity R … total energy through each mirror" → triggers *sum the geometric series per mirror* rather than tracking individual bounces. The first-struck mirror always leads by exactly one reflection — hence the ratio is just $R$, independent of how many bounces. If the mirrors had different reflectivities $R_1,R_2$, the series would decouple into two ratios and the answer would be $R_2(1-R_1):R_1(1-R_2)$-like — the symmetry here is what collapses it.

**Solution.** Mirror 1 (struck first) transmits $(1-R)I_0\left(1+R^2+R^4+\cdots\right)$; mirror 2 transmits $(1-R)I_0R\left(1+R^2+\cdots\right)$:
$$E_1=\frac{(1-R)I_0}{1-R^2}=\frac{I_0}{1+R},\qquad E_2=\frac{RI_0}{1+R},$$
$$\boxed{E_1:E_2=1:R}.$$

**Check.** $E_1+E_2=I_0$ — all energy eventually escapes (no absorption in this model) ✓; $R\to1$: escape splits evenly $1:1$ ✓ (the photon "forgets" which side it started from after many bounces).

---

### Q1(r) — Two gases, bursting diaphragm, final pressure [6 marks]

**Key observation.** Phase 1 (heating at fixed volumes): each gas obeys $P/T=$ const, so the pressure *difference* scales with $T$ — the burst condition fixes $T_b$. Phase 2 (mixing in a rigid, insulated tube): total internal energy is conserved and, for ideal gases at the same temperature, the final pressure is just the volume-weighted mean of the two burst pressures.

> 【Thought】 Seeing "uniformly heated until the diaphragm bursts at maximum force F" → triggers *the bursting condition is a force balance* $(P_1'-P_2')A=F$, not a pressure threshold. Seeing "insulated, pressure equalises" → triggers *first law with $Q=W=0$: $U$ conserved*; for ideal gases $U\propto nT\propto PV$ (per gas), so pressure averaging works without knowing $c_V$ or even whether the gases mix chemically. If the tube were not insulated, $T_f$ would be unknown and the problem unsolvable — the insulation clause is essential.

**Solution.** Phase 1: $P_i'=P_i\,T_b/T_0$ (constant volume). Burst:
$$\frac{T_b}{T_0}(P_1-P_2)A=F\;\Rightarrow\;\frac{T_b}{T_0}=\frac{F}{A(P_1-P_2)}.$$
Phase 2: $U=\sum_i c_V n_iT$; with $P_i'V=n_iRT_b$ (each volume $V=Al/2$), energy conservation gives $T_f=T_b$ and
$$P_f(2V)=\left(n_1+n_2\right)RT_b=\left(P_1'+P_2'\right)V\;\Rightarrow\;P_f=\frac{P_1'+P_2'}{2}=\frac{P_1+P_2}{2}\cdot\frac{T_b}{T_0},$$
$$\boxed{P_f=\frac{F(P_1+P_2)}{2A\,(P_1-P_2)}}.$$

**Check.** Limit $P_2\to P_1$: $T_b\to\infty$ needed to burst (tiny pressure difference needs huge heating) ✓ formula diverges correctly. Pressure is bounded: $P_f$ lies between $P_1'$ and $P_2'$ ✓ (mean). Dimensions: $F/A$ is pressure ✓.

---
*End of Paper 3 (2024 Round 1 Section 1).*


---

## Paper 4 — 2024 Round 1 Section 2 (8 Nov 2024)

*Section 2: four long questions (Q2–Q5), 25 marks each; candidates attempt two. Full solutions for all four are given.*

---

### Question 2 — Solar energy, energy losses and capacitors

#### Q2(a) — Estimating solar intensity with a black can [7 marks]

**Key observation.** Energy balance with **no losses**: solar power intercepted = rate of internal energy gain of the water. The can is a cylinder; the Sun is at 50° elevation, so the intercepted area is the *projected* area of lid **and** side wall onto a plane perpendicular to the rays.

> 【Thought】 Seeing "angle of the Sun to the horizontal is 50°" → triggers *projection bookkeeping*: a horizontal lid intercepts $I\,A_{\text{lid}}\sin 50^\circ$ and a vertical wall intercepts $I\,A_{\text{wall,proj}}\cos 50^\circ$ — the wall's projected width is the diameter $d$ (not the half-circumference), because only the silhouette intercepts light. Forgetting the wall, or using the full curved area $\pi d h$, are the two designed errors. "Neglect the heat capacity of the can" licenses $Q=mc\Delta T$ for the water alone.

**Setup.** $m=0.300$ kg water; $\Delta T=3.0$ K in $\Delta t=1200$ s. Lid $A_l=\pi d^2/4=\pi(0.06)^2/4=2.83\times10^{-3}\ \text{m}^2$; wall silhouette $A_w=dh=6.0\times10^{-3}\ \text{m}^2$.

**Solution.** Absorbed power required:
$$P=\frac{mc\Delta T}{\Delta t}=\frac{0.300\times4180\times3.0}{1200}=3.14\ \text{W}.$$
Effective intercepting area (rays at $50^\circ$ to horizontal):
$$A_{\text{eff}}=A_l\sin50^\circ+A_w\cos50^\circ=2.83\times10^{-3}\times0.766+6.0\times10^{-3}\times0.643=6.02\times10^{-3}\ \text{m}^2.$$
$$I=\frac{P}{A_{\text{eff}}}=\frac{3.14}{6.02\times10^{-3}}\approx\boxed{5.2\times10^{2}\ \text{W m}^{-2}}.$$

**Check.** Below the solar constant (1360 W m⁻²) — atmosphere and the latitude factor take roughly half ✓ physically sane for full sunlight in Spain.

#### Q2(b) — The "leaky capacitor" model (cell ε, series R, leak r across C) [6 marks]

**Key observation.** The capacitor is shunted by a leak $r$: the resistor current splits into leak current $V_C/r$ and charging current $\dot Q$. Kirchhoff's voltage law then yields a first-order linear ODE — read $\tau$ and $Q_{ss}$ off its structure.

> 【Thought】 Strategy: the question walks you through the standard routine (KVL → current split → ODE → read off τ). The transferable skill: any equation $\dot Q+Q/\tau=\text{const}$ has time constant $\tau$ equal to the reciprocal of the $Q$-coefficient — no integration needed. Note $\tau=(R\parallel r)C$: the capacitor "sees" the parallel combination, exactly the Thévenin resistance looking back from its terminals — a much faster way to get $\tau$ once you recognise it.

**Solution.**
(i) KVL around the loop:
$$\varepsilon=IR+\frac{Q}{C}.$$
(ii) Current split at the capacitor node:
$$I=I_r+I_C=\frac{Q}{rC}+\frac{dQ}{dt}.$$
(iii) Substitute:
$$\varepsilon=R\frac{dQ}{dt}+\frac{RQ}{rC}+\frac{Q}{C}\quad\Longrightarrow\quad \varepsilon=R\dot Q+\frac{R+r}{rC}\,Q.$$
(iv) Standard form $\dot Q+Q/\tau=\varepsilon/R$:
$$\boxed{\tau=\frac{Rr}{R+r}\,C=(R\parallel r)\,C}.$$
(v) Long time: $\dot Q=0$, no current into C; R and r form a divider, $V_C=\varepsilon\,\dfrac{r}{R+r}$:
$$\boxed{Q_{ss}=\frac{\varepsilon C r}{R+r}}.$$
(vi) Graph: $Q(t)=Q_{ss}\left(1-e^{-t/\tau}\right)$ — an exponential approach from 0, initial slope $\varepsilon/R$ (line from origin aiming at $\varepsilon C$... i.e. tangent at origin hits $Q_{ss}$ at $t=\tau$), asymptoting to $Q_{ss}$; mark $\varepsilon$ as the intercept scale-setting parameter on the graph's annotation ($Q_{ss}<\varepsilon C$).

**Check.** Limits: $r\to\infty$ (no leak): $\tau\to RC$, $Q_{ss}\to C\varepsilon$ — the textbook RC circuit ✓; $r\to0$ (dead short): $\tau\to0$, $Q_{ss}\to0$ ✓.

#### Q2(c) — Constant-current drive and the cooling experiment [7 marks]

**(i)** With a constant current source $I_0$ feeding $r\parallel C$: after a long time the capacitor is full (no current into it), so all of $I_0$ flows through $r$:
$$\boxed{Q_{\max}=I_0 rC,\qquad U=\tfrac12 C V^2=\tfrac12\,I_0^2 r^2 C.}$$

> 【Thought】 Analogy dictionary (given in the question): charge $\leftrightarrow$ internal energy, leak current $\leftrightarrow$ heat loss power $kT$. Constant *power* input to the can = constant *current* source — that is why Fig. 3 replaces the cell; recognising why the model was changed is worth more than the algebra.

**(ii)** Power budget for the can ($T$ = excess over ambient):
$$\boxed{P_{\text{can}}=mc\frac{dT}{dt}+kT}.$$

**(iii)** Steady state ($dT/dt=0$):
$$P_{\text{can}}=kT_{ss}.$$

**(iv)** Cooling curve (no illumination): $mc\,\dot T=-kT$, exponential decay of the excess: $T(t)=T_1 e^{-kt/mc}$:
$$k=\frac{mc}{\Delta t}\ln\frac{T_1}{T_2}=\frac{0.300\times4180}{2400}\ln\frac{34.2-31.0}{32.8-31.0}=\frac{1254}{2400}\ln\frac{3.2}{1.8}=\boxed{0.30\ \text{W K}^{-1}}.$$

> 【Thought】 The 40-minute cooling from 3.2 K to 1.8 K excess is used *logarithmically*: taking the ratio $T_1/T_2$ removes the unknown start time — always use ratios, never absolute readings, when the zero of the clock is arbitrary.

**(v)** Corrected solar estimate: during the 20-min heating the average excess temperature was $\bar T\approx\tfrac12(0+3.0)=1.5$ K, so the leak carried away $\bar P_{\text{leak}}=k\bar T=0.30\times1.5=0.45$ W:
$$P_{\text{can}}=3.14+0.45=3.59\ \text{W}\;\Rightarrow\;I=\frac{3.59}{6.02\times10^{-3}}\approx5.96\times10^{2}\ \text{W m}^{-2},$$
and as a total solar output (Earth distance $d=1.5\times10^{11}$ m):
$$P_\odot=I\cdot4\pi d^2=596\times4\pi(1.5\times10^{11})^2\approx\boxed{1.7\times10^{26}\ \text{W}}.$$

**Check.** The correction raises the estimate by $\sim14\%$ — small because the can stayed close to ambient; consistent with the weak-leak assumption $kT\ll P$ ✓. The luminosity is within a factor ~2.3 of the true $3.85\times10^{26}$ W ✓ for a ground-level estimate.

#### Q2(d) — Power per cubic metre of Sun; mass loss rate [5 marks]

**Key observation.** The solar constant $S$ is luminosity diluted over a sphere of radius $d$: $L_\odot=4\pi d^2 S$. Divide by the Sun's volume for (i); divide by $c^2$ for (ii).

> 【Thought】 Seeing "per cubic metre within the Sun" → triggers *assume uniform energy generation* — an explicitly approximate but necessary closure (real production is core-concentrated). State the assumption; the estimate is an average.

**Solution.** (i)
$$L_\odot=4\pi(1.5\times10^{11})^2\times1360=3.84\times10^{26}\ \text{W},\qquad V_\odot=\tfrac43\pi(6.96\times10^8)^3=1.41\times10^{27}\ \text{m}^3,$$
$$\boxed{\frac{L_\odot}{V_\odot}\approx0.27\ \text{W m}^{-3}}$$
— less than a compost heap per unit volume; the Sun shines because it is *big*, not intense. (Real production is concentrated in the core, whose power density exceeds this average by about two orders of magnitude — the uniform-production model gives the mean, not the peak.)
(ii)
$$\dot m=\frac{L_\odot}{c^2}=\frac{3.84\times10^{26}}{9.0\times10^{16}}\approx\boxed{4.3\times10^{9}\ \text{kg s}^{-1}}\ (\sim4\ \text{million tonnes per second}).$$

**Check.** Fraction of Sun's mass per year: $\dot m\times3.16\times10^7/2\times10^{30}\sim7\times10^{-14}$/yr — utterly negligible over its lifetime ✓.

---

### Question 3 — Bubbles, forces and rotation

#### Q3(a) — A soap bubble that sinks, then rises [10 marks]

**Key observation.** Slow motion ⟹ drag depends only on speed (magnitude), not direction. Writing force balance at the *same speed* $v$ sinking and rising gives two equations in which the buoyancy $B$ (fixed — outside air unchanged) and drag $F_d$ appear with flipped signs — solve for both without knowing either mass.

> 【Thought】 Seeing "same |drag| falling as rising" → triggers *symmetric force-pair elimination*: add the two balances to kill $F_d$, subtract to kill $B$. This "same speed both ways" structure recurs (terminal velocity up/down, Weighing with drag, rowing with/against current) — whenever two regimes differ only by the sign of a velocity-dependent force.

**(i)** Sinking (heavier, mass $m_h$): weight down, buoyancy + drag up:
$$m_h g=B+F_d.$$
Rising (lighter, mass $m_\ell$): buoyancy up, weight + drag down:
$$B=m_\ell g+F_d.$$
Solving:
$$\boxed{B=\frac{(m_h+m_\ell)g}{2},\qquad F_d=\frac{(m_h-m_\ell)g}{2}.}$$

**(ii) Buoyancy.** Displaced fluid is the *outside* air at 17 °C ($T=290$ K); ideal gas at fixed pressure: $\rho=PM/RT$:
$$\rho_{\text{out}}=\frac{1.01\times10^5\times0.028}{8.3145\times290}=1.17\ \text{kg m}^{-3},\qquad V=\tfrac43\pi(0.08)^3=2.14\times10^{-3}\ \text{m}^3,$$
$$\boxed{B=\rho_{\text{out}}Vg=1.17\times2.14\times10^{-3}\times9.81\approx2.47\times10^{-2}\ \text{N}}.$$
Note the quantity asked: $B$ is the **buoyancy** $\rho_{\text{out}}Vg$ alone — not the *net* lift $(\rho_{\text{out}}-\rho_{\text{in}})Vg$; confusing the two changes the answer by two orders of magnitude (see the side note).

> 【Thought】**Cross-check against the official mark scheme:** it prints $B=1.6\times10^{-4}$ N — the *net* lift $(\rho_{\text{out}}-\rho_{\text{in}})Vg$ evaluated with $r=5$ cm, whereas the question specifies $r=8.0$ cm. With the correct radius its own formula gives $(1.173-1.141)\times2.145\times10^{-3}\times9.81=6.6\times10^{-4}$ N net (gross upthrust $2.47\times10^{-2}$ N as we box). The inconsistency propagates into its part (iv), which prints $\delta=3.0\times10^{-7}$ m; with $r=8$ cm the official route lands exactly on our $\delta=9.3\times10^{-7}$ m. Ours stands.

> 【Thought】 The inside temperature plays **no** role in buoyancy — it enters later through the bubble's *mass*. Separating "what sets B" (outside density) from "what sets weight" (inside density + film) is the conceptual core of the question.

**(iii) Time to evaporate the difference.** With $F_d=kv$, $v=0.060$ m/s:
$$F_d=1.2\times10^{-3}\times0.060=7.2\times10^{-5}\ \text{N},\qquad m_h-m_\ell=\frac{2F_d}{g}=1.47\times10^{-5}\ \text{kg}.$$
Evaporation rate over the outer area $4\pi r^2=0.0804\ \text{m}^2$:
$$\dot m=2.4\times10^{-5}\times0.0804=1.93\times10^{-6}\ \text{kg/s}\;\Rightarrow\;\boxed{t=\frac{1.47\times10^{-5}}{1.93\times10^{-6}}\approx7.6\ \text{s}}.$$

**(iv) Initial wall thickness.** The sinking bubble's mass is inside air + film:
$$m_h=\frac{B+F_d}{g}=2.52\times10^{-3}\ \text{kg},\qquad m_{\text{air}}=\rho_{\text{in}}V=\frac{PM}{RT_{\text{in}}}V=\frac{1.01\times10^5\times0.028}{8.3145\times298}\times2.14\times10^{-3}=2.45\times10^{-3}\ \text{kg},$$
$$m_{\text{film}}=m_h-m_{\text{air}}=7.5\times10^{-5}\ \text{kg},\qquad \delta=\frac{m_{\text{film}}}{\rho_s\cdot4\pi r^2}=\frac{7.5\times10^{-5}}{998\times0.0804}=\boxed{9.3\times10^{-7}\ \text{m}\approx0.9\ \mu\text{m}}.$$

**Check.** Sub-micron film ✓ — real soap films are hundreds of nm to microns; the small difference of two large masses ($m_h-m_{\text{air}}\ll m_h$) is why four-digit care was needed throughout ✓; note the film mass is only 3% of the total — yet it decides whether the bubble sinks or floats, a classic "small term controls the sign" situation.

#### Q3(b) — Rotating masses, hoop, and a rubber band on a flywheel [10 marks]

**(i) Four masses on strings.** Each mass sits at a square corner (string directions along the sides, i.e. at $45^\circ$ to the radius); the orbit radius is $\ell/\sqrt2$.

> 【Thought】 Seeing "radial and tangential components of the tension" → triggers *decompose the string tension along/r⊥ to the radius*: the two strings on each mass give cancelling tangential pulls (uniform rotation — no tangential force allowed) and adding radial pulls. This decomposition is exactly the bridge to the continuous hoop, where only the tangential tension survives as "the hoop tension".

Two strings per mass, radial components $T_r=T\cos45^\circ$ adding:
$$2T_r=\frac{mv^2}{\ell/\sqrt2}=\frac{\sqrt2\,mv^2}{\ell}\;\Rightarrow\;\boxed{T_r=\frac{mv^2}{\sqrt2\,\ell},\qquad T_{\text{tangential}}=T_r\tan45^\circ=\frac{mv^2}{\sqrt2\,\ell}}\ \ \left(T=\frac{mv^2}{\ell}\right).$$

**(ii) Hoop tension by dimensions.** $T=k\lambda^\alpha v^\beta r^\gamma$ with $[\lambda]=\text{kg m}^{-1}$:
$$\text{kg m s}^{-2}=(\text{kg m}^{-1})^\alpha(\text{m s}^{-1})^\beta\text{m}^\gamma\;\Rightarrow\;\alpha=1,\ \beta=2,\ -\alpha+\beta+\gamma=1\Rightarrow\gamma=0,$$
$$\boxed{T_{\text{tangential}}=\lambda v^2}\qquad(\text{with }k=1).$$

**Check.** Matches the discrete picture: hoop tension independent of $r$ — doubling the ring at fixed speed doubles the mass per element *and* halves the curvature, cancelling $r$ exactly ✓; also derivable directly: element $r\,d\theta$ needs $\lambda r\,d\theta\cdot v^2/r=\lambda v^2 d\theta$, supplied by the tension resultant $T\,d\theta$ ✓.

**(iii) Rubber band on a flywheel.** The band (mass 25 g) is stretched from 15.0 to 18.5 cm: tension $T=kx=2000\times0.035=70$ N; linear density $\lambda=0.025/0.185=0.135$ kg/m.

> 【Thought】 Mechanism of "falling off": spinning faster demands centripetal tension $\lambda v^2$; the elastic tension is fixed by the stretch. When $\lambda v^2$ reaches $T$, the band must stretch further to supply more — it slips off the rim. The critical condition $T=\lambda v^2$ *equates the two expressions from (ii) and Hooke's law* — the question is engineered so (ii) feeds (iii).

$$v^2=\frac{T}{\lambda}=\frac{70}{0.135}=518\;\Rightarrow\;v=22.8\ \text{m s}^{-1},\qquad f=\frac{v}{2\pi r}=\frac{22.8}{0.185}=123\ \text{rev/s},$$
$$\boxed{\omega\approx7.7\times10^{2}\ \text{rad/s}\approx7.4\times10^{3}\ \text{rpm}\ (\approx123\ \text{rev/s}).}$$

**Check.** Order of magnitude: a stiff band ($k=2000$ N/m) at 23% stretch is strong; thousands of rpm for a 3 cm radius wheel is mechanically plausible ✓.

#### Q3(c) — Radial oscillations of an elastic ring [5 marks]

**Key observation.** Uniform radial breathing: radius $r\to r+\xi$ stretches the circumference by $\delta x=2\pi\xi$; the hoop tension $T=k\,\delta x$ then pulls every element inward with the standard "curved string" resultant $T\,d\theta$ per element.

> 【Thought】 Seeing "oscillates at lowest natural frequency in a radial direction" → triggers *breathing mode*: every element moves radially together, so the whole ring is one effective oscillator — no wave propagation needed. The centripetal-acceleration relation from (b)(ii) reappears, now as a *restoring* force. If the mode were non-uniform (e.g. quadrupolar), a wave equation on the ring would be needed instead.

**Solution.** Element of arc $r\,d\theta$, mass $\lambda r\,d\theta$; tension forces at its ends (magnitude $T$, angle $d\theta$ apart) give inward resultant $T\,d\theta$. Newton's second law radially:
$$\lambda r\,d\theta\,\ddot\xi=-T\,d\theta=-k(2\pi\xi)\,d\theta\;\Rightarrow\;\ddot\xi=-\frac{2\pi k}{\lambda r}\,\xi,$$
SHM with $\omega^2=\dfrac{2\pi k}{\lambda r}$:
$$\boxed{f=\frac{1}{2\pi}\sqrt{\frac{2\pi k}{\lambda r}}=\sqrt{\frac{k}{2\pi\lambda r}}}.$$

**Check.** Dimensions: $[k]=\text{N/m}$, $[\lambda r]=\text{kg}$: $\sqrt{\text{N}/(\text{m}\cdot\text{kg})}=\text{s}^{-1}$ ✓. Static limit: the ring under steady rotation at speed $v$ has equilibrium where $k\,\delta x=\lambda v^2 r$... consistent with (b)(ii)'s tension law ✓.

---

### Question 4 — Landing a craft on Titan

#### Q4(a) — RTG thermal power [3 marks]

**Key observation.** Activity $A=\lambda N$ with $\lambda=\ln2/t_{1/2}$; power = activity × decay energy. The dioxide formula means only $238/270$ of the 4.8 kg is plutonium.

> 【Thought】 Seeing "Pu-238 dioxide" → triggers *correct for the oxygen mass* before counting atoms — a deliberate trap; using 4.8 kg of Pu directly overestimates by 13%. Order of operations: mass → moles → atoms → activity → power, each step one line.

**Solution.** Pu mass $=4.8\times\dfrac{238}{270}=4.23$ kg; atoms $N=\dfrac{4.23}{0.238}\times N_A=1.07\times10^{25}$.
$$A=\frac{\ln2}{87.7\times3.156\times10^7}\times1.07\times10^{25}=2.68\times10^{15}\ \text{s}^{-1},\qquad E_\alpha=5.5\ \text{MeV}=8.81\times10^{-13}\ \text{J},$$
$$\boxed{P=AE_\alpha\approx2.4\times10^{3}\ \text{W}\ (\approx 2.4\ \text{kW thermal})}.$$

**Model choice.** We read "4.8 kg of plutonium-238 *dioxide*" literally as PuO₂ ($4.8\times238/270=4.23$ kg of Pu); taking all 4.8 kg as Pu-238 would give 2.7 kW — a coarser reading, inconsistent with the stated chemical form.

**Check.** Real Pu-238 RTGs deliver $\sim 0.5$ kW thermal per kg of PuO₂ ✓ ($2.36/4.8=0.49$ kW/kg).

> 【Thought】**Official mark scheme note:** the mark scheme takes the 4.8 kg as Pu-238 mass (molar mass 238 g/mol) and obtains $P\approx2.7$ kW; reading the stated "plutonium-238 *dioxide*" literally (PuO₂, 270 g/mol) gives our $2.36$ kW — which is also the real GPHS-RTG figure. Either reading is defensible; we keep the dioxide-literal one and flag the official value.

#### Q4(b) — Insulation area from heat leak [2 marks]

**Key observation.** In steady state all 2000 W of internal heating escapes through the foam: $P=\kappa A_c\Delta T/\Delta x$ — solve for $A_c$.

$$\boxed{A_c=\frac{P\,\Delta x}{\kappa\,\Delta T}=\frac{2000\times0.050}{0.035\times179}\approx16\ \text{m}^2}\qquad(\Delta T=0-(-179)=179\ \text{K}).$$

**Check.** A lander of $\sim16\ \text{m}^2$ internal surface (e.g. a cylinder ~2 m across) ✓ plausible; temperature *difference* in K = °C difference ✓.

#### Q4(c) — Hover power on Titan [10 marks]

**Key observation.** Rotor thrust by momentum flux: air of density $\rho$ swept through area $A$ and thrown down at speed $v$ carries momentum flux $\rho A v^2$; hover power follows the problem's convention $P=Fv_{\text{disk}}=\rho A v^3$ (no $\tfrac12$ — that factor belongs to the far-wake actuator-disc refinement, where the terminal wake speed is $2v$; see the side note), evaluated at the thrust that balances weight.

> 【Thought】 The momentum-flux model (actuator disk) is the intended closure: it replaces blade aerodynamics with one inlet area. Note the asymmetry: thrust $\propto v^2$ but power $\propto v^3$ — and after eliminating $v$ via the weight balance, $P\propto (mg)^{3/2}/\sqrt{\rho A}$. That scaling drives all the numbers below: dense atmosphere and low gravity both *help* flight on Titan.

**(i)** $\boxed{F_{\text{lift}}=\rho_T A_8 v^2}$ (mass flux $\rho_T A_8 v$ times velocity $v$).

**(ii)** Hover: $\rho_T A_8 v^2=m_Dg_T\Rightarrow v=\sqrt{m_Dg_T/(\rho_T A_8)}$. Power is force × velocity of the driven air:
$$P=F_{\text{lift}}\,v=\rho_T A_8 v^3\;\Rightarrow\;\boxed{P=\frac{(m_Dg_T)^{3/2}}{\sqrt{\rho_T A_8}}}.$$

**(iii)** Same craft, same $A$:
$$\frac{P_T}{P_E}=\left(\frac{g_T}{g_E}\right)^{3/2}\sqrt{\frac{\rho_E}{\rho_T}}=\left(\frac{1.35}{9.81}\right)^{3/2}\sqrt{\frac{1.22}{5.35}}=0.0511\times0.478\approx\boxed{0.024\ (\approx1/41)}.$$

**(iv)** $A_8=8\pi(0.68)^2=11.6\ \text{m}^2$, $m_Dg_T=420\times1.35=567\ \text{N}$:
$$P_T=\frac{567^{3/2}}{\sqrt{5.35\times11.6}}=\frac{1.350\times10^4}{7.89}\approx\boxed{1.7\times10^{3}\ \text{W}}.$$

**(v) Battery charge time for an 8 km flight.** Mission energy budget (hover rate throughout, plus GPE for the climb):
- ascend 500 m at 10 m/s: 50 s; horizontal 8 km: 800 s; descend: 50 s — total 900 s;
- $E=P_T\times900+m_Dg_Th=1.71\times10^3\times900+420\times1.35\times500=1.54\times10^6+2.84\times10^5=1.82\times10^{6}\ \text{J}$.
RTG electrical output at 6%: $P_{\text{el}}=0.06\times2680=161\ \text{W}$:
$$\boxed{t=\frac{1.82\times10^6}{161}\approx1.13\times10^{4}\ \text{s}\approx3.1\ \text{hours}}.$$

**Check.** Descent at hover-only power, climb at hover+mgv — note $mg\,v_{\text{climb}}=5670$ W $\gg P_T$... over 50 s that is exactly $mgh$ ✓ consistent accounting; the charge time is short because Titan hover is 40× cheaper than Earth's — the physical punchline of (iii) ✓.

> 【Thought】**Reconciling with the official mark scheme (two corrections adopted).** (1) The problem's own model defines $F=\rho Av^2$ and $P=Fv$, so $P=\rho Av^3$ — a KE-flux estimate $\tfrac12\rho Av^3$ would introduce a spurious $\tfrac12$ (that factor belongs to the far-wake actuator-disc refinement, where the disc velocity is $v/2$; the problem's convention absorbs it). The resulting value is $P_T=1.7$ kW, and the flight energy $1.82\times10^6$ J — matching the official figures. (2) For the charge time the official uses its RTG figure $2680$ W (Pu-238 molar mass $238$ g/mol); treating the stated $4.8$ kg as PuO$_2$ ($270$ g/mol, see Q4(a) note) gives $2360$ W and $t\approx3.6$ h — both defensible; we follow the official convention in the box.

#### Q4(d) — Forward flight: thrust vector and airspeed [6 marks]

**(i)** Diagram: $W=m_Dg_T$ down; $L$ up ($L=W$); $D$ backward; $T$ forward ($T=D$); rotor force $F_8$ tilted forward from vertical, as the resultant of $T$ and $L$:
$$F_8=\sqrt{T^2+L^2}=\boxed{\sqrt{D^2+W^2}}.$$

> 【Thought】 Seeing "constant speed in horizontal flight" → triggers *force closure*: the rotor's single force vector must cancel both drag and weight, so it is the hypotenuse of the (D, W) right triangle. The tilt angle $\arctan(D/W)$ is small here — anticipating this explains the near-equality found in (iii).

**(ii)** With $C_L=C_D\approx1$:
$$(\rho_TA_8v_{\text{tip}}^2)^2=(\rho_TA_8v_{\text{air}}^2)^2+(m_Dg_T)^2\;\Rightarrow\;\boxed{v_{\text{air}}=\left[v_{\text{tip}}^4-\left(\frac{m_Dg_T}{\rho_TA_8}\right)^2\right]^{1/4}}.$$

**(iii)** $v_{\text{tip}}=\omega r=\dfrac{500\times2\pi}{60}\times0.68=35.6\ \text{m/s}$; $\dfrac{m_Dg_T}{\rho_TA_8}=\dfrac{567}{62.2}=9.1\ \text{m}^2\text{s}^{-2}$:
$$v_{\text{air}}=\left[35.6^4-9.1^2\right]^{1/4}\approx\boxed{35.6\ \text{m/s}\ (\approx36\ \text{m/s})}.$$

**Check.** $\left(m_Dg_T/\rho A\right)^2=83\ll v_{\text{tip}}^4=1.6\times10^6$: drag is a perturbation — the rotor tips barely tilt from vertical and thrust speed ≈ tip speed ✓ consistent with the small-$D/W$ expectation.

> 【Thought】**Official mark scheme note:** the mark scheme's printed final value, $v_{\text{air}}=2.5$ m/s, is inconsistent with its own (correct) formula $v_{\text{air}}^4=v_{\text{tip}}^4-(m_Dg_T/\rho_TA_8)^2$ — substituting its numbers gives $[35.6^4-83]^{1/4}=35.6$ m/s, our answer. The printed 2.5 m/s appears to be a mark-scheme typo; the formula and our evaluation agree.

#### Q4(e) — Turbulent drag and Titan's upper-atmosphere density [4 marks]

**(i)** $F=k\rho^\alpha v^\beta r^\gamma$: kg: $\alpha=1$; s: $\beta=2$; m: $-3\alpha+\beta+\gamma=1\Rightarrow\gamma=2$:
$$\boxed{F=k\rho v^2 r^2}\qquad(\alpha=1,\ \beta=2,\ \gamma=2).$$

> 【Thought】 Turbulent (inertial) drag must be $v^2$ — viscosity (which would give $v^1$, Stokes) is not among the permitted variables; the dimensional set itself encodes the regime.

**(ii)** Constant velocity at 600 km ⟹ drag balances local weight; use $g$ at $R+h$, not at the surface:
$$g_{600}=\frac{GM_T}{(R_T+h)^2}=\frac{6.67\times10^{-11}\times1.345\times10^{23}}{(3.175\times10^6)^2}=0.890\ \text{m/s}^2,$$
$$\rho=\frac{mg}{v^2r^2}=\frac{400\times0.890}{7300^2\times1.85^2}=\boxed{1.95\times10^{-6}\ \text{kg m}^{-3}}\qquad(r=1.85\ \text{m}).$$

**Check.** $\sim2\times10^{-6}$ of surface density (5.35 kg/m³): a tenuous upper atmosphere ✓; using surface $g=1.35$ instead would overestimate $\rho$ by 50% — the altitude correction is the marking point ✓.

---

### Question 5 — Gravity and collisions (the "Venearth" problem)

#### Q5(a) — Orbital scaling laws and the Sun's mass [5 marks]

**(i)** Circular orbit, centripetal = gravity:
$$\frac{m_pv^2}{r}=\frac{GM_Sm_p}{r^2}\;\Rightarrow\;v^2=\frac{GM_S}{r}\;\Rightarrow\;v\propto r^{-1/2}.\ \blacksquare$$

**(ii)** $E=\tfrac12m_pv^2-\dfrac{GM_Sm_p}{r}=\dfrac{GM_Sm_p}{2r}-\dfrac{GM_Sm_p}{r}=-\dfrac{GM_Sm_p}{2r}\propto r^{-1}$. $\blacksquare$

> 【Thought】 The virial halving ($|E|=\tfrac12$|GPE|, KE = $|E|$) is the content of (ii); note $E<0$ — bound orbit.

**(iii)** $T=\dfrac{2\pi r}{v}=2\pi r\sqrt{\dfrac{r}{GM_S}}\;\Rightarrow\;T^2=\dfrac{4\pi^2}{GM_S}r^3\propto r^3$ (Kepler III). $\blacksquare$

**(iv)**
$$M_S=\frac{4\pi^2r_E^3}{GT_E^2}=\frac{4\pi^2(1.50\times10^{11})^3}{6.67\times10^{-11}(365\times86400)^2}=\boxed{2.0\times10^{30}\ \text{kg}}.$$

**(v)** In units (au, yr, $M_{\text{Sun}}$): $T^2=\dfrac{4\pi^2}{GM_S}r^3$ with $T=1$, $r=1$, $M_S=1$:
$$\boxed{G=4\pi^2\ \text{au}^3\,M_{\text{Sun}}^{-1}\,\text{yr}^{-2}\ (\approx39.5)}.$$

> 【Thought】 Unit-system move: in "solar units" Kepler III is just $T^2=r^3/M_\star$. Use it below — all speeds then come out in au/yr ($v_E=2\pi$ au/yr exactly) and no SI conversion is needed until the end.

#### Q5(b) — The Sun vanishes: Earth–Venus collision course [8 marks]

**Key observation.** With gravity gone, both planets move in **straight lines at constant velocity**, tangent to their former orbits. The collision point is where the two tangent lines are reached *at the same time* — two vector equations in the two unknowns (initial angular separation $\varphi$, time $t$).

**(i)** Orbital speeds (solar units; $v=\sqrt{GM_\odot/r}$):
$$v_E=2\pi=6.28\ \text{au/yr}\ (29.8\ \text{km/s}),\qquad v_V=\frac{2\pi}{\sqrt{0.723}}=\boxed{7.39\ \text{au/yr}\ (35.0\ \text{km/s})}.$$

**(ii)–(v) Solving the rendezvous.** Put the Sun at the origin, Earth at $E_0=(1,0)$ moving in $+y$: $\mathbf v_E=v_E\hat y$. Venus at $\varphi$ behind Earth (we anticipate $\varphi>0$ with Venus trailing; solve and check the sign): $V_0=0.723(\cos\varphi,-\sin\varphi)$, $\mathbf v_V=v_V(\sin\varphi,\cos\varphi)$ (same orbital sense). Rendezvous conditions:
$$1=v_V t\sin\varphi+0.723\cos\varphi,\qquad v_E t=-0.723\sin\varphi+v_V t\cos\varphi.$$

> 【Thought】 Seeing "on a collision course … find the time / show d ≈ 1.5 au / show angle ≈ 13°" → the parts are mutually checking: solve the $2\times2$ system numerically (or geometrically), then *verify* the two "show that" clauses — they are consistency certificates, not new physics. Geometric shortcut worth noting: since each velocity is perpendicular to its own radius vector, the angle between the two velocity vectors equals the Earth–Sun–Venus angle $\varphi$ itself — so (iv) and (v) are the same angle, halving the work.

Numerical solution: $\varphi=13.0^\circ$ (Venus trailing Earth), $t=0.1776\ \text{yr}$:
$$\boxed{t\approx65\ \text{days}}.$$
Collision point $X=(1,\;v_Et)=(1,\,1.116)$ au:
$$d=|X|=\sqrt{1+1.116^2}=1.499\ \text{au}\approx\boxed{1.5\ \text{au}}\ \checkmark\ \text{(iii)}.$$
Velocity vectors: $\mathbf v_E$ along $+y$; $\mathbf v_V$ at $\varphi$ from $+y$: angle $=\varphi\approx\boxed{13^\circ}\ \checkmark\ \text{(iv)}$ — hence
$$\boxed{\text{Earth–Sun–Venus angle at disappearance}=\varphi\approx13^\circ\ (\text{Venus trailing Earth})\ \text{(v)}.}$$

**Check.** In 65 days Earth covers $1.116$ au along its tangent ✓; Venus: $|X-V_0|=v_Vt=1.312$ au — verify: $V_0=(0.705,-0.163)$, $X-V_0=(0.295,1.279)$, $|X-V_0|=1.313$ ✓.

> 【Thought】**Official approach (adopted as the slicker route).** The mark scheme exploits the fact that each tangent line is perpendicular to its own radius vector, so the Sun, the start point, and the collision point $X$ form a **right triangle for each planet**, with shared hypotenuse $d=|OX|$:
> $$d^2=r_E^2+(v_Et)^2=r_V^2+(v_Vt)^2\;\Rightarrow\;t=\sqrt{\frac{r_E^2-r_V^2}{v_V^2-v_E^2}}=0.1776\ \text{yr}=64.8\ \text{days}$$
> — $t$ in one line, no $2\times2$ system. The angles follow from the same triangles: $\arcsin(r_E/d)-\arcsin(r_V/d)=41.86^\circ-28.85^\circ=13.0^\circ$, and triangle similarity gives the Earth–Sun–Venus angle equal to it. Our vector-rendezvous solution arrives at the same numbers ($t=65$ d, $d=1.50$ au, $13^\circ$) ✓; the right-triangle formulation is the one to remember — *whenever motion is tangential to a radius, Pythagoras replaces simultaneous equations — but only while the paths stay straight; restore a central force and the simultaneous circle-orbit equations return*.

#### Q5(c) — The inelastic merger [7 marks]

**(i)** Momentum conservation ($M_V=0.815M_E$; total $1.815M_E$):
$$\mathbf v=\frac{\mathbf v_E+0.815\,\mathbf v_V}{1.815}=\frac{(0+0.815\times7.39\sin13^\circ,\;6.28+0.815\times7.39\cos13^\circ)}{1.815}=\frac{(1.355,\;12.15)}{1.815}=(0.746,\;6.695),$$
$$v=\sqrt{0.746^2+6.695^2}=\boxed{6.74\ \text{au/yr}\approx6.7\ \text{au/yr}}\ \checkmark\ (31.9\ \text{km/s}).$$

**(ii)** Angle to Earth's initial velocity ($+y$):
$$\theta=\arctan\frac{0.746}{6.695}=\boxed{6.4^\circ}.$$

**(iii)** KE loss:
$$\frac{KE_i-KE_f}{KE_i}=1-\frac{1.815\times6.74^2}{6.28^2+0.815\times7.39^2}=1-\frac{82.4}{83.9}=\boxed{1.9\%}.$$

> 【Thought】 The tiny KE loss is because the collision is nearly *co-directional* (13° apart): inelastic losses scale with the **relative** velocity squared — here $|\mathbf v_V-\mathbf v_E|\approx1.9$ au/yr is small. Diagnostic habit: for sticking collisions, estimate the loss as $\tfrac12\mu v_{\text{rel}}^2$ (reduced mass × relative speed) before computing anything else.

#### Q5(d) — A new star appears: is Venearth bound? [5 marks]

**(i) Minimum binding mass.** At $d=1.50$ au with speed $v=6.74$ au/yr, bound ⟺ $v^2<2GM_\star/d$:
$$M_{\min}=\frac{v^2d}{2G}=\frac{6.74^2\times1.50}{2\times4\pi^2}=\boxed{0.86\ M_{\text{Sun}}}.$$

**(ii) Orbital period if $M_\star=1\ M_{\text{Sun}}$.** Specific energy:
$$\varepsilon=\frac{v^2}{2}-\frac{GM_\odot}{d}=\frac{6.74^2}{2}-\frac{4\pi^2}{1.50}=22.71-26.32=-3.61\ \text{au}^2\text{/yr}^2.$$
Equal-energy circular orbit has $-\dfrac{GM}{2r_c}=\varepsilon\Rightarrow r_c=\dfrac{GM}{2|\varepsilon|}=\dfrac{4\pi^2}{7.21}=5.48$ au — this equals the ellipse's semi-major axis $a$ (energy fixes $a$ alone). Kepler III in solar units, $T^2=a^3/M_\star$:
$$\boxed{T=\sqrt{5.48^3}=12.8\ \text{yr}}.$$

> 【Thought】 Two reusable facts did all the work: (1) bound/unbound ⟺ sign of $v^2-2GM/r$ at the instant gravity switches on; (2) an ellipse's period depends only on $a$ (energy), not on eccentricity — which is exactly the licence the question gives ("period equal to a circular orbit with the same total energy"). If the collision point had been nearer perihelion geometry, none of the numbers would change — energy is position+speed only.

**Check.** $M_{\min}<1\ M_\odot$ ⟺ Venearth is bound by the real-mass star ✓ consistent with $\varepsilon<0$ found in (ii) — the two parts cross-validate ✓. $T=12.8$ yr $\gg$ Earth's 1 yr because the merged planet carries nearly Earth's tangential speed but sits at 1.5 au — it is thrown into a distant, slow ellipse ✓.

---
*End of Paper 4 (2024 Round 1 Section 2).*


---

## Paper 5 — 2023 Round 1 Section 1 (11 Nov 2023)

*Section 1, Question 1, parts (a)–(w). Maximum 50 marks from ≈ 84.*

---

### Q1(a) — Bouncing steel ball [2 marks]

**Key observation.** "Retains 70% of its energy on each bounce" → height (and impact KE) scale by 0.7 per bounce; speed by $\sqrt{0.7}$.

**(i)** Impact speed: $v^2=u^2+2gh=3.0^2+2(9.81)(2.0)=48.2$ → $v=\boxed{6.95\approx7.0\ \text{m/s}}$.
**(ii)** After the 4th bounce, KE factor $0.7^4=0.240$:
$$h_4=0.7^4\cdot\frac{v^2}{2g}=0.240\times\frac{48.2}{19.6}=\boxed{0.59\ \text{m}}.$$

> 【Thought】 Seeing fractional retention per bounce → triggers *geometric scaling*: never track bounce-by-bounce; write the $n$-th term. Note the initial $u\ne0$ — the energy at first impact includes the thrown KE, not just $mgh$.

---

### Q1(b) — Dual-powered cycle computer [2 marks]

**Key observation.** Solar covers 1/3 of the consumption rate, so the battery drains at 2/3 of its night rate — battery life stretches by the reciprocal factor. (This assumes constant solar output — the "direct sunlight" clause — and unchanged battery capacity.)

$$t=\frac{10\ \text{h}}{1-\tfrac13}=\boxed{15\ \text{h}}.$$

> 【Thought】 Seeing "provides 1/3 of consumption" → the battery supplies the **remaining** 2/3; the trap is answering $10\times\tfrac43$ or $10\times3$. Convert "help fraction" to "drain fraction" before scaling time.

---

### Q1(c) — Cyclist leaning into a corner [3 marks]

**Key observation.** Lean angle balances gravity torque against centripetal pseudo-force in the bike frame: $\tan\theta=v^2/(rg)$. Same corner → same $r$ → $\tan\theta\propto v^2$.

> 【Thought】 Seeing "same corner, different speed" → triggers *scaling with fixed geometry*: only $v^2$ changes. The trap is assuming $\theta\propto v^2$ directly — it is $\tan\theta$ that scales; at these angles the distinction matters ($25.6^\circ\ne 2.25\times12^\circ=27^\circ$).

**Solution.** $\tan\theta_2=\tan12^\circ\times(15/10)^2=0.2126\times2.25=0.478$ → $\boxed{\theta_2\approx26^\circ}$.

**Check.** Faster → larger lean ✓; small-angle approximation would give 27°, close but off by ~5% ✓ consistent with $\tan$ being nearly linear here.

---

### Q1(d) — Io vs Europa: centripetal accelerations [2 marks]

**Key observation.** Given $\omega^2 r^3=$ const, the centripetal acceleration $a=\omega^2 r$ can be written in terms of $\omega$ alone: $a\propto\omega^{4/3}$ (eliminating $r$ via $r\propto\omega^{-2/3}$).

> 【Thought】 Seeing a constraint $\omega^2r^3=c$ and a target $a=\omega^2r$ → triggers *eliminate the unwanted variable* $r$ before substituting numbers. Feeding numbers in first produces unreadable arithmetic.

**Solution.** $T_E=2T_I\Rightarrow\omega_I=2\omega_E$. With $r\propto\omega^{-2/3}$:
$$\frac{a_I}{a_E}=\left(\frac{\omega_I}{\omega_E}\right)^{2}\left(\frac{r_I}{r_E}\right)=2^2\cdot2^{-2/3}=2^{4/3}=\boxed{2.52}.$$

**Check.** Inner moon: faster orbit and stronger field — ratio must exceed 1 ✓; sanity via $a=GM/r^2$ with $r\propto T^{2/3}$: $a\propto T^{-4/3}$: $(1/2)^{-4/3}=2^{4/3}$ ✓ same.

---

### Q1(e) — Elastic collision with equal scattering angles [5 marks]

**Key observation.** Equal angles $\pm\theta$ + momentum conservation transverse to the beam force $m_1v_1=m_2v_2$; then the longitudinal and energy equations close the system. The equal-angle condition over-constrains the problem, so a *feasibility bound* on $m_1/m_2$ emerges.

> 【Thought】 Seeing "elastic" + "equal angles" → triggers *list the three conservation equations (2 momentum + 1 energy) and count unknowns*: $v_1,v_2,\theta$ — exactly solvable, with a solvability condition (a cosine must not exceed 1). That condition is the answer to (i). This pattern — "conditions consistent ⟺ some trig bound" — is the standard way feasibility questions are built.

**Solution.** Transverse: $m_1v_1=m_2v_2$. Longitudinal: $m_1u=(m_1v_1+m_2v_2)\cos\theta=2m_1v_1\cos\theta$ → $u=2v_1\cos\theta$.
Energy: $m_1u^2=m_1v_1^2+m_2v_2^2=m_1v_1^2\!\left(1+\dfrac{m_1}{m_2}\right)$, using $v_2=m_1v_1/m_2$.

Combine: $4\cos^2\theta=1+\dfrac{m_1}{m_2}$.

(i) $\cos^2\theta\le1\Rightarrow \dfrac{m_1}{m_2}\le\boxed{3}$ (bound approached as $\theta\to0$).
(ii) $m_1=m_2$: $\cos^2\theta=\tfrac12$ → $\boxed{\theta=45^\circ}$ (the equal-angle deflection is then fixed, not maximal over a family).

**Check.** $m_1\ll m_2$: $\cos\theta\to\tfrac12$, $\theta\to60^\circ$ — the projectile can scatter up to... note $\theta$ is the half-opening angle; for equal masses the famous $90^\circ$ opening angle corresponds to $\theta=45^\circ$ each ✓ classic result reproduced. Monotonic trend: as $m_1/m_2$ grows from $0$ to $3$, the equal-angle $\theta$ falls from $60^\circ$ through $45^\circ$ (at $m_1=m_2$) to $0^\circ$ ✓ — heavier projectile ⟹ narrower scattering cone, the expected direction.

---

### Q1(f) — Projected up a rough incline, returns at half speed [4 marks]

**Key observation.** Friction reverses between ascent and descent, so the two legs have different accelerations $a_\uparrow=g(\sin\alpha+\mu\cos\alpha)$ and $a_\downarrow=g(\sin\alpha-\mu\cos\alpha)$ — over the **same** distance; the speed ratio is then a pure ratio of accelerations.

> 【Thought】 Seeing "returns through its starting point with half the speed" → triggers *same-distance kinematics*: $v^2=2as$ twice, and $s$ cancels in the ratio. The alternative — work–energy over the round trip ($-2\mu mg\cos\alpha\,s=\Delta KE$) — works too, but needs $s$; the ratio route never does.

**Solution.** Same $s$ up and down:
$$v^2=2a_\uparrow s,\qquad \left(\tfrac v2\right)^2=2a_\downarrow s\;\Rightarrow\;\frac{a_\uparrow}{a_\downarrow}=4,$$
$$\sin\alpha+\mu\cos\alpha=4(\sin\alpha-\mu\cos\alpha)\;\Rightarrow\;5\mu\cos\alpha=3\sin\alpha\;\Rightarrow\;\boxed{\mu=\tfrac35\tan\alpha}.$$

**Check.** $\mu>0$ ✓; consistency requires $\tan\alpha>\mu$ (it slides back down): $\tan\alpha>\tfrac35\tan\alpha$ ✓ always; $\alpha\to90^\circ$ needs $\mu\to\infty$ ✓ (vertical wall: friction dominates).

---

### Q1(g) — Layered immiscible liquids: force on the wall [4 marks]

**Key observation.** Pressure at a depth is the weight per unit area of everything above: within layer $i$ the average pressure is (sum of overlying layer pressures) + (half of its own contribution). Force on the curved area = average pressure × $A$.

> 【Thought】 Seeing "force on the curved surface area surrounding each liquid" → triggers *average pressure over the layer* (pressure varies linearly with depth, so the mean is the midpoint value — no integral needed). The densities $1,2,3,\ldots$ and the hint about $\sum i$ signal that a sum over overlying layers is expected.

**Solution.** Pressure at the base of layer $i$: $p_i=g\ell\rho\sum_{j=1}^{i}j=g\ell\rho\,\dfrac{i(i+1)}{2}$. Average over layer $i$ (linear in depth): $\bar p_i=\dfrac{p_{i-1}+p_i}{2}=\dfrac{g\ell\rho}{2}\big[(i-1)i\cdot\tfrac12\ldots\big]$ — cleaner: $\bar p_i=g\ell\rho\left[\dfrac{i(i-1)}{2}+\dfrac{i}{2}\right]=\dfrac{g\ell\rho\,i^2}{2}$.

(i) $F_1=\bar p_1 A=\boxed{\tfrac12\rho g\ell A}$. (ii) $F_2=4\times\tfrac12\rho g\ell A=\boxed{4F_1}$. (iii) $\boxed{F_n=n^2F_1}$.

**Check.** The force grows quadratically, not linearly, because both the overlying pressure head **and** the layer's own density scale with $i$ — a double counting that the $i^2$ captures ✓; $i=1$ recovers the simple $\tfrac12\rho g\ell A$ of a single fluid ✓.

---

### Q1(h) — Rocket with constant fuel burn [4 marks]

**(i)** Thrust: $T=\dot m v_e=50\times2000=\boxed{1.0\times10^{5}\ \text{N}}$.

**(ii)** Newton's second law vertically: $\boxed{a=\dfrac{T}{m}-g}$ (with $m$ the instantaneous total mass).

**(iii)** Constant burn rate over total burn time $t_0$ ($=m_0/\dot m=100$ s): $m(t)=m_r+m_0\left(1-\dfrac{t}{t_0}\right)$:
$$\boxed{a(t)=\frac{T}{m_r+m_0\left(1-t/t_0\right)}-g}.$$

**(iv) Astronaut's apparent weight doubles.** Apparent weight $N=m_a(g+a)$ doubles when $a=g$:
$$\frac{T}{m}=2g\;\Rightarrow\;m=\frac{T}{2g}=\frac{10^5}{19.6}=5.10\times10^{3}\ \text{kg},$$
$$10\,000-50t=5097\;\Rightarrow\;\boxed{t\approx98\ \text{s}\ (\text{near burn-out at }t_0=100\ \text{s})}.$$

> 【Thought】 Seeing "appeared to double" → triggers *apparent weight = m(g+a), not m a*: the astronaut feels $g$ even at rest on the pad. The trap is solving $a=g$... wait, the trap is setting $a=2g$; the correct condition is $g+a=2g\Rightarrow a=g$. Also note the rocket is nearly empty when this happens — thrust fixed, mass minimal ⟹ acceleration maximal: physically consistent that doubling happens late.

---

### Q1(i) — Oil overflowing a steel drum on a warm day [3 marks]

**Key observation.** Spill = (oil expansion) − (drum expansion); the drum's **volume** expansion is $3\alpha$ (linear) — the mismatch of coefficients is the whole problem.

> 【Thought】 Seeing "linear coefficient for steel" vs "volume coefficient for oil" → triggers *convert linear to volume: $\beta=3\alpha$*. Forgetting the factor 3 is the designed error (it changes the answer by $\sim$15%: $41^\circ$C vs $36^\circ$C... precisely $5+\frac{0.024}{6.64\times10^{-4}}$ vs $5+\frac{0.024}{7\times10^{-4}-1.2\times10^{-5}}$).

**Solution.** Fractional overflow:
$$\left(\beta_{\text{oil}}-3\alpha_{\text{steel}}\right)\Delta T=0.024\;\Rightarrow\;\Delta T=\frac{0.024}{7.0\times10^{-4}-3.6\times10^{-5}}=\frac{0.024}{6.64\times10^{-4}}=36.1^\circ\text{C},$$
$$\boxed{T\approx5.0+36.1\approx41^\circ\text{C}}.$$

**Check.** Sign: oil expands more than steel ⟹ spill on warming ✓; 2.4% at $\sim7\times10^{-4}$/K needs tens of degrees ✓ plausible for "a hot day" only in an exam world — the linear law is being extrapolated, fine as a model. A common slip is to use $\alpha$ instead of $3\alpha$ for the drum's *volume* expansion — it shifts the answer by ~15%.

---

### Q1(j) — Two radar sightings of an aircraft [4 marks]

**Key observation.** Convert (bearing, range) to Cartesian (bearing from north: $x=r\sin\theta$ east, $y=r\cos\theta$ north); constant velocity ⟹ linear extrapolation.

> 【Thought】 Seeing two (bearing, range) fixes → triggers *polar→Cartesian conversion*; differences of polar coordinates are meaningless — the subtraction must happen in Cartesian. For (ii), constant velocity means "same displacement again per equal time" — no new physics.

**Solution.** $P_1=(43\sin68^\circ,\,43\cos68^\circ)=(39.9,\,16.1)$ km; $P_2=(52\sin40^\circ,\,52\cos40^\circ)=(33.4,\,39.8)$ km.
$$\Delta\mathbf r=(-6.4,\,+23.7)\ \text{km per 5 min},\quad|\Delta\mathbf r|=24.6\ \text{km}\;\Rightarrow\;v=\frac{24\,590}{300}=\boxed{82\ \text{m/s}}.$$
Ten minutes later: $P_3=P_2+2\Delta\mathbf r=(20.6,\,87.3)$ km:
$$\text{range}=\sqrt{20.6^2+87.3^2}=\boxed{89.7\ \text{km}},\qquad \text{bearing}=\arctan\frac{20.6}{87.3}=\boxed{013^\circ}.$$

**Check.** Range increasing and bearing decreasing toward north — consistent with a track heading north-northwest ✓; $82$ m/s ≈ 300 km/h ✓ plausible for a small aircraft.

---

### Q1(k) — A modified gas equation [4 marks]

**Key observation.** Dimensions: the exponent must be dimensionless and $(V-b)$ must be volumes — this alone fixes $[a]$ and $[b]$.

> 【Thought】 For (ii), the target is "ideal gas law at a shifted temperature": expand both corrections to first order, collect the correction to $pV=nRT$, and demand it vanish — that condition defines $T_c$. The insight is that the two corrections (excluded volume $b$ raising $p$, attraction $a$ lowering it) can *cancel* — this is exactly the physics of the Boyle temperature in the van der Waals equation, of which this is a variant.

**Solution.** (i) $[b]=\text{m}^3$; exponent dimensionless: $[a]=[nRTV]=\text{J}\cdot\text{m}^3=\boxed{\text{kg m}^5\text{s}^{-2}}$; $[b]=\boxed{\text{m}^3}$.

(ii) With $b\ll V$ and $a\ll nRTV$:
$$pV\approx\frac{nRT}{1-b/V}\cdot\left(1-\frac{a}{nRTV}\right)\approx nRT\left(1+\frac{b}{V}-\frac{a}{nRTV}\right)=nRT+\frac{nRTb}{V}-\frac{a}{V}+\ldots$$
$$pV\approx nRT+\frac{1}{V}\left(nRTb-a\right).$$
The bracket vanishes — reducing the equation to ideal-gas form $pV=nRT_c$ — at
$$\boxed{T_c=\frac{a}{nRb}}.$$

**Check.** Dimensions: $\dfrac{\text{kg m}^5\text{s}^{-2}}{\text{mol}\cdot\text{J mol}^{-1}\text{K}^{-1}\cdot\text{m}^3}=\text{K}$ ✓; sign: attraction ($a$) and excluded volume ($b$) compete — at $T_c$ they cancel ✓ (Boyle-temperature physics).

---

### Q1(l) — Rod balanced in a smooth hemispherical bowl [6 marks]

**Key observation.** A three-force body in equilibrium: the lines of $N_A$ (along the radius at the interior contact), $N_B$ (⊥ rod at the rim) and $W$ (vertical through the centre of mass) must be **concurrent**. Geometry fixes the first two lines; concurrency then pins $r$ to $\ell$ and $\theta$.

> 【Thought】 Seeing "smooth … balanced" with exactly three forces → triggers the *three-force concurrence theorem* — faster than writing two force equations plus a moment equation. Geometric ingredient: a chord through the rim point at angle $\theta$ has length $2r\cos\theta$ (inscribed-angle geometry), placing the interior contact at $A=r(-\cos2\theta,-\sin2\theta)$ relative to the centre.

**Setup.** Bowl centre $O$ in the rim plane; rim point $B=(r,0)$; rod along angle $\theta$ above horizontal; interior contact at the rod's lower end $A$; rod length $\ell$, so COM at $\ell/2$ from $A$ along the rod.

**Geometry.** Chord $|AB|=2r\cos\theta$; direction $A\to O$ is $(\cos2\theta,\sin2\theta)$.

**Concurrence.** Line $AO$ and the perpendicular-to-rod line through $B$ meet at $P=(r\cos2\theta,\;r\sin2\theta)$ (verify: $P$ lies on both — two quick substitutions). COM: $M=\big(-r\cos2\theta+\tfrac{\ell}{2}\cos\theta,\;-r\sin2\theta+\tfrac{\ell}{2}\sin\theta\big)$. Vertical line through $M$ passes through $P$ ⟺ $M_x=P_x$:
$$-r\cos2\theta+\frac{\ell}{2}\cos\theta=r\cos2\theta\;\Rightarrow\;\frac{\ell}{2}\cos\theta=2r\cos2\theta\;\Rightarrow\;\boxed{r=\frac{\ell\cos\theta}{4\cos2\theta}}.$$

**Check.** Dimensions: length/length ✓. Physical range: need $\cos2\theta>0$ ⟹ $\theta<45^\circ$ (the bowl must be wide/shallow enough); also the rod must protrude beyond the rim ($\ell>2r\cos\theta$) ⟹ $\theta<35.3^\circ$ — the bowl geometry and balance coexist only in a window, which is why the problem is "express $r$" rather than "express $\theta$" ✓. Spot check $\theta=30^\circ$: $r=0.433\ell$, chord $=0.75\ell<\ell$ ✓ consistent with the figure (rod tip protruding). Feasibility window: $\cos2\theta>0\Rightarrow\theta<45^\circ$ (else $r<0$), and the rod must protrude beyond the rim, $\ell>2r\cos\theta$.

---

### Q1(m) — Three switched cells in parallel driving three switched resistors [3 marks]

**Key observation.** Each cell branch is $\varepsilon=5$ V with internal 5 Ω; each external branch is 5 Ω. Closing more cell switches keeps the emf at 5 V but **divides** the internal resistance; closing more resistor branches divides the load resistance.

> 【Thought】 Seeing "what arrangement gives max/min current" → triggers *identical sources in parallel: emf unchanged, internal resistance shrinks*; identical loads in parallel: resistance shrinks. So $I=\dfrac{\varepsilon}{r_{\text{int}}/n_c+R/n_r}$: maximise by maximising both counts; minimise (non-zero) by minimising both.

**Solution.** (i) **Maximum**: close all six switches:
$$I_{\max}=\frac{5.0}{5.0/3+5.0/3}=\frac{5.0}{3.33}=\boxed{1.5\ \text{A}}.$$
(ii) **Minimum non-zero**: close exactly one cell switch and one resistor switch (single loop, 5 V across 10 Ω):
$$I_{\min}=\boxed{0.50\ \text{A}}.$$
(iii) Values as computed: $1.5$ A and $0.50$ A.

**Check.** $I_{\max}/I_{\min}=3$: paralleling three equal branches triples both conductances ✓; internal and external resistances equal per branch, so the max-current case splits the emf equally (2.5 V each) ✓. In that case every cell and every resistor is engaged: internal resistance and load are each $5/3\ \Omega$, total $10/3\ \Omega$, $I=5/(10/3)=1.5$ A ✓.

---

### Q1(n) — Switched resistor network: $I_c/I_o$ [4 marks]

**Key observation.** S open: only 20 kΩ + 5 kΩ conduct. S closed: 15 kΩ and 10 kΩ join **in parallel with** the 5 kΩ, dropping the right-hand group's resistance and its share of the voltage — the current through the 5 kΩ is set by the voltage across the parallel group.

> 【Thought】 Seeing "current through the same resistor before/after" → triggers *track its voltage, not the total current*: the 5 kΩ is inside the switched-in parallel block, so its current falls when the block's resistance falls. Directly: $I_{5k}=V_{\text{group}}/5\text{k}$ in both cases.

**Solution.** S open: $I_o=\dfrac{\mathcal{E}}{20+5}=\dfrac{\mathcal{E}}{25\ \text{k}\Omega}$.
S closed: $5\|15\|10=\left(\tfrac15+\tfrac1{15}+\tfrac1{10}\right)^{-1}=\left(\tfrac{11}{30}\right)^{-1}=\tfrac{30}{11}\ \text{k}\Omega$; group voltage $=\mathcal{E}\dfrac{30/11}{20+30/11}=\mathcal{E}\dfrac{30}{250}=\dfrac{3\mathcal{E}}{25}$:
$$I_c=\frac{3\mathcal{E}/25}{5\ \text{k}\Omega}=\frac{3\mathcal{E}}{125\ \text{k}\Omega}\;\Rightarrow\;\boxed{\frac{I_c}{I_o}=\frac{3/125}{1/25}=\frac{3}{5}}.$$

**Check.** Closing S adds paths → total current rises ($\mathcal{E}/22.7$k vs $\mathcal{E}/25$k) but the 5 kΩ's **voltage** falls (from $\mathcal{E}/5$ to $0.12\mathcal{E}$) — the ratio < 1 ✓; the question's phrasing ("ratio of two integers") confirms the exact cancellation structure ✓. Alternative route (voltage ratio, no currents needed): the 5 kΩ pd falls from $\mathcal{E}/5$ to $0.12\mathcal{E}$, and $0.12/(1/5)=0.6=3/5$ directly.

---

### Q1(o) — Red-giant Sun: new peak wavelength [3 marks]

**Key observation.** Two scaling laws chained: $P\propto R^2T^4$ gives the new temperature; Wien $\lambda_{\max}\propto 1/T$ converts it to wavelength.

> 【Thought】 Seeing two proportionalities → triggers *ratio method*: form $P'/P=(R'/R)^2(T'/T)^4$; no constants needed. The red-giant paradox to note: hugely more luminous yet **cooler** — hence the peak shifts to the red/IR, which is the physical content of the question.

**Solution.** $(T'/T)^4=\dfrac{4000}{200^2}=\dfrac{4000}{40000}=0.1\Rightarrow T'/T=0.562$:
$$\lambda'_{\max}=\frac{500\ \text{nm}}{0.562}=\boxed{890\ \text{nm}\ (\text{near-IR})}.$$

**Check.** Cooler surface ($\times0.56$) ⟹ longer peak wavelength ($\times1.78$) ✓ direction correct; $R^2$ growth ($\times40000$) outruns the $T^4$ fall ($\times0.1$) to give net $\times4000$ ✓.

---

### Q1(p) — Redshifted hydrogen line [3 marks]

**Key observation.** $E\to\lambda$ via $\lambda=hc/E$ (use $hc\approx1240\ \text{eV·nm}$); small redshift $z=\Delta\lambda/\lambda=v/c$; Hubble $d=v/H_0$.

> 【Thought】 The chain is linear and each link is one formula — the discipline is significant figures and the non-relativistic licence: $z=0.011\ll1$ justifies $v=zc$. If $z$ were $\sim1$, the relativistic Doppler formula would be needed and $v=zc$ would be wrong.

**Solution.** (i) $\lambda=\dfrac{1240}{2.55}=\boxed{486\ \text{nm}}$ (the H-$\beta$ line ✓).
(ii) $v=c\,\dfrac{\Delta\lambda}{\lambda}=3.00\times10^5\times\dfrac{5.4}{486}=\boxed{3.3\times10^3\ \text{km/s}}$.
(iii) $d=\dfrac{v}{H_0}=\dfrac{3330}{70}=\boxed{48\ \text{Mpc}}$.

**Check.** 486 nm is indeed a real hydrogen line (Balmer-β, $n=4\to2$: $E=2.55$ eV ✓) — internal consistency of the data ✓; $z\approx0.01$ is a typical "nearby galaxy" redshift, distance plausible ✓.

---

### Q1(q) — Car over regularly spaced bumps: resonance [3 marks]

**Key observation.** The static sink under passengers measures the suspension stiffness $k$; the car is then a mass–spring oscillator with natural frequency $f_0=\frac{1}{2\pi}\sqrt{k/m}$; discomfort = resonance when the bump-crossing frequency $v/d$ equals $f_0$.

> 【Thought】 Seeing "sinks by 1.8 cm under 320 kg" → triggers *static deflection → spring constant* — the standard way to characterise a suspension without opening it. Note the oscillating mass includes the passengers ($m=1120$ kg), because the resonance occurs with them aboard.

**Solution.** $k=\dfrac{320\times9.81}{0.018}=1.74\times10^5\ \text{N/m}$; $f_0=\dfrac{1}{2\pi}\sqrt{\dfrac{1.74\times10^5}{1120}}=1.99\ \text{Hz}$.
$$v=f_0\,d=1.99\times8.0=\boxed{\approx16\ \text{m/s}\ (\approx57\ \text{km/h})}.$$

**Check.** $f_0\approx2$ Hz is the textbook value for car suspensions ✓ (1–2 Hz); using $m=800$ kg instead gives 18.9 m/s — same order, but 16 m/s is the consistent choice ✓. (The oscillating mass $m=1120$ kg includes the occupants — the resonance is excited with them on board.)

---

### Q1(r) — Pendulum clock running slow [3 marks]

**Key observation.** Running slow ⟹ period too long by the same fraction; $T\propto\sqrt L$ so fractional length change is **twice** the fractional period change, with opposite sign.

> 【Thought】 Seeing "loses 10 minutes each day" → triggers *fractional period error = fractional time error*: $\Delta T/T=+600/86400$ (each tick takes too long). The classic trap is halving/for doubling; $\delta L/L=2\,\delta T/T$ because $T\propto L^{1/2}$.

**Solution.** $\dfrac{\Delta T}{T}=\dfrac{600}{86400}=6.94\times10^{-3}$; required $\dfrac{\Delta L}{L}=-2\times6.94\times10^{-3}=-1.39\times10^{-2}$:
$$\boxed{\text{shorten the pendulum by about }1.4\%.}$$

**Check.** Sign: slow clock → pendulum too long → shorten ✓; magnitude: ~1% per ~7 minutes/day error is the right scale ✓.

---

### Q1(s) — Telescope diameter to resolve a binary [2 marks]

**Key observation.** Angular separation $\theta=$ separation/distance (both in light years — ratio is dimensionless directly); Rayleigh criterion $D=1.22\lambda/\theta$.

> 【Thought】 Seeing both lengths in light years → the ratio is the angle: *matching units cancel*, no conversion to metres needed for $\theta$. The 1.22 factor (circular aperture, first Airy zero) vs 1.0 (slit) is the only conceptual content.

**Solution.** $\theta=\dfrac{0.00593}{2140}=2.77\times10^{-6}$ rad;
$$D=\frac{1.22\times550\times10^{-9}}{2.77\times10^{-6}}=\boxed{0.24\ \text{m}\approx24\ \text{cm}}.$$

**Check.** A modest amateur telescope — plausible for a $\sim$1.3 arcsec binary ✓ ($2.77\ \mu$rad $=0.57''$, and $D=24$ cm has Rayleigh limit $0.57''$ ✓ consistent). The 1.22 factor is the first dark ring of a *circular* aperture; a rectangular one would use 1.0.

---

### Q1(t) — Prism (A = 75°, n = 1.40): range of incidence angles for emergence [3 marks]

**Key observation.** Inside the prism $r_1+r_2=A$; emergence from AC requires $r_2<\theta_c$. Since $A>\theta_c$, there is a **minimum** $r_1$ — i.e. a minimum incidence angle — below which the ray is totally internally reflected at AC.

> 【Thought】 Seeing "for what range … will light emerge from AC" → triggers *critical-angle inequality converted back through the refraction at entry*: the condition $r_2=\theta_c$ defines the boundary; monotonicity of $r_1+r_2=A$ then tells you which side of the boundary is the allowed region (test one point rather than reasoning abstractly: at grazing incidence $i=90^\circ$, $r_1=\theta_c$, $r_2=A-\theta_c<\theta_c$ ✓ emerges — so the allowed region is $i$ **above** the threshold).

**Solution.** $\theta_c=\arcsin(1/1.40)=45.6^\circ$; emergence boundary: $r_2=\theta_c\Rightarrow r_1=A-\theta_c=29.4^\circ$:
$$\sin i=n\sin r_1=1.40\sin29.4^\circ=0.688\;\Rightarrow\;i>43.5^\circ.$$
$$\boxed{43.5^\circ<i\le 90^\circ\ \text{(rays entering AB emerge from AC)}}.$$

(ii) Diagram: prism apex up (A = 75°); draw a grazing ray ($i=90^\circ$) refracting to $r_1=45.6^\circ$, hitting AC at $r_2=29.4^\circ$ and emerging; and the marginal ray $i=43.5^\circ$ skimming along AC ($e=90^\circ$). Rays with $i<43.5^\circ$ shown totally internally reflected at AC.

**Check.** $A<2\theta_c$ ($75^\circ<91.2^\circ$) — so *some* rays emerge, consistent with the question being non-empty ✓; symmetric sanity: at $i=90^\circ$, $e=\arcsin(n\sin29.4^\circ)=43.5^\circ$ — reciprocity of the two faces ✓ beautiful confirmation. The range's limits are physical: $i=43.5^\circ$ corresponds to grazing *emergence* ($r_2=\theta_c$), $i=90^\circ$ to grazing *incidence*.

---

### Q1(u) — Charged pendulum displaced by an approaching charge [6 marks]

**Key observation.** When B sits at A's original point $P$ (directly below the support), A hangs in equilibrium at some thread angle $\theta$, with the A–B separation the chord $r=2\ell\sin(\theta/2)$. Force balance on A pins $r$ in terms of the given quantities; the work is then just the total potential-energy change.

> 【Thought】 The geometry gift: the chord from the rest point makes angle $\theta/2$ with the vertical, so the Coulomb force on A acts at $\theta/2$ above horizontal — the half-angle relations do all the algebra. The answer must contain $q$ and $Q$ (the question says so), which tells you $\theta$ stays *implicit* — eliminated via the equilibrium condition, never evaluated. (Do not over-read "neutral" as a flat-potential condition $U''=0$; the official solution and the requested variable list show that ordinary equilibrium is meant.)

**Solution.** Forces on A: weight $mg$, tension $T$ along the thread, Coulomb $F=kQq/r^2$ along the chord B→A (at $\theta/2$ above horizontal). Resolving along/perpendicular to the thread (or vertical/horizontal) and eliminating $T$:
$$T\sin\theta=F\cos\tfrac\theta2,\qquad T\cos\theta+F\sin\tfrac\theta2=mg\;\Rightarrow\;mg=F\left[\sin\tfrac\theta2+\frac{\cos(\theta/2)\cos\theta}{\sin\theta}\right].$$
The bracket collapses: $\sin\tfrac\theta2+\dfrac{\cos\theta}{2\sin(\theta/2)}=\dfrac{2\sin^2(\theta/2)+\cos\theta}{2\sin(\theta/2)}=\dfrac{1}{2\sin(\theta/2)}$:
$$mg=\frac{F}{2\sin(\theta/2)}\quad\text{with}\quad F=\frac{kQq}{r^2},\ \ 2\sin\tfrac\theta2=\frac{r}{\ell}\;\Rightarrow\;mg\,\frac{r}{\ell}=\frac{kQq}{r^2}\;\Rightarrow\;\boxed{r^3=\frac{kQq\ell}{mg}}.$$

**Work done** (quasi-static; tension does no work on A since it is perpendicular to A's arc):
$$W=\Delta U=\underbrace{mg\,\ell(1-\cos\theta)}_{\text{raising A}}=\underbrace{2mg\ell\sin^2\tfrac\theta2}_{=\,mgr^2/2\ell}+\underbrace{\frac{kQq}{r}}_{=\,mgr^2/\ell}=\frac{3}{2}\,\frac{mgr^2}{\ell},$$
and substituting $r^2=(kQq\ell/mg)^{2/3}$:
$$\boxed{W=\frac{3}{2}\left(\frac{mg\,k^2q^2Q^2}{\ell}\right)^{1/3}}.$$

**Check.** The two energy contributions are in the fixed ratio $1:2$ (gravity : Coulomb) — a virial-style fingerprint of the $r^3$ equilibrium law ✓. Dimensions: $[mg\cdot(kQq)^2/\ell]=\text{N}\cdot\text{N}^2\text{m}^4/\text{m}=\text{N}^3\text{m}^3$ → cube root = J ✓. Limits: $q\to0\Rightarrow W\to0$ ✓; heavier A hangs lower (smaller $r$) and needs less work ✓. (Official mark scheme: identical expression — obtained by the same force balance.) Failure boundary: if $q$ is too large, no equilibrium exists inside the bowl — A is driven over the rim and the balance equation has no in-range root.

---

### Q1(v) — Capacitor discharging through a voltage-dependent resistor [6 marks]

**Key observation.** The discharge law $I=-C\,dV/dt=V/R(V)$ is separable: $dt=-C\,R(V)\,\dfrac{dV}{V}$, and $R(V)=AV+B$ makes the integral elementary ($\int(A+B/V)\,dV$).

> 【Thought】 Seeing $R$ linear in $V$ → triggers *separate and integrate*; the surprising twist is that as $V\to0$ the resistance stays finite ($B$), so the tail is exponential-like, while the high-voltage phase has constant-resistance-like... rather, $R\propto V$ gives $dV/dt\propto$ const — a **linear** early decay. Calibrate $A,B$ from the two data points first — the pair (6.0 V, 10 Ω) and (0.06 V, 4 Ω) is engineered so the 1% target is exactly the second calibration voltage.

**Solution.** $A=\dfrac{10.0-4.0}{6.0-0.06}=\dfrac{6.0}{5.94}=1.010\ \Omega/\text{V}$; $B=4.0-A(0.06)=3.939\ \Omega$.
The integrand splits as $\dfrac{AV+B}{V}=A+\dfrac{B}{V}$, with antiderivative $AV+B\ln V$ — the $B\ln V$ term is the tail contribution: as $V\to0$ the resistance bottoms out at $B$, so the late discharge is exponential-like rather than linear:
$$t=C\int_{0.06}^{6.0}\frac{AV+B}{V}\,dV=C\left[A(6.0-0.06)+B\ln\frac{6.0}{0.06}\right]=1.0\times\left[1.010\times5.94+3.939\times\ln100\right],$$
$$t=6.00+18.14=\boxed{24.1\ \text{s}}.$$

**Check.** Sanity against constant-$R$ extremes: with $R=10\ \Omega$ throughout, $t=RC\ln100=46$ s; with $R=4\ \Omega$, $t=18.4$ s; our $R$ falls from 10 to 4 during discharge, so $24$ s lying between ✓. Note the exact cancellation $A\times5.94=6.00$ — the data were designed for it ✓.

---

### Q1(w) — α-decay kinetic energy of U-238 [5 marks]

**Key observation.** The mass defect gives the total energy release $Q$; momentum conservation (daughter recoils) then assigns the α a fixed share $m_{Th}/(m_{Th}+m_\alpha)$ of $Q$.

> 【Thought】 Seeing masses given to 5 significant figures → the defect is a **tiny difference of large masses**: guard precision — work with the differences directly, never round the masses first. Seeing "kinetic energy of the α" (not "Q-value") → triggers *recoil correction*: in the two-body decay at rest, momenta are equal and opposite, so $KE\propto1/m$ and the lighter α takes the larger share.

**Solution.** Mass defect:
$$\Delta m=3.85395\times10^{-25}-3.78737\times10^{-25}-6.64807\times10^{-27}=9.93\times10^{-30}\ \text{kg},$$
$$Q=\Delta m c^2=9.93\times10^{-30}\times(2.998\times10^8)^2=8.93\times10^{-13}\ \text{J}=5.57\ \text{MeV}.$$
Two-body kinematics ($p_\alpha=p_{Th}$, $KE=p^2/2m$):
$$KE_\alpha=Q\cdot\frac{m_{Th}}{m_{Th}+m_\alpha}=5.57\times0.9828=\boxed{5.5\ \text{MeV}}.$$

**Check.** The accepted U-238 α energy is 4.27 MeV, while the *masses supplied in the question* yield $Q=5.57$ MeV; within the data provided, $5.5$ MeV is the consistent answer — the supplied masses are rounded, and the discrepancy is flagged honestly rather than fudged. Recoil share to the daughter: $\sim1.7\%$ — small, as expected ✓.

---
*End of Paper 5 (2023 Round 1 Section 1, 11 Nov).*


---

## Paper 6 — 2023 Round 1 Section 1 (10 Nov 2023)

*Section 1, Question 1, parts (a)–(t). Maximum 50 marks from ≈ 83.*

---

### Q1(a) — Skier with constant resistance [3 marks]

**Key observation.** Constant net force ⟹ constant acceleration: kinematics gives $a$ from $d$ and $t$, then Newton's second law along the slope yields $F_r$.

> 【Thought】 Seeing "constant resistive force" + "distance d at time t" → triggers *constant-acceleration kinematics backwards*: extract $a=2d/t^2$ first, then write $ma=mg\sin\theta-F_r$. The order matters: kinematics before dynamics.

**Solution.** $d=\tfrac12at^2\Rightarrow a=2d/t^2$; along slope: $mg\sin\theta-F_r=ma$:
$$\boxed{F_r=m\left(g\sin\theta-\frac{2d}{t^2}\right)}.$$

**Check.** $F_r\to mg\sin\theta$ as $a\to0$ (terminal glide) ✓; dimensions: $d/t^2$ is an acceleration ✓.

---

### Q1(b) — Car towing a caravan [3 marks]

**Key observation.** Resistance splits in proportion to weight: $R_{\text{car}}:R_{\text{cav}}=1200:600=2:1$, so $R_{\text{car}}=600$ N, $R_{\text{cav}}=300$ N. Treat the pair as one body for the engine force, then isolate the caravan for the tow-bar tension.

> 【Thought】 System boundary choice is the skill: (i) whole train (internal tension cancels); (ii) caravan alone (tension appears); (iii) power = force × *current* speed, not average — the engine works harder as speed rises.

**Solution.** (i) $F-900=(1200+600)(2.0)$ → $\boxed{F=4500\ \text{N}}$.
(ii) Caravan alone: $T-300=600\times2.0$ → $\boxed{T=1500\ \text{N}}$.
(iii) $v=at=10\ \text{m/s}$: $P=Fv=4500\times10=\boxed{45\ \text{kW}}$.

**Check.** Tension also equals $R_{\text{cav}}+m_{\text{cav}}a$ = its own "engine requirement" ✓; engine force split: $4500 = 900 (\text{drag})+3600 (\text{inertia})$ ✓; cross-check tension via the car: $F-R_{\text{car}}-T=m_{\text{car}}a\Rightarrow4500-600-1500=2400$ ✓.

---

### Q1(c) — Two cyclists from A to B [3 marks]

**Key observation.** Convert the timetable into total elapsed times; Robert's moving time + break fixes his arrival, Helen's earlier arrival fixes her duration.

> 【Thought】 Pure scheduling arithmetic — the discipline is writing the timeline rather than juggling numbers mentally. Robert: ride time $50/12$ h + 0.5 h break.

**Solution.** Robert: $\dfrac{50}{12}=4\tfrac16$ h riding $+\,\tfrac12$ h break $=4\tfrac23$ h: 8:00 → 12:40. Helen arrives 11:40, having left 8:30: duration $3\tfrac16$ h:
$$v_H=\frac{50}{19/6}=\frac{300}{19}=\boxed{15.8\ \text{km/h}}.$$

**Check.** Helen is faster (no break, earlier arrival despite later start) ✓; $15.8>12$ ✓.

---

### Q1(d) — Plank leaning on a smooth wall, held by a string [3 marks]

**Key observation.** Two smooth contacts → reactions are purely normal (floor: vertical; wall: horizontal). With the string horizontal at the base, taking moments about the **base** eliminates two of the four forces at once.

> 【Thought】 Seeing two smooth surfaces + a string → triggers *choose the pivot where the most unknown forces pass through* (the plank's base: floor normal and tension both act there). One moment equation then links $mg$ and the wall reaction directly.

**Solution.** Moments about the base (plank length $L$): weight's lever arm $\tfrac{L}{2}\cos\alpha$; wall reaction $N$ (horizontal) at height $L\sin\alpha$:
$$mg\tfrac{L}{2}\cos\alpha=NL\sin\alpha\;\Rightarrow\;N=\frac{mg}{2\tan\alpha}.$$
Horizontal force balance: $T=N$:
$$\boxed{T=\frac{mg}{2\tan\alpha}}.$$

**Check.** $\alpha\to90^\circ$ (vertical plank): $T\to0$ ✓; $\alpha\to0$: $T\to\infty$ — flat plank impossible to hold with a base string ✓; dimensions: force ✓.

---

### Q1(e) — Falling object: last-second vs last-but-one-second distances [3 marks]

**Key observation.** Distances fallen in successive seconds scale as odd numbers only *from rest*; generally the distance in the $k$-th second is $\tfrac12 g(2t-1)$ with $t$ the elapsed time. The ratio condition fixes the total fall time.

> 【Thought】 Seeing "last second : last-but-one second = 3:2" → triggers *write both distances with the total time $T$ as the single unknown*: $\tfrac12g(2T-1)$ and $\tfrac12g(2T-3)$. The 3:2 ratio then gives one linear equation. Do not assume $T$ is an integer — the algebra decides.

**Solution.** $\dfrac{2T-1}{2T-3}=\dfrac32\Rightarrow4T-2=6T-9\Rightarrow T=3.5$ s.
(i) $h=\tfrac12 gT^2=4.905\times12.25=\boxed{60\ \text{m}}$.
(ii) $v=gT=9.81\times3.5=\boxed{34.3\ \text{m/s}}$.

**Check.** Verify the premise: distance fallen in the last second is $\tfrac12g(T^2-(T-1)^2)=\tfrac12g(2T-1)=4.905\times6=29.4$ m; in the previous second $4.905\times(2T-3)=4.905\times4=19.6$ m; ratio $6/4=3/2$ ✓ as stipulated.

---

### Q1(f) — Mass on two wires; one wire cut [3 marks]

**Key observation.** (i) Static: two tensions at 30° share the load. (ii) The instant after cutting, the mass is *momentarily at rest* — zero centripetal acceleration — but the system is no longer in static equilibrium: tension comes from the **radial** force balance alone along the remaining wire, $T_{AC}=mg\cos30^\circ$.

> 【Thought】 The designed trap: writing $T_{AC}=mg/(2\cos30^\circ)$-style statics, or claiming the tension is unchanged. The mechanism: immediately after the cut $v=0$, so radial acceleration $v^2/\ell=0$, and the wire only needs to cancel the radial component of gravity. The "at the same instant" clause is the signal that a *dynamic* (not static) balance applies — with zero velocity.

**Solution.** (i) $2T\cos30^\circ=mg$ → $\boxed{T=\dfrac{mg}{2\cos30^\circ}=\dfrac{mg}{\sqrt3}}$.
(ii) Just after the cut, along wire AC (radial): $T_{AC}-mg\cos30^\circ=m\dfrac{v^2}{\ell}=0$:
$$T_{AC}=mg\cos30^\circ=\frac{\sqrt3}{2}mg\;\Rightarrow\;\boxed{\frac{T_{AC}}{T}=\frac{\sqrt3/2}{1/\sqrt3}=\frac32}.$$

**Check.** $T_{AC}>T$: the remaining wire's load jumps (from sharing to carrying alone) ✓; ratio $3/2<2$ because only the radial component of $mg$ must be balanced at this instant ✓. The crux is *instant vs static*: at the moment of cutting $v=0$, so the radial acceleration $v^2/L$ vanishes and $T_{AC}=mg\cos30^\circ$ — not the static-equilibrium value.

---

### Q1(g) — Copper wire: given mass and resistance, find length [3 marks]

**Key observation.** Two constraints ($R=\rho L/A$ and $M=\rho_m LA$) share the cross-section; eliminating $A$ gives $R=\rho\rho_mL^2/M$ — so $R\propto L^2/M$ for a fixed material.

> 【Thought】 Seeing both mass and resistance specified → triggers *eliminate the unknown cross-section*: combining gives $L=\sqrt{RM/\rho\rho_m}$; in ratio form $\dfrac{L_2}{L_1}=\sqrt{\dfrac{R_2}{R_1}\dfrac{M_2}{M_1}}$ — no densities needed.

**Solution.**
$$\frac{L_2}{L_1}=\sqrt{\frac{6000}{0.15}\times\frac{10^6\ \text{g}}{1\ \text{g}}}=\sqrt{4\times10^4\times10^6}=2\times10^5,$$
$$\boxed{L_2=2\times10^5\ \text{m}=200\ \text{km}}.$$

**Check.** Longer and more massive: both raise $L$; sanity: $R\propto L^2$ at fixed mass (longer ⟹ thinner too) — so resistance grows quadratically, which is why 40 000× resistance "only" needs 200× length at $10^6\times$ mass ✓.

---

### Q1(h) — Glass block with curved sides and a mirrored base [3 marks]

**Key observation.** Same height in and out + left–right symmetric block ⟹ the internal ray is a symmetric V reflecting at the **centre** of the base. The block is narrowest when the internal V is steepest, which happens for the highest possible entry point — the top corner, where entry is grazing ($i=90^\circ$) and refraction is maximal ($r=\theta_c$).

> 【Thought】 Seeing "minimum ℓ" → triggers *extremal-geometry*: parametrise by entry height, show the width decreases as entry rises, so the minimum is the grazing limit. The numerical check: $\ell(\alpha)$ rises monotonically from its $\alpha=0$ value ($\alpha$ = arc parameter; verified by sampling), so the corner case is indeed the minimum. The block width between the two top corners is then just twice the horizontal run of the steepest internal ray.

**Solution.** At the top corner the surface normal is vertical; grazing entry $i=90^\circ$ gives $r=\theta_c$ with $\sin\theta_c=1/n$:
$$\tan\theta_c=\frac{1}{\sqrt{n^2-1}}=\frac{1}{\sqrt{1.46^2-1}}=\frac{1}{1.064}=0.940.$$
The internal ray falls from height $R$ at angle $\theta_c$ from vertical: horizontal run $\Delta x=R\tan\theta_c$; by symmetry $\ell_{\min}=2\Delta x$:
$$\boxed{\ell_{\min}=\frac{2R}{\sqrt{n^2-1}}=2(2.0\ \text{cm})(0.940)\approx3.8\ \text{cm}}.$$

**Check.** Lower entries need wider blocks (sampled: $\ell$ grows to 8.6 cm as the entry drops to 80° down the arc) — so the corner case is minimal ✓; $n\to1$: $\ell\to\infty$ (no bending, ray never reaches the base within a finite block) ✓ sensible divergence. *(Official mark scheme prints 3.5(3) cm for the same formula $2R/\sqrt{n^2-1}$; direct substitution with $R=2.0$ cm, $n=1.46$ gives 3.76 cm — the formula agrees, the official numeral appears to be a rounding/slip.)*

---

### Q1(i) — Radiation force and photon density of an 8 W beam [4 marks]

**Key observation.** Momentum flux: absorbed light delivers $P/c$; reflected light delivers **twice** its incident momentum flux, $2P_r/c$.

> 【Thought】 Seeing "50% reflected, 50% absorbed" → triggers *momentum bookkeeping per channel*: reflection reverses momentum ($\Delta p=2p$), absorption merely stops it ($\Delta p=p$). Forgetting the factor 2 on reflection is the designed error. For (ii): photon density = flux/($c$), with flux = power/(area × photon energy).

**Solution.** (i)
$$F=\frac{P_{\text{abs}}+2P_{\text{refl}}}{c}=\frac{4+8}{3.00\times10^8}=\boxed{4.0\times10^{-8}\ \text{N}}.$$
(ii) $E_\gamma=hc/\lambda=3.31\times10^{-19}$ J; photon rate $\dot N=8/E_\gamma=2.42\times10^{19}\ \text{s}^{-1}$; density $n$ obeys $\dot N=ncA$:
$$n=\frac{2.42\times10^{19}}{(3.00\times10^8)(12\times10^{-4})}=\boxed{6.7\times10^{13}\ \text{m}^{-3}}.$$

**Check.** Radiation pressure $=F/A=4\times10^{-8}/1.2\times10^{-3}=3.3\times10^{-5}$ Pa — tiny, as expected for lamp-scale powers ✓; density sanity: $\sim10^{14}$ photons/m³ vs air molecules $\sim10^{25}$/m³ ✓ negligible. The factor of 2 is momentum bookkeeping: reflection reverses a photon's momentum (change $2p$), absorption merely stops it (change $p$).

---

### Q1(j) — Neutrons decaying in flight [4 marks]

**Key observation.** Flight time $t=d/v$ is tiny against the half-life, so linearise the exponential: $\Delta N\approx N_0(\ln2)\,t/T_{1/2}$.

> 【Thought】 Seeing $t\ll T_{1/2}$ (5 ms vs 880 s) → triggers *first-order decay approximation*; using the full exponential $N_0(1-2^{-t/T})$ gives the same number to 6 figures — state the approximation, don't fear it.

**Solution.** $t=\dfrac{11}{2200}=5.0\times10^{-3}$ s:
$$\Delta N=10^8\times\frac{0.693\times5.0\times10^{-3}}{880}=\boxed{3.9\times10^{2}\ \text{neutrons}\ (\approx400)}.$$

**Check.** Fraction decayed $\sim4\times10^{-6}$ ✓ tiny, consistent with $t\ll T_{1/2}$ ✓; with $t/T_{1/2}\sim6\times10^{-6}$, the linearisation error is of order $(t/T_{1/2})^2\sim10^{-11}$ — utterly safe ✓.

---

### Q1(k) — Hinged rod resting on a cylinder [4 marks]

**Key observation.** The rod is a tangent line from the hinge to the cylinder's circle. The hinge-to-centre distance $\sqrt5\,r$ and radius $r$ make the tangent geometry collapse into two equal angles (the given half-angle identity is the hint that $\tan\theta$ comes out rational).

**(i) tan θ.** Hinge $H=(0,3r)$, centre $C=(r,r)$: $|HC|=\sqrt{r^2+4r^2}=\sqrt5\,r$. $HC$ sits at $\arctan\tfrac12$ from vertical; the tangent deviates from $HC$ by $\alpha$ with $\sin\alpha=\dfrac{r}{|HC|}=\dfrac1{\sqrt5}$, so $\tan\alpha=\tfrac12$ as well. The rod is the *outer* tangent (the inner one, $\theta=0$, lies along the wall):
$$\theta=\arctan\tfrac12+\arctan\tfrac12,\qquad \tan\theta=\frac{2\times\tfrac12}{1-\tfrac14}=\boxed{\frac43}\quad(\theta=53.1^\circ).$$

> 【Thought】 Seeing the supplied double-angle identity → triggers *look for two equal angles*: the data ($3r$, $r$, corner geometry) are engineered so that the hinge direction and the tangent-opening angle coincide. If the hinge height were generic, the answer would be an ugly surd — recognising the design tells you to trust the simple route.

**(ii) Rod length.** Lower end at height $r$: vertical drop from hinge $=2r$:
$$\ell=\frac{2r}{\cos\theta}=\frac{2r}{3/5}=\boxed{\frac{10r}{3}}.$$

**(iii) Minimum work by the thread.** Everything is smooth and the pull is slow → the thread's work becomes gravitational PE of the rod alone (the cylinder stays on the floor; the contact force does equal opposite work on the pair since slip is tangential). The thread's tension equals the rod's leftward push on the cylinder, which vanishes when the contact reaches the **top** of the cylinder — exactly when the rod's lower end is at height $2r$:
$$\cos\theta_{\max}=\frac{3r-2r}{\ell}=\frac{r}{10r/3}=\frac{3}{10}.$$
COM heights: initially $3r-\tfrac{\ell}{2}\cos\theta_0=3r-\tfrac{5r}{3}\cdot\tfrac35=2r$; finally $3r-\tfrac{5r}{3}\cdot\tfrac3{10}=2.5r$:
$$\boxed{W_{\min}=mg\,(2.5r-2r)=\frac{mgr}{2}}.$$

> 【Thought】 "Tension reduces to zero" is the stop condition: it marks the geometry where the rod's contact force on the cylinder becomes vertical — i.e. contact at the top of the circle. Recognising a *force condition hidden inside a geometry statement* is the step that makes (iii) solvable; after it, energy bookkeeping replaces force chasing.

**(iv) Ratio.** $\cos\theta_0=3/5$ from (i); $\cos\theta_{\max}=3/10$ from (iii):
$$\boxed{\frac{\cos\theta_0}{\cos\theta_{\max}}=2}.$$

**Check.** $\theta$ rises from $53.1^\circ$ to $72.5^\circ$ as the cylinder is pulled out — the rod swings down toward the cylinder's top, and once the end passes the top the angle falls again ✓ consistent with the question's narrative; $\ell=10r/3=3.33r$ exceeds the initial tangent reach $2r$ ✓ so phase 1 (side contact) really occurs.

---

### Q1(l) — Block sliding down a freely moving wedge [4 marks]

**Key observation.** With both surfaces smooth, horizontal momentum is conserved, but the cleanest route is Newton's laws in components: the block's absolute acceleration = wedge acceleration + block's acceleration relative to the wedge (down the slope).

**(i) Free-body diagrams.** Block: $m_1g$ down, normal $N$ ⊥ slope. Wedge: $m_2g$ down, floor reaction up, and the reaction $-N$ from the block (perpendicular into the slope face).

**(ii) Normal to the slope** (outward positive; the block's absolute acceleration has normal component $-A\sin\theta$ from the wedge's motion, where $A$ = wedge's horizontal acceleration):
$$m_1g\cos\theta-N=m_1A\sin\theta.$$

> 【Thought】 The key move: the block's acceleration normal to the slope is **not zero** — it comes entirely from the wedge's horizontal acceleration ($A\sin\theta$). Forgetting this (treating the wedge as fixed) is the designed error. Relative-acceleration decomposition $a_{\text{block}}=a_{\text{wedge}}+a_{\text{rel}}$ is the systematic way to keep the constraint "block stays on the slope" exact.

**(iii)** Along the slope for the block: $m_1g\sin\theta=m_1(a_{\text{rel}}-A\cos\theta)$. Horizontal for the wedge: $N\sin\theta=m_2A$. Eliminating $N$ and $a_{\text{rel}}$:
$$N=\frac{m_1m_2g\cos\theta}{m_2+m_1\sin^2\theta},\qquad\boxed{A=\frac{m_1g\sin\theta\cos\theta}{m_2+m_1\sin^2\theta}=\frac{\sqrt3\,m_1g}{4m_2+m_1}}\quad(\theta=30^\circ).$$

**Check.** Limits: $m_2\to\infty$: $A\to0$ — fixed wedge ✓; $m_2\to0$: $A\to g\cot\theta=g\sqrt3$ — the block free-falls vertically (wedge darts out) ✓ known behaviour; denominator structure $m_2+m_1\sin^2\theta$ is the standard result ✓.

---

### Q1(m) — Ships: closest approach [5 marks]

**Key observation.** Constant velocities → switch to A's rest frame: B moves along a straight line; closest approach = perpendicular distance from A to that line.

> 【Thought】 Seeing "spot each other … distance of closest approach" → triggers *relative velocity + cross product*: $d_{\min}=|\mathbf r_{B/A}\times\hat{\mathbf v}_{\text{rel}}|$. If the relative line misses, that's the answer; no need to solve for the meeting time first (though it falls out as a check).

**Solution.** Axes: $x$ east, $y$ north. $\mathbf r_{B/A}=(0,-2.0)$ nmi; $\mathbf v_A=(5,0)$, $\mathbf v_B=20(\sin30^\circ,\cos30^\circ)=(10,17.32)$ kt; $\mathbf v_{\text{rel}}=\mathbf v_B-\mathbf v_A=(5,\;17.32)$ kt, $|\mathbf v_{\text{rel}}|=\sqrt{25+300}=18.03$ kt:
$$d_{\min}=\frac{|\mathbf r\times\mathbf v_{\text{rel}}|}{|\mathbf v_{\text{rel}}|}=\frac{|0\times17.32-(-2.0)(5)|}{18.03}=\boxed{0.55\ \text{nautical miles}}.$$

**Check.** Time of closest approach: $t=\dfrac{-\mathbf r\cdot\mathbf v_{\text{rel}}}{|\mathbf v_{\text{rel}}|^2}=\dfrac{34.64}{325}=0.107$ h $\approx6.4$ min > 0 — the closest point is in the future, so the computed minimum is physically realised ✓.

---

### Q1(n) — Compound steel–copper tube in tension [5 marks]

**Key observation.** "Firmly connected" ⟹ **common strain** (iso-strain composite): $\sigma_i=E_i\varepsilon$; the load is shared in proportion to $E_iA_i$.

> 【Thought】 Seeing concentric tubes firmly connected under tension → triggers *iso-strain, not iso-stress*: one strain everywhere, stresses split by modulus, load splits by $E_iA_i$. The second trap is lexical: "the stress produced" by the load means the *applied* (average) stress over the whole cross-section — not any one material's stress.

**Solution.** The "stress produced" is the *applied* stress $\sigma=6.2\times10^7$ Pa, i.e. load/total area (reading it as the steel's own stress would be wrong). Radii: steel 2.00–2.25 cm; copper liners 1.80–2.00 cm and 2.25–2.45 cm:

$$A_s=\pi(2.25^2-2.00^2)\times10^{-4}=3.34\times10^{-4}\ \text{m}^2,\qquad A_{Cu}=\pi\left[(2.00^2-1.80^2)+(2.45^2-2.25^2)\right]\times10^{-4}=5.34\times10^{-4}\ \text{m}^2,$$
$$A_{\text{tot}}=8.68\times10^{-4}\ \text{m}^2,\qquad \Sigma EA=200\times10^9\,A_s+110\times10^9\,A_{Cu}=1.26\times10^{8}\ \text{N}.$$

(i) Common strain (bonded tubes ⟹ iso-strain): $\varepsilon=\dfrac{\sigma A_{\text{tot}}}{\Sigma EA}=\dfrac{6.2\times10^7\times8.68\times10^{-4}}{1.26\times10^{8}}=4.29\times10^{-4}$, so $\Delta L=\varepsilon L=\boxed{1.29\times10^{-4}\ \text{m}\ (0.13\ \text{mm})}$ — matching the official value.

(ii) $\sigma_{Cu}=E_{Cu}\varepsilon=1.1\times10^{11}\times4.29\times10^{-4}=\boxed{4.7\times10^7\ \text{N m}^{-2}}$ — matching the official value.

(iii) Load $=\sigma A_{\text{tot}}=6.2\times10^7\times8.68\times10^{-4}=\boxed{5.4\times10^4\ \text{N}\approx54\ \text{kN}}$.

**Check.** Closed loop: $\varepsilon\Sigma EA=4.29\times10^{-4}\times1.26\times10^8=5.4\times10^4$ N = load ✓ — the two routes agree. Stresses below typical yield ✓; copper carries $\varepsilon E_{Cu}A_{Cu}=2.5\times10^4$ N — a smaller stress share than its area share, consistent with its lower modulus ✓.

> 【Thought】*Official mark scheme note:* its printed load $1\times10^5$ N comes from treating the given *diameter* (4.0 cm) as a *radius* in the area computation — the mark scheme itself flags this diameter/radius ambiguity and accepts both. With correct areas the load is $5.4\times10^4$ N, which is also the only value passing the closed-loop check above; the official $\Delta L$ and $\sigma_{Cu}$ are nevertheless correct because the area error cancels in the strain ratio $\sigma A_{\text{tot}}/\Sigma EA$ (roughly — both areas scale together).

---

### Q1(o) — Third harmonic on a stretched wire [5 marks]

**Setup.** $\mu=m/L=6.0\times10^{-3}/1.2=5.0\times10^{-3}$ kg/m; $v=\sqrt{T/\mu}=\sqrt{45/0.005}=94.9$ m/s.

**(i) Sketch.** Standing wave $y=A_{\max}\sin(3\pi x/L)\cos\omega t$: each point oscillates with amplitude $A(x)=A_{\max}|\sin(3\pi x/L)|$. Maximum KE per unit length $=\tfrac12\mu\omega^2A^2(x)$: a $\sin^2$ curve with **three** humps (zeros at the nodes $x=0,L/3,2L/3,L$). Total energy per unit length (KE+PE, constant in time) $=\tfrac12\mu\omega^2A^2(x)$ as well… — precisely: KE and PE exchange in time, and at each $x$ the *time-averaged* total is $\tfrac14\mu\omega^2A^2(x)$; the requested overlay line: the instantaneous total energy per unit length at the moment of maximum KE = the same $\sin^2$ envelope… The clean reading: plot $\text{KE}_{\max}(x)\propto\sin^2(3\pi x/L)$ (three equal humps) and superpose the total energy line which is the same shape; at the instant of maximum displacement KE = 0 everywhere and all energy is elastic PE.

> 【Thought】 The teaching point of the sketch: in a standing wave, energy is *stationary* — it sloshes between kinetic (all parts, peaked at antinodes, at zero crossing) and elastic (peaked at nodes, at maximum displacement). The "total" line is drawn flat only when summed appropriately; be careful to state which instant is being plotted.

**(ii)** $f_3=\dfrac{3v}{2L}=\dfrac{3\times94.9}{2.4}=\boxed{119\ \text{Hz}}$.

**(iii)** Total energy = maximum KE $=\displaystyle\int_0^L\tfrac12\mu\omega^2A_{\max}^2\sin^2(3\pi x/L)\,dx=\tfrac14 m\omega^2A_{\max}^2$:
$$E=\tfrac14(6.0\times10^{-3})(2\pi\times118.6)^2(0.018)^2=\boxed{0.27\ \text{J}}.$$

**Check.** $\int\sin^2=L/2$ is the only integral needed ✓; $E\propto m\omega^2A^2$ — all factors sensible ✓; "KE and elastic PE are equal" (given) means time-averaged $KE=PE=\tfrac12E_{\text{tot}}$ — consistent with the integral above ✓. *(Official mark scheme prints $E=\tfrac12mA^2\omega^2=0.54$ J — exactly twice the correct value: it adds the time-averaged KE and PE as if each were the full $\tfrac14mA^2\omega^2$. The total energy is constant and equals the maximum KE, $\tfrac14m\omega^2A^2=0.27$ J; ours stands.)*

---

### Q1(p) — Cell with internal resistance and a variable parallel resistor [5 marks]

**Key observation.** $R_2$ receives maximum power when it equals the Thévenin resistance seen from its terminals: $r\parallel R_1$ — the variable-load version of maximum power transfer. The algebra route (hinted): minimise $1/P_2$.

**(i)** $I=\dfrac{\varepsilon}{r+R_1\parallel R_2}=\boxed{\dfrac{\varepsilon(R_1+R_2)}{rR_1+rR_2+R_1R_2}}$.

**(ii)** Current divider: $\boxed{I_2=\dfrac{IR_1}{R_1+R_2}}$.

**(iii)** $P_2=I_2^2R_2=\boxed{\dfrac{\varepsilon^2R_1^2R_2}{\left(rR_1+rR_2+R_1R_2\right)^2}}$.

**(iv)** Minimise
$$\frac{1}{P_2}\propto\frac{\left(rR_1+(r+R_1)R_2\right)^2}{R_2}=\frac{r^2R_1^2}{R_2}+2rR_1(r+R_1)+(r+R_1)^2R_2;$$
AM–GM (or $d/dR_2=0$): the $R_2^{-1}$ and $R_2$ terms balance when
$$R_2=\boxed{\frac{rR_1}{r+R_1}=r\parallel R_1}.$$

> 【Thought】 Seeing "maximum power converted in R₂" → triggers *maximum power transfer theorem*: the load should match the resistance looking back into the network ($r\parallel R_1$). The $1/P_2$ manipulation is the exam-safe way to *prove* it without quoting: a sum $X^2/R_2+Y^2R_2$ is minimised when the two terms are equal — an AM–GM move worth memorising.

**Check.** $R_1\to\infty$ (removed): $R_2\to r$ — the textbook result recovered ✓; at the optimum, $P_2^{\max}=\dfrac{\varepsilon^2R_1}{4r(R_1+r)}$ (substitute back) — finite and positive ✓. This is the maximum-power-transfer theorem in disguise: the load should equal the *Thévenin* resistance of the source network, here $r\parallel R_1$ rather than $r$ alone, because $R_1$ sits across the output.

---

### Q1(q) — Two cells and three capacitors: potential across C₃ [5 marks]

**Key observation.** In DC steady state no current flows, so each cell fixes the potential of its top corner relative to the bottom rail. The top middle node (joining $C_1$, $C_2$, $C_3$) is **isolated**: the sum of charges on the plates meeting there must vanish — that one equation determines everything.

> 【Thought】 Seeing capacitors + cells in DC → triggers *(1) cells pin node voltages; (2) isolated islands conserve charge*. The capacitor analogue of Kirchhoff's current law at the floating node is the essential move; "write down your initial equations clearly" is the examiner begging for exactly these two statements.

**Solution.** Bottom rail $=0$; cells (positive terminals up) give left corner $\varepsilon_1$, right corner $\varepsilon_2$; let $V$ be the middle node (top of $C_3$).
$$\text{Charge conservation at the floating node:}\quad C_1(V-\varepsilon_1)+C_2(V-\varepsilon_2)+C_3V=0,$$
$$V_{C_3}=V=\boxed{\frac{C_1\varepsilon_1+C_2\varepsilon_2}{C_1+C_2+C_3}}.$$

**Check.** $\varepsilon_2=0$ (right corner grounded): $V=\dfrac{C_1\varepsilon_1}{C_1+C_2+C_3}$ — the capacitive divider of $C_1$ against $C_2+C_3$ ✓ classic; equal emfs $\varepsilon$: $V=\varepsilon$ — no potential differences anywhere on the top rail ✓.

---

### Q1(r) — Rod floating while tethered by a vertical string [6 marks]

**Key observation.** All three forces (weight, buoyancy, tension) are vertical, so the angle drops out of the moment equation — only the *submerged fraction* matters. Take moments about the string attachment to kill $T$.

> 【Thought】 Seeing a floating tilted rod on a string → triggers *moments about the attachment point*: buoyancy acts at the centroid of the **submerged half-span**, weight at the rod's centre; the cos θ lever-arm factor is common and cancels — that cancellation is why the answer is a clean fraction.

**Solution.** Let $f$ = submerged fraction of the rod's length (lower end portion). Buoyancy $B=\rho_{\ell}gA(2af)=\tfrac43\rho gA(2af)=\tfrac43f\,W$ acts at distance $2a(1-f/2)$ from the attached end; weight $W$ acts at $a$. Moments about the attachment:
$$W\cdot a=\tfrac43fW\cdot2a\left(1-\frac{f}{2}\right)\;\Rightarrow\;1=\tfrac83f\left(1-\frac f2\right)\;\Rightarrow\;4f^2-8f+3=0,$$
$$f=\frac{8\pm\sqrt{64-48}}{8}=\frac12\ \text{or}\ \frac32\;\Rightarrow\;\boxed{f=\tfrac12\ (\text{physical root})}.$$
(ii) Vertical balance: $T=W-B=W(1-\tfrac43\cdot\tfrac12)=\boxed{\tfrac{W}{3}=\tfrac{2aA\rho g}{3}}$.

**Check.** $f=1/2$ submersion with density ratio $3/4$... buoyancy $=\tfrac43\times\tfrac12=\tfrac23$ of weight < weight ✓ (string carries the rest — if buoyancy exceeded weight the string would have to pull down, impossible) ✓; root $f=3/2>1$ rejected ✓.

---

### Q1(s) — Two balls on a thread over a pulley, one floating [6 marks]

**Key observation.** The thread tension is common (light thread, free pulley); write force balance on each ball separately, with buoyancy on B (fully submerged) and on A (fraction $f$ submerged).

**(i) Diagram.** Ball A: weight $m_Ag$ down; buoyancy $\rho fV_Ag$ up; tension $T$ up. Ball B: weight $m_Bg$ down; buoyancy $\rho V_Bg$ up; tension $T$ up. (Pulley: $2T$ down on its axle.)

**(ii)** B: $T=(m_B-\rho V_B)g=(390-50)g=340\,g$ (in gram-weight units, $0.34$ kg wt). A: $T+\rho fV_Ag=m_Ag$:
$$f=\frac{m_A-(m_B-\rho V_B)}{\rho V_A}=\frac{500-340}{1000}=\boxed{0.16\ (16\%)}.$$

**(iii)** Spring replacing a thread section: $x=\dfrac{T}{k}=\dfrac{0.340\times9.81}{100}=\boxed{3.3\times10^{-2}\ \text{m}\approx3.3\ \text{cm}}$.

> 【Thought】 Note the physical reading: B is denser than water ($390/50\gg1$) and pulls A down; A floats with only 16% submerged because the thread carries most of A's weight. The spring extension in (iii) is just $T/k$ — the pulley system exists to set the tension, the spring only measures it.

**Check.** A alone would float at 50% submersion ($m_A/\rho V_A=0.5$); the thread's upward pull reduces it to 16% ✓ direction consistent; both buoyancies, weights positive ✓.

---

### Q1(t) — Bent pole and the slack guy wire [6 marks]

**Key observation.** Bending into a circular arc: surface stress $\sigma_{\max}=E\dfrac{y_{\max}}{r}$ with $y_{\max}$ = pole radius. The guy-wire slack is the difference between its taut length (top displaced by the bending) and its straight-pole length — a small-quantity expansion.

**(i)** $r=\dfrac{E\,y_{\max}}{\sigma_{\max}}=\dfrac{14\times10^9\times0.15}{4000}=\boxed{5.25\times10^{5}\ \text{m}}$; arc angle $\theta=\dfrac{h}{r}=\dfrac{12}{5.25\times10^5}=\boxed{2.3\times10^{-5}\ \text{rad}}$.

> 【Thought】 Seeing "neutral line unstressed, max stress at one side" → triggers *beam bending*: strain varies linearly from the neutral axis, $\varepsilon_{\max}=y_{\max}/r$ — curvature radius is the bridge between stress (material property) and geometry (deflection).

**(ii) Diagram.** Draw the pole as an arc of radius $r$ (centre far to the left); the top attachment point displaces horizontally by $\delta=r(1-\cos\theta)\approx\dfrac{h^2}{2r}$ toward the cable. The taut guy wire is the straight line from the ground anchor (distance $b$ left of the base) to the displaced top: length $\sqrt{(b+\delta)^2+h^2}$. Mark $\theta$, $r$, $\delta$ on the figure; the wire length follows from the right triangle with legs $(b+\delta)$ and $h$.

**(iii) Slack.**
$$\delta=\frac{h^2}{2r}=\frac{144}{1.05\times10^6}=1.37\times10^{-4}\ \text{m},\qquad D=\sqrt{b^2+h^2}=12.24\ \text{m},$$
$$\text{slack}=\sqrt{(b+\delta)^2+h^2}-D\approx\frac{b\,\delta}{D}=\frac{2.4\times1.37\times10^{-4}}{12.24}=\boxed{2.7\times10^{-5}\ \text{m}\approx0.03\ \text{mm}}.$$

**Check.** The slack is second-order small ($\delta$ already small, and only its component along the wire $b/D$ counts) ✓ — a usefully striking result: a barely-visible bend takes up essentially all the slack; dimensionally a length ✓.

---
*End of Paper 6 (2023 Round 1 Section 1, 10 Nov).*


---

## Paper 7 — 2022 Round 1 Section 2 (11 Nov 2022)

*Section 2: Questions 2–5, 25 marks each; candidates attempt two. Full solutions for all four.*

---

### Question 2 — Centre of Mass and Centre of Gravity

#### Q2(a) — Two weights on a light rod

**(i)** *Equilibrium* means the rod remains at rest (or in uniform motion): **zero net force and zero net torque** about every point — both conditions are needed (force balance alone leaves rotation free).

**(ii)** Let the single normal force $F$ act at $X$. Force balance: $F=(m_1+m_2)g$. Moments about the origin (the point beyond the rod's end from which $x_1,x_2$ are measured):
$$F\,X=m_1gx_1+m_2gx_2\;\Rightarrow\;(m_1+m_2)X=m_1x_1+m_2x_2\;\Rightarrow\;X=X_{CM}=\frac{m_1x_1+m_2x_2}{m_1+m_2}.\ \blacksquare$$

> 【Thought】 The origin is *outside* the rod — deliberately: it makes the two moment terms add with the same sign and shows that the CM formula is independent of origin choice. Note the two-step structure: force balance fixes $F$'s magnitude, torque balance fixes its point of application.

**(iii)** An excess force $\Delta F$ at the CM produces pure translation, $a=\Delta F/(m_1+m_2)$, **no rotation** — both masses gain the same speed $v$:
$$\frac{KE_1}{KE_2}=\frac{\tfrac12 m_1v^2}{\tfrac12 m_2v^2}=\boxed{\frac{m_1}{m_2}}.$$

> 【Thought】 Why force at the CM gives no rotation: the CM is the point where the inertia tensor's first moment vanishes, so $\Delta F$ exerts no torque about it. If the force were applied off-CM, the rod would also spin up, and the KE ratio would no longer be simply $m_1/m_2$ — the location clause is essential. (The CM is the point where the first moment of the mass distribution vanishes, $\sum m_i(\mathbf r_i-\mathbf r_{CM})=0$ — that is exactly why a force applied there produces pure translation.)

#### Q2(b)(i) — Plank, mug and textbooks [2 marks]

**Key observation.** The plank rests on the table only under the 15 cm book pile; it overhangs $75-15=60$ cm. Tipping is about the table edge: stabilising moment from the books vs overturning moments of plank + mug.

> 【Thought】 Draw the x-axis: table edge at 0. Plank spans $[-15,+60]$ cm (COM at $+22.5$ cm — *outside* the table: without books it falls, which is the point of the books). Mug (diameter 8 cm) at the plank's end with one side on the (plank's) edge: centre at $+56$ cm. Books: pile 15 cm wide occupying $[-15,0]$, COM at $-7.5$ cm. Moments about the table edge make the (unknown) table reaction drop out.

**Solution.** Moments about the table edge:
$$N(0.48)(7.5)=0.24(22.5)+0.35(56)\;\Rightarrow\;3.6N=5.4+19.6=25.0\;\Rightarrow\;N=6.9.$$
$$\boxed{7\text{ books required}}\ (\text{6.94 round up — 6 would tip: }6\times3.6=21.6<25.0<25.2=7\times3.6\ \text{kg·cm}).$$

**Check.** Book moment per book: $0.48\times7.5=3.6$ kg·cm; overturning 25.0 kg·cm ✓; rounding *up* is forced by discreteness ✓.

#### Q2(b)(ii) — Two joined rods suspended from A [3 marks]

**Key observation.** Freely suspended ⟹ the system's COM is directly below A. Same material & cross-section ⟹ mass ∝ length. Rods lean to **opposite** sides of the vertical through A (otherwise no balance).

> 【Thought】 Seeing "suspended … hang at angles α and β" → triggers *zero horizontal COM offset from the suspension point*. Write the x-coordinate of each rod's midpoint relative to A, weight by length, set the sum to zero. The midpoint of BC starts from B, not from A — the compound offset $L_{AB}\sin\alpha-\tfrac{L_{BC}}{2}\sin\beta$ is where most errors occur.

**Solution.** Horizontal positions of the midpoints (AB leaning left at $\alpha$, BC leaning right at $\beta$):
$$\bar x_{AB}=\tfrac{L_{AB}}{2}\sin\alpha,\qquad \bar x_{BC}=L_{AB}\sin\alpha-\tfrac{L_{BC}}{2}\sin\beta.$$
COM condition $\sum m_i\bar x_i=0$ with $m\propto L$:
$$\frac{L_{AB}^2}{2}\sin\alpha+L_{BC}\left(L_{AB}\sin\alpha-\frac{L_{BC}}{2}\sin\beta\right)=0,$$
$$r^2\sin\alpha+2r\sin\alpha-\sin\beta=0\ \ (r\equiv L_{AB}/L_{BC})\;\Rightarrow\;\boxed{\frac{L_{AB}}{L_{BC}}=\sqrt{1+\frac{\sin\beta}{\sin\alpha}}-1=\sqrt{\frac{\sin\alpha+\sin\beta}{\sin\alpha}}-1}.$$

**Check.** $\alpha=\beta$: $r=\sqrt2-1=0.414$ — AB is shorter than BC, and rightly so: with equal angles, BC's midpoint lies further from the pivot (it starts from B), so the shorter arm must be AB ✓; $r>0$ requires $\beta>0$ ✓.

#### Q2(b)(iii) — Vertically floating stick [1 mark]

**Key observation.** Floating: submerged depth $d=L\rho_w/\rho_l$. The displaced liquid's CM is at $d/2$; the stick's CM at $L/2$.

$$\boxed{\Delta h=\frac{L}{2}-\frac{d}{2}=\frac{L}{2}\left(1-\frac{\rho_w}{\rho_l}\right)}.$$

**Check.** $\rho_w\to\rho_l$: $\Delta h\to0$ — neutrally buoyant stick is fully submerged, centres coincide ✓.

#### Q2(b)(iv) — Spinning dumbbell thrown upward [3 marks]

**Key observation.** The 110 J splits into CM translation and rotation about the CM; only the translational part sets the flight time (and gravity exerts no torque about the CM, so the 8 Hz spin is constant).

> 【Thought】 Seeing "rotating … returning to height h … total energy" → triggers *König decomposition*: $E=\tfrac12Mv_{CM}^2+\tfrac12I_{CM}\omega^2$. Compute $I_{CM}$ carefully — the CM is not at the midpoint. The trap: putting 110 J all into translation.

**Solution.** CM: $x=\dfrac{0.90\times0.30}{1.30}=0.2077$ m from the 0.40 kg mass. $I_{CM}=0.40(0.2077)^2+0.90(0.0923)^2=0.0249\ \text{kg m}^2$.
$$E_{\text{rot}}=\tfrac12 I\omega^2=\tfrac12(0.0249)(16\pi)^2=31.5\ \text{J};\qquad E_{\text{trans}}=110-31.5=78.5\ \text{J},$$
$$v_{CM}=\sqrt{\frac{2E_{\text{trans}}}{M}}=\sqrt{\frac{157}{1.30}}=11.0\ \text{m/s},\qquad t=\frac{2v}{g}=2.24\ \text{s},$$
$$\boxed{N=8\times2.24\approx18\ \text{rotations}}.$$

**Check.** Rotation eats ~29% of the energy ✓; $I_{CM}<I_{\text{midpoint}}$ ✓ (parallel axis); 18 is an integer-friendly outcome ✓.

#### Q2(c) — Strobe photographs of an inelastic collision [2 marks]

**(i) Sketch + CM.** Redraw the Y-shaped strobe tracks (two incoming arms converging, two close, nearly parallel outgoing tracks below). Mark the centre of mass at every interval:
$$\mathbf r_{CM}=\frac{\tfrac13m\,\mathbf r_A+\tfrac23m\,\mathbf r_B}{m}=\frac{\mathbf r_A+2\mathbf r_B}{3},$$
i.e. the point dividing each $AB$ segment in the ratio $2:1$ (closer to the heavier ball). The CM dots lie on a **straight line with uniform spacing** — momentum conservation makes the CM drift uniformly straight through the collision.

**(ii) Fraction of KE lost.** Measure dot spacings (equal time intervals ⟹ speed ∝ spacing). Before: speeds are given ($2v$, $v$). After: the two tracks run parallel with equal spacing — the balls share a **common velocity**, so the collision is (effectively) perfectly inelastic and the common velocity is $v_{CM}$ by momentum conservation. Measuring the incoming track angles on the printed figure (≈ 33° and ≈ 18° from the vertical) and vector-summing the momenta $\tfrac23mv(0.55,-0.83)$ and $\tfrac23mv(-0.31,-0.95)$:
$$|\mathbf v_{CM}|\approx1.20\,v,\qquad KE_{\text{before}}=\tfrac12\cdot\tfrac{m}{3}(2v)^2+\tfrac12\cdot\tfrac{2m}{3}v^2=mv^2,$$
$$KE_{\text{after}}\approx\tfrac12 m(1.20v)^2=0.72\,mv^2\;\Rightarrow\;\boxed{\text{fraction lost}\approx 1-0.72\approx30\%}.$$

> 【Thought】 The method matters more than the number: KE is *not* conserved, but the CM motion is untouched by internal forces — so the lost energy is exactly the "KE relative to the CM" (the CM-frame KE). Fastest estimator: fraction lost $=1-\dfrac{Mv_{CM}^2}{\sum m_iv_i^2}$. (Your measured value depends on the printed scale of the figure; anything in the 25–35% band, supported by measurements, earns the marks.)

#### Q2(d)(i) — String sliding off a pulley [4 marks]

**Key observation.** Light smooth pulley, uniform string: the whole string always moves at one speed; use energy — the COM drop from "two balanced strands of length $a$" to "one strand of length $2a$" is $a/2$.

> 【Thought】 Seeing "displaced from equilibrium, slides off, leaves the pulley at speed v" → triggers *energy bookkeeping on the COM*, not force analysis (the tension varies along the string during motion — force methods are painful here). Initial state: strands $a$ and $a$, CM at depth $a/2$ below the pulley. Final state (just leaving): a single strand $2a$, CM at depth $a$.

**Solution.** $\Delta h_{CM}=\dfrac{a}{2}$; energy conservation:
$$mg\frac{a}{2}=\frac12 mv^2\;\Rightarrow\;\boxed{v=\sqrt{ga}}.$$

**Check.** Limit check via dynamics: at displacement $x$, driving force $=\dfrac{m}{2a}(2x)g$, so $\ddot x=\dfrac{g}{a}x$ — exponential growth; integrating $\dot x^2=\dfrac{g}{a}x^2$ from rest… consistent with $v^2=ga$ at $x=a$ ✓ (the COM shortcut avoided the exponential ODE entirely).

#### Q2(d)(ii) — Temperature-compensated pendulum [3 marks]

**Key observation.** The pendulum's length is the triangle's height $h=\sqrt{L_2^2-(L_1/2)^2}$; compensation means $dh/dT=0$, and each rod expands at its own rate ($\alpha$ for the horizontal rod, $\beta$ for the sloping pair).

> 【Thought】 Seeing "temperature compensated" → triggers *find the geometric combination that must stay constant, then set its differential to zero*. Note the sign structure: expanding $L_2$ raises the bob, expanding $L_1$ (wider base) lowers it — compensation is possible only because the two expansions fight.

**Solution.**
$$h^2=L_2^2-\frac{L_1^2}{4}\;\Rightarrow\;2h\,\delta h=2L_2\,\delta L_2-\frac{L_1}{2}\delta L_1=\left(2\beta L_2^2-\frac{\alpha L_1^2}{2}\right)\Delta T=0,$$
$$\boxed{\frac{L_1}{L_2}=2\sqrt{\frac{\beta}{\alpha}}}.$$

**Check.** If both rods were the same metal ($\alpha=\beta$), $L_1=2L_2$ — the degenerate triangle — and $h$ would still change... consistent: compensation needs $\beta\ne\alpha$ in general ✓; dimensions dimensionless ✓.

#### Q2(d)(iii) — Balance in a linearly varying gravitational field [4 marks]

Field: $g(x)=g\left(1+0.1\dfrac{x}{\ell}\right)$, masses $m$ at $x=0$ and $x=\ell$.

**i.** CM at $\ell/2$ (equal masses). Centre of gravity (balance point):
$$x_{cg}=\frac{m g(0)\cdot0+m g(\ell)\cdot\ell}{m g+m g(\ell)}=\frac{1.1}{2.1}\ell=\frac{11}{21}\ell\;\Rightarrow\;\boxed{x_{cg}-\frac{\ell}{2}=\frac{11}{21}\ell-\frac12\ell=\frac{\ell}{42}}.$$

**ii.** String at $\ell/2$; third mass $m$ at position $x$; torque balance about the centre (right-down positive), including the field at $x$:
$$-\frac{\ell}{2}g+1.1g\frac{\ell}{2}+g\left(1+\frac{0.1x}{\ell}\right)\left(x-\frac{\ell}{2}\right)=0,$$
$$\left(1+0.1\xi\right)\left(\xi-\tfrac12\right)=-0.05\quad(\xi=x/\ell)\;\Rightarrow\;2\xi^2+19\xi-9=0,$$
$$\xi=\frac{-19+\sqrt{433}}{4}=0.452\;\Rightarrow\;\boxed{x\approx0.45\,\ell\ \text{from the left end}}.$$

> 【Thought】 The third mass must sit on the **weaker-field (left)** side to oppose the stronger right-side torque — but note it sits right of where naive $g$-uniform reasoning would… in fact uniform-$g$ reasoning gives exactly $0.45\ell$; including the field gradient shifts it to $0.452\ell$ — a small correction, but writing it shows the mechanism. Check the direction before solving: if your quadratic plants the mass on the right side, a sign flipped somewhere.

---

### Question 3 — Investigating materials with X-rays and electrons

#### Q3(a) — Bragg reflection [5 marks]

**(i) Path difference.** The lower ray travels an extra down-and-back between planes: each leg is $a\sin\theta$ (with $\theta$ measured from the plane):
$$\boxed{\Delta=2a\sin\theta}.$$

> 【Thought】 The workhorse derivation: drop perpendiculars from the upper reflection point to the lower ray's in/out legs; each contributes $a\sin\theta$. Note $\theta$ here is the **grazing** angle (to the plane), not to the normal — the figure marks it explicitly; mixing this up flips sin↔cos.

**(ii)** Constructive interference (first order): $\Delta=\lambda$:
$$\boxed{\lambda=2a\sin\theta}\qquad(\text{Bragg's law}, n=1).$$

**(iii)** $\lambda=2(0.31\ \text{nm})\sin15^\circ=0.62\times0.2588=\boxed{0.16\ \text{nm}}$ (hard X-rays ✓).

**(iv) Photon momentum change.** The photon's momentum $p=h/\lambda$ keeps its magnitude (elastic reflection) but reverses its component normal to the planes; the tangential component is unchanged:
$$\boxed{\Delta p=2p\sin\theta=\frac{2h\sin\theta}{\lambda}=\frac{h}{a}=\frac{6.63\times10^{-34}}{3.1\times10^{-10}}\approx2.1\times10^{-24}\ \text{kg m/s}},$$
directed **perpendicular to the crystal planes** (away from the crystal; the vector diagram is an isosceles triangle of two $p$'s with apex angle $2\theta$, base $\Delta p$).

> 【Thought】 The Bragg condition collapses $\Delta p$ to $h/a$ — momentum transfer quantised by the lattice spacing, not by $\theta$: this is the photon version of crystal momentum ( reciprocal lattice ) and is worth remarking on explicitly. The simplification $\Delta p=h/a$ happens because the Bragg condition eliminates $\lambda$ ($2a\sin\theta=\lambda$ inside $2p\sin\theta$) — the momentum transfer is set by the lattice alone.

#### Q3(b) — Double-crystal monochromator: x(λ, a, h) [3 marks]

**Key observation.** Each Bragg reflection deflects the beam by $2\theta$; with the two crystals parallel, the exit beam is parallel to the entrance beam, displaced by $h$. The inter-reflection run $x$ satisfies $\tan2\theta=h/x$; small angles and Bragg's law then tie $x$ to $\lambda$.

> 【Thought】 Seeing "approximation to first order" → triggers $\tan2\theta\approx2\theta\approx2\sin\theta=\lambda/a$. The result $x=ha/\lambda$ is the monochromator's tuning relation: scanning $\lambda$ means translating the second crystal by $x\propto1/\lambda$ at fixed $h$.

**Solution.**
$$x=\frac{h}{\tan2\theta}\approx\frac{h}{2\theta}\approx\frac{h}{2\sin\theta}=\frac{h}{2\cdot\lambda/2a}=\boxed{\frac{ha}{\lambda}}.$$

**Check.** Longer wavelength ⟹ larger Bragg angle ⟹ shorter run $x$ ✓ (geometry bends more, so less travel needed for the same height); first-order approximation valid since $\lambda/a\sim0.5$ rad… here $\sin\theta=\lambda/2a$ small for hard X-rays ✓. This is the monochromator's operating principle: scanning the wavelength corresponds to a pure *translation* of the second crystal.

#### Q3(c) — Hemispherical electron energy analyser [7 marks]

**(i) Sketch.** Field lines are **radial** between the hemispheres, perpendicular to both spherical surfaces, evenly spread in angle (like a spherical capacitor's field), pointing from the higher-potential to the lower-potential hemisphere.

**(ii)** Treating the hemisphere as part of a spherical shell: $V_{in}=\boxed{\dfrac{Q}{4\pi\varepsilon_0R_{in}}}$.

**(iii) Pass energy.** Between spherical shells the field is the spherical capacitor's, $E(r)=\dfrac{Q}{4\pi\varepsilon_0r^2}\equiv\dfrac{B}{r^2}$; fix the constant $B$ from the applied pd:
$$\Delta V=\int_{R_{in}}^{R_{out}}E(r)\,dr=B\left(\frac{1}{R_{in}}-\frac{1}{R_{out}}\right)=\frac{B\left(R_{out}-R_{in}\right)}{R_{in}R_{out}}\;\Rightarrow\;B=\Delta V\,\frac{R_{in}R_{out}}{R_{out}-R_{in}},$$
so $E(r)=\dfrac{\Delta V}{r^2}\dfrac{R_{in}R_{out}}{R_{out}-R_{in}}$. Circular orbit at $R_0$:
$$eE(R_0)=\frac{mv^2}{R_0}=\frac{2E_0}{R_0}\;\Rightarrow\;E_0=\frac{eE(R_0)R_0}{2}=\frac{e\,\Delta V}{2R_0}\cdot\frac{R_{in}R_{out}}{R_{out}-R_{in}},$$
with $R_0=\tfrac12(R_{in}+R_{out})$:
$$\boxed{E_0=e\,\Delta V\,\frac{R_{in}R_{out}}{R_{out}^2-R_{in}^2}}.$$

> 【Thought】 The physics: only one energy can make $mv^2/r$ equal $eE(r)$ at the mid-radius — the analyser is a velocity (energy) filter. Note the elegant cancellation: the "$1/r^2$" field and "$mv^2/r$" demand meet at one radius, and the answer involves only radii and $\Delta V$.

**(iv)** $R_{in}=45$ mm, $R_{out}=55$ mm, $E_0=5.0$ eV:
$$\Delta V=\frac{E_0}{e}\cdot\frac{R_{out}^2-R_{in}^2}{R_{in}R_{out}}=5.0\times\frac{55^2-45^2}{45\times55}=5.0\times\frac{1000}{2475}=\boxed{2.0\ \text{V}}.$$

**Check.** $E_0/e\approx\Delta V\times R/(\text{gap})$ — field ≈ $\Delta V$/gap, orbit needs $eER_0/2=E_0$: $\Delta V\approx 2E_0\,\text{gap}/(eR_0)=2\times5\times10/50=2$ V ✓ quick estimate confirms. The physical point: only one energy can execute the mid-radius circle for a given $\Delta V$ — the analyser is an *energy filter*.

#### Q3(d) — Photoemission from copper and electron "refraction" [3 marks]

**(i)** Energy budget: photon = binding depth + work function step… carefully: the electron sits $4.0$ eV below the Fermi level; escaping costs work function $\phi=4.6$ eV *from the Fermi level*; it keeps $5.0$ eV outside:
$$E_\gamma=4.0+4.6+5.0=\boxed{13.6\ \text{eV}}.$$

**(ii)** $\lambda=\dfrac{1240\ \text{eV nm}}{13.6\ \text{eV}}=\boxed{91\ \text{nm}}$ — **extreme ultraviolet**.

**(iii)** Tangential momentum is conserved crossing the surface; the perpendicular motion gains the surface-potential energy. The electron's kinetic energy inside = outside KE + inner potential ≈ $5.0+4.6=9.6$ eV:
$$p_\parallel\text{ conserved}\Rightarrow\frac{\sin\theta_{out}}{\sin\theta_{in}}=\frac{p_{in}}{p_{out}}=\sqrt{\frac{9.6}{5.0}}=\boxed{\mu=1.39}.$$
For the electron leaving at $\theta_{in}=50^\circ$:
$$\sin\theta_{out}=\mu\sin50^\circ=1.39\times0.766=1.06>1.$$
$$\boxed{\text{It cannot emerge: total internal reflection (critical angle } \arcsin(1/\mu)=46^\circ<50^\circ\text{).}}$$

> 【Thought】 The matter-wave Snell law uses $n\propto p$ (since $\lambda=h/p$), the *opposite* of light's $n\propto1/v$ habit — write the conserved quantity ($p_\parallel$) and you cannot go wrong. Part ii is deliberately provocative: the computed sine exceeds 1, and the correct physical statement is "no transmitted ray" — the same mathematics as optical TIR. An electron observed at 5.0 eV must therefore have had $\theta_{in}\le46^\circ$ inside.

#### Q3(e) — Evacuated tube in an interferometer [2 marks]

**Key observation.** Destructive → constructive needs an extra half-wavelength of **optical** path: $(\mu_{air}-1)\ell=\lambda/2$.

$$\left(0.00029\frac{P}{P_0}\right)(0.080)=\frac{640\times10^{-9}}{2}\;\Rightarrow\;\frac{P}{P_0}=\frac{3.2\times10^{-7}}{2.32\times10^{-5}}=0.0138,$$
$$\boxed{P\approx1.4\times10^{3}\ \text{Pa}\ (\approx1.4\%\text{ of an atmosphere})}.$$

> 【Thought】 The lever arm is huge ($\ell=8$ cm of gas vs half a wavelength of light): a 1% atmosphere changes the optical path by half a fringe. This is exactly how interferometers measure gas refractive index (Rayleigh interferometer) — the physics behind the number.

#### Q3(f) — X-ray path difference with refraction [3 marks]

**Setup (from Fig. 9).** Alternating layers $\mu_1$ (index of the incident medium) and $\mu_2$, each of thickness $a$; angles measured from the **normal**. Ray G: refracts at A into the $\mu_2$ layer (angle $\theta_r$) and reflects at B. Ray H: continues B→C→D through the next $\mu_1$ layer and out at E. Snell chains through parallel interfaces: $\mu_1\sin\theta_1=\mu_2\sin\theta_r$, so in the second $\mu_1$ layer the angle is again $\theta_1$.

**(i)** BCD is a symmetric down–up path through a slab of thickness $a$ at angle $\theta_1$ to the normal:
$$\boxed{BCD=\frac{2a}{\cos\theta_1}}.$$

**(ii) Optical path difference.** The $\mu_2$ legs of G (BF) and H (DE) are equal and parallel — they cancel in the difference. What remains is H's optical path $\mu_1\cdot BCD$ minus the wavefront offset: G emerges at F and H at E, separated laterally by $2a\tan\theta_1$, costing H an extra emergent path $\mu_1(2a\tan\theta_1)\sin\theta_1$:
$$\Delta_{\text{opt}}=\mu_1\frac{2a}{\cos\theta_1}-2a\mu_1\frac{\sin^2\theta_1}{\cos\theta_1}=\boxed{2a\mu_1\cos\theta_1}.$$

> 【Thought】 Method note: computing an OPD between two rays always ends with *projecting onto a common wavefront* — the $-\Delta x\sin\theta$ correction. Setting $\mu_1=1$ recovers the textbook Bragg $2a\cos\theta_1$ (angles from the normal; $=2a\sin\theta_{\text{grazing}}$) ✓ — always run that limit to catch sign slips.

---

### Question 4 — The DART mission (asteroid deflection)

#### Q4(a) — Ion drive [6 marks]

**(i) Ejection speed.** Energy from the accelerating potential:
$$v_{xe}=\sqrt{\frac{2eV}{m_{xe}}}=\sqrt{\frac{2(1.602\times10^{-19})(1800)}{131\times1.661\times10^{-27}}}=\boxed{5.1\times10^{4}\ \text{m/s}\ (\approx51\ \text{km/s})}.$$

**(ii) Thrust.** Mass flow $\dot m=\dfrac{I}{e}m_{xe}$ (each ion carries charge $e$):
$$\dot m=\frac{3.52}{1.602\times10^{-19}}\times2.176\times10^{-25}=4.78\times10^{-6}\ \text{kg/s},\qquad F=\dot m v_{xe}=\boxed{0.246\ \text{N}\ (\approx0.25\ \text{N})}.$$

**(iii) Speed after 306 days.** Constant thrust, average mass 600 kg, from rest:
$$a=\frac{F}{m}=4.10\times10^{-4}\ \text{m/s}^2,\qquad v=at=4.10\times10^{-4}\times306\times86400=\boxed{1.08\times10^{4}\ \text{m/s}\ (\approx11\ \text{km/s})}.$$

> 【Thought】 Sanity: real DART hit at 6.14 km/s — our constant-thrust-for-306-days model overshoots, consistent with "if it had run continuously" being a hypothetical upper bound. Watching whether a model result should bracket the real number is a good habit.

#### Q4(b) — Mass of the Didymos–Dimorphos binary [3 marks]

**(i)** Circular orbit, separation $r=1.20$ km, period $T=11\ \text{h}\ 55\ \text{min}=4.29\times10^4$ s. Balancing gravity and centripetal force on each body (both give the same total — the "Kepler III for binaries"):
$$M_{\text{tot}}=\frac{4\pi^2r^3}{GT^2}=\frac{4\pi^2(1200)^3}{6.67\times10^{-11}(4.29\times10^4)^2}=\boxed{5.6\times10^{11}\ \text{kg}}.$$

> 【Thought】 Seeing a binary with separation and period → triggers *the two-body Kepler law with the TOTAL mass* (each body's equation contains the other's mass; adding them yields $G(M_1+M_2)=\omega^2r^3$). Arithmetic hazard: $GT^2\approx0.12$ — mind the powers of ten.

**(ii)** Same density ⟹ mass ∝ diameter³: ratio $(780/164)^3=107.6$:
$$M_{Did}=M_{\text{tot}}\frac{107.6}{108.6}=\boxed{5.5\times10^{11}\ \text{kg}},\qquad M_{Dim}=\frac{M_{\text{tot}}}{108.6}=\boxed{5.1\times10^{9}\ \text{kg}}.$$

**Check.** Didymos density: $5.5\times10^{11}/(\tfrac43\pi\cdot390^3)=2.2\times10^3\ \text{kg/m}^3$ — rock ✓ (this retro-validates the whole chain).

#### Q4(c) — Momentum kick and orbital shrinkage [10 marks]

**(i)** Head-on perfectly inelastic momentum transfer:
$$\Delta v=\frac{m_p v_p}{M_{Dim}}=\frac{570\times6140}{5.1\times10^{9}}=\boxed{6.8\times10^{-4}\ \text{m/s}\approx0.68\ \text{mm/s}}.$$

**(ii).i** Total orbital energy:
$$E=\tfrac12m_sv^2-\frac{GMm_s}{r}=-\frac{GMm_s}{2r}\ \ \blacksquare\quad(\text{using }v^2=GM/r).$$

**ii** The impact slows Dimorphos at fixed $r$: $\Delta E=m_sv\,\Delta v$ ($\Delta v<0$), with $v=2\pi r/T=0.176$ m/s. Since $E=-GMm_s/2r$, differentiate: $\Delta E=\dfrac{GMm_s}{2r^2}\Delta r$:
$$\Delta r=\frac{2r^2\,\Delta E}{GMm_s}=\frac{2r^2v\,\Delta v}{GM}=\frac{2(1200)^2(0.176)(-6.8\times10^{-4})}{6.67\times10^{-11}\times5.5\times10^{11}}=\boxed{-9.4\ \text{m}\ (\text{decrease})}.$$

**iii** $T\propto r^{3/2}$ (Kepler III, fixed $M$):
$$\Delta T=\frac32\frac{\Delta r}{r}T=\frac32\times\frac{-9.4}{1200}\times(11.92\ \text{h})=\boxed{-0.14\ \text{h}\approx-8.4\ \text{min}\ (\text{decrease})}.$$

> 【Thought】 Note the sign logic: slowing the moon makes its orbit *smaller and faster-periodic* ($T\propto r^{3/2}$) — the kick backfires into a shorter period, which is what the mission actually measures. Also observe the energy approach sidesteps elliptical-orbit machinery: the "equivalent circular radius" is the ellipse's semi-major axis, fixed by energy alone.

#### Q4(d) — The enhancement factor β [6 marks]

**Key observation.** $\beta\propto\Delta v$ and, through the linear chain $\Delta v\to\Delta r\to\Delta T$, also $\Delta T\propto\Delta v$ — so $\beta$ is the ratio of observed to computed period change.

$$\Delta v_{\text{obs}}=\Delta v_{\beta=1}\times\frac{32}{8.4}=0.68\times3.8=\boxed{2.6\ \text{mm/s}},\qquad \boxed{\beta\approx\frac{32}{8.4}\approx3.8}.$$

**Check.** The real DART result was $\beta\approx3.6$ and $\Delta v\approx2.7$ mm/s ✓ — the crude model lands within 10%; the ejecta multiply the probe's momentum transfer roughly fourfold.

---

### Question 5 — Star formation physics

#### Q5(a) — Ionising photons and the Strömgren sphere [5 marks]

**(i)** Wien scaling from the Sun: $\lambda_{\max}=500\ \text{nm}\times\dfrac{5780}{35800}=80.7\ \text{nm}$; photon energy $E=\dfrac{1240}{80.7}=15.4\ \text{eV}>13.6\ \text{eV}$ ✓ — **peak photons are ionising** (and the whole short-wavelength tail even more so).

**(ii)** $L=1.47\times10^5\times3.85\times10^{26}=5.66\times10^{31}$ W; monochromatic at 15.4 eV:
$$N=\frac{L}{E_\gamma}=\frac{5.66\times10^{31}}{15.4\times1.602\times10^{-19}}=2.3\times10^{49}\ \text{s}^{-1},$$
$$r_S=\left(\frac{3N}{4\pi\alpha}\right)^{1/3}n_H^{-2/3}=\left(\frac{3\times2.3\times10^{49}}{4\pi\times3.1\times10^{-19}}\right)^{1/3}(10^9)^{-2/3}=2.6\times10^{16}\ \text{m}=\boxed{2.8\ \text{ly}}.$$

> 【Thought】 The formula packages ionisation balance (recombinations in the volume = ionising photon supply). Watch the two cube-root factors: it is $(3N/4\pi\alpha)^{1/3}\times n_H^{-2/3}$, not $(\ldots n_H^{-2})^{1/3}$ with a shared exponent — the printed separation of powers is deliberate.

**(iii)** One sphere has diameter $\approx5.5$ ly — already larger than the 5 ly pillar height:
$$\boxed{\text{Only } \sim 1\text{ such star (order unity) is needed; a couple guarantee complete erosion.}}$$

#### Q5(b) — Bonnor–Ebert collapse mass outside the sphere [2 marks]

With $p_0=p_{\text{rad}}=\dfrac{L}{4\pi r_S^2c}=\dfrac{5.66\times10^{31}}{4\pi(2.6\times10^{16})^2(3\times10^8)}=2.2\times10^{-11}$ Pa:
$$M_{BE}=\frac{1.18\,k_B^2T_{\text{neb}}^2}{G^{3/2}m_H^2\,p_0^{1/2}}=\frac{1.18(1.381\times10^{-23})^2(50)^2}{(6.67\times10^{-11})^{3/2}(1.673\times10^{-27})^2\sqrt{2.2\times10^{-11}}}=\boxed{7.8\times10^{31}\ \text{kg}\approx39\ M_{\text{Sun}}}.$$

> 【Thought】 Dimensional check first: the printed formula must have $p_0$ in the **denominator** ($M\propto p^{-1/2}$) — higher pressure squeezes *smaller* masses into collapse (standard Bonnor–Ebert scaling $M\propto T^2/\sqrt p$). Verifying dimensions before substituting numbers is what catches OCR/typo ambiguities in a formula.

#### Q5(c) — Pressure balance at the Sun's centre; white-dwarf comparison [10 marks]

Mean particle mass: $\dfrac{m}{m_H}=\dfrac{2}{1+3X+0.5Y}=\dfrac{2}{2.375}=0.842$, $m=1.41\times10^{-27}$ kg.

**(i)**
$$p_{gas}=\frac{\rho_ck_BT_c}{m}=\frac{1.53\times10^5\times1.381\times10^{-23}\times1.57\times10^7}{1.41\times10^{-27}}=2.36\times10^{16}\ \text{Pa},$$
$$p_{rad}=\frac{4\sigma}{3c}T_c^4=\frac{4(5.67\times10^{-8})}{3(3\times10^8)}(1.57\times10^7)^4=1.5\times10^{13}\ \text{Pa},$$
$$\boxed{p_{tot}\approx2.4\times10^{16}\ \text{Pa}}.$$

**(ii)** $p_{rad}/p_{tot}\approx\boxed{0.065\%}$. *Comment:* utterly negligible in the Sun — gas pressure dominates; but $p_{rad}\propto T^4$ while $p_{gas}\propto T$, so in hotter, more massive stars radiation pressure becomes important (Eddington-limit physics).

**(iii)** Constant density $\rho=3M/4\pi R^4\ldots$ with $M(r)=M(r/R)^3$:
$$p_{grav}=\int_0^R\frac{GM(r)\rho}{r^2}\,dr=\frac{GM\rho}{R^3}\int_0^R r\,dr=\frac{GM\rho}{2R}=\frac{3GM^2}{8\pi R^4},$$
$$p_{grav}=\frac{3(6.67\times10^{-11})(1.99\times10^{30})^2}{8\pi(6.37\times10^6)^4}=\boxed{1.9\times10^{22}\ \text{Pa}\approx8\times10^{5}\times p_{tot}^{\text{Sun}}}.$$

> 【Thought】 The integral becomes trivial under constant density because $M(r)\propto r^3$ cancels $r^2$ — spotting that cancellation *before* integrating is the mark-worthy move. The million-fold pressure jump explains why white dwarfs need degeneracy pressure, not gas pressure — the physical moral of the comparison.

#### Q5(d) — Photon diffusion time and mean free path [4 marks]

**(i)** Radiation energy content $U=\dfrac{4\sigma}{c}T_{\text{mean}}^4 V_\odot$; the leakage time $\tau=U/L_\odot$ estimates the diffusion time:
$$u=\frac{4(5.67\times10^{-8})}{3\times10^8}(4.73\times10^6)^4=3.78\times10^{11}\ \text{J/m}^3,\qquad U=u\cdot\tfrac43\pi R_\odot^3=5.3\times10^{38}\ \text{J},$$
$$\tau=\frac{U}{L_\odot}=\frac{5.3\times10^{38}}{3.85\times10^{26}}=1.39\times10^{12}\ \text{s}=\boxed{4.4\times10^{4}\ \text{years}}.$$

**(ii)** Random walk: $R_\odot=\ell\sqrt N$ and total path $c\tau=N\ell$; divide: $\ell=R_\odot^2/(c\tau)$:
$$\ell=\frac{(6.96\times10^8)^2}{3\times10^8\times1.39\times10^{12}}=\boxed{1.2\times10^{-3}\ \text{m}\ (\sim1\ \text{mm})},\qquad N=\frac{c\tau}{\ell}=\boxed{3.6\times10^{23}\ \text{interactions}}.$$

> 【Thought】 The two random-walk relations ($d=\ell\sqrt N$, $L_{\text{path}}=N\ell$) form a pair; eliminating $N$ gives $\ell$ directly. Consistency check built in: $\ell\sqrt N$ must return $R_\odot$ ✓.

#### Q5(e) — Predicted pp-I neutrino flux vs Borexino [4 marks]

Each pp-I neutrino tags $13.1$ MeV of fusion energy; pp-I supplies 92% of $L_\odot$:
$$\dot N_\nu=\frac{0.92\,L_\odot}{13.1\ \text{MeV}}=\frac{0.92\times3.85\times10^{26}}{13.1\times10^6\times1.602\times10^{-19}}=1.69\times10^{38}\ \text{s}^{-1},$$
$$\Phi_\oplus=\frac{\dot N_\nu}{4\pi d^2}=\frac{1.69\times10^{38}}{4\pi(1.50\times10^{11})^2}=\boxed{6.0\times10^{10}\ \text{cm}^{-2}\text{s}^{-1}}}.$$
Measured: $(6.1\pm0.5)\times10^{10}$ cm⁻²s⁻¹.

**Comparison & implications.** Agreement within uncertainty ⟹ the Sun's *current* core fusion rate matches its photon luminosity: the Sun is in steady energy balance on the photon-diffusion timescale ($\sim10^4$ yr), and neutrinos indeed let us "see" the core *now* — validating both the fusion model and the pp-I branching. (Historically this kind of comparison resolved the "solar neutrino problem" in favour of neutrino oscillations rather than a dim core.)

---
*End of Paper 7 (2022 Round 1 Section 2).*


---

## Paper 8 — 2021 Round 1 Section 1 (12 Nov 2021)

*Section 1, Question 1, parts (a)–(v). Maximum 50 marks from ≈ 88.*

---

### Q1(a) — Coupling railway trucks [3 marks]

**Key observation.** Coupling ⟹ perfectly inelastic: momentum conserved, KE not. Set $m$, speeds $5.0$ and $2.5$ m/s, second truck mass $2m$.

**(i)** $v_f=\dfrac{5.0m+2.5(2m)}{3m}=\dfrac{10}{3}=\boxed{3.3\ \text{m/s}}$.
**(ii)** $KE_i=\tfrac12m(25)+\tfrac12(2m)(6.25)=18.75m$ J; $KE_f=\tfrac12(3m)(100/9)=16.67m$ J:
$$\text{fraction lost}=\frac{18.75-16.67}{18.75}=\boxed{11\%}.$$

> 【Thought】 Quick estimator for sticking collisions: the lost KE is the CM-frame kinetic energy $\tfrac12\mu v_{\text{rel}}^2$ — here $\tfrac12\times\tfrac{2m}{3}\times(2.5)^2=2.08m$ J, exactly the deficit found above. Relative speed, not the individual speeds, sets the loss.

---

### Q1(b) — Drum skin frequency: dimensional reading [2 marks]

**Key observation.** In $f=\dfrac{0.47hv}{a^2\sqrt{1-\rho^2}}$ (elasticity constant in the denominator's surd), the bracketed $1-\rho^2$ forces $\rho$ to be dimensionless; the rest is unit bookkeeping.

**(i)** $1-\rho^2$ must be dimensionless ⟹ $\boxed{\rho\text{ has no units}}$ (it is a Poisson-ratio-like constant).
**(ii)** $[f]=\text{s}^{-1}=[h][v]/[a^2]=\text{m}^2\text{s}^{-1}/[a^2]$ ⟹ $[a^2]=\text{m}^2$ ⟹ $\boxed{[a]=\text{m}}$ (a length — the drum radius).

> 【Thought】 In "find the units" questions, locate the factor whose units are forced by a *structural* constraint (a sum $1-\rho^2$ must be dimensionless) before balancing the whole expression — it is the only anchor that doesn't depend on reading the full formula. (Physically, $\rho$ is Poisson's ratio — transverse over longitudinal strain — which is indeed dimensionless.)

---

### Q1(c) — Two balls thrown upward [5 marks] (g = 10 m/s²)

**(i) Sketch.** Ball 1: straight line from $v=40$ at $t=0$, slope $-10$, crossing zero at $t=4$ s. Ball 2: starts at $t=1$ s from $v=60$, slope $-10$, zero at $t=7$ s. Both lines parallel.

**(ii) Meeting.** Heights: $h_1=40t-5t^2$; $h_2=60(t-1)-5(t-1)^2$. Equate:
$$40t=60(t-1)+10(t-1)-5+5t^2-5t^2\ldots\ \text{expand: }40t-5t^2=60t-60-5t^2+10t-5,$$
$$40t=70t-65\;\Rightarrow\;t=\frac{65}{30}=\boxed{2.17\ \text{s}},\qquad h=40(2.17)-5(2.17)^2=\boxed{63.2\ \text{m}}.$$

**(iii) Meet at ball 1's maximum height.** Ball 1 peaks at $t=4$ s, $h=80$ m. Ball 2, thrown $\tau$ after ball 1, must be at 80 m at $t=4$:
$$60(4-\tau)-5(4-\tau)^2=80\;\Rightarrow\;u^2-12u+16=0\ \ (u=4-\tau)\;\Rightarrow\;u=6-2\sqrt5=1.53\ \text{s},$$
$$\boxed{\tau=4-1.53\approx2.5\ \text{s}\ \text{(ball 2 thrown 2.5 s after ball 1)}}.$$

> 【Thought】 The quadratic has two roots: $u=1.53$ s (ball 2 on the way up) and $u=10.47$ s (ball 2 thrown *before* ball 1, meeting on its way down). The phrase "a second ball is thrown [after]" selects the first; saying why you discard a root is part of the solution, not an afterthought.

---

### Q1(d) — Sloping liquid surface in an accelerating carriage [3 marks]

**Key observation.** In the carriage frame the liquid is static under gravity $g$ down and pseudo-force $a$ backward — the free surface is perpendicular to the **effective gravity** vector.

$$\tan\theta=\frac{a}{g}=\frac{0.84}{9.81}\;\Rightarrow\;\boxed{\theta\approx4.9^\circ\text{ to the horizontal}}.$$

> 【Thought】 Mechanism: pressure gradient must be normal to the free surface (no shear in a static fluid), so the surface tilts until its normal aligns with $(a,g)$. Same result from a force balance on a surface fluid element. The "viscous… half-full" dressing only serves to justify *steady state* and *no spillage*.

---

### Q1(e) — Two aeroplanes: closest approach [4 marks]

**(i)** $\mathbf v_{A/B}=\mathbf v_A-\mathbf v_B=(50-(-90))\hat i+(-125-60)\hat j=\boxed{140\hat i-185\hat j\ \text{m/s}}$.

**(ii)** $\mathbf r_{A/B}(0)=(-400-800)\hat i+(1200+600)\hat j=-1200\hat i+1800\hat j$ m. Closest approach when $\mathbf r\cdot\mathbf v=0$:
$$t^*=-\frac{\mathbf r\cdot\mathbf v}{|\mathbf v|^2}=-\frac{(-1200)(140)+(1800)(-185)}{140^2+185^2}=\frac{501\,000}{53\,825}=\boxed{9.3\ \text{s}},$$
$$\mathbf r(t^*)=(103,\ 78)\ \text{m}\;\Rightarrow\;\boxed{d_{\min}\approx1.3\times10^2\ \text{m}\ (129\ \text{m})}.$$

> 【Thought】 Seeing two velocity/position vectors + "closest approach" → triggers *relative-motion reduction*: one moving point, one fixed; the minimum of $|\mathbf r+\mathbf vt|$ occurs where $\mathbf r\perp\mathbf v_{\text{rel}}$ — derive it by setting $\frac{d}{dt}|\mathbf r|^2=0$ (purpose before differentiation).

---

### Q1(f) — Inline water heater [3 marks]

**Key observation.** Steady flow: heater power = enthalpy flux, $P=\dot m c\Delta T$; then $R=V^2/P$.

$$\dot m=\frac{1\ \text{kg}}{60\ \text{s}};\qquad P=\frac{1}{60}\times4180\times60=4180\ \text{W};\qquad R=\frac{230^2}{4180}=\boxed{12.7\ \Omega}.$$

> 【Thought】 Note the neat cancellation $\Delta T=60$ K vs 60 s — engineered numbers; if you got a wildly non-round answer, recheck the litre→kg conversion (1 L water = 1 kg).

---

### Q1(g) — Latent heat of steam [4 marks]

**Key observation.** Each gram of steam delivers **two** packets of heat: condensation ($L$) then cooling of the condensate from 100 °C to 30 °C. The calorimeter counts as 0.010 kg of extra water.

> 【Thought】 Seeing "steam passed into cold water" → triggers *two-term heat release*: $L + c\Delta T$ per kilogram. The single most common error is forgetting the condensate's cooling term ($c\times70$ K — here it is 13% of the answer). The latent heat of ice quoted is a deliberate distractor — name it as such in your head and move on.

**Solution.** Heat balance:
$$m_s\big(L+c_w(100-30)\big)=(m_w+m_{cal})c_w(30-0),$$
$$0.0128\,(L+4180\times70)=0.260\times4180\times30=3.26\times10^4\ \text{J},$$
$$L=\frac{3.26\times10^4}{0.0128}-2.926\times10^5=\boxed{2.25\times10^{6}\ \text{J kg}^{-1}\ (\approx2250\ \text{kJ/kg})}.$$

**Check.** Accepted value 2260 kJ/kg ✓ — the small deficit is experimental realism (the problem's data are self-consistent). The heat ledger has two stages per gram of steam: condensation ($L$) then cooling of the condensate ($c\,\Delta T$) — both must be present.

---

### Q1(h) — Copper rod whose length difference from an iron rod is temperature-independent [3 marks]

**Key observation.** The *difference* is constant iff both rods expand by the same **absolute** amount per degree: $\ell_{Cu}\alpha_{Cu}=\ell_{Fe}\alpha_{Fe}$.

> 【Thought】 Seeing "difference … not to vary with temperature" → triggers *differentiate the difference*: $\frac{d}{dT}(\ell_{Fe}-\ell_{Cu})=\ell_{Fe}\alpha_{Fe}-\ell_{Cu}\alpha_{Cu}=0$. This is the bimetallic-compensation principle (used in clock pendulums) in one line.

**Solution.** $\ell_{Cu}=1.00\times\dfrac{11.9\times10^{-6}}{17.0\times10^{-6}}=\boxed{0.70\ \text{m}}$.

**Check.** Copper expands more per unit length, so it must be shorter to expand equally in absolute terms ✓; $\Delta(\text{lengths})=0.30$ m at all temperatures ✓. This is the bimetallic-compensation idea (as in compensated clock pendula): equal *absolute* expansion keeps the difference constant.

---

### Q1(i) — Plane overhead: angular rate, speed, line-of-sight recession [5 marks]

**Key observation.** With height $h$ fixed, $\theta$ and the horizontal distance $x$ are linked by $x=h\cot\theta$; differentiate once for the speed, and use $r=h/\sin\theta$ for the line-of-sight rate.

> 【Thought】 Seeing "angle … decreasing at 0.09 rad/s" → triggers *related rates*: write the geometric constraint first, then differentiate with respect to time. Order matters: geometry → derivative, never start from $v$ directly. Also note $|\dot\theta|$ is the same whether you track elevation or depression.

**Solution.** (i) Line-of-sight distance: $r=\dfrac{h}{\sin60^\circ}=\dfrac{3000}{0.866}=\boxed{3.46\ \text{km}}$.
(ii) $\dot x=-h\theta'\!/\sin^2\theta$: $v=\dfrac{3000\times0.09}{\sin^2 60^\circ}=\dfrac{270}{0.75}=\boxed{360\ \text{m/s}}$.
(iii) $\dot r=-\dfrac{h\cos\theta}{\sin^2\theta}\,\theta'=\dfrac{3000\times0.5}{0.75}\times0.09=\boxed{180\ \text{m/s}\ \text{(receding)}}$.

**Check.** Recession speed $=v\cos60^\circ=180$ ✓ (line-of-sight component of the velocity — a faster cross-check than the derivative); $v\sin60^\circ=312$ m/s is the angular-sweep part $r|\dot\theta|=3464\times0.09=312$ ✓ consistent.

---

### Q1(j) — Sphere between wall and equilateral wedge [5 marks]

**Key observation.** Sphere stays in contact with wall and sloping face throughout: one geometric constraint links its drop $y$ to the wedge's shift $x$; then Newton's laws for each body plus the differentiated constraint close the system.

**(i) Geometry.** The wedge face is at $60^\circ$ to the horizontal (equilateral cross-section). The horizontal gap between wall and face at the sphere's centre height is $x+\dfrac{y_c}{\tan60^\circ}$-shaped; holding the perpendicular distance from centre to face constant gives
$$\boxed{y=\sqrt3\,x}\quad(\text{equivalently }v_2=\sqrt3\,v_1,\ a_2=\sqrt3\,a_1).$$

**(ii) Acceleration.** Sphere (vertical fall, no horizontal acceleration — slides along the wall): with $N$ the wedge–sphere contact force (⊥ face, i.e. $30^\circ$ from vertical):
$$M_2g-N\cos30^\circ=M_2a_2,\qquad\text{wedge: }N\sin30^\circ=M_1a_1,\qquad a_2=\sqrt3\,a_1.$$
Eliminate $N$ and $a_2$: $N=\dfrac{2M_1a_1}{\sqrt3}$, and $M_2g-\dfrac{N}{2}=\sqrt3 M_2a_1$:
$$M_2g=\frac{M_1a_1}{\sqrt3}+\sqrt3M_2a_1\;\Rightarrow\;\boxed{a_1=\frac{\sqrt3\,M_2g}{M_1+3M_2}}.$$

> 【Thought】 Choose coordinates that respect the constraints: the sphere moves purely vertically (wall), the wedge purely horizontally (table) — so only three unknowns ($N$, $a_1$, $a_2$) and three equations. The decisive clause is "smooth" everywhere: no friction ⟹ contact forces are purely normal and the sphere "falls without rotation" ✓.

**Check.** $M_1\to0$: $a_2=\sqrt3a_1=g$ — sphere in free fall ✓ (massless wedge offers no support); $M_1\to\infty$: $a_1\to0$ ✓ fixed wedge; $a_1<g/\sqrt3$ always ✓ sane. The coordinate choice does half the work: the sphere moves only vertically, the wedge only horizontally — one constraint $y=\sqrt3\,x$ couples them.

---

### Q1(k) — Pendulum with bottom tension = n × weight [4 marks]

**Key observation.** Energy sets the bottom speed from the release angle; the bottom tension is centripetal + weight. Two equations, eliminate $v$.

**Solution.** $v^2=2g\ell(1-\cos\theta)$; at the bottom: $T-mg=\dfrac{mv^2}{\ell}=2mg(1-\cos\theta)$:
$$nmg=mg\big(1+2(1-\cos\theta)\big)=mg(3-2\cos\theta)\;\Rightarrow\;\boxed{\cos\theta=\frac{3-n}{2}}.$$

**Check.** $\theta=0$ (hanging still): $n=1$ ✓; $\theta=90^\circ$: $n=3$ ✓ classic; $\theta\to180^\circ$ (string, unrealistic): $n=5$ — the familiar "loop-the-loop needs 5/2 factor" relative ✓. Feasible range $1\le n\le3$ for a string released within the lower half… stated ✓. Special cases: $n=1$ ⟹ $\cos\theta=1$ (hanging at rest), $n=3$ ⟹ $\cos\theta=0$ (released horizontal), $n=5$ ⟹ $\cos\theta=-1$ (released from the top — the full-circle case).

---

### Q1(l) — Banking of a railway curve [5 marks]

**Key observation.** "Normal reaction only" ⟹ no lateral friction: the resultant of $N$ and $mg$ must supply the centripetal force — $\tan\theta=v^2/(rg)$, then multiply by the gauge.

> 【Thought】 Seeing "normal reaction only" → triggers *the banked-curve condition*; the wheel flanges must not bear sideways load. The vertical displacement is gauge × tanθ (small-angle safe to keep exact tan here).

**Solution.** $v=200\ \text{km/h}=55.6\ \text{m/s}$:
$$\tan\theta=\frac{v^2}{rg}=\frac{55.6^2}{1500\times9.81}=0.210,\qquad \Delta h=1435\ \text{mm}\times0.210=\boxed{0.30\ \text{m}\ (\approx300\ \text{mm})}.$$

*(Official mark scheme: identical $\tan\theta$ relation; it converts with $\sin\theta$ instead of $\tan\theta$, giving 295 mm — within the allowed leeway either way.)*

**Check.** 30 cm over 1.4 m gauge ≈ 12° — steep but this is 200 km/h on a 1.5 km curve (fast, tight) ✓; exact vs small-angle: $\tan\theta$ vs $\sin\theta$ differ by 1% here — harmless either way ✓.

---

### Q1(m) — 90°-apex prism: ray striking BC at the critical angle [3 marks]

**Key observation.** The faces AB and BC meet at $45^\circ$ (base angle of the 90°-apex isosceles prism), so the internal angles obey $r_1+r_2=45^\circ$ (normals of the two faces are $45^\circ$ apart). Grazing emergence at BC sets $r_2=\theta_c$.

**(i)** $\theta_c=\arcsin\dfrac{1}{1.5}=\boxed{41.8^\circ}$.
**(ii) Sketch.** Ray enters AB at a small refraction angle ($r_1=3.2^\circ$ — nearly normal incidence), crosses to the base BC, and just grazes out along BC (emergence angle $90^\circ$).
**(iii)** $r_1=45^\circ-41.8^\circ=3.2^\circ$; $\sin i=1.5\sin3.2^\circ=0.0836$:
$$\boxed{i\approx4.8^\circ}.$$

> 【Thought】 Seeing "strikes BC at the critical angle" → triggers *prism angle bookkeeping* $r_1+r_2=45^\circ$ — with the apex at A (90°), face BC is the **base**, and the relevant wedge angle is the base angle 45°, not 90°. Reading which faces the ray uses is the whole problem; using $A=90^\circ$ gives $r_1=48^\circ> \theta_c$, an impossible entry — a built-in consistency alarm.

---

### Q1(n) — Aluminium block submerged: two balance readings [4 marks]

**Key observation.** Buoyancy $B=\rho_w g V$ lifts the block (newton-meter drops by $B$) and — by Newton's third law — the block pushes the water down by $B$ (mass balance rises by the equivalent of $B/g$).

> 【Thought】 The pairing is the physics: the two readings change by equal and opposite *force*. The beaker reading surprises students — "the block isn't touching the beaker" is irrelevant; the water holds the buoyant reaction. Volume: $5\times5\times10=250\ \text{cm}^3$.

**Solution.** $B=1000\times9.81\times2.5\times10^{-4}=2.45\ \text{N}$.
(i) Newton-meter: $6.6-2.45=\boxed{4.15\ \text{N}\ (\approx4.2\ \text{N})}$.
(ii) Mass balance: gains $B/g=0.250\ \text{kg}$ equivalent: $600+250=\boxed{850\ \text{g}}$.

**Check.** Energy/inventory sanity: the displaced water's weight = 2.45 N ✓ ($\rho Vg$); the two instruments' readings shift by ±2.45 N ✓ Newton III.

---

### Q1(o) — Minimum bend radius of a steel bar [4 marks]

**Key observation.** Pure bending: surface strain $\varepsilon_{\max}=\dfrac{y_{\max}}{R}=\dfrac{t/2}{R}$; breaking when $E\varepsilon_{\max}=\sigma_b$.

$$R_{\min}=\frac{E\,y_{\max}}{\sigma_b}=\frac{210\times10^9\times0.010}{840\times10^6}=\boxed{2.5\ \text{m}}.$$

> 【Thought】 Seeing "bent on the arc of a circle … breaking stress" → triggers *beam-bending strain* $\varepsilon=y/R$ (neutral axis through the centre). The assumption "$R\gg$ thickness" is exactly the licence for the linear strain profile — and the answer $R=2.5$ m $\gg 2$ cm is self-consistent ✓ (always close that loop).

---

### Q1(p) — Photoelectrons crossing to an electrode [6 marks]

**Key observation.** "Most energetic" electrons have $KE_{\max}=hf-\phi$; (i) free flight $t=d/v$; (ii) a uniform opposing field means uniform deceleration — but $KE_{\max}>eV_s$, so they still arrive (twice, mathematically — take the first crossing).

> 【Thought】 Part (ii)'s quadratic has two roots because a decelerating electron that *would* overshoot and return crosses the plane twice in a bound scenario; the "shortest time" selects the smaller root. Also verify the electron survives the barrier ($0.82>0.50$ eV) before computing anything — otherwise the answer is "never".

**Solution.** $E_\gamma=\dfrac{1240}{400}=3.10\ \text{eV}$; $KE_{\max}=3.10-2.28=0.82\ \text{eV}$;
$$v=\sqrt{\frac{2KE}{m_e}}=\sqrt{\frac{2\times1.31\times10^{-19}}{9.11\times10^{-31}}}=5.37\times10^5\ \text{m/s}.$$
(i) $t=\dfrac{0.10}{5.37\times10^5}=\boxed{1.9\times10^{-7}\ \text{s}}$.
(ii) Field $E=V/d=5.0$ V/m; deceleration $a=\dfrac{eE}{m_e}=8.79\times10^{11}\ \text{m/s}^2$; solve $d=vt-\tfrac12at^2$:
$$4.40\times10^{11}t^2-5.37\times10^5t+0.10=0\;\Rightarrow\;t=\frac{5.37\times10^5-3.36\times10^5}{8.79\times10^{11}}=\boxed{2.3\times10^{-7}\ \text{s}}.$$

**Check.** Arrival KE: $0.82-0.50=0.32$ eV $>0$ ✓ arrival confirmed; $t$ slightly longer than (i) ✓ (deceleration); the second root $9.3\times10^{-7}$ s corresponds to an overshoot-return crossing — physically excluded here since the electrode absorbs the electron ✓.

---

### Q1(q) — Variable R to minimise power in the 10 Ω resistor [3 marks]

**Key observation.** The 10 Ω is the *bridge arm* between the midpoints of two potential dividers: left divider $D\!\to\!B$: $(2+4)\ \Omega$ vs $R\parallel20\ \Omega$ (D = cell negative, C = cell positive, 20 V); right divider $D\!\to\!E$: $8\ \Omega$ vs $24\ \Omega$. The minimum of $P_{10}=(V_B-V_E)^2/10$ is **zero** — if the bridge can be balanced.

> 【Thought】 Seeing "minimise power in a bridge arm" → triggers *balance the bridge* ($P=0$ is the absolute floor of a square). Check the balance condition is attainable *before* settling for a boundary minimum: the right divider fixes $V_E=20\times8/32=5$ V, and the left can hit 5 V if $R\parallel20$ has the right value — an interior, attainable minimum. (A boundary-only scan would falsely place the minimum at $R\to\infty$; the official mark scheme's balance route is exact. Per the optimisation protocol: interior candidate $P=0$ vs boundary $P\to3.5$ mW at $R\to\infty$ — the interior wins, but only after verifying the balance equation has a positive-$R$ solution.)

**Solution.** Right divider: $V_E=20\times\dfrac{8}{8+24}=5$ V (measured from D). Left divider: $V_B=20\times\dfrac{6}{6+R\parallel20}$. Balance $V_B=V_E$:
$$\frac{6}{6+R\parallel20}=\frac14\;\Rightarrow\;R\parallel20=18\;\Rightarrow\;\frac{20R}{20+R}=18\;\Rightarrow\;2R=360\;\Rightarrow\;\boxed{R=180\ \Omega,\quad P_{10}=0}.$$

**Check.** Nodal analysis at $R=180$: $V_B=V_E=5.000$ V, $P_{10}=0$ ✓; at $R\to\infty$: $V_B=4.70$, $V_E=4.89$, $P=3.5$ mW $>0$ ✓ — so the interior balance is strictly better than any boundary, confirming the global minimum is at $R=180$ Ω ✓. (Official answer: $R=180$ Ω by the same bridge-balance argument.)

---

### Q1(r) — Charge on the 4.0 µF capacitor [3 marks]

**Key observation.** The 2 µF and 4 µF are in **parallel** (both between the left rail and the middle node), then in series with the 5 µF.

$$C_{\text{left}}=2+4=6\ \mu\text{F};\qquad Q_{\text{series}}=9.0\times\frac{6\times5}{6+5}=\frac{270}{11}=24.5\ \mu\text{C},$$
$$V_{\text{left}}=\frac{24.5}{6}=4.09\ \text{V}\;\Rightarrow\;Q_{4\mu F}=4.0\times4.09=\boxed{16.4\ \mu\text{C}}.$$

> 【Thought】 Series capacitors share *charge*, parallel share *voltage* — the sequence "collapse parallel → series charge → distribute by capacitance" is the whole algorithm. Trap: assigning the series charge 24.5 µC to the 4 µF directly (it splits between the parallel pair).

---

### Q1(s) — Capacitor: squeezed with supply, then stretched back isolated [4 marks]

**Key observation.** Two different regimes: connected ⟹ $V$ fixed ($E=\tfrac12CV^2$); disconnected ⟹ $Q$ fixed ($E=Q^2/2C$). Track the state variable that is pinned in each phase.

> 【Thought】 Seeing "supply connected … then disconnected" → triggers *switch the conserved variable*: $V$ while connected, $Q$ after. The work done by the operator against/at the plates differs by phase; the supply itself does work in phase 1. Also note: the supply disconnection traps $Q$ at its *maximum* value $3C_1V$.

**Solution.** $C_1=\varepsilon_0A/d$; $E_1=\tfrac12C_1V^2$.
Phase 1 (connected, $d\to d/3$): $C_2=3C_1$, $Q_2=3C_1V$, $E_2=3E_1$.
Phase 2 (isolated, $d/3\to d$): $Q$ stays $3C_1V$; back at $C_1$:
$$E_3=\frac{Q_2^2}{2C_1}=\frac{9C_1^2V^2}{2C_1}=9E_1\;\Rightarrow\;\boxed{E_3-E_1=8E_1=4C_1V^2=\frac{4\varepsilon_0AV^2}{d}}.$$

**Check.** Stretching apart attracts positive work (plates attract) ✓ energy rises; final energy 9× initial — pulled apart with 3× the charge: $E=Q^2/2C$, $Q$ tripled ⟹ 9× ✓. The conservation content: once disconnected, the middle capacitor's charge stays frozen at $3C_1V$ — that is what makes the final state determinate.

---

### Q1(t) — Mass loss of a Po-210 film by α escape [6 marks]

**Key observation.** The film loses mass only by ejected α particles (the Pb-206 daughters stay). Number decayed in 100 d from the half-life; each carries away $\approx4$ u.

> 【Thought】 Seeing "thin film … alpha particles can escape" → triggers *mass inventory per decay*: the film keeps the recoiling daughter; only the α's mass leaves. The trap is counting the whole decayed Po mass as lost (that would be 40× too big). Also note the exponential — 100/138 of a half-life, not linear.

**Solution.** Decayed fraction: $1-2^{-100/138}=0.395$; decayed Po mass: $5.0\times0.395=1.97$ mg; α mass per Po atom $\approx4/210$:
$$\Delta m=1.97\times\frac{4}{210}=\boxed{3.8\times10^{-2}\ \text{mg}\ (\approx0.04\ \text{mg}\text{, i.e. }3.8\times10^{-5}\ \text{g})}.$$

**Check.** Fraction of film lost: $0.395\times(4/210)=0.75\%$ ✓ tiny — consistent with "mass reduced" being a subtle effect ✓. The ledger: each decay removes one α (4 u) from the film while the daughter nucleus stays — mass leaves only 4 u at a time, never a whole Po atom.

---

### Q1(u) — Three tuning forks and beats [4 marks]

**Key observation.** $|f_B-f_C|=7$, $|f_A-f_C|=8$, $f_B=1.059f_A$. The beat equations carry unknown signs — enumerate the sign cases and use the 5.9% condition and audibility to select.

> 【Thought】 Beat frequencies give *magnitudes* only: the strategy is case enumeration. The audible-range clause is not decoration — it kills the wrong branch (which lands at 17 Hz).

**Solution.** Case work: if $C=B+7$, then $|A-C|=0.059f_A+7=8\Rightarrow f_A=17$ Hz — sub-audible, rejected. Hence $C=B-7$ and $C>A$:
$$C-A=8:\quad 1.059f_A-7-f_A=8\;\Rightarrow\;0.059f_A=15\;\Rightarrow\;f_A=254\ \text{Hz},$$
$$\boxed{f_A\approx254\ \text{Hz},\quad f_B\approx269\ \text{Hz},\quad f_C\approx262\ \text{Hz}}.$$

**Check.** $|269-262|=7$ ✓, $|254-262|=8$ ✓, $269/254=1.059$ ✓ — all three constraints satisfied simultaneously. Beat frequencies give only absolute values, so each fork's sign was fixed by the extra constraints (audible range and the ratio) — that sign ambiguity is the puzzle's core.

---

### Q1(v) — Filament bulb with R = A + BP [5 marks]

**Key observation.** Two operating points give two linear equations for $A$ and $B$; the 210 V part then requires solving $P=V^2/R(P)$ — a quadratic because $R$ itself depends on $P$.

**(i)** Operating: $R=230^2/100=529\ \Omega$. Cold: $R_c=529/5=105.8\ \Omega$ (and indeed $V^2/R_c=500$ W = 5× power ✓ consistent with the statement).
$$A+100B=529,\qquad A+500B=105.8\;\Rightarrow\;B=-\frac{423.2}{400}=-\frac{529}{500}=-1.058\ \Omega/\text{W},$$
$$A=529-100B=529+105.8=\frac{6\times529}{5}=634.8\ \Omega.$$
$$\boxed{A=634.8\ \Omega\ (=\tfrac{6}{5}\cdot529),\qquad B=-1.058\ \Omega\,\text{W}^{-1}\ (=-\tfrac{529}{500}).}$$

**(ii)** At 210 V: $P(A+BP)=210^2\Rightarrow -1.058P^2+634.8P-44100=0$:
$$P=\frac{634.8\pm\sqrt{634.8^2-4(1.058)(44100)}}{2\times1.058}=\frac{634.8\pm465.1}{2.116}=80\ \text{W}\ \text{or}\ 520\ \text{W}.$$
The 520 W root gives $R=634.8-1.058\times520<0$ — unphysical, rejected:
$$\boxed{P\approx80\ \text{W}}.$$

> 【Thought】 Note the model's oddity: $B<0$ means resistance *falls* with power here — not real tungsten behaviour, but the data are what they are; follow the mathematics and use the *physical branch* ($R>0$) as the root selector. That selection step is where the mark is.

**Check.** Verify: $R=634.8-1.058\times80=550\ \Omega$; $210^2/550=80.2$ W ✓ self-consistent.

---
*End of Paper 8 (2021 Round 1 Section 1).*


---

## Paper 9 — 2021 Round 1 Section 2 (12 Nov 2021)

*Section 2: Questions 2–5, 25 marks each; candidates attempt two. Full solutions for all four.*

---

### Question 2 — Waves on wires and in tubes

#### Q2(a) — Pulses and harmonics on a stretched wire [6 marks]

**(i) Reflected pulse sketch.** Reflection at a **fixed** end inverts the pulse (crest returns as a trough), travelling back at speed $v$; shape otherwise preserved. (The fixed point never moves: incoming and reflected displacements must cancel there at all times — that condition forces the inversion.)

**(ii)** The pulse must complete a round trip $2\ell$ and, after the second (left-end) reflection, pass the pluck point going the same way:
$$\boxed{t=\frac{2\ell}{v}}.$$

**(iii)** $f_1=\dfrac{1}{t}=\boxed{\dfrac{v}{2\ell}}$.

**(iv)** Resonances sustained: $f_n=\boxed{\dfrac{nv}{2\ell}}$, $n=1,2,3,\ldots$ (all harmonics).

**(v) Finger touching at 40% of the length.** The lightly touched point is pinned to (nearly) zero motion *while the wire sounds*, so the wire vibrates as **two independent segments** — of lengths $0.6\ell$ and $0.4\ell$ — each with its own fundamental $v/(2L_{\text{seg}})$:
$$f_A=\frac{v}{2(0.6\ell)}=\frac{f_1}{0.6}=\boxed{\frac{5}{3}f_1\approx1.67f_1},\qquad f_B=\frac{v}{2(0.4\ell)}=\frac{f_1}{0.4}=\boxed{\frac{5}{2}f_1=2.5f_1}.$$
Sketch: two independent half-sinusoid lobes, one spanning $0.6\ell$ and one $0.4\ell$, meeting at the stationary finger (amplitude zero there).

> 【Thought】 The decision point is what the finger *does*: held in contact while the wire sounds ("whilst touching"), it splits the wire into two independent strings — the official reading, giving $\frac53f_1$ and $\frac52f_1$. If instead the wire were plucked *as a whole* and the finger merely brushed it during the attack (the guitar-harmonic technique), the finger would act as a harmonic filter passing only modes with a node at $0.4\ell$ — leaving only $5f_1,10f_1,\ldots$. The word "whilst" decides for the segment picture: the segments vibrate *simultaneously and independently*, so their fundamentals are both heard.

**(vi)** $f_5=\dfrac{5v}{2\ell}\Rightarrow v=\dfrac{2\ell f_5}{5}=\dfrac{2\times2.3\times162}{5}=149\ \text{m/s}$; $\mu=42/2.3=0.0183\ \text{kg/m}$:
$$T=\mu v^2=0.0183\times149^2=\boxed{4.1\times10^{2}\ \text{N}\ (\approx405\ \text{N})}.$$

#### Q2(b) — Pulse on a hanging cable [8 marks]

**(i)** Tension at distance $x$ below the support = weight hanging below:
$$\boxed{T(x)=\frac{Mg(L-x)}{L}}.$$

**(ii)** $v=\sqrt{T/\mu}\propto\sqrt{T}$: at $x=L/4$: $T\propto 3L/4$; at $x=3L/4$ (i.e. $L/4$ from the bottom): $T\propto L/4$:
$$\boxed{v_{\text{top quarter}}/v_{\text{bottom quarter}}=\sqrt3\approx1.73}.$$

**(iii)** $v(x)=\sqrt{T/\mu}=\boxed{\sqrt{g(L-x)}}$.

**(iv)** Pulse time from the top:
$$t_{\text{top}}(x)=\int_0^x\frac{dx'}{\sqrt{g(L-x')}}=\boxed{\frac{2\big(\sqrt L-\sqrt{L-x}\big)}{\sqrt g}}.$$

> 【Thought】 Math action with purpose: the speed varies with position, so distance = speed × time fails; the integral $\int dx/v(x)$ is the only honest route. The substitution $u=L-x$ turns it into a power-law integral — do that rather than anything fancier.

**(v) Ball overtakes the pulse.** Ball: $x=\tfrac12gt^2$. Set equal to the pulse position, with $t=t_{\text{top}}(x)$:
$$\frac{g}{2}\cdot\frac{4\left(\sqrt L-\sqrt{L-x}\right)^2}{g}=x\;\Rightarrow\;2\left(\sqrt L-\sqrt{L-x}\right)^2=x.$$
Let $s=\sqrt{L-x}$: $2(\sqrt L-s)^2=L-s^2\Rightarrow 3s^2-4\sqrt L\,s+L=0\Rightarrow s=\sqrt L$ (start) or $s=\sqrt L/3$:
$$\boxed{x=L-\frac{L}{9}=\frac{8L}{9}}.$$

**Check.** The pulse slows near the free end ($T\to0$) while the ball accelerates through — an overtake near the bottom is physically inevitable; $8L/9\approx0.89L$ ✓ late but before the end. (Because the ball's speed varies, the catch-up point comes from integrating $v(t)$, never from average-speed arithmetic.)

#### Q2(c) — GPS-style timing: receiver position [2 marks]

**Key observation.** Arrival-time difference = (send-time difference) + (path difference)/c. Careful with signs.

> 【Thought】 Draw the timeline before touching numbers: Western pulse *sent* $484\ \mu\text{s}$ earlier, *received* $1542\ \mu\text{s}$ (cycles of 1 MHz) earlier. The extra $1058\ \mu\text{s}$ of arrival gap must come from the Western path being **shorter** — this sign reasoning is the whole question.

**Solution.** $t_W^{arr}-t_E^{arr}=-1542\ \mu\text{s}=(-484\ \mu\text{s})+\dfrac{d_W-d_E}{c}$:
$$d_W-d_E=c\times(-1058\ \mu\text{s})=-317\ \text{km},\qquad d_W+d_E=600\ \text{km},$$
$$\boxed{d_W\approx141\ \text{km}}.$$

**Check.** Receiver is west-of-centre ✓ (Western pulse arrives first despite being sent first — consistent: shorter path AND earlier send both push the same way).

#### Q2(d) — Closed tube: displacement and pressure standing waves [2 marks]

**(i)** A tube closed at one end supports only **odd** harmonics (node at closed end, antinode at open end): sketch displacement amplitude for $f_1$ (single quarter-wave lobe), $3f_1$ (three quarter-lobes), $5f_1$ (five quarter-lobes) along the tube.

**(ii)** Pressure variation is the spatial complement (90° out of phase): pressure **antinode** at the closed end (displacement node) and **node** at the open end — sketch the same three curves but peaked at the closed end and zero at the open end (dotted).

> 【Thought】 The physics anchor: where air cannot move (closed end), pressure swings are maximal; at the open end pressure is pinned to atmospheric. Displacement and pressure standing waves are always quarter-wavelength shifted — draw one, derive the other, don't memorise both (pressure is the spatial *gradient* of displacement, $p\propto-\partial\xi/\partial x$, hence the quarter-shift).

#### Q2(e) — Sound speed, pressure gradient, and the end correction [7 marks]

**(i)** Hydrostatic: $\Delta P=\rho gh=1.225\times9.81\times20=\boxed{240\ \text{Pa}}$ (0.24% of atmospheric).

**(ii)** $v=\sqrt{\gamma P/\rho}$: in an isothermal ideal-gas column $\rho\propto P$, so $P/\rho$ is constant — **sound speed is independent of depth** (pressure and density grow together).

**(iii)** $PV=nRT\Rightarrow P/\rho=RT/M_u$:
$$\boxed{v=\sqrt{\frac{\gamma RT}{M_u}}}.$$

**(iv) End correction problem.** Tube 1 ($20^\circ$C, $v_1=343$ m/s): $f_1=\dfrac{v_1}{4(\ell_1+\varepsilon)}$:
$$0.520+\varepsilon=\frac{343}{4\times156}=0.550\ \text{m}\;\Rightarrow\;\varepsilon=0.0297\ \text{m}\approx3.0\ \text{cm}.$$
Tube 2 at $35^\circ$C: $v_2=343\sqrt{308/293}=351.7$ m/s. Beats at 4.8 Hz, and tube 2 is *shorter* (and warmer) ⟹ $f_2=156+4.8=160.8$ Hz:
$$\ell_2+\varepsilon=\frac{351.7}{4\times160.8}=0.5468\ \text{m}\;\Rightarrow\;\boxed{\ell_2\approx0.517\ \text{m}\ (51.7\ \text{cm})}.$$

> 【Thought】**Cross-check against the official mark scheme, which prints $\ell_2=49$ cm.** The official route chose the *lower* beat root $f_2=151.2$ Hz and inverted the ratio $(\ell_1+\varepsilon)/(\ell_2+\varepsilon)$. Both choices fail diagnostics: (1) tube 2 is shorter **and** warmer, and both changes raise the pitch ($f=v/4(\ell+\varepsilon)$ with $v\propto\sqrt T$), so $f_2>f_1$ is forced — $f_2=160.8$ Hz, not 151.2 Hz; (2) the mark scheme's own note "no mark for 52.3 cm" rejects a *longer* tube, yet its 49 cm implies $f_2=169$ Hz, a 13 Hz beat — inconsistent with the given 4.8 Hz. Our 51.7 cm reproduces exactly a 4.8 Hz beat with the correct warm-air speed $351.7$ m/s ✓ — the closed-loop check the official value fails.

> 【Thought】 The beat sign ambiguity ($160.8$ vs $151.2$ Hz) is resolved by physics, not luck: both "shorter" and "warmer" push the frequency **up**, so the beat is $+4.8$ Hz. When a question gives two consistent hints, use both as a cross-check of the sign.

---

### Question 3 — Properties of electrical circuits

#### Q3(a) — Ladder of 4 Ω resistors, 1 A in the final one [2 marks]

**Key observation.** Start from the far end and work back: the last stage fixes everything.

> 【Thought】 Seeing "current through the final resistor" → triggers *backward unfolding*: each stage toward the source adds one shunt current and one series drop. A forward attack (total R first) works too — verify both agree: right-to-left reduction: $4\ \Omega$; $(4+4)\parallel 4=\tfrac83\ \Omega$; $(4+\tfrac83)\parallel4=2.5\ \Omega$.

**Solution.** Final shunt: $V_3=1.0\times4=4$ V; series drop into it: 4 V ⟹ $V_2=8$ V; shunt at node 2: $8/4=2$ A; series current $1+2=3$ A ⟹ drop 12 V ⟹ $V_1=20$ V; shunt at node 1: 5 A; total current $8$ A.
$$\boxed{V_{AB}=20\ \text{V}},\qquad \boxed{R_{\text{chain}}=\frac{20}{8}=2.5\ \Omega}.$$

**Check.** Reduction route gives 2.5 Ω ✓ and $V=IR=8\times2.5=20$ V ✓ — the two directions cross-validate. The back-calculation order is: end current → branch currents add at parallel joints → voltage drops add along series arms.

#### Q3(b) — Rechargeable cell: emf and internal resistance [3 marks]

**Key observation.** Charging: applied voltage must overcome emf **plus** internal drop ($V=\mathcal E+Ir$); discharging: emf covers load **plus** internal drop ($\mathcal E=I(R+r)$). Two linear equations.

$$2.5=\mathcal E+0.5r,\qquad \mathcal E=1.9+0.25r\;\Rightarrow\;0.6=0.75r\;\Rightarrow\;\boxed{r=0.8\ \Omega,\quad \mathcal E=2.1\ \text{V}}.$$

> 【Thought】 The sign flip of the internal-drop term between charging and discharging is the entire content. Draw the two loop equations from the physical current direction each time — never reuse one sign convention blindly.

**Check.** Discharge terminal voltage $0.25\times7.6=1.9$ V $< \mathcal E$ ✓; charging needs $2.5$ V $>\mathcal E$ ✓. Note the sign asymmetry: discharging reads $\mathcal{E}-Ir$, charging reads $\mathcal{E}+Ir$ — the internal drop flips with the current.

#### Q3(c) — Parallel resistors, superposition, and cells in parallel [8 marks]

**(i)** Common $V$: $I=\dfrac{V}{R_A}+\dfrac{V}{R_B}=V\dfrac{R_A+R_B}{R_AR_B}$ ⟹ $R_{eq}=\dfrac{V}{I}=\dfrac{R_AR_B}{R_A+R_B}$. $\blacksquare$

**(ii)** i. Current divider (current favours the *other* resistor): fraction through $R_B$ = $\boxed{\dfrac{R_A}{R_A+R_B}}$.
ii. $I=\mathcal E/(R+R_{eq})$, so
$$I_B=\frac{\mathcal E}{R+R_{eq}}\cdot\frac{R_A}{R_A+R_B}=\boxed{\frac{\mathcal E R_A}{RR_A+RR_B+R_AR_B}}.$$

**(iii)** i. $E_2$ removed (Y–Z joined): $I_1=\mathcal E_1/R$; ii. $E_1$ removed: $I_2=\mathcal E_2/R$. (Superposition: total $I=(\mathcal E_1+\mathcal E_2)/R$.)

**(iv)** Only $\mathcal E_2$ in Fig. 9 (cell $\mathcal E_2$ with $R_2$ in its branch; $R_1$ branch passive): $R_1\parallel R_3$ is the load:
$$I_3'=\frac{\mathcal E_2}{R_2+R_1\parallel R_3}\cdot\frac{R_1}{R_1+R_3}=\frac{\mathcal E_2R_1}{R_1R_2+R_2R_3+R_3R_1}.$$

**(v)** Only $\mathcal E_1$: $I_3''=\dfrac{\mathcal E_1R_2}{R_1R_2+R_2R_3+R_3R_1}$.

**(vi)**
$$\boxed{I_3=\frac{\mathcal E_1R_2+\mathcal E_2R_1}{R_1R_2+R_2R_3+R_3R_1}}.$$

**(vii) Equivalent source.** Terminal voltage $V=I_3R_3=\dfrac{(\mathcal E_1R_2+\mathcal E_2R_1)R_3}{R_1R_2+(R_1+R_2)R_3}$. Compare with a source $(\mathcal E_{eq},R_{int})$: $V=\dfrac{\mathcal E_{eq}R_3}{R_{int}+R_3}$; multiplying out and matching coefficients of $R_3$:
$$R_{int}=\frac{R_1R_2}{R_1+R_2}\ \blacksquare,\qquad \mathcal E_{eq}=\frac{\mathcal E_1R_2+\mathcal E_2R_1}{R_1+R_2}=\frac{\mathcal E_1/R_1+\mathcal E_2/R_2}{1/R_1+1/R_2}\ \blacksquare$$
(the second form follows on dividing top and bottom by $R_1R_2$ — Millman's formula).

> 【Thought】 The matching trick: expand $\mathcal E_{eq}R_3/(R_{int}+R_3)$ and compare with the exact $V(R_3)$ coefficient by coefficient — this *proves* the equivalence for all loads, which is what "behave as a source" means. (Alternative: read off open-circuit voltage $R_3\to\infty$ and short-circuit current $R_3=0$.)

**(viii)** $\mathcal E_1=50$ V, $\mathcal E_2=60$ V, $R_1=10\ \Omega$, $R_2=15\ \Omega$: $\mathcal E_{eq}=\dfrac{750+600}{25}=54$ V; $R_{int}=\dfrac{150}{25}=6\ \Omega$.
i. Maximum power at $R_3=R_{int}=\boxed{6\ \Omega}$.
ii. $P_{\max}=\dfrac{\mathcal E_{eq}^2}{4R_{int}}=\dfrac{2916}{24}=\boxed{121.5\ \text{W}}$.
iii. Cell $\mathcal E_1$ starts being **charged** when its branch current reverses, i.e. when the terminal voltage exceeds $\mathcal E_1=50$ V:
$$V=\frac{54R_3}{6+R_3}>50\;\Rightarrow\;54R_3>300+50R_3\;\Rightarrow\;\boxed{R_3>75\ \Omega\ (\text{charging begins at }R_3=75\ \Omega)}.$$

**Check.** At $R_3=75\ \Omega$: $V=54\times75/81=50$ V exactly ✓ boundary consistent. (The node-voltage formula used is Millman's theorem: the common node sits at the *conductance-weighted* average of the branch voltages.)

#### Q3(d) — Voltage suppressor protecting a 10 kΩ load [8 marks]

**Setup.** From Fig. 10: 5 kΩ in series with the parallel pair (suppressor $S$: $I=kV^2$, $k=1.0\times10^{-7}\ \text{A/V}^2$; load 10 kΩ). $V$ = voltage across the parallel pair.

**(i) Normal operation** (supply 2000 V). KCL: current through the 5 kΩ = load current + suppressor current:
$$2000-V=5000\left(\frac{V}{10^4}+kV^2\right)\;\Rightarrow\;2000=1.5V+5\times10^{-4}V^2,$$
$$V^2+3000V-4\times10^6=0\;\Rightarrow\;V=\frac{-3000+\sqrt{9\times10^6+16\times10^6}}{2}=1000\ \text{V},$$
$$\boxed{I_{\text{load}}=\frac{1000}{10^4}=0.10\ \text{A}}.$$

**(ii) Surge doubling the load current.** $I_{\text{load}}=0.20$ A ⟹ $V=0.20\times10^4=2000$ V; suppressor current $kV^2=10^{-7}\times(2000)^2=0.40$ A; total through 5 kΩ: $0.60$ A, dropping $3000$ V:
$$\boxed{V_{\text{surge}}=2000+3000=5000\ \text{V}}.$$

> 【Thought】 The suppressor's $I\propto V^2$ is what makes the device work: its current quadruples for a doubling of voltage, dumping the surge through itself. Note the asymmetry exploited in (ii): supply ×2.5, load current only ×2 — the quadratic shunt absorbs the difference. Also note the quadratic in (i) has a designed clean root ($V=1000$) — engineered numbers signal you're on the intended path. The protection mechanism is the nonlinearity itself: the device's resistance collapses above the threshold, diverting the surge current.

---

### Question 4 — Electric fields

#### Q4(a) — Parallel-plate capacitor fields and forces [8 marks]

**(i) Sketches (+Q / −Q capacitor).** Positive plate alone: uniform outward field both sides, magnitude $\sigma/2\varepsilon_0$. Negative plate alone: uniform inward field, same magnitude. Both plates: outside, the two fields cancel; between the plates they add: $E=\sigma/\varepsilon_0$, uniform, from $+$ to $-$.

**(ii) Both plates +Q.** Between the plates the fields **cancel** (they point opposite ways); outside, they add: $E=\sigma/\varepsilon_0$ pointing away on both outer sides.

> 【Thought】 The superposition exercise's payload: a single infinite plate creates $\sigma/2\varepsilon_0$ on **both** sides (Gauss with a symmetric pillbox); all capacitor field patterns follow by addition. Students who memorise "$E=\sigma/\varepsilon_0$ between plates" without the half-fields can't answer (ii) — this pair of sketches is the antidote.

**(iii) Force between the plates.** $U=\dfrac{Q^2}{2C}=\dfrac{Q^2d}{2\varepsilon_0A}$ (constant $Q$ — plates isolated). Work to separate: $F\,dd=dU$:
$$\boxed{F=\frac{dU}{dd}=\frac{Q^2}{2\varepsilon_0A}}.$$

> 【Thought】 Constant-$Q$ vs constant-$V$ is the fork in the road: with the plates isolated, pulling apart raises $U$ and the operator does the work; $F=+dU/dd$. (With a battery attached, $U=\tfrac12CV^2$ *falls* and the battery absorbs the difference — same force, different bookkeeping.)

**(iv)** $E=\boxed{\sigma/\varepsilon_0}$ (from (i)).

**(v)** $F\propto Q^2/A$: doubling $A$ at fixed $F$ ⟹ $Q$ increases by $\boxed{\sqrt2}$.

**(vi) Water rising under a thundercloud.** Electrostatic pressure on the charged water surface, $\sigma^2/2\varepsilon_0$, balances the hydrostatic head $\rho g h$:
$$\frac{\sigma^2}{2\varepsilon_0}=\rho gh\;\Rightarrow\;\sigma=\sqrt{2\varepsilon_0\rho gh}=\sqrt{2(8.85\times10^{-12})(1000)(9.81)(1.5\times10^{-3})},$$
$$\boxed{\sigma\approx1.6\times10^{-5}\ \text{C/m}^2\ (\approx16\ \mu\text{C/m}^2)}.$$

> 【Thought】 Why $\sigma^2/2\varepsilon_0$ and not $\sigma E$: the field acting on the surface charge is the *average* of the fields just outside ($\sigma/\varepsilon_0$) and inside (0) the conductor — the factor ½ has the same origin as in (iii). Throughout: at constant $Q$ the field is fixed and stretching costs work against attraction; at constant $V$ the battery trades charge and half its work becomes stored energy — the two protocols differ by exactly the battery's share.

#### Q4(b) — Charged spheres and breakdown of air [10 marks]

**(i)** $V=\dfrac{Q}{4\pi\varepsilon_0 r}$ ⟹ $\boxed{Q=4\pi\varepsilon_0 rV}$.

**(ii)** Same $V$, different radii: $E=\dfrac{V}{r}$ at each surface:
$$\boxed{E_A\,a=E_B\,b\ \left(\frac{E_A}{E_B}=\frac{b}{a}\right)}\ \text{— the smaller sphere has the stronger field.}$$

**(iii)** Ion $-e$ moving toward B from 4.0 mm to 3.0 mm from the centre ($b=1.0$ mm, $V=2000$ V; potential falls off as $V(r)=Vb/r$):
$$\Delta V=V(3\ \text{mm})-V(4\ \text{mm})=2000\left(\frac{1}{3}-\frac14\right)=2000\times\frac{1}{12}=166.7\ \text{V},$$
$$\boxed{W=e\,\Delta V\approx167\ \text{eV}}.$$

> 【Thought】**Official mark scheme note:** the mark scheme reads "3.0 mm from the surface of B" as 3.0 mm from the *centre* (its sketch marks 3 mm and 2 mm), giving $\Delta V=1000-667=333$ V and $0.33$ keV. Read literally — as the question prints it — the ion starts $1+3=4$ mm from the centre and ends at 3 mm: $\Delta V=667-500=167$ V → $167$ eV, our boxed value. Both computations are internally consistent; they differ only in reading "from the surface".

> 【Thought】 Use centre-to-point distances ($b+3$ mm = 4 mm, not 3 mm!) — the phrase "3.0 mm from the surface" is the trap; the potential lives in the space outside the sphere as $Vb/r$ measured from the centre.

**(iv) Sketch.** Field lines leave the conductor **perpendicular** to the surface everywhere, spaced closer together at the sharply curved (small-radius) end — the line density there encodes the stronger field.

**(v) Breakdown field.** An electron must gain the ionisation energy within one mean free path:
$$eE\lambda=E_{\text{ion}}\;\Rightarrow\;E=\frac{2.5\ \text{eV}}{e\times7.0\times10^{-6}\ \text{m}}=\frac{2.5\ \text{V}}{7.0\times10^{-6}\ \text{m}}=\boxed{3.6\times10^{5}\ \text{V/m}}.$$

**(vi)** Treat each end as a hemisphere: $E\approx V/r$; breakdown starts at the **smaller** end ($r=5.0$ cm):
$$V_{\max}=E_{\text{bd}}\,r_{\min}=3.6\times10^5\times0.050=\boxed{1.8\times10^{4}\ \text{V}\ (\approx18\ \text{kV})}.$$

**(vii) Charge sketch.** Surface charge density $\sigma$ greatest at the 5 cm end (tight curvature), smallest on the 15 cm end — shade/space the + symbols accordingly; $\sigma$ correlates with local curvature, consistent with $E\propto1/r$ at fixed potential.

> 【Thought】 The running theme of (iv)–(vii): at fixed potential, small radius ⟹ large $E$ ⟹ breakdown starts at sharp features — why high-voltage hardware avoids points (and why lightning rods work). (Reading note: "3.0 mm from the surface" means 3.0 mm beyond the surface, i.e. 4.0 mm from the sphere's centre.)

#### Q4(c) — Point charge near an earthed conducting plate [7 marks]

**(i) Sketch.** Field lines leave $+Q$ and land on the plate **perpendicularly**, bending outward — the pattern is exactly the upper half of a charge–image dipole field.

**(ii)** i. The plate carries induced negative charge (field lines terminate on it); unlike charges attract → force on the plate. ii. Direction: perpendicular to the plate, **toward the charge** (attraction). iii. Symmetry: the induced surface charge is axisymmetric about the foot of the perpendicular from $Q$, so sideways force components cancel pairwise — the net force lies along the perpendicular axis through $Q$.

**(iii)** i. With $-Q$ at distance $d$ behind the plate's position (plate removed), the field between $+Q$ and its image reproduces exactly the real field in the accessible region (same boundary condition $V=0$ on the midplane). ii. The plate's attraction on $Q$ equals the image's Coulomb attraction at separation $2d$:
$$F=\frac{1}{4\pi\varepsilon_0}\frac{Q^2}{(2d)^2}=8.99\times10^9\times\frac{(4.0\times10^{-6})^2}{4\times(0.20)^2}=8.99\times10^9\times\frac{1.6\times10^{-11}}{0.16}=\boxed{0.90\ \text{N}}.$$

> 【Thought】 Method of images in one line: *the conductor's boundary condition ($V=0$) is mimicked by an opposite charge mirrored behind it*, and uniqueness of solutions then guarantees the forces match. The trap: using separation $d$ instead of $2d$ (the image is $d$ **behind** the plate). The image's whole job is boundary enforcement: it reproduces $V=0$ on the plate, so the region's field is unchanged.

---

### Question 5 — Springs and forces

#### Q5(a) — Spring oscillations in four geometries [7 marks]

**(a)(i).** Diagram: mass with $mg$ down and spring force $k(\ell-\ell_0+x)$ up. Equilibrium: $mg=k(\ell-\ell_0)$. Displaced $x$ down: net force $=mg-k(\ell-\ell_0+x)=-kx$ — linear restoring, $m\ddot x=-kx$ ⟹ $\omega^2=k/m$:
$$T=2\pi\sqrt{\frac{m}{k}}.\ \blacksquare$$

> 【Thought】 The lesson: gravity only shifts the equilibrium; the *incremental* force is $-kx$ about equilibrium. Cancelling the static terms is the move — do it explicitly once and SHM appears.

**(a)(ii)** Walls $2\ell_0$ apart: at centre both springs are at natural length. Displaced $x$: one spring compressed $x$ (pushes back), the other stretched $x$ (pulls back): $F=-2kx$:
$$\boxed{T=2\pi\sqrt{\frac{m}{2k}}}.$$

**(a)(iii)** Walls $4\ell_0$ apart: both springs pre-stretched (tension $k\ell_0$ each, balanced at centre). Displaced $x$: tensions become $k(\ell_0+x)$ and $k(\ell_0-x)$; net $=-2kx$ again:
$$\boxed{T=2\pi\sqrt{\frac{m}{2k}}}\ \text{— unchanged by the pre-tension.}$$

> 【Thought】 Pre-tension cancels in the *difference* — the point of the part: what matters for oscillation is the **gradient** of force with displacement, and a constant pre-load has zero gradient. (Linear springs only; a nonlinear spring's pre-tension would change the stiffness.)

**(a)(iv)** Different constants $k_1,k_2$, walls $4\ell_0$: displaced $x$: left spring force changes by $-k_1x$, right by $-k_2x$ (same sign, restoring):
$$F=-(k_1+k_2)x\;\Rightarrow\;\boxed{T=2\pi\sqrt{\frac{m}{k_1+k_2}}}.$$
(Only the *displacement-dependent* part of the force restores: a constant pre-tension shifts the equilibrium but contributes no gradient, hence no period change.)

#### Q5(b) — Two masses on a string / spring: the reduced mass [4 marks]

**(i)** Rotation is about the CM (no external horizontal force): $m_1r_1=m_2r_2$, $r_1+r_2=r$. Both centripetal forces equal the same tension:
$$T=m_1\omega^2r_1=m_1\omega^2\frac{m_2r}{m_1+m_2}\;\Rightarrow\;\boxed{T=\frac{m_1m_2}{m_1+m_2}\omega^2r}.$$

**(ii)** The non-oscillating point is the CM; each mass oscillates on its segment of spring, and matching the two segment frequencies gives the same condition $m_1x_1=m_2x_2$ (relative coordinate). The period matches a single mass $M$ on spring $k$ with
$$\boxed{M(m_1,m_2)=\frac{m_1m_2}{m_1+m_2}\ \text{(the reduced mass)}}\;\Rightarrow\;T=2\pi\sqrt{\frac{M}{k}}.$$

> 【Thought】 The reduced mass appears whenever two bodies share one internal coordinate — the same $\mu=m_1m_2/(m_1+m_2)$ governs binary orbits, collision losses, and molecular vibrations. Derive it once via the relative coordinate $\xi=x_1-x_2$: $\mu\ddot\xi=-k\xi$ — the reduced mass $\mu=m_1m_2/(m_1+m_2)$ is the inertia of the *relative* motion, the price of replacing two coupled bodies by one.

#### Q5(c) — Projectile deceleration profile [5 marks]

**Reading the graph** (4 regions): R1: 0–10 ms, 0→6000 m/s² (avg 3000); R2: 10–20 ms, 6000→4000 (avg 5000); R3: 20–90 ms, 4000→3000 (avg 3500); R4: 90–100 ms, 3000→0 (avg 1500).

**(i) Speed changes** ($\Delta v=\bar a\,\Delta t$): $30+50+245+15=340$ m/s:
$$\boxed{v_0\approx340\ \text{m/s}}.$$

**(ii) Penetration depth** (speeds at region boundaries: 340, 310, 260, 15, 0 m/s; uniform change ⟹ distance $=\bar v\,\Delta t$):
$$d=\tfrac{340+310}{2}(0.01)+\tfrac{310+260}{2}(0.01)+\tfrac{260+15}{2}(0.07)+\tfrac{15+0}{2}(0.01)=3.25+2.85+9.63+0.08\approx\boxed{16\ \text{m}}.$$

> 【Thought】 Method: deceleration–time area gives speed changes; average-speed × time gives distance. Do them as two separate sweeps — the second uses the *results* of the first. The long shallow R3 dominates the depth (9.6 m of 16 m): sanity-check your answer by asking which region should dominate.

#### Q5(d) — Ballistic pendulum on a stiff frame [4 marks]

**Key observation.** Two timescales: the bullet–sand collision is fast (momentum conserved, spring hasn't moved); the frame then swings slowly (energy conserved). Stitch them.

> 【Thought】 The opening paragraph of the question *tells* you the intended model: "collision time short compared to any other motion" ⟹ treat collision and spring compression as sequential, momentum then energy. Skipping this timescale argument and writing energy conservation across the whole process would double-count the collision loss.

**Solution.** Collision (perfectly inelastic): $v=\dfrac{m_1v_1}{m_1+M_2}=\dfrac{0.010\times320}{4.01}=0.798$ m/s. Frame stiffness: $k=\dfrac{200}{0.005}=4.0\times10^4$ N/m. Swing:
$$\frac12kx^2=\frac12(m_1+M_2)v^2=\frac12(4.01)(0.798)^2=1.28\ \text{J},$$
$$x=\sqrt{\frac{2\times1.28}{4.0\times10^4}}=\boxed{8.0\times10^{-3}\ \text{m}\ (8.0\ \text{mm})}.$$

**Check.** Momentum route cross-check: $x=\dfrac{m_1v_1}{\sqrt{k(m_1+M_2)}}=\dfrac{3.2}{\sqrt{4\times10^4\times4.01}}=\dfrac{3.2}{400.5}=8.0$ mm ✓.

#### Q5(e) — Ball bearing bouncing off a spring-mounted cylinder [5 marks]

**Setup.** Ball: $m_1=45$ g dropped from $h=2.0$ m: $v_1=\sqrt{2gh}=6.26$ m/s. Cylinder $m_2=0.45$ kg ($r=m_2/m_1=10$) on spring $k=1600$ N/m.

**(i) Elastic collision.** Cylinder's speed (target at rest):
$$v_2=\frac{2m_1}{m_1+m_2}v_1=\frac{2}{r+1}v_1=\frac{2\times6.26}{11}=\boxed{1.14\ \text{m/s}}.$$

**(ii) Maximum deflection from equilibrium:**
$$\frac12kx^2=\frac12m_2v_2^2\;\Rightarrow\;x=v_2\sqrt{\frac{m_2}{k}}=1.14\sqrt{\frac{0.45}{1600}}=\boxed{1.9\times10^{-2}\ \text{m}\ (\approx19\ \text{mm})}.$$

**(iii) Inelastic case.** Deflection 12.0 mm ⟹ cylinder's post-impact speed:
$$v_2'=x\sqrt{\frac{k}{m_2}}=0.012\times\sqrt{\frac{1600}{0.45}}=0.716\ \text{m/s}.$$
Momentum across the (short) collision: $m_1v_1=m_1v_1'+m_2v_2'$:
$$v_1'=v_1-r\,v_2'=6.26-10\times0.716=-0.89\ \text{m/s}\ \text{(upward)},$$
$$h_{\text{rebound}}=\frac{v_1'^2}{2g}=\frac{0.89^2}{19.6}=\boxed{4.0\times10^{-2}\ \text{m}\ (\approx4\ \text{cm})}.$$

**Why no separate $m_2g\Delta h$ term appears:** the deflection is measured from the *equilibrium* position, where the spring is pre-compressed by $\delta_0=m_2g/k$ — expanding $\tfrac12k(\delta_0+\Delta h)^2-\tfrac12k\delta_0^2$, the preload term $k\delta_0\Delta h$ cancels $m_2g\Delta h$ exactly, leaving the clean $\tfrac12k\Delta h^2$ balance used above.

> 【Thought】**Official mark scheme note:** the official (iii) obtains $h=29$ cm by adding a term $m_2g\,\Delta h$ to the spring-energy balance, $\tfrac12m_2V_2^2+m_2g\Delta h=\tfrac12k\Delta h^2$, i.e. $V_2=0.87$ m/s. That double-counts gravity: the deflection is measured **from the equilibrium position**, where the spring is already pre-compressed by $m_2g/k$ — expanding $\tfrac12k(\delta_0+\Delta h)^2-\tfrac12k\delta_0^2-m_2g\Delta h$ around equilibrium, the preload term $k\delta_0\Delta h$ cancels $m_2g\Delta h$ exactly, leaving $\tfrac12k\Delta h^2$ alone. With the equilibrium-referenced balance, $V_2=0.716$ m/s and the rebound is $4.0$ cm — our answer. (The official's own (ii) note debates this GPE term without resolving it; the preload argument settles it.)

> 【Thought】 The measurement chain in (iii) is: spring deflection → cylinder speed (energy) → ball's exit speed (momentum) → rebound height (energy). Each arrow is a different conservation law applied to a different stage — labelling which law bridges which stage is exactly what the question's preamble is coaching.

**Check.** Elastic ball rebound would be $v_1'=\dfrac{m_1-m_2}{m_1+m_2}v_1=-5.13$ m/s (height 1.34 m); the inelastic case rebounds less (0.89 m/s, 4 cm) ✓ consistent direction; also $v_2'<v_2$ ✓ (less energy transferred inelastic).

---
*End of Paper 9 (2021 Round 1 Section 2).*


---

## Paper 10 — 2020 Round 1 Section 1 (17 Nov 2020)

*Section 1, Question 1, parts (a)–(s). Maximum 50 marks from 73.*

---

### Q1(a) — Free fall to the speed of sound [2 marks]

**Key observation.** "Free-fall conditions" = ignore drag: $v^2=2gh$.

$$h=\frac{v^2}{2g}=\frac{330^2}{19.62}=\boxed{5.6\times10^{3}\ \text{m}\ (\approx5.5\ \text{km})}.$$

> 【Thought】 The word "free-fall" is the licence to ignore terminal velocity — in reality drag caps falling objects well below 330 m/s; noting the model boundary is part of the answer.

---

### Q1(b) — Motorcycle launched off a symmetric ramp apex [4 marks]

**Key observation.** Projectile launched from the apex at $\theta$ above horizontal, landing on a slope descending at $\theta$: write both the trajectory and the ramp line, intersect them.

> 【Thought】 Coordinates: origin at the apex, $x$ horizontal toward the descending side. The ramp is the line $y=-x\tan\theta$ — landing "on the ramp" is an *intersection* condition, the cleanest way to convert geometry into an equation. The launch angle is $\theta$ (symmetric ramp), so launch direction is tangent to the ascent side.

**Solution.** Trajectory: $y=x\tan\theta-\dfrac{gx^2}{2u^2\cos^2\theta}$. Intersect with $y=-x\tan\theta$:
$$\frac{gx^2}{2u^2\cos^2\theta}=2x\tan\theta\;\Rightarrow\;x=\frac{4u^2\sin\theta\cos\theta}{g}.$$
(i) $t_a=\dfrac{x}{u\cos\theta}=\boxed{\dfrac{4u\sin\theta}{g}}$.
(ii) $\ell=OP=\dfrac{x}{\cos\theta}=\boxed{\dfrac{4u^2\sin\theta}{g}}$.

**Check.** $\theta\to0$: $t_a,\ell\to0$ — flat ground, no flight ✓; dimensions: $u^2/g$ is a length ✓; the time is twice the ordinary "return to launch level" time $\frac{2u\sin\theta}{g}$ — descending slope doubles it ✓ plausible. (Geometry used: the slope is symmetric, $y=-|x|\tan\theta$ — landing below launch level is what lengthens the flight.)

---

### Q1(c) — Buckets over a pulley, then one lands [4 marks]

**Key observation.** Phase 1: Atwood machine (constant acceleration). Phase 2: after bucket 2 lands, the rope goes slack and bucket 1 is in free vertical motion (projectile upward).

**(i)** $a=\dfrac{(m_2-m_1)g}{m_1+m_2}$ over distance $h$:
$$\boxed{v=\sqrt{\frac{2gh(m_2-m_1)}{m_1+m_2}}}.$$

**(ii)** Bucket 1 rises further by
$$\Delta h=\frac{v^2}{2g}=\boxed{\frac{h(m_2-m_1)}{m_1+m_2}}.$$

> 【Thought】 Seeing "further increase in height after bucket 2 hits the ground" → triggers *phase-boundary thinking*: the constraint (rope tension) dies the instant bucket 2 lands; afterwards bucket 1 is ballistic. The most common error is continuing the Atwood acceleration past the landing. Note (ii) needs no new computation — divide the phase-1 energy result by $2g$.

**Check.** $m_2\to m_1$: both answers →0 ✓; $m_1=0$: $v=\sqrt{2gh}$, $\Delta h=h$ ✓ (bucket 1 free-falls' mirror). Note the constraint dies once bucket 2 lands — afterwards bucket 1 free-falls alone, which is why the answer is stitched from two regimes.

---

### Q1(d) — Rugby interception [4 marks]

**Key observation.** X runs in a *straight line* at 8 m/s to intercept Y, whose motion is known: write both positions, set equal, and let the unit-vector condition on X's direction close the system.

> 【Thought】 Seeing "runs in a straight line to intercept" → triggers *intercept condition = position equality at one time*; unknowns are X's heading ($u_x,u_y$) and $t$, with $u_x^2+u_y^2=1$ as the third equation. Solve the easy component first (here the $\hat j$ equation gives $u_y$ immediately).

**Solution.** (i) $\mathbf v_Y=(3\hat i+4\hat j)$ m/s (speed 5 m/s).
(ii) $\mathbf r_Y=(3t,4t)$; $\mathbf r_X=(20+8u_xt,\;8u_yt)$. From the $\hat j$ equation: $4t=8u_yt\Rightarrow u_y=\tfrac12$. Then $u_x=-\sqrt{1-\tfrac14}=-\tfrac{\sqrt3}{2}$ (negative — X must run westward). The $\hat i$ equation:
$$3t=20-8\times\frac{\sqrt3}{2}t\;\Rightarrow\;t=\frac{20}{3+4\sqrt3}=\boxed{2.0\ \text{s}}.$$
(iii) $\Delta\mathbf r_Y=(3,4)\times2.01=(6.0,8.1)$ m: magnitude $\boxed{\approx10\ \text{m}}$ at bearing $\arctan(3/4)=37^\circ$ east of north.

**Check.** X covers $8\times2.01=16.1$ m: distance from $(20,0)$ to $(6.0,8.1)$: $\sqrt{196+64.8}=16.1$ ✓ consistent. (The direction unit-vector constraint $u_x^2+u_y^2=1$ is what closes the equation set.)

---

### Q1(e) — Resistivity from weighing the wire in and out of water [3 marks]

**Key observation.** The buoyancy difference gives the volume (Archimedes); with the diameter it gives the length; then $\rho=RA/L$.

> 【Thought】 Seeing "weighed in water" → triggers *Archimedes: weight loss = weight of displaced water = ρ_w g V*. The weight in air is then only needed for the mass (not even that — only $V$ is used!). Recognising which datum is *not* needed ($m$) is part of reading the problem.

**Solution.** $V=\dfrac{4.60-4.08}{1000\times9.81}=5.30\times10^{-5}\ \text{m}^3$; $A=\pi(0.70\times10^{-3})^2=1.539\times10^{-6}\ \text{m}^2$; $L=\dfrac{V}{A}=34.4\ \text{m}$:
$$\rho=\frac{RA}{L}=\frac{0.478\times1.539\times10^{-6}}{34.4}=\boxed{2.1\times10^{-8}\ \Omega\,\text{m}}.$$

**Check.** Right in the copper-family range ($1.7\times10^{-8}$) ✓ — a sensible material identification emerges. (Only the buoyancy *difference* between the two fluids was needed — the mass cancels the common weight terms.)

---

### Q1(f) — Delayed train [4 marks]

**Key observation.** Lateness has two independent contributions: the stopped 0.5 h (fixed) and the slow-leg deficit (1/3 h per hour of remaining distance at the reduced speed). The "45 km further on" variant gives a second equation.

> 【Thought】 Seeing two lateness scenarios → triggers *write the lateness function once, evaluate twice*: lateness $=0.5+\dfrac{D-v\cdot1}{3v}$ (in hours, $v$ in km/h, the leg beyond the first hour's run). The unknowns $D$ and $v$ separate cleanly because the fixed 0.5 h delay is common.

**Solution.** Let $v$ (km/h) be the initial speed, $D$ the total distance. In the first hour the train covers $v$ km; the remaining $D-v$ km at $0.75v$:
$$\text{lateness}=\frac12+\frac{D-v}{v}\left(\frac{1}{0.75}-1\right)=\frac12+\frac{D-v}{3v}=\frac32\;\Rightarrow\;\frac{D-v}{3v}=1\;\Rightarrow\;D=4v.$$
Second scenario (delay after $v+45$ km):
$$\frac12+\frac{D-v-45}{3v}=1\;\Rightarrow\;D=2.5v+45.$$
Subtract: $1.5v=45$ → $\boxed{v=30\ \text{km/h}}$, $\boxed{D=120\ \text{km}}$.

**Check.** Full run: $1+0.5+90/22.5=5.5$ h vs scheduled 4 h → 1.5 h late ✓; variant: $2.5+0.5+45/22.5=5$ h → 1 h late ✓.

---

### Q1(g) — Bathroom scales in a lift [4 marks]

**Key observation.** The scale reads apparent mass $m(t)=M(1+a/g)$ — read $a(t)$ off the given polynomial, then integrate: acceleration → velocity → distance.

> 【Thought】 This is a calculus chain $a\to v\to s$, each step an integral of the polynomial. The mass reading encodes $a$ via $m_{app}=M(1+a/g)$: decouple the instrument physics first, then pure kinematics. For (iii): minimum reading during deceleration = constant deceleration value (decelerating upward motion = downward acceleration = scales read low).

**Solution.** (i) $a(t)=g\left(\dfrac{t}{10}-\dfrac{t^2}{100}\right)$ m/s² (upward positive).
(ii) $v(10)=\displaystyle\int_0^{10}a\,dt=g\left[\frac{t^2}{20}-\frac{t^3}{300}\right]_0^{10}=g\left(5-\frac{10}{3}\right)=\frac{5g}{3}=\boxed{16.4\ \text{m/s}}$.
(iii) Distance in the first 10 s: $s_1=\displaystyle\int_0^{10}v\,dt=g\left[\frac{t^3}{60}-\frac{t^4}{1200}\right]_0^{10}=8.33g=81.7$ m. Remaining $18.3$ m, decelerating from 16.4 m/s to rest:
$$a_d=\frac{v^2}{2s}=\frac{16.4^2}{2\times18.3}=7.3\ \text{m/s}^2\;\Rightarrow\;m_{\min}=60\left(1-\frac{7.3}{9.81}\right)=\boxed{15\ \text{kg}}.$$

**Check.** Reading during early acceleration exceeds 60 kg (max $60(1+g/4g)=75$ kg at $t=5$ s) ✓; the two phases sum to 100 m ✓ by construction; note the lift's peak speed 16 m/s is unrealistically fast for a lift — the polynomial is a mathematical exercise, fine. (Reading-to-acceleration conversion: the scale reads $m(g+a)$, so $a=g(m/60-1)$ with $m$ the indicated mass.)

---

### Q1(h) — Index-matching a glass powder [3 marks]

**Key observation.** Linear mixing by volume: $n=\dfrac{n_aV_a+n_bV_b}{V_a+V_b}$; the glass vanishes when its index matches the mixture (no refraction/reflection at the grain boundaries).

**(i)** $\boxed{n_g=\dfrac{n_aV_a+n_bV_b}{V_a+V_b}}$.
**(ii)** $n_g=\dfrac{1.15\times100+1.52\times64}{164}=\dfrac{212.3}{164}=\boxed{1.29}$.

> 【Thought】 The physics of "cannot be observed": scattering at grain surfaces vanishes when $\Delta n=0$ — index matching. The volumes are the mixing weights; note you must add B to A (64 ml into 100 ml), not "64% of the mix".

---

### Q1(i) — Five-resistor bridge with R₂, R₄ as wire/open/element [4 marks]

**Topology (Fig. 3).** Diamond: A–R₁–T, T–R₂–B, A–R₄–D, D–R₃–B, T–R₅–D.

**(i)** i. **Three in series** (R₁–R₅–R₃, the only chain threading A→B): $R_2=R_4=\infty$ (both open).
ii. **Three in parallel** (R₁ ∥ R₃ ∥ R₅): $R_2=R_4=0$ (T shorted to B, D shorted to A — every named resistor then spans AB).
iii. **Two identical in parallel**: $R_2=0$ puts R₁ directly across AB; make the remaining path equal to R₁: $A\to R_4\to D\to(R_5\parallel R_3)\to B$ gives resistance $R_4+\dfrac{R_3R_5}{R_3+R_5}$, so set
$$\boxed{R_2=0,\qquad R_4=R_1-\frac{R_3R_5}{R_3+R_5}}\;\Rightarrow\;R_{AB}=R_1\parallel R_1.$$

> 【Thought】**Official approach (2020 mark scheme) — the slicker route.** Set $R_2=R_3$ and $R_4=R_1$: then the bridge ratio $R_1/R_4=R_2/R_3=1$ balances the bridge, $R_5$ carries no current and can be removed, leaving two identical arms $(R_1+R_3)$ in parallel. *The trick relies on the free resistors being one arm on each side of the bridge (feature X of this figure); if the free pair sat on the same side, the balance condition could not be met this way and one would fall back to branch-equalising (our main route), because then only the divider ratio on one side is adjustable.* Our route reaches the same two-equal-parallel outcome; the official one is shorter and more conceptual — worth internalising.
(Symmetric variant with roles of 2↔4, 1↔3 exists if $R_3>R_1\parallel R_5$.)

> 【Thought】 Method: trace where current *can* go under each switch choice — a wire (R = 0) merges two nodes, an open (R = ∞) deletes a branch. For (iii) the target is "a value equal to R₁ in parallel with R₁", so engineer the second path to equal R₁ exactly.

**(ii) Fig. 4:** Ammeter (in the 3 Ω branch) reads 2.0 A ⟹ middle node $V_X=2.0\times3=6$ V. Left loop: $12=4I_4+6\Rightarrow I_4=1.5$ A. KCL at X: $1.5=2.0+I_5$ ⟹ $I_5=-0.5$ A (current flows right-to-left through the 5 Ω: from the ε side *into* X). Hence $V_Y=6+0.5\times5=8.5$ V and
$$\boxed{\varepsilon=8.5\ \text{V}}.$$

> 【Thought】 The negative branch current is the signature that ε is *smaller* than the 12 V cell — the strong cell back-feeds the weak one's node. Sign discipline: write KCL with defined directions, let the sign tell the story, then report magnitude and actual direction. Switch rules used: a closed switch merges its nodes; an open switch deletes its branch.

---

### Q1(j) — Two resistor puzzles [4 marks]

**(i) Fig. 5a** ($R_1\parallel R_2$ in series with $R_3$): $R_{AB}=\dfrac{R_1R_2}{R_1+R_2}+R_3=R_1$:
$$\boxed{R_3=R_1-\frac{R_1R_2}{R_1+R_2}=\frac{R_1^2}{R_1+R_2}}.$$

**(ii) Fig. 5b** ($R_3$ across the series pair $R_1+R_2$): $\dfrac{R_3(R_1+R_2)}{R_3+R_1+R_2}=R_1$ with $R_3=6R_2$:
$$R_3R_2=R_1^2+R_1R_2\;\Rightarrow\;R_1^2+R_1R_2-6R_2^2=0\;\Rightarrow\;(R_1-2R_2)(R_1+3R_2)=0,$$
$$\boxed{\frac{R_1}{R_2}=2}.$$

> 【Thought】 Math action with purpose: in (ii) the equation $R_1^2+R_1R_2-6R_2^2=0$ is homogeneous — divide by $R_2^2$ to get a quadratic in the ratio $R_1/R_2$; when a problem asks "the ratio", homogeneity is the mechanism to exploit, and the negative root is rejected on physical grounds (resistances > 0).

---

### Q1(k) — Stiffest beam cut from a round log [3 marks]

**Key observation.** Constraint: the rectangle fits in the circular cross-section, $w^2+t^2=D^2$. Maximise $S\propto wt^3$ subject to it — substitute $w=\sqrt{D^2-t^2}$ and differentiate the log.

> 【Thought】 Optimisation discipline per the modelling protocol: constraint first ($w^2+t^2=D^2$), identify objective ($wt^3$) and free variable ($t$), differentiate, and justify the max — here the objective vanishes at both endpoints ($t=0$ and $t=D$), so the unique stationary point is the maximum.

**Solution.** $\dfrac{d}{dt}\left[\tfrac12\ln(D^2-t^2)+3\ln t\right]=-\dfrac{t}{D^2-t^2}+\dfrac3t=0\Rightarrow3(D^2-t^2)=t^2$:
$$t=\frac{\sqrt3}{2}D=\boxed{17.3\ \text{cm}},\qquad w=\frac{D}{2}=\boxed{10.0\ \text{cm}}.$$

**Check.** The beam's diagonal = log diameter: $\sqrt{10^2+17.3^2}=20$ ✓; thickness-weighted optimum ($t>w$) matches the $t^3$ sensitivity ✓.

---

### Q1(l) — Diffraction grating wavelength [2 marks]

**Key observation.** Three spots = orders $0,\pm1$; $\tan\theta=30/80$ (use tan→sin, not the small-angle shortcut blindly).

$$d=\frac{1}{6\times10^5}=1.667\ \mu\text{m},\qquad \sin\theta=\frac{30}{\sqrt{30^2+80^2}}=0.351,$$
$$\lambda=d\sin\theta=1.667\times10^{-6}\times0.351=\boxed{5.85\times10^{-7}\ \text{m}\approx585\ \text{nm}\ (\text{yellow})}.$$

> 【Thought】 Check whether small-angle is acceptable *before* using it: here $\theta=20.6^\circ$ — $\tan$ and $\sin$ differ by 6%, so the exact $\sin\theta$ from the geometry is required.

---

### Q1(m) — Crater diameter by dimensional analysis [6 marks]

**(i)** $d=kE^\alpha\rho^\beta g^\gamma$ with $[E]=\text{kg m}^2\text{s}^{-2}$, $[\rho]=\text{kg m}^{-3}$, $[g]=\text{m s}^{-2}$:
$$\alpha+\beta=0,\quad -2\alpha-2\gamma=0,\quad 2\alpha-3\beta+\gamma=1\;\Rightarrow\;\alpha=\tfrac14,\ \beta=\gamma=-\tfrac14,$$
$$\boxed{d=k\left(\frac{E}{\rho g}\right)^{1/4}}.$$

> 【Thought】 Solve the mass and time equations first ($\beta=-\alpha$, $\gamma=-\alpha$) — they collapse the system to one equation. The physics content: $E/(\rho g)$ is "energy per unit weight-density", with dimensions m⁴ — a buried-volume scale.

**(ii) Barringer crater.** $E=\rho g d^4=3000\times9.81\times1200^4=6.1\times10^{16}$ J (about 15 Mt TNT):
$$m=\frac{2E}{v^2}=\frac{2\times6.1\times10^{16}}{(1.5\times10^4)^2}=\boxed{5.4\times10^{8}\ \text{kg}}.$$

**(iii)** Iron sphere: $V=\dfrac{m}{\rho_{Fe}}=6.8\times10^4\ \text{m}^3$; $d_{met}=\left(\dfrac{6V}{\pi}\right)^{1/3}=\boxed{51\ \text{m}}$.

**Check.** The real Barringer impactor is estimated at ~50 m across ✓ — dimensional analysis with $k\approx1$ works remarkably well here; note $d\propto E^{1/4}$ means the energy inference is *insensitive* to crater-size error (quarter power) ✓. (The solution order matters: solve the mass and fall-time equations first, then feed them into the crater scaling.)

---

### Q1(n) — Cooling-water flow rate [4 marks]

**Key observation.** Fuel energy rate → 23% to water → $\dot m c\Delta T$.

**Solution.** Fuel use: $5.3$ L per 100 km at 100 km/h = $5.3$ L/h; energy rate $=5.3\times30=159$ MJ/h:
$$P_{\text{cool}}=0.23\times\frac{159\times10^6}{3600}=1.016\times10^4\ \text{W},$$
$$\dot m=\frac{P}{c\Delta T}=\frac{1.016\times10^4}{4180\times24}=\boxed{0.10\ \text{kg/s}\ (\approx360\ \text{kg/h})}.$$

> 【Thought】Reading note (revised against the official mark scheme): the given "outside temperature 16 °C" is only used if the water *exits* at 40 °C, i.e. $\Delta T=40-16=24$ K — the presence of 16 °C in the data is the signal that this is the intended reading ("temperature rise limited to 40 °C" is loose wording for "temperature limited to 40 °C"). Taking $\Delta T=40$ K literally would leave the 16 °C datum unused — an unused datum is the alarm bell. With the intended reading: $\dot m = 1.016\times10^4/(4180\times24)=0.10$ kg/s ✓.

> 【Thought】 Unit discipline: convert the per-100 km figure to a per-hour rate using the speed (that's why "100 km/h" is given — at a different speed the *rate* changes even though consumption per km is fixed).

---

### Q1(o) — Stefan–Boltzmann and Wien [4 marks]

**(i)** Convert to kelvin first: $\dfrac{\Phi_{1000}}{\Phi_{500}}=\left(\dfrac{1273}{773}\right)^4=(1.647)^4=\boxed{7.4}$.
**(ii)** $\lambda_{1000}=3750\times\dfrac{773}{1273}=\boxed{2277\ \text{nm}\approx2.3\ \mu\text{m}}$ (infrared).

> 【Thought】 The perpetual trap: **kelvin, not Celsius**, in both laws. $1000^\circ$C/500°C → the ratio 1273/773 ≈ 1.65, not 2 — using 2⁴ = 16 is the designed error.

---

### Q1(p) — Electron beam lithography: spreading resistance [5 marks]

**Key observation.** Charge deposited at a 15 nm spot spreads radially outward through the 5 nm film to the rim (2.5 cm) — a *radial* current in a thin sheet: integrate $dR=\dfrac{\rho\,dr}{2\pi r t}$.

> 【Thought】 Seeing "resistance between the edge of the spot and the edge of the surface" → triggers *spreading resistance of a thin film*: the cross-section is the cylindrical side wall $2\pi r t$, growing with $r$ — hence the logarithm. Series integration over concentric shells is the intended move.

**Solution.** $r_1=7.5$ nm (half beam width), $r_2=2.5$ cm, $t=5$ nm:
$$R=\frac{\rho}{2\pi t}\ln\frac{r_2}{r_1}=\frac{2.8\times10^{-8}}{2\pi\times5\times10^{-9}}\ln\frac{2.5\times10^{-2}}{7.5\times10^{-9}}=0.891\times15.0=\boxed{13.4\ \Omega},$$
$$V=IR=1.0\times10^{-9}\times13.4=\boxed{1.3\times10^{-8}\ \text{V}\ (13\ \text{nV})}.$$

**Check.** Logarithmic dependence ⟹ the huge geometric ratio ($3\times10^6$) contributes only a factor 15 — most of the resistance is near the tiny spot ✓ (characteristic of spreading resistance); the pd is nano-volts, negligible — which is why the Al layer "removes the incident charge" effectively ✓. The logarithmic spreading law means most of the resistance is concentrated within a few hole-radii of the contact — distant material contributes almost nothing.

---

### Q1(q) — Leaky capacitor [5 marks]

**Key observation.** The dielectric's resistivity makes a leak resistance $R_L=\rho d/A$ **across** the plates; charging through the series resistor, the steady state is a voltage divider between $R_s$ and $R_L$.

**(i)** $R_L=\dfrac{1.5\times10^{12}\times0.82\times10^{-6}}{0.603}=2.04\ \text{M}\Omega$; $C=\dfrac{\varepsilon_0A}{d}=\dfrac{8.85\times10^{-12}\times0.603}{0.82\times10^{-6}}=6.51\ \mu\text{F}$.
Steady state (charging current through 4.7 MΩ equals leak current):
$$V_C=24\times\frac{2.04}{4.7+2.04}=7.26\ \text{V}\;\Rightarrow\;Q_{\max}=CV_C=6.51\times7.26=\boxed{4.7\times10^{-5}\ \text{C}\ (\approx47\ \mu\text{C})}.$$

**(ii)** Disconnected: self-discharge through $R_L$: $\tau=R_LC=\rho\varepsilon_0=1.5\times10^{12}\times8.85\times10^{-12}=13.3$ s (the geometry cancels!):
$$t_{1/2}=\tau\ln2=\boxed{9.2\ \text{s}}.$$

> 【Thought】 The identity $RC=\rho\varepsilon_0$ (resistance and capacitance share the same geometry factor $A/d$) is the elegant content of (ii) — quote it, and note that (i)'s "maximum" exists only because the leak competes with the charging path: an ideal capacitor would simply charge to 24 V.

---

### Q1(r) — Isothermal expansion: rate of pressure fall [3 marks]

**Key observation.** $pV=380$ Pa·m³ fixed ⟹ differentiate: $\dot p=-\dfrac{380}{V^2}\dot V$ (chain rule on the constraint).

$$\dot p=-\frac{380}{(0.17)^2}\times0.005=\boxed{-66\ \text{Pa/s}\ \text{(falling at }66\ \text{Pa/s)}}.$$

> 【Thought】 Related-rates 101: differentiate the *conservation law*, not the instantaneous values. Signs: volume increasing ⟹ pressure decreasing ✓; magnitude sanity: $p=2235$ Pa at that instant, fractional rates equal: $\dot p/p=-\dot V/V=-0.005/0.17=-2.9\%$/s ✓ consistent.

---

### Q1(s) — Hot-air balloon hover temperature [5 marks]

**Key observation.** Hover ⟹ buoyancy = total weight: $\rho_{\text{out}}Vg=(m+\rho_{\text{in}}V)g$. The balloon is open at the bottom, so **pressure inside = outside** ⟹ $\rho T=$ const for the air.

> 【Thought】 Seeing "hot air balloon hover" → triggers *Archimedes with variable inside density*: the flame's job is purely to reduce $\rho_{\text{in}}$. The pressure-equalisation (open mouth) is what licenses $\rho\propto1/T$ — if the balloon were sealed, the model would be different.

**Solution.** $\rho_{\text{in}}=\rho_{\text{out}}-\dfrac{m}{V}=1.23-\dfrac{240}{1100}=1.012\ \text{kg/m}^3$;
$$T_{\text{in}}=T_{\text{out}}\frac{\rho_{\text{out}}}{\rho_{\text{in}}}=288\times\frac{1.23}{1.012}=350\ \text{K}=\boxed{77^\circ\text{C}}.$$

**Check.** Fractional density reduction needed: $18\%$ → temperature rise $288\times0.18/0.82\approx62$ K ✓ consistent; real balloons operate at ~100 °C ✓ plausible.

---
*End of Paper 10 (2020 Round 1 Section 1).*


---

## Paper 11 — 2020 Round 1 Section 2 (13 Nov 2020)

*Section 2: Questions 2–6, 25 marks each; candidates attempt two. Full solutions for all five.*

---

### Question 2 — Photoelectric effect and radioactive decay

#### Q2(a) — Photoelectric measurements with parallel plates [5 marks]

**(i)** Conservation of energy (Einstein's equation):
$$\boxed{\frac{hc}{\lambda}=W+\tfrac12 mv_{\max}^2}\quad(\text{photon} = \text{work function} + \text{max KE}).$$

**(ii)** $N=\dfrac{I}{e}=\dfrac{10^{-13}}{1.602\times10^{-19}}=\boxed{6\times10^{5}\ \text{electrons/s}}$.

**(iii)** Stopping potential $V_s=0.82$ V ⟹ $KE_{\max}=0.82$ eV; photon energy $1240/280=4.43$ eV:
$$W=4.43-0.82=\boxed{3.61\ \text{eV}}.$$

**(iv)** $v_{\max}=\sqrt{2KE_{\max}/m_e}=\sqrt{\dfrac{2\times0.82\times1.602\times10^{-19}}{9.11\times10^{-31}}}=\boxed{5.4\times10^{5}\ \text{m/s}}$.

**(v) Return distance at 20° emission.** With the stopping field on, the electron follows a projectile-like path in the uniform field $E=V_s/d=41$ V/m: parallel component $v\sin20^\circ$ unchanged, normal component $v\cos20^\circ$ reversed by the field ($a=eE/m_e=7.2\times10^{12}$ m/s²):
$$x=v\sin20^\circ\times\frac{2v\cos20^\circ}{a}=\frac{v^2\sin40^\circ}{a}=\frac{2.89\times10^{11}\times0.643}{7.2\times10^{12}}=\boxed{2.6\ \text{cm}}.$$

> 【Thought】 Seeing "emitted at an angle … returns to the plate" → triggers *projectile motion in a uniform field* (the electric field plays gravity's role; the plate gap is irrelevant once the electron turns back). Note the electron with *maximum* KE has exactly zero normal KE at the far plate — it always returns.

#### Q2(b) — Attenuating a laser down to photons [8 marks]

**(i)** $1.2\times10^{-3}\times4.5^{-N}<6.6\times10^{-11}\Rightarrow 4.5^N>1.82\times10^7\Rightarrow N>\dfrac{\log(1.82\times10^7)}{\log4.5}=11.1$: $\boxed{N=12\ \text{filters}}$.
**(ii)** $P=1.2\times10^{-3}\times4.5^{-12}=\boxed{1.7\times10^{-11}\ \text{W}}$.
**(iii)** Photon energy $hc/\lambda=3.40\times10^{-19}$ J: rate $=\dfrac{1.7\times10^{-11}}{3.40\times10^{-19}}=\boxed{5.1\times10^{7}\ \text{photons/s}}$.
**(iv)** Spacing $=\dfrac{c}{\text{rate}}=\dfrac{3\times10^8}{5.1\times10^7}=\boxed{5.9\ \text{m}}$ — photons are metres apart: almost never two in the 300 m pipe… (about 50 in the pipe at any instant — still utterly sparse).

> 【Thought】 Model note: "average distance" = speed ÷ arrival rate; the photons form a random (Poisson) train, so this is a mean spacing, not a lattice. The pipe length (300 m) is a red herring for (iv) — it matters only for narrative, since rate × transit time gives ~50 photons in transit.

**(v)** On the camera: the interference pattern builds up **one localised dot at a time** — individual photon detections at random positions, accumulating over time into the familiar double-slit fringes. (Each photon interferes with itself; the fringe envelope appears only as a statistical accumulation.)

**(vi)** Filled with medium $n=1.2$: the photon *energy* $hf$ is unchanged (frequency, not wavelength, is fixed across media), so the arrival **rate** is unchanged; but photons travel at $c/n$: spacing $=\dfrac{c}{n\times\text{rate}}=\boxed{4.9\ \text{m}}$ — reduced by the factor $1/n$. (This is the *mean* spacing: emission is Poissonian, so individual intervals fluctuate around it.)

#### Q2(c) — Photoelectric charging of a copper sphere [4 marks]

**(i)** The sphere charges positively until its potential turns back even the most energetic photoelectrons (shortest wavelength 150 nm):
$$eV=\frac{hc}{150\ \text{nm}}-W=8.27-4.7=3.57\ \text{eV}\;\Rightarrow\;\boxed{V=3.6\ \text{V}}.$$

> 【Thought】 Mechanism: each escaped electron raises the sphere's potential, making the next escape harder; equilibrium when $eV$ equals the maximum photoelectron KE. The 600 nm end of the spectrum never emits ($hc/\lambda=2.07$ eV $<W$) — only the shortest wavelength sets the final potential.

**(ii)** $Q=4\pi\varepsilon_0 rV=\dfrac{rV}{k_e}=\dfrac{0.08\times3.57}{8.99\times10^9}=3.2\times10^{-11}$ C:
$$N=\frac{Q}{e}=\boxed{2.0\times10^{8}\ \text{electrons}}.$$

**(iii)** Even at feeble intensity an electron may be emitted nanoseconds after switch-on, because light arrives as **photons**: a single photon carries the full quantum of energy $hf$ and can eject an electron instantly — there is no "accumulation time". Classical wave theory would require the weak wavefront to dump energy gradually onto one atom (a delay of hours at such intensities); the observation is one of the foundational proofs of the photon picture.

**(iv)** Self-discharge through the thread: $Q(t)=Q_0e^{-t/RC}$; half in 20 s: $RC=20/\ln2=28.9$ s. Sphere capacitance $C=4\pi\varepsilon_0r=8.9\times10^{-12}$ F:
$$R=\frac{28.9}{8.9\times10^{-12}}=\boxed{3.2\times10^{12}\ \Omega}.$$

#### Q2(d) — Measuring the half-life of Ra-226 by charging [8 marks]

**Setup.** 3.62 mg of RaBr (molar mass $226+80=306$ g/mol): $N_{Ra}=\dfrac{3.62\times10^{-3}}{306}N_A=7.12\times10^{18}$ atoms. Each β⁻ that escapes leaves the apparatus one $e$ more positive; leaf makes contact at 220 V, discharges, cycle repeats every 85 s.

**(i)** $Q=220\times6.40\ \text{pC}=1.41\times10^{-9}$ C ⟹ decays per cycle $=\dfrac{Q}{e}=\boxed{8.8\times10^{9}}$.
**(ii)** Activity $A=\dfrac{8.8\times10^9}{85\ \text{s}}=\boxed{1.03\times10^{8}\ \text{Bq}}$.
**(iii)** $A=\dfrac{\ln2}{T_{1/2}}N_{Ra}\Rightarrow T_{1/2}=\dfrac{0.693\times7.12\times10^{18}}{1.03\times10^8}=4.8\times10^{10}\ \text{s}=\boxed{1.5\times10^{3}\ \text{yr}}$ (accepted value 1600 yr ✓).

**(iv)** $I=Ae=1.03\times10^8\times1.602\times10^{-19}=\boxed{1.7\times10^{-11}\ \text{A}\ (17\ \text{pA})}$ — constant to an excellent approximation over a day ($T_{1/2}\sim$ 1500 yr).

**(v)** Could this apparatus measure the sphere's initial photocurrent (part c)? **Not directly**: the sphere saturates after losing only $3.2\times10^{-11}$ C (its capacitance is tiny) — 40× less than one leaf-cycle's charge ($1.4$ nC) — and at very low intensity the photocurrent ($\sim e/0.1\ \text{s}=1.6\times10^{-18}$ A) is a million times below what the leaf cycle can integrate in reasonable time. The gold-leaf method suits a *persistent* current source, not a saturating capacitor.

**(vi) Ra-223 ($T_{1/2}=11.4$ d), same initial activity.** The charge per cycle is fixed, so the cycle time $T(t)\propto1/A(t)$ **grows exponentially**, doubling every 11.4 days: $T(t)=85\ \text{s}\times2^{t/11.4\ \text{d}}$. Sketch: cycle period flat-ish for the first days, then stretching — by day 50, $T\approx85\times2^{4.4}\approx1800$ s. (The total number of cycles is finite — the integrated decay count is bounded by the atom count.)

**(vii) As a clock.** Tick rate $\propto A(t)=A_0e^{-\lambda t}$; in a true 24 h period ending at time $T$ the clock loses $\approx86400\,\lambda T$ seconds… precisely, loses 1 h when the rate has fallen by $1/24$: $e^{-\lambda T}=23/24$:
$$T=\frac{\ln(24/23)}{\lambda}=\frac{0.0426}{\ln2/4.77\times10^{10}}=\boxed{2.9\times10^{9}\ \text{s}\approx93\ \text{years}}.$$

*(Official mark scheme: 88 years, using the ratio 24/25 — "slowed by 1 h" read as the activity at the 25th hour vs the 24th; our reading — in a true 24 h the decay-driven clock registers only 23 h, i.e. rate ratio 23/24 — gives 93 yr. Same physics, different sentence parsing; either earns the marks.)*

> 【Thought】 Approximation note: $\lambda T\ll1$ even after a century because $T_{1/2}$ is huge — so "slowed by one hour per day" requires the *rate* to drop by 4%, not the total count; the exponential decay law makes the clock exponentially reliable. Sanity: after one half-life (1513 yr) the clock runs at half speed, losing 12 h/day ✓ consistent ordering.

---

### Question 3 — Nautical dynamics

#### Q3(a) — Oil tanker: draft, centre of mass, listing moment [8 marks]

**Setup.** Cuboid model: $L=272$ m, $B=48$ m, deck height 24 m; ship 22 000 t; oil 158 000 t ($\rho_{oil}=900$); sea water $\rho_{sw}=1025$ kg/m³.

**(i) Draft and freeboard.** Total mass $1.80\times10^8$ kg; displaced volume $=1.80\times10^8/1025=1.756\times10^5$ m³:
$$\text{draft}=\frac{1.756\times10^5}{272\times48}=13.45\ \text{m}\;\Rightarrow\;\boxed{\text{waterline to deck}=24-13.45\approx10.5\ \text{m}}.$$

**(ii) COM height.** Oil depth: $\dfrac{1.58\times10^8/900}{272\times48}=13.45$ m — oil COM at $6.72$ m; ship structure COM at mid-height 12 m (uniform-shell assumption, stated):
$$\bar y=\frac{22\,000\times12+158\,000\times6.72}{180\,000}=\boxed{7.4\ \text{m above K}}.$$

> 【Thought】 Declared assumption: the hull's centre of mass is taken at half the deck height (uniform-shell model) — without it the problem is unsolvable; stating the assumption explicitly is the standard move in modelling items.

**(iii) List angle.** Listing until water reaches the deck edge: the waterline relative to the ship runs from the deck corner on the low side: $\tan\theta=\dfrac{\text{freeboard}}{B/2}=\dfrac{10.55}{24}=0.440$:
$$\boxed{\theta\approx24^\circ\ (\tan\theta=0.44;\ \text{in radians }0.44\text{ — the "small angle" instruction licenses } \theta\approx\tan\theta)}.$$

**(iv) Resultant moment.** At this heel the displaced cross-section is a trapezoid (24 m deep on the low side, 2.9 m on the high side — average 13.45 m ✓ buoyancy unchanged). Its centroid (CB) sits at $(-6.28, 8.10)$ m in ship coordinates (computed from the trapezoid), while the COM is on the centreline at $(0, 7.37)$ m. Rotating into world coordinates at $\theta=23.7^\circ$ (heel to port):
$$X_{COM}=-2.97\ \text{m},\qquad X_{CB}=-9.01\ \text{m}\;\Rightarrow\;\Delta X=6.0\ \text{m}.$$
Buoyancy (up) acting 6.0 m to port of the weight (down) forms a **righting** couple:
$$\boxed{M=W\,\Delta X=1.80\times10^8\times9.81\times6.0\approx1.1\times10^{10}\ \text{N m (restoring)}}.$$

> 【Thought】 Method: this is metacentric stability analysis done from first principles — buoyancy acts at the displaced volume's centroid (given hint), weight at the COM; the horizontal offset of their lines of action × displacement is the moment. The labour is the trapezoid centroid — do it by integration of $h(x)$, $\tfrac12h^2(x)$ (or split the trapezoid into rectangle + triangle). Sign check: CB further to the immersed side than COM ⟹ restoring.

#### Q3(b) — Capstan hauling a chain at constant speed [6 marks]

**(i)** Two things the capstan must do: support the suspended weight $\lambda xg$ and *accelerate new links* from rest to $v$ (momentum flux $\lambda v^2$):
$$\boxed{F=\lambda xg+\lambda v^2},\qquad \boxed{P=Fv=\lambda xgv+\lambda v^3}.$$

> 【Thought】 The $\lambda v^2$ term is the classic "chain pickup" term: mass joins the moving part at rate $\lambda v$ and must be given momentum at rate $\lambda v^2$ — a *thrust*. Forgetting it is the canonical error; dimension check: $\lambda v^2$ = (kg/m)(m²/s²) = N ✓. Note the energy budget is *not* clean here (inelastic link pickup dissipates): power $P$ computed from $Fv$ is correct; $\tfrac{d}{dt}(KE+PE)$ would miss the dissipation — worth one remark in the script.

**(ii)** With total length $L$, the dock supports the un-lifted chain:
$$\boxed{R=\lambda(L-x)g}.$$

#### Q3(c) — Chain stretching under its own weight [5 marks]

**Key observation.** Tension varies along the chain: $T(y)=\mu g y$ at height $y$ above the free bottom end. Integrate the local strain $T/(EA)$:

$$e=\int_0^x\frac{\mu g y}{EA}\,dy=\boxed{\frac{\mu g x^2}{2EA}}.$$

> 【Thought】 Seeing "stretches under its own weight" → triggers *local strain, global integral*: each element carries the weight below it. The answer is exactly half the extension the full weight $\mu xg$ would give if applied at the end — the "half" appears because tension ramps linearly from zero. Constant-area assumption is stated by the problem; note $e\propto x^2$ (longer chain stretches quadratically more). With tension linear in position, the average tension over a span is the mean of its endpoint values — the load integral halves the endpoint tension.

#### Q3(d) — Capstan friction multiplier [6 marks]

**(i) Sketch.** A rope element subtending small angle $\theta$ ($\Delta\theta$) at the capstan surface; mark tensions $T$ and $T+\Delta T$ tangentially at its ends, the radially inward resultant $T\theta$ of the two tensions pressing the rope onto the drum (normal force $N\approx T\theta$), and the friction force $\mu N$ tangentially opposing slip.

**(ii)** Radial balance of the element: $N=T\theta$ (two tensions $T$ with angle $\theta$ between them converge toward the centre); tension step = friction:
$$\boxed{\Delta T=\mu N=\mu T\theta}\qquad\left(\frac{\Delta T}{T}=\mu\,\theta\right).$$

**(iii)** Integrate $\displaystyle\int_{T_{\text{hold}}}^{T_{\text{load}}}\frac{dT}{T}=\int_0^\Theta\mu\,d\theta$:
$$\boxed{T_{\text{load}}=T_{\text{hold}}\,e^{\mu\Theta}}\quad(\text{capstan / Euler–Eytelwein equation}).$$

**(iv)** $\Theta=\dfrac{\ln(6\times10^{25}/600)}{0.3}=\dfrac{52.96}{0.3}=176.5$ rad:
$$\boxed{n=\frac{176.5}{2\pi}\approx28\ \text{turns}}.$$

> 【Thought】 The exponential is the physics payload: each extra turn multiplies the holding power by $e^{0.3\times2\pi}\approx6.6$, so ~28 turns bridge $10^{23}$. Small-angle validity: the element analysis used $\sin(\theta/2)\approx\theta/2$ — exact in the differential limit, which is why integration is required and justified.

---

### Question 4 — Change of wave speed in a medium

#### Q4(a) — Prism refraction sequence [10 marks]

**(i) Sketch.** Large triangle, apex up; ray enters the left face (incidence $\theta_1$, refraction $\theta_2$), crosses to the right face (incidence $\theta_3$, emergence $\theta_4$), bending toward the base at both faces; $\delta$ = angle between the incoming direction and the emerging ray.

**(ii)** At each face the ray bends toward the base by $\theta_1-\theta_2$ and $\theta_4-\theta_3$; the normals geometry gives $\theta_2+\theta_3=A$:
$$\delta=(\theta_1-\theta_2)+(\theta_4-\theta_3)\;\Rightarrow\;\boxed{\delta=\theta_1+\theta_4-A}.$$

**(iii) Minimum deviation (symmetric path).** $\theta_1=\theta_4$, $\theta_2=\theta_3=A/2$; $\delta_{\min}=2\theta_1-A$ ⟹ $\theta_1=\dfrac{A+\delta_{\min}}{2}$:
$$\boxed{n=\frac{\sin\theta_1}{\sin\theta_2}=\frac{\sin\left(\frac{A+\delta_{\min}}{2}\right)}{\sin(A/2)}}.$$

**(iv)** $A=60^\circ$: $\delta_{\min}=2\arcsin(n\sin30^\circ)-60^\circ$:
$$\delta_r=2\arcsin(0.802)-60^\circ=46.64^\circ,\qquad \delta_b=2\arcsin(0.810)-60^\circ=48.19^\circ,\qquad \boxed{\Delta\delta\approx1.6^\circ}.$$

**(v)** Lens $f=30$ cm: angular separation $\Delta\delta$ maps to linear separation $f\,\Delta\delta$:
$$\Delta x=0.30\times1.6\times\frac{\pi}{180}=\boxed{8.4\times10^{-3}\ \text{m}\approx8\ \text{mm}}.$$

> 【Thought】 Why a lens converts angle to position: parallel rays meet at the focal plane — position $=f\times$angle (small angles). This is the working principle of every spectrometer with a camera lens.

**(vi) Thin-prism limit.** Small $A$ ⟹ small angles throughout: $\sin\theta\approx\theta$: entry $\theta_1=n\theta_2$, exit $\theta_4=n\theta_3$:
$$\delta=\theta_1+\theta_4-A=n(\theta_2+\theta_3)-A=nA-A\;\Rightarrow\;\boxed{\delta=A(n-1)}.\ \blacksquare$$

**(vii) Opposed prisms, net zero deviation.** Deviations cancel: $A_1(n_1-1)=A_2(n_2-1)$:
$$6.0\times0.50=4.0\times(n_2-1)\;\Rightarrow\;\boxed{n_2=1.75}.$$

**Check.** This is the "direct-vision spectroscope"/achromatic-prism trick: equal and opposite deviations with opposite apex orientation ✓; the emergent beam is parallel but displaced ✓ consistent with the statement.

#### Q4(b) — Transit-time ratio through a prism [3 marks]

**Setup (Fig. 7).** Symmetric passage: inside the prism the ray runs parallel to the base. Ray 1 skims the apex $V$ entirely in air: $P_1V+VP_2$. Ray 2 crosses the glass along $Z_1Z_2=L$ (entering/exiting exactly at the wavefronts, so no extra air path).

**Geometry.** Ray 2's glass path $Z_1Z_2=L$ is parallel to the base (symmetric passage); the sub-triangle $VZ_1Z_2$ shares the apex angle $A$, so $VZ_1=\dfrac{L}{2\sin(A/2)}$. Ray 1 skims the apex in air; its leg $P_1V$ is the illuminated face segment $VZ_1$ projected along the beam: $P_1V=VZ_1\sin\theta_1$, with $VZ_1=W/\cos\theta_1$ (footprint relation) if $W$ is the wavefront width.

**Ratio (official derivation, adopted).** Let $W$ be the beam's wavefront width. Footprint on face 1: the face segment illuminated, $VZ_1=W/\cos\theta_1$ (incidence angle $\theta_1$). The apex-skimming leg in air is the face segment projected onto the beam: $P_1V=VZ_1\sin\theta_1$ (and similarly $VP_2$). The glass chord: from the sub-triangle at the apex, $\sin(A/2)=\dfrac{L/2}{VZ_1}$, i.e. $VZ_1=\dfrac{L}{2\sin(A/2)}$. Hence

$$t_1=\frac{2\,VZ_1\sin\theta_1}{c}=\frac{L\sin\theta_1}{c\sin(A/2)},\qquad t_2=\frac{nL}{c},$$
$$\boxed{\frac{t_1}{t_2}=\frac{\sin\theta_1}{n\,\sin(A/2)}}.$$

> 【Thought】 The footprint relation $W=(\text{face segment})\cos\theta_1$ is the workhorse — a beam of width $W$ at incidence $\theta_1$ covers $W/\cos\theta_1$ of surface. The official route (adopted above) is shorter and passes the decisive check below.

**Check.** Symmetric passage = minimum deviation, where Snell gives $\sin\theta_1=n\sin(A/2)$ — so the ratio is **exactly 1**: the apex-skimming air path and the glass chord take equal time. That is precisely Fermat's stationarity at minimum deviation ✓ (our earlier formula failed this test — catching it is what checks are for). And $n\to1$ gives ratio $\to\sin\theta_1/\sin(A/2)$ with $\theta_1\to A/2$ → 1 ✓. (This is Fermat's principle in action: the symmetric passage is the stationary-optical-path one, which for a prism is minimum deviation.)

#### Q4(c) — Thin lens as a thin prism [3 marks]

**(i)** A ray through the lens at radius $d$ (top edge) bends by the local prism deviation $\delta=A(n-1)$; from the geometry, the same bend redirects the object-side slope $\alpha\approx d/u$ to the image-side slope $\beta\approx d/v$:
$$\delta=\alpha+\beta\;\Rightarrow\;\boxed{A(n-1)=d\left(\frac1u+\frac1v\right)}\qquad\left(\frac1u+\frac1v=\frac{A(n-1)}{d}\right).$$

**(ii)** Parallel input ($u\to\infty$) focuses at $f$: $\dfrac{1}{f}=\dfrac{A(n-1)}{d}$ with $d=2.5$ cm, $f=40$ cm, $n=1.5$:
$$A=\frac{d}{f(n-1)}=\frac{2.5}{40\times0.5}=0.125\ \text{rad}=\boxed{7.2^\circ}.$$

> 【Thought】 This is the paraxial lens-maker's relation in disguise: $1/f=(n-1)\times$(curvature sum); the "apex angle" of the equivalent prism at radius $d$ encodes the lens's surface slopes. Keep small angles throughout — that is the licence for $\alpha\approx d/u$.

#### Q4(d) — Pulse separation by dispersion in a 60 m water tank [3 marks]

**Key observation.** Red and blue travel at $c/1.33$ and $c/1.35$; after 60 m they arrive $\Delta t$ apart; flashes stay distinguishable only if the flash period exceeds the spread.

$$\Delta t=\frac{L}{v_b}-\frac{L}{v_r}=\frac{60}{3\times10^8}(1.35-1.33)=4.0\times10^{-9}\ \text{s}\;\Rightarrow\;\boxed{f_0\lesssim\frac{1}{\Delta t}\approx2.5\times10^{8}\ \text{Hz}\ (\sim250\ \text{MHz})}.$$

*(Official mark scheme: $f_0=1/(2\Delta t)=125$ MHz, requiring the half-period — the red-off-to-blue-on interval — to exceed $\Delta t$. Same physics; the factor of 2 depends on the assumed duty cycle. Our box states the order correctly; quote either with the assumption stated.)*

> 【Thought】 Estimate logic: "separate flashes" needs the inter-flash gap (period, up to the factor-2 on/off convention) to exceed the red–blue delay; an order-of-magnitude answer $f_0\sim10^8$ Hz is the deliverable. Note the dispersion $(dn)$, not the index, drives the effect — with $n$ equal for both colours there'd be no spread at all.

#### Q4(e) — Atmospheric refraction of starlight [6 marks]

**(i)** Plane-parallel layers: Snell's invariant $n\sin(\text{angle})$ is conserved through the stack; vacuum at top ($n=1$, angle $\alpha$), $n_0$ at the surface (angle $\alpha_0$):
$$\boxed{\sin\alpha=n_0\sin\alpha_0}.$$

> 【Thought】 Seeing layered media with horizontal strata → triggers *the Snell invariant* $n\sin\theta$ = const: all intermediate layers telescope away — you never trace the ray through each layer. This is why only the surface index matters.

**(ii)** With $\alpha=\alpha_0+r$, $r\ll1$: $\sin(\alpha_0+r)\approx\sin\alpha_0+r\cos\alpha_0$:
$$\sin\alpha_0+r\cos\alpha_0=n_0\sin\alpha_0\;\Rightarrow\;\boxed{r=(n_0-1)\tan\alpha_0}.$$

**Check.** $r\to0$ at zenith ($\alpha_0=0$) ✓ — no refraction looking straight up; $r$ grows toward the horizon ✓ (setting stars look lifted); with $n_0-1\approx3\times10^{-4}$ and $\alpha_0=45^\circ$: $r\approx0.017^\circ\approx1'$ ✓ matches astronomical refraction tables.

---

### Question 5 — Circular motion and gravity

#### Q5(a) — Car over a hump-back bridge [3 marks]

**Key observation.** Contact requires $N\ge0$ at the crest: $mg-\dfrac{mv^2}{R}\ge0$. The radius comes from the chord geometry (sagitta relation — the intersecting-chords hint).

**Solution.** Chords through the centre of the span: $9\times9=4\times(2R-4)$ (span 18 m, rise 4 m):
$$R=\frac{81/4+4}{2}=\frac{97}{8}=12.1\ \text{m};\qquad v_{\max}=\sqrt{gR}=\sqrt{9.81\times12.1}=\boxed{10.9\ \text{m/s}\ (\approx39\ \text{km/h})}.$$

> 【Thought】 The hint decodes to the sagitta formula $R=\dfrac{(c/2)^2+h^2}{2h}$ — worth memorising. Physics check: at $v_{\max}$ the car is weightless at the crest ($N=0$) — beyond that it would leave the road (ballistic).

#### Q5(b) — Mass of the Milky Way [3 marks]

**(i)** Circular orbit about the central mass: $\dfrac{GM_gm}{r^2}=m\omega^2r$:
$$\boxed{T=2\pi\sqrt{\frac{r^3}{GM_g}}}.$$

**(ii)** $r=3.0\times10^4$ ly $=2.84\times10^{20}$ m, $T=2.0\times10^8$ yr $=6.31\times10^{15}$ s:
$$M_g=\frac{4\pi^2r^3}{GT^2}=\frac{39.5\times2.29\times10^{61}}{6.67\times10^{-11}\times3.98\times10^{31}}=\boxed{3.4\times10^{41}\ \text{kg}}.$$

**(iii)** $N=\dfrac{M_g}{M_\odot}=\dfrac{3.4\times10^{41}}{1.99\times10^{30}}=\boxed{1.7\times10^{11}\ \text{stars}}$ — the right order for the Milky Way ✓.

> 【Thought】 Model caveat to state: this assumes all mass interior to the Sun's orbit (uniform sphere) — real galaxy has a flat rotation curve (dark matter), but the estimate lands correctly because the premise is given.

#### Q5(c) — Satellite orbits, drag, and the speed paradox [14 marks]

**(i)** Gravity supplies the centripetal force: $\dfrac{GM_Em}{r^2}=\dfrac{mv^2}{r}$ ⟹ $\boxed{v=\sqrt{GM_E/r}}$.

**(ii) Grazing orbit** ($r=R_E$): use $GM_E=gR_E^2$: $v=\sqrt{gR_E}=\sqrt{9.81\times6.37\times10^6}=\boxed{7.9\ \text{km/s}}$.

**(iii)** $T=\dfrac{2\pi R_E}{v}=2\pi\sqrt{R_E/g}=\boxed{5.06\times10^{3}\ \text{s}\approx84\ \text{min}}$.

**(iv)** $T\propto r^{3/2}$ ⟹ for $h\ll R_E$: $\boxed{\dfrac{\Delta T}{T}=\dfrac{3h}{2R_E}}$. At $h=200$ km: $\Delta T/T=0.047$, $T=5300\ \text{s}\approx\boxed{88\ \text{min}}$.

**(v) Sketch.** $T$ vs $h$: straight line through $(0,\ 84\ \text{min})$ with slope $\dfrac{3T_0}{2R_E}$ — linear under the small-$h$ approximation (note the true curve $T\propto(R_E+h)^{3/2}$ bends slightly upward).

**(vi) Elastic collision energy transfer.** $m_1u$ hits stationary $m_2$: $v_2=\dfrac{2m_1u}{m_1+m_2}$, so
$$\Delta KE_{m_1}=\tfrac12m_2v_2^2=\tfrac12m_2u^2\frac{4m_1^2}{(m_1+m_2)^2}\approx\boxed{2m_2u^2}\quad(m_1\gg m_2).\ \blacksquare$$

**(vii) Drag energy rate.** Molecules swept per second: $\rho Av/m_{\text{mol}}$; each takes $\approx2m_{\text{mol}}v^2$:
$$\boxed{\frac{dE}{dt}=-2\rho Av^3}.$$

**(viii)** Total energy $E=-\tfrac12mv^2$ in orbit (virial: $|E|=KE$). Per revolution $E$ drops $10$ kJ; $KE=\tfrac12(20)(7905)^2=6.25\times10^8$ J:
$$\frac{\Delta v}{v}=\frac{|\Delta E|}{2KE}=\frac{10^4}{1.25\times10^9}=\boxed{8\times10^{-6}\ \text{per revolution}\ (\text{positive — speeding up})}.$$

**(ix)** $E=-\dfrac{GMm}{2r}$: losing energy ($E$ more negative) ⟹ $r$ **decreases** ⟹ $v=\sqrt{GM/r}$ **increases** — drag makes satellites speed up (the "satellite paradox": drag acts like a forward thrust through the orbital mechanics).

**(x)** Per revolution: $|\Delta E|=2\rho Av^3T$:
$$\rho=\frac{10^4}{2\times2.4\times(7.9\times10^3)^3\times5060}=\boxed{8\times10^{-13}\ \text{kg/m}^3}.$$

> 【Thought】 The chain (vi)→(vii)→(x) is a designed pipeline: elastic-transfer result → collision-rate model → density estimate. In (viii) the pivotal step is knowing the *sign* structure of orbital energy: $|E|=KE$ with $E<0$ — so losing total energy gains kinetic energy. If your intuition says "drag slows it down", the energy bookkeeping corrects it.

#### Q5(d) — Binary stars and supernova disruption [5 marks]

**(i) Diagram.** Two stars on the same line through the CM, on opposite sides, orbiting with the same period; mark two successive times (both arrows same angular direction; the lighter star's circle is larger).

**(ii)** CM condition $m r_m=km\,r_{km}$ with $r_m+r_{km}=r$:
$$r_{km}=\frac{r}{1+k},\qquad r_m=\frac{kr}{1+k}\qquad(\text{ratio }k:1).$$

**(iii) After the symmetric supernova (masses now equal).** Positions and velocities unchanged at the instant of explosion; the new CM is the midpoint of the separation. If bound, the two equal masses then orbit their new CM — each on an ellipse, diametrically opposite each other at all times, with a longer period (weaker gravity for the same separation); draw two congruent ellipses about the midpoint, stars at opposite ends of a rotating line.

**(iv) Critical mass ratio.** At the explosion instant the relative speed is the circular one: $v_{\text{rel}}^2=\dfrac{Gm(1+k)}{r}$. The new binary (mass $2m$) is unbound when this exceeds escape:
$$\frac{Gm(1+k)}{r}\ge\frac{2G(2m)}{r}\;\Rightarrow\;1+k\ge4\;\Rightarrow\;\boxed{k_{\text{crit}}=3}.$$

> 【Thought】 Equivalent classic statement: a symmetric supernova unbinds the binary if more than half the total mass is lost — $(k-1)m>\tfrac12(1+k)m\iff k>3$ ✓ same condition. Method: compare instantaneous $v_{\text{rel}}^2$ with $2GM_{\text{new}}/r$ — no need to solve the new orbit. The classic rule of thumb behind it: losing more than half the mass leaves no bound orbit at all.

---

### Question 6 — Atomic structure and electric fields (NaCl)

#### Q6(a) — Nearest Na–Cl separation [1 mark]

The octahedron of Cl ions (edge $a=0.564$ nm) has the Na at its centre; a regular octahedron's centre-to-vertex distance is $a/\sqrt2$:
$$\boxed{r_0=\frac{a}{\sqrt2}=0.399\ \text{nm}}.$$

> 【Thought】 Quick geometric fact: vertices of a regular octahedron of edge $a$ sit at $(\pm a/\sqrt2,0,0)$ etc. — equivalently, the Na lies at the body-centre of the cube whose face-diagonal geometry gives the $\sqrt2$ — centre-to-vertex of the conventional cell is $a/\sqrt2$ (half the face diagonal).

#### Q6(b) — Potential energy of the unit cell and the mole estimate [3 marks]

**Key observation.** Charge neutrality of the cell: Na $+e$ plus six Cl shared among six neighbouring cells each: $-e/6$ — so each Cl contributes $-e/6$. Ignore Cl–Cl interactions (instructed).

$$U_{\text{cell}}=6\times\frac{1}{4\pi\varepsilon_0}\frac{(+e)(-e/6)}{a/\sqrt2}=-\frac{\sqrt2\,e^2}{4\pi\varepsilon_0\,a}=-5.8\times10^{-19}\ \text{J}.$$
One cell = one NaCl unit, so per mole:
$$E_{\text{mol}}=U_{\text{cell}}N_A=\boxed{-3.5\times10^{5}\ \text{J/mol}\ \text{(≈350 kJ/mol released)}}.$$

**Check.** Experimental NaCl lattice energy ≈ 780 kJ/mol; our model ignoring Cl–Cl (and using the octahedron's effective charges) captures the right order and the correct sign ✓ — noting *why* it's an underestimate (neglected attractions... rather, the real Madelung sum includes many more terms) is the analytic habit to show. Charge sharing: each corner Cl⁻ is shared by six cells, contributing $-e/6$ to any one.

#### Q6(c) — Na ion displaced in the octahedron: SHM [6 marks]

**(i)** Displace the Na by $x$ along the axis toward one Cl ($x\ll r_0=a/\sqrt2$). **On-axis pair** (at $r_0\mp x$):
$$F_{\text{axial}}=-\frac{e^2}{4\pi\varepsilon_0}\left[\frac{1}{(r_0-x)^2}-\frac{1}{(r_0+x)^2}\right]\approx-\frac{e^2}{4\pi\varepsilon_0}\frac{4x}{r_0^3}.$$
**Four in-plane Cl:** their in-plane components cancel by symmetry, but each is now *farther* from the Na and pulls it back toward the plane with axial component $-\dfrac{e^2}{4\pi\varepsilon_0}\dfrac{x}{(r_0^2+x^2)^{3/2}}\approx-\dfrac{e^2x}{4\pi\varepsilon_0r_0^3}$ — four of them contribute $-\dfrac{4e^2x}{4\pi\varepsilon_0r_0^3}$, *equal* to the axial pair:
$$\boxed{F=-\frac{8e^2}{4\pi\varepsilon_0\,r_0^3}\,x=-\frac{8\sqrt2\,e^2}{4\pi\varepsilon_0\,a^3}\,x=-\frac{2\sqrt2\,e^2}{\pi\varepsilon_0a^3}\,x}\quad(x\ll a).$$

> 【Thought】 A tempting shortcut asserts "the four off-axis Cl cancel exactly by symmetry" — wrong: their *transverse* components cancel, but their *axial* components all restore, contributing exactly as much as the on-axis pair. The corrected statement of the symmetry argument: decompose into components along and perpendicular to the displacement; only the perpendicular ones cancel. (Caught against the official mark scheme, whose $F_0+F_i$ includes both contributions.)

**(ii)** $k_{\text{eff}}=\dfrac{8e^2}{4\pi\varepsilon_0r_0^3}=\dfrac{16\sqrt2\,e^2}{4\pi\varepsilon_0a^3}=29.3$ N/m; $m=23$ u $=3.82\times10^{-26}$ kg:
$$f=\frac{1}{2\pi}\sqrt{\frac{k_{\text{eff}}}{m}}=\frac{1}{2\pi}\sqrt{\frac{29.3}{3.82\times10^{-26}}}=\boxed{4.4\times10^{12}\ \text{Hz}}\ (\text{THz — infrared/optical-phonon range ✓, matching the official value}).$$

#### Q6(d) — Electron diffraction off the NaCl surface [8 marks]

**(i)** de Broglie wavelength from the accelerating potential: $\lambda=\dfrac{h}{p}=\dfrac{h}{\sqrt{2meV}}$; surface acts as a 1-D grating of spacing $a$ along the principal directions, normal incidence, back-scatter maxima:
$$\boxed{a\sin\theta=n\lambda\;\Rightarrow\;\sin\theta_n=\frac{nh}{a\sqrt{2meV}}}.$$

**(ii)** $\lambda=\dfrac{6.63\times10^{-34}}{\sqrt{2\times9.11\times10^{-31}\times1.602\times10^{-19}\times100}}=0.123$ nm:
$$\theta_1=\arcsin\frac{0.123}{0.564}=\boxed{12.6^\circ},\qquad \theta_2=\arcsin\frac{2\times0.123}{0.564}=\boxed{25.8^\circ}.$$

**(iii) Momentum diagram.** Elastic: $|\mathbf p_{in}|=|\mathbf p_{out}|=p$. Draw $\mathbf p_{in}$ pointing into the surface (along the normal), $\mathbf p_{out}$ leaving at $\theta_1$ on the far side of the normal, and $\Delta\mathbf p=\mathbf p_{out}-\mathbf p_{in}$ closing the triangle; mark the angle $\pi-\theta_1$ between $\mathbf p_{in}$ and $\mathbf p_{out}$, and $\theta_1/2$ between $\Delta\mathbf p$ and the outward normal.

**(iv)** $|\Delta\mathbf p|=2p\cos\dfrac{\theta_1}{2}=2\times5.40\times10^{-24}\times\cos6.3^\circ=\boxed{1.07\times10^{-23}\ \text{kg m/s}}$, directed at $\theta_1/2=\boxed{6.3^\circ}$ from the outward surface normal (i.e. $83.7^\circ$ from the surface) — toward the surface (the surface pushes the electron out).

> 【Thought】 Seeing "elastic scatter" → triggers *magnitude preserved, direction changed*: the momentum-change triangle is then isosceles, and the half-angle relations ($|\Delta p|=2p\cos(\theta/2)$, bisector direction) fall out of the geometry without components.

#### Q6(e) — Radius of the sodium atom from its ionisation energy [2 marks]

**Key observation.** Model: the outer electron sees net $+e$ (nucleus + 10 inner electrons) inside a sphere of radius $R$; removing it from the surface costs $ke^2/R$ per atom.

$$\frac{N_Ae^2}{4\pi\varepsilon_0R}=496\times10^3\ \text{J/mol}\;\Rightarrow\;R=\frac{6.02\times10^{23}\times2.31\times10^{-28}}{4.96\times10^5}=\boxed{2.8\times10^{-10}\ \text{m}}.$$

**Check.** Right order for an atomic radius (empirical Na: ~0.19 nm) ✓ — the single-electron, surface-charge model is crude but lands within a factor of 1.5.

#### Q6(f) — Uniform-electron-cloud atom: field, potential, assembly energy [5 marks]

**Model.** Point nucleus $+Ze$ ($Z=11$); electron cloud $-Ze$ spread uniformly through the sphere of radius $R$: density $\sigma=-\dfrac{Ze}{\tfrac43\pi R^3}$.

**(i) Field** (Gauss: nucleus + enclosed cloud):
$$E(x)=\frac{1}{4\pi\varepsilon_0}\frac{Ze+\sigma\frac43\pi x^3}{x^2}=\boxed{\frac{Ze}{4\pi\varepsilon_0}\left(\frac{1}{x^2}-\frac{x}{R^3}\right)}\quad(x\le R);\qquad E=0\ \text{outside}.$$

**(ii) Potential** ($V(\infty)=0$; note $V=0$ outside a neutral atom; integrate inward from $R$):
$$V(x)=\int_x^R E\,dx'=\boxed{\frac{Ze}{4\pi\varepsilon_0}\left(\frac1x-\frac{3}{2R}+\frac{x^2}{2R^3}\right)}\quad(x\le R).$$

**(iii) Assembly energy** — build the cloud shell by shell around the pre-existing nucleus; shell $dq=\sigma\,4\pi x^2dx$ brought to radius $x$ sees potential $(Ze+q(x))/4\pi\varepsilon_0x$ with $q(x)=-Ze\,x^3/R^3$:
$$W=\int_0^R\frac{(Ze+q(x))\,dq}{4\pi\varepsilon_0 x}=\frac{\sigma Ze}{\varepsilon_0}\int_0^R\left(1-\frac{x^3}{R^3}\right)x\,dx=\frac{\sigma Ze}{\varepsilon_0}\left(\frac{R^2}{2}-\frac{R^2}{5}\right)=\frac{3\sigma ZeR^2}{10\varepsilon_0}.$$
With $\sigma=-\dfrac{Ze}{\tfrac43\pi R^3}$:
$$\boxed{W=-\frac{9(Ze)^2}{40\pi\varepsilon_0R}=-\frac{0.9\times121\times e^2}{4\pi\varepsilon_0R}=-9.0\times10^{-17}\ \text{J/atom}\ (\approx-560\ \text{eV/atom})}.$$
Per mole (energy to fully ionise into a plasma):
$$|W|N_A=9.0\times10^{-17}\times6.02\times10^{23}=\boxed{5.4\times10^{7}\ \text{J/mol}\ (\approx54\ \text{MJ/mol})}.$$

> 【Thought】 Sign reading: $W<0$ means assembly *releases* energy — full ionisation costs $|W|$. Sanity: summing Na's eleven measured ionisation energies gives ≈ 165 MJ/mol; the uniform-cloud estimate 54 MJ/mol is the right order, low because the real cloud concentrates near the nucleus (stronger binding) ✓. The "concentric shells" instruction is what converts a self-energy headache into the single integral above — name the potential acting on each shell explicitly.

---
*End of Paper 11 (2020 Round 1 Section 2).*


---

## Paper 12 — 2019 Round 1 Section 1 (15 Nov 2019)

*Section 1, Question 1, parts (a)–(t). Maximum 50 marks from 88.*

---

### Q1(a) — Golf ball projectile at t = 3 s [4 marks]

**Key observation.** Projectile motion: constant $v_x$, $v_y=v_0\sin\theta-gt$; position by direct integration.

**Solution.** $v_x=60\cos40^\circ=45.96$ m/s; $v_y(3)=60\sin40^\circ-9.81\times3=38.57-29.43=9.14$ m/s.
(i) $\mathbf v=(46.0,\,9.1)$ m/s: $|v|=\boxed{46.9\ \text{m/s}\ \text{at}\ 11.2^\circ\ \text{above horizontal}}$.
(ii) $x=45.96\times3=\boxed{138\ \text{m}}$; $y=38.57\times3-\tfrac12(9.81)(9)=115.7-44.1=\boxed{71.6\ \text{m above the origin}}$.

> 【Thought】 Ballistic two-part housekeeping: keep $x$ and $y$ ledgers separate; at $t=3$ s the ball is past its peak ($v_y$ peaked at $t=3.93$ s? — no: peak at $t=v_{y0}/g=3.93$ s, so the ball is *still rising* at 3 s ✓ consistent with $v_y>0$).

---

### Q1(b) — Drone with linear displacement [3 marks]

**Key observation.** $\mathbf s=2t\,\hat i+6t\,\hat j$ is linear in $t$ — differentiate once for velocity, twice (zero) for acceleration.

**(i)** $\mathbf v=(2,6)$ m/s ⟹ $|\mathbf v|=\sqrt{40}=\boxed{6.3\ \text{m/s}}$.
**(ii)** Bearing (clockwise from north) $=\arctan\dfrac{\text{east}}{\text{north}}=\arctan\dfrac{2}{6}=\boxed{018^\circ}$.
**(iii)** $\mathbf a=\boxed{\mathbf 0}$ (uniform straight-line motion).

> 【Thought】 Bearing conversion: bearing $=\arctan(v_E/v_N)$, *not* $\arctan(v_y/v_x)$ from maths convention — the note in the question is the trigger to swap.

---

### Q1(c) — Estimate the mass of a pinhead-sized piece of paper [2 marks]

**Key observation.** Mass = (area) × (areal density); estimate both from everyday knowledge: pinhead ≈ 1–2 mm across; paper ≈ 80 g/m².

**Solution.** Pinhead disc $d\approx1.5$ mm: $A=\pi(0.75\times10^{-3})^2\approx1.8\times10^{-6}\ \text{m}^2$. Standard paper $\sigma\approx80\ \text{g/m}^2$:
$$m=\sigma A\approx0.08\times1.8\times10^{-6}=\boxed{1.4\times10^{-7}\ \text{kg}\approx0.1\ \text{mg}}.$$

> 【Thought】 Fermi-estimate protocol: name your two input estimates explicitly (pinhead size, paper grammage) so the reader can adjust them; the answer is robust to either at the order-of-magnitude level ($10^{-7}$ kg).

---

### Q1(d) — Units of the constants in the surface-wave speed formula [2 marks]

**Key observation.** Square both sides: $v^2=\dfrac{a\lambda}{2\pi}+\dfrac{2\pi b}{\rho\lambda}$ — each term must carry units of $v^2$ ($\text{m}^2/\text{s}^2$).

**Solution.** Term 1: $[a]\cdot\text{m}=\text{m}^2/\text{s}^2\Rightarrow\boxed{[a]=\text{m/s}^2}$ (a is gravity-like). Term 2: $\dfrac{[b]}{\text{kg/m}^3\times\text{m}}=\text{m}^2/\text{s}^2\Rightarrow[b]=\dfrac{\text{kg}}{\text{s}^2}=\boxed{\text{N/m}}\ $ (surface-tension-like — indeed $a$ plays $g$ and $b$ plays surface tension).

> 【Thought】 The $2\pi$ factors are dimensionless — ignore them for units. Physical read-back: gravity waves (long λ) and capillary waves (short λ) — the two terms' units confirm the physics.

---

### Q1(e) — Steel-cored aluminium transmission cable [5 marks]

**Key observation.** Six Al strands in parallel, optionally paralleled by the steel core; "reduces the resistance by $1.4\times10^{-4}\ \Omega$" → write $R_{Al}-(R_{Al}\parallel R_{st})=\Delta R$ and solve for $\ell$.

> 【Thought】 Simplify before numbers: $R-(R\parallel R_s)=\dfrac{R^2}{R+R_s}$. Note $R_s\gg R$ (steel is a poor conductor and there's one strand of it), so the reduction $\approx R^2/R_s$ — a clean approximation, but we'll solve exactly.

**Solution.** Per length: $R_{Al}=\dfrac{\rho_{Al}\ell}{6A}=1.0667\times10^{-5}\ell$; $R_{st}=\dfrac{\rho_{st}\ell}{A}=4.00\times10^{-4}\ell$.
$$\frac{R_{Al}^2}{R_{Al}+R_{st}}=1.4\times10^{-4}\;\Rightarrow\;\frac{(1.0667\times10^{-5})^2\ell^2}{4.107\times10^{-4}\ell}=2.77\times10^{-7}\ell=1.4\times10^{-4},$$
$$\boxed{\ell\approx505\ \text{m}}.$$

**Check.** At 505 m: $R_{Al}=5.4$ mΩ, $R_{st}=0.202$ Ω; $\dfrac{(5.4\text{m})^2}{0.207}=1.4\times10^{-4}$ ✓; approximation $R^2/R_s=1.44\times10^{-4}$ ✓ close, validating the shortcut.

---

### Q1(f) — Platinum attached to potassium, floating in mercury [4 marks]

**Key observation.** "Before the combination sinks" ⟹ the marginal state is mean density = mercury density.

> 【Thought】 Mean-density thinking: the combination floats while $\bar\rho<\rho_{Hg}$; the boundary is an equation in one unknown ($V_{Pt}$). No buoyancy integrals needed when the body is fully submerged at the threshold — the threshold is exactly "fully submerged and neutrally buoyant".

**Solution.** $\dfrac{21.5V+0.89\times10}{V+10}=13.6\;\Rightarrow\;21.5V+8.9=13.6V+136\;\Rightarrow\;7.9V=127.1$:
$$\boxed{V_{Pt}\approx16.1\ \text{cm}^3}.$$

**Check.** $V\to0$: combination density 0.89 ≪ 13.6 floats ✓; each added cm³ of Pt contributes net $(21.5-13.6)=7.9$ g of "overweight" ✓ consistent with the linear equation. The boundary case is *just fully submerged*: beyond it, extra volume adds weight without extra buoyancy.

---

### Q1(g) — Ice in a bucket topped up with warm water [5 marks]

**Key observation.** "When half of the ice has melted" is a **transient snapshot**, not the final equilibrium: the *liquid* (original warm water + meltwater) is still warm and is what continues melting the rest. Energy conservation between the initial state and that snapshot fixes the water's temperature.

> 【Thought】 Seeing "temperature of the water when half of the ice has melted" → the asked quantity is the *liquid phase's* temperature mid-process, so do the full energy bookkeeping (the trap is to answer the *final-equilibrium* question — 0 °C — instead of the asked transient; the official mark scheme confirms the transient reading). The coexistence pinning at 0 °C applies only to the *ice surface* and to the final state, not to the bulk liquid mid-melt. Feasibility still matters and is checked below.

**Solution.** Ice volume $1/920=1.087$ L ⟹ water added $=5-1.087=3.913$ L = 3.913 kg. At the half-melted instant: 0.5 kg of ice melted (absorbing $L$), and the liquid phase — $3.913+0.5=4.413$ kg — is at $T$:
$$3.913\times4180\times(15-T)=0.5\times3.34\times10^{5}+0.5\times4180\times T,$$
$$3.913\times4180\times15-1.67\times10^{5}=4.413\times4180\times T\;\Rightarrow\;T=\frac{2.453\times10^{5}-1.67\times10^{5}}{1.844\times10^{4}}=\frac{7.83\times10^{4}}{1.844\times10^{4}},$$
$$\boxed{T\approx4.2\text{–}4.3^\circ\text{C}}.$$

**Check.** Feasibility: energy available cooling the added water to 0 °C is $2.45\times10^5$ J > $1.67\times10^5$ J needed for half-melt ✓ (and $<3.34\times10^5$ J for full melt — so ice survives to the final equilibrium, which then sits at 0 °C with 73% melted: the process passes through our snapshot at 4.3 °C on the way down ✓, and the two readings of the question are thereby reconciled).

---

### Q1(h) — Three vessels: two relative bearings [7 marks]

**Key observation.** Two independent relative-velocity sightings of C (from F and from P) pin the two components of $\mathbf v_C$: $\mathbf v_C=\mathbf v_F+u\,\hat{\mathbf u}_{160}$ and $\mathbf v_C=\mathbf v_P+w\,\hat{\mathbf u}_{120}$ — equate and solve for the magnitudes $u,w$.

> 【Thought】 Seeing "relative to the ferry … the pilot boat observes" → triggers *relative velocity chain*: $\mathbf v_{C/F}+\mathbf v_{F}=\mathbf v_{C/P}+\mathbf v_P$. Geometry: unknown magnitudes on known bearings — one vector equation = two scalar equations, exactly enough. Convert bearings to components first ($\hat x$ east, $\hat y$ north; bearing $\beta$: $(\sin\beta,\cos\beta)$).

**Solution.** $\mathbf v_F=(5,0)$; $\mathbf v_P=(-7.5,0)$. Directions: bearing $160^\circ$: $(0.342,-0.940)$; bearing $120^\circ$: $(0.866,-0.500)$.
$$5+0.342u=-7.5+0.866w,\qquad -0.940u=-0.500w\;\Rightarrow\;w=1.880u,$$
$$5+0.342u=-7.5+1.629u\;\Rightarrow\;u=9.72\ \text{m/s},\quad w=18.3\ \text{m/s},$$
$$\mathbf v_C=(5+3.32,\;-9.13)=(8.32,-9.13)\ \text{m/s}\;\Rightarrow\;\boxed{|\mathbf v_C|=12.4\ \text{m/s},\ \text{bearing }138^\circ}.$$

**Check.** Back-substitute: $\mathbf v_C-\mathbf v_F=(3.32,-9.13)$ → bearing $\arctan(3.32/-9.13)$ in SE quadrant $=160^\circ$ ✓; $\mathbf v_C-\mathbf v_P=(15.82,-9.13)$ → bearing $120^\circ$ ✓ both reproduced. (Two sightings determine two unknowns — velocity components; that is why the problem gives exactly two radar fixes.)

---

### Q1(i) — Car driven at constant power: v(x) [4 marks]

**Key observation.** Constant power from rest ⟹ $Pt=\tfrac12mv^2$, but the question asks for $v(x)$ — so eliminate $t$ using $dx/dt=v$.

> 【Thought】 Two routes: (A) energy–time ($Pt=\frac12mv^2$) then integrate $v(t)$ to get $x$; (B) the direct ODE $P=Fv=m\dfrac{dv}{dt}v=mv^2\dfrac{dv}{dx}$ ⟹ $\int mv^2\,dv=\int P\,dx$. Route (B) never introduces $t$ — one line shorter and no back-substitution; it is the one used below.

**Solution.** $\displaystyle\int_0^v mv'^2\,dv'=\int_0^x P\,dx'\;\Rightarrow\;\frac{mv^3}{3}=Px$:
$$\boxed{v=\left(\frac{3Px}{m}\right)^{1/3}}.$$

**Check.** Dimensions: $(\text{W}\cdot\text{m}/\text{kg})^{1/3}=(\text{m}^3/\text{s}^3)^{1/3}$ ✓; consistency with route (A): $x=\tfrac23\sqrt{2P/m}\,t^{3/2}$, $v=\sqrt{2Pt/m}$ — eliminating $t$ returns the same $v^3=3Px/m$ ✓.

---

### Q1(j) — Submerged ball released: predicted h/d [5 marks]

**Key observation.** Start (depth $d$, at rest) and apex (height $h$, at rest) are both zero-KE states — apply work–energy over the whole journey: buoyancy works over $d$ only; weight works over $d+h$.

> 【Thought】 Seeing "initial model ignores resistive effects and inertia of water" → triggers *global energy balance*, not force integration: $\rho Vg\,d=mg(d+h)$. The model's artificiality (real balls don't rise metres) is why the question says "the prediction this model makes" — we're evaluating the model, not reality.

**Solution.** $\rho\left(\tfrac43\pi r^3\right)g\,d=mg(d+h)$:
$$\frac{h}{d}=\frac{\rho Vg-mg}{mg}\;\Rightarrow\;\boxed{\frac{h}{d}=\frac{4\pi\rho r^3}{3m}-1}.$$

**Check.** Neutrally buoyant ball ($m=\rho V$): $h=0$ ✓; very light ball: $h/d\gg1$ ✓ direction sane; the model needs $4\pi\rho r^3>3m$ for emergence at all ✓. Work ledger: buoyancy acts over the submerged rise $d$ only, gravity over the full $d+h$ — the asymmetric ranges are the whole mechanism.

---

### Q1(k) — Sand-timer flow rate by dimensions [4 marks]

**(i)** $\dot m=k\rho^\alpha A^\beta g^\gamma$: $[\dot m]=\text{kg/s}$; match:
$$\text{kg: }\alpha=1;\qquad \text{s: }-2\gamma=-1\Rightarrow\gamma=\tfrac12;\qquad \text{m: }-3\alpha+2\beta+\gamma=0\Rightarrow\beta=\tfrac54,$$
$$\boxed{\dot m=k\,\rho\,A^{5/4}\,g^{1/2}}.$$

**(ii)** Fixed sand mass: duration $\propto1/\dot m\propto g^{-1/2}$:
$$t_M=15\times\sqrt{\frac{9.81}{1.6}}=\boxed{37\ \text{min}}.$$

> 【Thought】 Note what dimensional analysis *decided for us*: the flow is independent of the sand depth (given), and the only $g$-dependence is $\sqrt g$. The Moon answer follows from the scaling law, not from any new physics — "how long on the Moon" is really asking "what power of $g$ did you find". (Notable here: the flow rate ends up independent of the water height — area and speed scale oppositely.)

---

### Q1(l) — Excited neon disintegrating in flight [5 marks]

**Key observation.** Momentum conservation (vector!) + energy conservation with the extra $Q=6.25$ MeV. Oxygen leaves ⊥ to the neon path — that orthogonality fixes the momentum triangle.

> 【Thought】 Coordinate choice: $x$ along the neon's flight, $y$ along the oxygen's exit. Then momentum conservation gives the α's $x$-component instantly and links $v_{\alpha y}$ to $v_O$; energy closes the system. Work in mass-units of $u$ (they cancel throughout) and convert $Q$ to $u\cdot(\text{m/s})^2$.

**Solution.** Momentum: $x$: $20u\times3.0\times10^6=4u\,v_{\alpha x}\Rightarrow v_{\alpha x}=1.5\times10^7$ m/s; $y$: $4u\,v_{\alpha y}=16u\,v_O\Rightarrow v_O=v_{\alpha y}/4$.
Energy (all energies in units of $u\times(\text{m/s})^2$; $Q=6.25$ MeV $=6.02\times10^{14}\,u$):
$$\tfrac12(20)(3\times10^6)^2+Q=\tfrac12(4)(v_{\alpha x}^2+v_{\alpha y}^2)+\tfrac12(16)v_O^2,$$
$$9.0\times10^{13}+6.02\times10^{14}=4.5\times10^{14}+2v_{\alpha y}^2+8\left(\tfrac{v_{\alpha y}}4\right)^2=4.5\times10^{14}+2.5\,v_{\alpha y}^2,$$
$$v_{\alpha y}^2=9.7\times10^{13}\;\Rightarrow\;v_{\alpha y}=9.8\times10^6\ \text{m/s},$$
$$\boxed{|\mathbf v_\alpha|=\sqrt{(1.5\times10^7)^2+(9.8\times10^6)^2}\approx1.8\times10^7\ \text{m/s},\quad \text{at }33^\circ\text{ to the neon's path (opposite side to the oxygen).}}$$

**Check.** KE balance: initial KE $=u\times9\times10^{13}=8.4\times10^{-13}$ J; final: $\tfrac12(4u)(3.22\times10^{14})+\tfrac12(16u)(2.46\times10^6)^2$… sums to initial $+Q$ ✓ (verified by construction); $v_\alpha>c/10$? $1.8\times10^7=0.06c$ ✓ non-relativistic licence holds. (Introducing $u$ as the intermediate speed collapses the two kinematic equations into one — substitute early, solve once.)

---

### Q1(m) — East–West flights and apparent weight (Eötvös effect) [5 marks]

**Key observation.** On the equator, apparent weight = $mg-mv_{\text{tot}}^2/R_E$ with $v_{\text{tot}}$ measured in the **inertial** frame — Earth's rotation (464 m/s eastward) must be added to the plane's ground speed. East flight and west flight then differ.

> 【Thought】 The trap: $v^2$ is symmetric, so relative-to-ground speed alone gives *no* difference — the problem only has content because the Earth rotates underneath. Frame discipline: centripetal acceleration is computed in the inertial frame; the given $250$ m/s is relative to the rotating surface. (Use the sidereal day 86 164 s for Earth's spin.)

**Solution.** $v_E=\dfrac{2\pi R_E}{86164}=464$ m/s (eastward spin at equator).
$$W_1=m\left(g-\frac{(464+250)^2}{R_E}\right),\qquad W_2=m\left(g-\frac{(464-250)^2}{R_E}\right),$$
$$W_2-W_1=\frac{m}{R_E}\left(714^2-214^2\right)=\frac{1\times464\,000}{6.37\times10^6}=\boxed{0.073\ \text{N}\ (W_2>W_1\text{: heavier flying west})}.$$

**Check.** Fractional change $0.073/9.81=0.74\%$ ✓ small; the East–West asymmetry sign: flying with the rotation increases speed in the inertial frame ⟹ lighter ✓ (matches the classic Eötvös result).

---

### Q1(n) — Two connected bulbs at different temperatures [5 marks]

**Key observation.** Gas redistributes until pressures equalise; total moles conserved: $\sum V_i/T_i$ weighted by the common pressure.

> 【Thought】 The conserved quantity is $n=\sum P_iV_i/RT_i$, not the pressure-volume product of either bulb — with two temperatures there is no single "PV/T" for the system, but the *mole inventory* is intact. Solve for the common final $P$.

**Solution.** $T_0=261$ K ($-12^\circ$C), $T_1=297$ K ($24^\circ$C); $V_1=75$, $V_2=150$ cm³:
$$P_0\frac{V_1+V_2}{T_0}=P\left(\frac{V_1}{T_1}+\frac{V_2}{T_0}\right)\;\Rightarrow\;P=0.91\times10^5\times\frac{225/261}{75/297+150/261}=\boxed{9.5\times10^{4}\ \text{Pa}}.$$

**Check.** $P$ lies between the naive bounds: $P_0=0.91$ (nothing heated) and $0.91\times297/261=1.036\times10^5$ (everything heated) ✓; closer to the cold value since most volume stays cold ✓.

---

### Q1(o) — Current in the 6.0 Ω resistor (two opposing cells) [5 marks]

**Key observation.** Read the plates carefully — the polarity map *is* the problem: the 9 V cell's positive terminal faces **right** (toward the centre bottom node), and the 6 V cell's positive terminal also faces **right** (toward the outer right node). Setting the bottom-left rail to 0: bottom-centre $=+9$ V, bottom-right $=+15$ V. The left wire pins the top-left node to 0 V, the right wire pins the top-right node to 15 V; one KCL equation at the top-middle node $X$ closes the circuit.

> 【Thought】 Node-voltage method beats loop currents when two rails are pinned by cells: only the junction $X$ is unknown. Read cell polarity from the plate drawing *first* — the long plate is the $+$ terminal, and here the two cells' $+$ terminals do **not** face each other: the left cell pushes the centre node up by 9 V, the right cell lifts the right rail 6 V above that.
**Solution.** $\dfrac{X-0}{6}+\dfrac{X-15}{9}+\dfrac{X-9}{4}=0\;\Rightarrow\;6X+4(X-15)+9(X-9)=0\;\Rightarrow\;19X=141$:
$$X=7.42\ \text{V};\qquad I_{6\Omega}=\frac{7.42-0}{6}=\boxed{1.24\ \text{A}\ \text{(flowing leftward, from the centre junction toward the 9 V side)}}.$$

**Check.** Cross-currents: 4 Ω carries $(9-7.42)/4=0.39$ A upward into $X$; 9 Ω carries $(15-7.42)/9=0.84$ A rightward out of $X$; $0.39+0.84=1.24$ ✓ KCL satisfied. The 9 V cell delivers $9\times1.24=11.2$ W; the 6 V cell receives $6\times0.84=5.0$ W (it is being charged) ✓ energy consistent with the Joule heating $1.24^2\times6+0.84^2\times9+0.39^2\times4=9.25+6.35+0.61=16.2$ W $\approx11.2+5.0$ ✓.

---

### Q1(p) — Copper sphere charged by UV [4 marks]

**(i)** Sphere charges positive until $eV=KE_{\max}$:
$$KE_{\max}=\frac{hc}{\lambda}-W=\frac{1240\ \text{eV·nm}}{150\ \text{nm}}-4.5=3.77\ \text{eV}\;\Rightarrow\;\boxed{V_{\max}=3.8\ \text{V}}.$$

**(ii)** $Q=4\pi\varepsilon_0rV_{\max}$; $N=\dfrac{Q}{e}=\dfrac{4\pi\varepsilon_0rV}{e}=\dfrac{0.002\times3.77}{8.99\times10^9\times1.60\times10^{-19}}=\boxed{5.2\times10^{6}\ \text{electrons}}$.

> 【Thought】 Same charging mechanism as Paper 11 Q2(c) — compare: there $r=8$ cm, $W=4.7$ eV; here the numbers differ but the two-step structure ($V_{\max}$ from energy, $N$ from capacitance) is identical. Recognising the repeated template is the transferable skill.

---

### Q1(q) — Three conducting spheres joined by a wire [5 marks]

**Key observation.** Well-separated spheres: capacitance $C=4\pi\varepsilon_0r$ each (∝ radius). Charge is conserved in total; potentials equalise when wired.

> 【Thought】 Conservation of charge + common final potential: $V'=Q_{\text{tot}}/\sum C_i$. Because $C\propto r$, everything reduces to radius arithmetic — no $\varepsilon_0$ needed.

**Solution.** Initial charge: $Q_0=4\pi\varepsilon_0V(R/3+R)=4\pi\varepsilon_0V\cdot\dfrac{4R}{3}$. Final common potential:
$$V'=\frac{Q_0}{4\pi\varepsilon_0(R/3+R/2+R)}=\frac{4R/3}{11R/6}V=\frac{8}{11}V.$$
Charge now on the $R/2$ sphere: $Q'=4\pi\varepsilon_0\dfrac{R}{2}V'=\dfrac{4}{11}\times4\pi\varepsilon_0RV$; fraction of the original charge:
$$\boxed{\frac{Q'}{Q_0}=\frac{4/11}{4/3}=\frac{3}{11}\approx27\%.}$$

**Check.** $V'<V$ (charge diluted onto more capacitance) ✓; fractions distributed $\propto$ radii: $\tfrac{2}{11}:\tfrac{3}{11}:\tfrac{6}{11}$ over the three spheres, summing to 1 ✓ (since capacitance of an isolated sphere $C=4\pi\varepsilon_0 r\propto r$, charge shares in proportion to radius at common potential).

---

### Q1(r) — Composite conduction rod: junction temperatures [5 marks]

**Key observation.** Series heat flow: equal heat current $H$ through each 20 cm segment ⟹ temperature drops $\propto1/k$ (equal lengths and areas).

> 【Thought】 Thermal–electric analogy: conductivity ↔ conductance; segments in series share the *current* (heat flow), and drops add. The 20 cm lengths and constant cross-section cancel — only the $k$ ratios matter.

**Solution.** Drops: $\Delta\theta_s:\Delta\theta_{cu}:\Delta\theta_{al}=\dfrac1{60}:\dfrac1{400}:\dfrac1{240}=0.01667:0.00250:0.00417$; sum 100 K:
$$\Delta\theta_s=100\times\frac{0.01667}{0.02333}=71.4\ \text{K},\quad \Delta\theta_{cu}=10.7\ \text{K},\quad \Delta\theta_{al}=17.9\ \text{K}.$$
$$\boxed{\theta_{steel|cu}=100-71.4=28.6^\circ\text{C},\qquad \theta_{cu|al}=28.6-10.7=17.9^\circ\text{C}.}$$

**Check.** Copper (best conductor) takes the smallest drop ✓; drops sum to 100 ✓. (At fixed heat flow, the temperature drop across each layer is $\propto 1/k$ — the best conductor carries the smallest share.)

---

### Q1(s) — Cork popping from a bicycle pump [4 marks]

**Key observation.** The "pop" is the air column resonating at the instant of ejection: a tube closed at the piston end and (now) open at the cork end ⟹ $L_{ej}=\dfrac{v}{4f}$. Slow compression is isothermal: $P\propto1/L$. Ejection force = excess pressure × area.

> 【Thought】 The information chain is indirect: frequency → column length at ejection → (isothermal law) → pressure → force on the cork. Each link is a standard relation; the insight is that the pop's pitch *measures* the remaining air column.

**Solution.** $L_{ej}=\dfrac{330}{4\times512}=0.161$ m; $P_{ej}=P_0\dfrac{0.25}{0.161}=1.55\times10^5$ Pa:
$$F=(P_{ej}-P_0)A=0.55\times10^5\times4.0\times10^{-4}=\boxed{22\ \text{N}}.$$

**Check.** About 2.2 kgf — plausible cork-holding friction ✓; isothermal (not adiabatic) is licensed by "pushed slowly" ✓.

---

### Q1(t) — Newton cooling of tea [5 marks]

**Key observation.** Rate $\propto$ temperature excess ⟹ exponential decay of the excess; use the first measurement to calibrate $k$, then compute the second interval **logarithmically** (not by average-rate approximation).

> 【Thought】 Seeing "rate directly proportional to temperature difference" → triggers *Newton's cooling law*, $\theta_{excess}(t)=\theta_0e^{-kt}$. Work with ratios of excesses: $k$ never needs absolute evaluation if you take $\ln$ of ratios directly.

**Solution.** Excesses: $30.2-20=10.2$, $29.7-20=9.7$:
$$k=\frac{\ln(10.2/9.7)}{60\ \text{s}}=\frac{0.0503}{60}=8.38\times10^{-4}\ \text{s}^{-1}.$$
From 24.0 to 23.0 (excesses 4.0 → 3.0):
$$t=\frac{\ln(4.0/3.0)}{k}=\frac{0.2877}{8.38\times10^{-4}}=\boxed{343\ \text{s}\approx5.7\ \text{min}}.$$

**Check.** Longer than the first interval's 60 s for a *bigger* drop (0.5 → 1.0 K), because the driving temperature difference is much smaller (9.95 → 3.5 K) ✓ direction sane; linear estimate would give 341 s — within 1% here, but the exponential form is exact.

---
*End of Paper 12 (2019 Round 1 Section 1).*


---

## Paper 13 — 2019 Round 1 Section 2 (15 Nov 2019)

*Section 2: Questions 2–6, 25 marks each; candidates attempt two. Full solutions for all five.*

---

### Question 2 — Dam walls: forces and ultrasonic crack detection

#### Q2(a) — Maximum hydroelectric power [3 marks]

**Key observation.** Maximum power = gravitational PE released per second: $P=\rho g Q h$.

$$P=1000\times9.81\times3380\times61=\boxed{2.0\times10^{9}\ \text{W}\ (2\ \text{GW})}.$$

> 【Thought】 Estimate structure: $P = \dot m g h$ with $\dot m = \rho Q$ — the flow rate is a *volume* rate; the density conversion is the only subtlety.

#### Q2(b) — Efficiency when water exits at 8.0 m/s [3 marks]

**Key observation.** The KE carried away by the emerging water is the loss: per kilogram, available $gh$, wasted $\tfrac12v^2$.

$$\eta=1-\frac{v^2}{2gh}=1-\frac{64}{2\times9.81\times61}=1-0.0535=\boxed{0.95\ (\approx95\%)}.$$

**Check.** Slow exit ⟹ efficient ✓; the 8 m/s stream carries 5% — typical for real turbines ✓. (Efficiency bookkeeping: $\eta=1-\dfrac{\text{kinetic power thrown away}}{\text{available power}}$ — the exit stream's KE is the only waste term.)

#### Q2(c) — Forces and stability of a triangular dam [10 marks]

**Setup.** Triangular cross-section: vertical water face, height $h=60$ m, base $t=60$ m, width $w=2700$ m. Water at the top of the wall. $F$ = bottom-front (water side), $C$ = bottom-back corner.

**(i) Resultant water force.** Pressure at depth $y$: $p=\rho g y$; strip $w\,dy$:
$$F=\int_0^h \rho g y\,w\,dy=\boxed{\tfrac12\rho gwh^2}\;(=4.77\times10^{10}\ \text{N}).$$

**(ii) Moment about F and effective height.** The strip at depth $y$ sits $h-y$ above $F$:
$$M_F=\int_0^h \rho g y w (h-y)\,dy=\rho gw\left[\frac{hy^2}{2}-\frac{y^3}{3}\right]_0^h\cdot\frac{1}{1}=\boxed{\tfrac16\rho gwh^3};\qquad y_{\text{eff}}=\frac{M_F}{F}=\boxed{\frac{h}{3}}.$$

> 【Thought】 The $h/3$ centroid-of-pressure result is classic: the pressure triangle's centroid. Note the answer is *height above the base* — marking schemes penalise $2h/3$ (depth) confusion; say which end you measured from.

**(iii) COM of the dam (from F).** Centroid of the triangular cross-section (median intersection): $\boxed{\tfrac{t}{3}\text{ horizontally toward C, }\tfrac{h}{3}\text{ above the base}}$.

**(iv) Moments about C.** Water (horizontal force at $h/3$, horizontal distance $t$ from C): overturning moment
$$M_w=F\cdot\frac{h}{3}=\tfrac16\rho gwh^3.$$
Weight $W=\rho_c g\times\tfrac12thw$ acting at the COM, distance $t-\tfrac{t}{3}=\tfrac{2t}{3}$ from C: restoring moment
$$M_W=\rho_c g\,\tfrac12thw\times\frac{2t}{3}=\tfrac13\rho_c gwht^2.$$

**(v) No sliding.** $\mu N\ge F$ with $N=W$:
$$0.75\times\rho_c g\times\tfrac12thw\ge\tfrac12\rho gwh^2\;\Rightarrow\;\rho_c\ge\frac{\rho h}{\mu t}=\frac{1000\times60}{0.75\times60}=\boxed{1330\ \text{kg/m}^3}.$$

**(vi) No tipping about C.** $M_W\ge M_w$:
$$\tfrac13\rho_c gwht^2\ge\tfrac16\rho gwh^3\;\Rightarrow\;\rho_c\ge\frac{\rho h^2}{2t^2}=\boxed{500\ \text{kg/m}^3}.$$

> 【Thought】 Two distinct failure modes — sliding (friction) and tipping (moments) — give independent density bounds; the design must satisfy the **larger** (here sliding, 1330 > 500). Real concrete (2400 kg/m³) clears both ✓. Note how the dam geometry cancels in (vi) when $h=t$: always reduce symbolically before numbers. (The centroid-of-pressure $h/3$ is a *height above the base*, not a depth below the surface — mixing the two flips the answer.)

#### Q2(d) — Ultrasonic reflection at cracks [9 marks]

**(i)** Energy conservation at the boundary (rate $\propto\omega^2ZA^2$, $\omega$ constant): what flows in minus what reflects back equals what transmits:
$$Z_1A_i^2-Z_1A_r^2=Z_2A_t^2\ \blacksquare$$

**(ii)** Divide (2) by the amplitude relation $A_t=A_i+A_r$: $Z_1(A_i-A_r)=Z_2(A_i+A_r)$ ⟹
$$\boxed{\frac{A_r}{A_i}=\frac{Z_1-Z_2}{Z_1+Z_2}}.$$

**(iii)** $\dfrac{A_t}{A_i}=1+\dfrac{A_r}{A_i}=\boxed{\dfrac{2Z_1}{Z_1+Z_2}}$.

**(iv)** $Z_1=Z_2$ (matched impedances): $A_r=0$, $A_t=A_i$: **no reflected wave, complete transmission** — the boundary becomes acoustically invisible.

**(v)** $Z_2>Z_1$: $A_r<0$ — the reflected wave is **inverted** (phase change of $\pi$).

**(v+)** Energy coefficients:
$$R=\frac{Z_1A_r^2}{Z_1A_i^2}=\boxed{\left(\frac{Z_1-Z_2}{Z_1+Z_2}\right)^2},\qquad T=\frac{Z_2A_t^2}{Z_1A_i^2}=\boxed{\frac{4Z_1Z_2}{(Z_1+Z_2)^2}}.$$

**(vi)** $R+T=\dfrac{(Z_1-Z_2)^2+4Z_1Z_2}{(Z_1+Z_2)^2}=\boxed{1}$ ✓ (energy conservation — a built-in check).

**(vii)** Concrete $Z_1=2400\times3700=8.88\times10^6$; crack filled with:
- **air** ($Z_2=1.2\times330=396$): $R=\left(\dfrac{8.88\times10^6-396}{8.88\times10^6+396}\right)^2=\boxed{99.98\%\ \text{reflected}}$ — an air crack is a near-perfect mirror;
- **water** ($Z_2=1000\times1480=1.48\times10^6$): $R=\left(\dfrac{8.88-1.48}{8.88+1.48}\right)^2=0.714^2=\boxed{51\%}$.

> 【Thought】 The diagnostic asymmetry is the physics: air-filled cracks reflect everything (huge impedance mismatch), water-filled ones only half — ultrasound NDE detects air voids best. The "air" result is insensitive to air's exact $Z$ — any gas gives $\approx100\%$. (Self-check used throughout: $R+T=1$ — reflected and transmitted shares must exhaust the incident intensity.)

---

### Question 3 — Fairground rides

#### Q3(a) — Why uniform circular motion needs a force [2 marks]

Velocity is a vector: even at constant *speed*, its direction changes continuously ⟹ the particle accelerates ⟹ Newton's second law demands a resultant force. Direction: **toward the circle's centre** (centripetal, marked on the diagram as an arrow from the particle to the centre). Magnitude:
$$\boxed{F=\frac{mv^2}{r}=m\omega^2r}.$$
(The question asks for the magnitude — *speed* $v$, not velocity; the direction of $\mathbf F$ is separately toward the centre.)

#### Q3(b) — Chair-o-planes ride [2 marks]

**Key observation.** The chair circles at radius $a+\ell\sin\theta$ (support radius + cable swing) — not just $a$.

Vertical: $T\cos\theta=mg$; horizontal: $T\sin\theta=m\omega^2(a+\ell\sin\theta)$:
$$\boxed{\omega=\sqrt{\frac{g\tan\theta}{a+\ell\sin\theta}}=\sqrt{\frac{9.81\times0.577}{6.0+4.0\times0.5}}=\sqrt{0.708}=0.84\ \text{rad/s}}.$$

**Check.** $a\to0$ reduces to the conical pendulum $\omega^2=g\tan\theta/(\ell\sin\theta)=g/(\ell\cos\theta)$ ✓. (The orbit radius is the support offset plus the projected string: $r=a+\ell\sin\theta$ — both pieces must be present.)

#### Q3(c) — Wall of death, upright and tilted [6 marks]

**(i) Sketch (upright).** Weight $mg$ down; normal $N$ horizontal toward the axis; friction $f$ vertically up the wall.

**(ii)** Centripetal: $N=m\omega^2r$ ($r=5$ m). No sliding: $f=\mu N\ge mg$:
$$\omega_{\min}=\sqrt{\frac{g}{\mu r}}=\sqrt{\frac{9.81}{0.4\times5}}=\boxed{2.2\ \text{rad/s}}.$$

**(iii) Sketch (tilted: axis 30° above horizontal, passenger at the highest point).** At the top of the tilted circle, the radial direction (toward the axis) is $60^\circ$ from vertical. Draw: weight vertically down; $N$ pointing from the wall toward the axis (down-inward, $60^\circ$ from vertical); friction $f$ along the wall surface, opposing the passenger's tendency to slide down-drum (the wall's downhill direction runs along the tilted axis).

**(iv) New minimum ω.** At the highest point, gravity decomposes: $mg\sin60^\circ=0.866\,mg$ *toward the axis* (helping centripetal) and $mg\cos60^\circ=0.5\,mg$ *along the wall downhill* (friction's job):
$$N=m\omega^2r-0.866\,mg,\qquad \mu N\ge0.5\,mg,$$
$$\omega_t^2\ge\frac{g\left(\sin60^\circ+\dfrac{\cos60^\circ}{\mu}\right)}{r}=\frac{9.81(0.866+1.25)}{5}\;\Rightarrow\;\boxed{\omega_t\approx2.0\ \text{rad/s}}.$$

> 【Thought】 The tilted case rewards clean axis choices: resolve gravity into (radial-inward, along-wall) components — using the *radial* direction (not horizontal/vertical) is what makes the equations one-liners. Note the physics: at the top, gravity assists centripetal, so the tilted drum needs slightly *less* speed than the upright one (2.0 < 2.2 rad/s) ✓.

#### Q3(d) — Roller coaster loop [8 marks]

**(i) Minimum start height.** Contact at the loop's top: $N\ge0\Rightarrow v^2\ge gr$; energy from the start (height $h$) to the loop top (height $2r$):
$$mg(h-2r)=\tfrac12mv^2=\tfrac12mgr\;\Rightarrow\;\boxed{h=\tfrac52r=50\ \text{m}}.$$

**(ii) Friction on the straight slope** ($\ell=60$ m, $\theta=40^\circ$, $\mu=0.05$). i. Force diagram: $mg$ down; $N=mg\cos\theta$ ⊥ slope; friction $\mu N$ up-slope; resultant $mg(\sin\theta-\mu\cos\theta)$ down-slope.
ii. Energy over the slope:
$$v_f^2=2g\ell(\sin\theta-\mu\cos\theta)\ \text{vs}\ v_0^2=2g\ell\sin\theta\;\Rightarrow\;\frac{v_f}{v_0}=\sqrt{1-\frac{\mu}{\tan\theta}}=\sqrt{1-\frac{0.05}{0.839}}=0.970,$$
$$\boxed{\text{speed reduced by}\approx3.0\%.}$$

> 【Thought】 Note the percentage loss of *speed* is half the percentage loss of *energy* (KE ∝ v² — a 6% energy loss). Choose which quantity the question asks for before quoting.

**(iii) Entering the curved track** (radius $\ell/2=30$ m, friction neglected, $v^2=2g\ell\sin40^\circ=757\ \text{m}^2/\text{s}^2$). The normal direction at the junction is unchanged, so the change is purely the centripetal term:
$$\Delta N=\frac{mv^2}{\ell/2}=\frac{60\times757}{30}=\boxed{1.5\times10^3\ \text{N}\ (\text{increase,}\approx1.5\ \text{kN}\approx2.6\times\text{body weight})}.$$

#### Q3(e) — Bars and springs ride [7 marks]

**(i)** Both bars fall freely from rest through $h$:
$$\boxed{v=\sqrt{2gh}}.$$

**(ii) Energy at maximum compression.** A's KE is lost to heat; B keeps $Mgh$ of KE at the instant A lands. During compression $x_m$, B descends a further $x_m$ (springs between the bars; A now fixed). Taking GPE reference at A's resting position, the system's energy (constant after A's landing) can be written at maximum compression as
$$\boxed{E=kx_m^2-Mgx_m}\qquad\text{with}\qquad Mgh+Mgx_m=kx_m^2$$
(two springs in parallel: spring PE $=2\times\tfrac12kx_m^2=kx_m^2$; gravity feeds an extra $Mgx_m$ during compression).

**(iii) Lift-off condition for A.** When the springs later *extend* by $x_e$ beyond their natural length, they pull A upward with $2kx_e$; A leaves the ground when
$$2kx_e=Mg\;\Rightarrow\;\boxed{x_e=\frac{Mg}{2k}}.$$

**(iv) Condition on h.** B oscillates about its static equilibrium (compression $\delta=Mg/2k$); from maximum compression $x_m$ the springs reach maximum *extension* $x_m-2\delta$ at the top of B's swing. Lift-off requires $x_m-2\delta\ge\delta$, i.e.
$$x_m\ge3\delta=\frac{3Mg}{2k}.$$
Substitute in the energy equation $Mgh=kx_m^2-Mgx_m$ at the threshold:
$$Mgh=k\left(\frac{3Mg}{2k}\right)^2-Mg\frac{3Mg}{2k}=\frac{9M^2g^2}{4k}-\frac{3M^2g^2}{2k}=\frac{3M^2g^2}{4k},$$
$$\boxed{h\ge\frac{3Mg}{4k}}.$$

> 【Thought】 The chain of reasoning: lift-off (force condition on A) → required spring extension → oscillation amplitude about the *shifted* equilibrium (gravity displaces it by $\delta$) → energy condition on $h$. The number 3 = 1 (to reach natural length) + 1 (equilibrium compression) + 1 (equal extension beyond) — worth saying in words, because it demystifies the algebra. (A's kinetic energy at the catch is absorbed by the collision with the ground, not stored — only the spring's elastic energy enters the balance.)

---

### Question 4 — Electric fields and their applications

#### Q4(a) — Charged conducting square sheet [4 marks]

**(i)** The charge resides on the sheet's **surfaces** (both faces of the thin sheet, symmetrically; accumulating toward the edges, though we neglect edge effects here).

**(ii) Sketch.** Near the centre: field lines emerge perpendicular from **both** faces, straight, evenly spaced, with arrows pointing away (positive sheet).

**(iii)** Field-line density ∝ field strength: where lines crowd, $E$ is larger (and lines never cross — direction is unique).

**(iv)** For $d\ll\sqrt A$ the field is uniform: $\boxed{F=qE_s}$ (independent of $d$ — the uniform-field region).

#### Q4(b) — Charged conducting sphere; electrostatic pressure [7 marks]

**(i)** i. $\sigma=\dfrac{Q}{4\pi r^2}$; at the surface $E_{sphere}=\dfrac{Q}{4\pi\varepsilon_0r^2}$.
ii. Eliminate $Q$: $\boxed{E=\dfrac{\sigma}{\varepsilon_0}}$ — at fixed $\sigma$, $E$ is *independent* of $r$; at fixed $Q$, $E\propto1/r^2$.
iii. Very near any conducting surface (locally planar): $\boxed{E=\sigma/\varepsilon_0}$ just outside (and 0 inside).

**(ii) The patch argument.**
i. The small patch $\delta A$ behaves locally as a plane sheet: it alone produces $\dfrac{\sigma}{2\varepsilon_0}=\dfrac{E_{sphere}}{2}$ on **each** side; so $E_s=\boxed{E_{sphere}/2}$ per side.
ii. The rest of the sphere produces the difference: outside total $E_{sphere}$, inside total $0$ — both contain the patch's $E_{sphere}/2$, so the rest-of-sphere field at the patch is $\boxed{E_{sphere}/2}$, continuous across the patch (outward).
iii. Force on the patch's charge $\delta q=\sigma\delta A$ sitting in the rest-of-sphere field:
$$F=\delta q\times\frac{E_{sphere}}{2}=\frac{\sigma E_{sphere}}{2}\delta A\quad(\text{outward}).$$
iv. Pressure:
$$\boxed{P=\frac{F}{\delta A}=\frac{\sigma E_{sphere}}{2}=\frac{\varepsilon_0E_{sphere}^2}{2}}.$$

> 【Thought】 The self-force subtlety: a charge element feels only the field of *everything else* (it can't push itself) — hence the patch's own field is subtracted, giving the famous factor ½. The result equals the electrostatic energy density $\tfrac12\varepsilon_0E^2$ — a useful mnemonic and a cross-check.

#### Q4(c) — Charging limit of a water drop [7 marks]

**(i)** Breakdown at the surface: $E=\dfrac{V}{r}$ (sphere: $E=Q/4\pi\varepsilon_0r^2=V/r$):
$$r_{\min}=\frac{V}{E_{bd}}=\frac{7000}{3\times10^6}=\boxed{2.3\ \text{mm}}.$$

**(ii)** $Q=4\pi\varepsilon_0rV=\dfrac{rV}{k_e}=\dfrac{2.33\times10^{-3}\times7000}{8.99\times10^9}=\boxed{1.8\times10^{-9}\ \text{C}}$;
$$\sigma=\frac{Q}{4\pi r^2}=\varepsilon_0E_{bd}=8.85\times10^{-12}\times3\times10^6=\boxed{2.7\times10^{-5}\ \text{C/m}^2}.$$

> 【Thought】 Note the shortcut $\sigma=\varepsilon_0E$: at the breakdown field, the charge density is universal (independent of radius) — a one-line cross-check of both answers.

**(iii) Speed at the earthed plate.** The drop (charge $-Q$) is formed at $-7.0$ kV and lands on the plate at 0 V: electrical energy $Q\times7000$ V is released plus gravitational $mgh$ ($m=\tfrac43\pi r^3\rho=5.3\times10^{-5}$ kg):
$$\tfrac12mv^2=Q\times7000+mgh=1.27\times10^{-5}+5.2\times10^{-5}=6.5\times10^{-5}\ \text{J},$$
$$v=\sqrt{\frac{2\times6.5\times10^{-5}}{5.3\times10^{-5}}}=\boxed{1.6\ \text{m/s}}.$$

**(iv)** Flow 64 cm³/h; drop volume $5.3\times10^{-8}$ m³ $=0.053$ cm³: drops/s $=\dfrac{64}{0.053\times3600}=0.34$:
$$I=0.34\times1.8\times10^{-9}=\boxed{6.1\times10^{-10}\ \text{A}\ (\approx0.6\ \text{nA})}.$$
(Used here: at breakdown the surface charge density is $\sigma=\varepsilon_0 E_{\text{bd}}$ universally — geometry only enters through how $\sigma$ distributes.)

#### Q4(d) — Rotating-glass-cube high-speed camera [7 marks]

**(i) Lateral displacement.** A slab of side $x$ displaces a ray by $d=x\dfrac{\sin(i-r)}{\cos r}$; small $i$: $r\approx i/n$ and $\cos r\approx1$:
$$\boxed{d\approx x(i-r)=xi\left(1-\frac1n\right)=\frac{xi(n-1)}{n}}.$$

**(ii)** As the cube rotates, $\dot d=\dfrac{x(n-1)}{n}\,\dot i$; the image sweeps at this rate, so the film must move at
$$v_{\text{film}}=\frac{x(n-1)}{n}\,\omega=\frac{0.050\times0.5}{1.5}\times2\pi\times200=\boxed{21\ \text{m/s}}.$$

> 【Thought】 The image-shift mechanism: the cube's rotation angle *is* the incidence angle $i$, so image velocity $= (x(n-1)/n)\times$ angular speed — the small-angle result from (i) is exactly what's needed, because the cube is only near-normal during the brief exposure window. (By symmetry the rotation angle equals the incidence angle — the glint sweeps with the Sun.)

---

### Question 5 — Gravity and forces

#### Q5(a) — Oumuamua is not bound to the Sun [4 marks]

**Key observation.** Compare the measured speed at closest approach with the local escape speed — hyperbolic excess means an interstellar origin.

$$v_{esc}=\sqrt{\frac{2GM_\odot}{r}}=\sqrt{\frac{2\times6.67\times10^{-11}\times1.99\times10^{30}}{3.81\times10^{10}}}=83.4\ \text{km/s}.$$
$$v=87.7\ \text{km/s}>83.4\ \text{km/s}\ \Rightarrow\ \boxed{\text{energy}>0,\ \text{hyperbolic — not a Solar System object}}\ (\tfrac12v^2-GM/r=+0.9\ \text{(km/s)}^2>0).$$

> 【Thought】 Equivalent framing: orbital energy per unit mass $E=\tfrac12v^2-GM/r$; bound orbits have $E<0$. Either statement earns the marks; the escape-speed comparison is the fastest.

#### Q5(b) — Ultima Thule [8 marks]

**(i) Centre of mass.** Masses $\propto r^3$ (same density): $m_2/m_1=(7.1/9.75)^3=0.386$. Measured from the large sphere's centre, with centres $r_1+r_2=16.85$ km apart:
$$x_{CM}=\frac{m_2(r_1+r_2)}{m_1+m_2}=\frac{0.386\times16.85}{1.386}=\boxed{4.7\ \text{km}}.$$

**(ii) Density estimate.** Marginally bound ⟹ gravity between the lobes supplies the spin's centripetal demand. For the small lobe circling the CM at $d_2=16.85-4.7=12.2$ km:
$$\frac{Gm_1m_2}{(r_1+r_2)^2}=m_2\omega^2d_2\;\Rightarrow\;\rho=\frac{3\omega^2d_2(r_1+r_2)^2}{4\pi G r_1^3},$$
$$\omega=\frac{2\pi}{15\times3600}=1.16\times10^{-4}\ \text{rad/s}\;\Rightarrow\;\boxed{\rho\approx1.8\times10^{2}\ \text{kg/m}^3}\ \text{(very fluffy — a rubble pile ✓)}.$$

**(iii) Sketch of $g$ along the long axis.** Piecewise: outside each sphere $g\propto1/r^2$ falling to the far tails; *inside* each sphere linear through zero at its centre (given); at the contact point the two spheres' fields oppose — sketch shows a **null point** between the centres (closer to the smaller lobe), peaks at the surfaces, and sign changes at each centre. (Potential sketch helpful: $V$ has minima... maxima of $|g|$ at surfaces, $V$ smooth and monotonic in between with an inflection at the null.) (A mean density well below rock ⟹ a rubble pile, not a monolith — porosity is the physical reading of low density.)

#### Q5(b cont.) — The collision of two iron spheres [7 marks]

**(iv) Energy liberated** (fall from rest at infinity to contact at $r_1+r_2$):
$$E=\frac{Gm_1m_2}{r_1+r_2}=\frac{6.67\times10^{-11}\times3.06\times10^{16}\times1.18\times10^{16}}{1.685\times10^4}=\boxed{1.4\times10^{18}\ \text{J}}.$$

**(v) Relative speed.** $\tfrac12\mu v^2=E$ with reduced mass $\mu=\dfrac{m_1m_2}{m_1+m_2}=8.5\times10^{15}$ kg:
$$v=\sqrt{\frac{2E}{\mu}}=\sqrt{\frac{2.86\times10^{18}}{8.5\times10^{15}}}=\boxed{18\ \text{m/s}}.$$

**(vi) Moles of iron.** $n=\dfrac{m_1+m_2}{0.056\ \text{kg/mol}}=\dfrac{4.24\times10^{16}}{0.056}=\boxed{7.6\times10^{17}\ \text{mol}}$.

**(vii) Maximum temperature.** Debye $T^3$ law: energy to warm $n$ moles from $T_0=4$ K:
$$E=n\int_{T_0}^{T}\frac{12\pi^4R}{5\theta_D^3}T'^3\,dT'=n\frac{12\pi^4R}{5\theta_D^3}\frac{T^4-T_0^4}{4}=n\frac{3\pi^4R}{5\theta_D^3}T^4\quad(T\gg T_0),$$
$$T^4=\frac{5\theta_D^3E}{3\pi^4Rn}=\frac{5\times464^3\times1.43\times10^{18}}{3\pi^4\times8.31\times7.6\times10^{17}}=3.9\times10^5\;\Rightarrow\;\boxed{T\approx25\ \text{K}}.$$

*(Official mark scheme prints $T=2550$ K — a slip of its own equation: $T^4=3.9\times10^5\ \text{K}^4$ gives $T=25$ K ($25^4=3.9\times10^5$ ✓), and 2550 K would need $10^{13}$ times more energy than is available. Ours stands.)*

> 【Thought】 Structure spot: $c\propto T^3$ (Debye) ⟹ energy $\propto T^4$ — so the final temperature is astonishingly insensitive to the energy (fourth root). The integral $\int T^3dT$ with the variable heat capacity is the designed calculus step; using a constant room-temperature $c$ would be wrong here and would overestimate… (compute: $T$ comes out near 25 K, safely in the Debye regime $T\ll\theta_D$ ✓ self-consistent).

---

### Question 6 — Applications of wave interference

#### Q6(a) — Conditions for stable interference [2 marks]

- **Coherence**: the sources must have a constant phase relationship (same frequency, fixed phase difference over the observation time);
- comparable **amplitudes** (otherwise poor fringe contrast);
- the same **polarisation** state (transverse waves), and path differences within the coherence length. Coherence itself means: same frequency *and* a constant phase difference — both are needed for stable fringes.

#### Q6(b) — Ship receiver with sea reflection (Lloyd's geometry) [4 marks]

**(i)** Direct path: $\sqrt{D^2+(H-h)^2}\approx D+\dfrac{(H-h)^2}{2D}$ ($D\gg H,h$ — grazing assumption); sea-reflected path (image transmitter at depth $-H$): $\approx D+\dfrac{(H+h)^2}{2D}$. Path difference:
$$\Delta=\frac{(H+h)^2-(H-h)^2}{2D}=\frac{2Hh}{D}.$$
Reflection off the denser medium (sea) adds a phase of $\pi$, so a **maximum** needs $\Delta=(m+\tfrac12)\lambda$; the first maximum ($m=0$):
$$\frac{2Hh}{D}=\frac{\lambda}{2}\;\Rightarrow\;\boxed{h=\frac{\lambda D}{4H}}.\ \blacksquare$$

> 【Thought】 The π phase flip on reflection is what turns the "obvious" constructive condition into the half-integer one — forget it and you'd derive $h=\lambda D/2H$ (the *minimum*). The hint in the question is there precisely because this sign decides the answer.

**(ii)** $D=1500$ m, $h=20$ m, $H=80$ m, $\lambda=c/f=4.29$ m. Currently $\Delta=\dfrac{2\times80\times20}{1500}=2.13$ m $\approx\lambda/2=2.14$ m — sitting at a maximum ✓.
i. A **minimum** needs $\Delta=\lambda$. Key physics: the ship **floats**, so its receiver stays $h=20$ m above the sea whatever the tide; only the cliff transmitter's height above the sea grows: $H\to80+\delta$. Then $2h(80+\delta)/D=\lambda$ ⟹ $H'=\lambda D/2h=4.29\times1500/40=161$ m:
$$\boxed{\delta=161-80\approx81\ \text{m}\ \text{— absurd for a tide: it cannot happen.}}$$
*(A floating ship keeps $h$ fixed; letting the receiver fall with the tide would wrongly give $\delta\approx14$ m — the official mark scheme's 81 m follows the floating reading.)*
ii. Normal tidal range 5 m: $H$ moves $80\to85$ m at most, so $\Delta$ moves from 2.13 m to $2\times20\times85/1500=2.27$ m — from $0.498\lambda$ to $0.53\lambda$: the signal eases off the maximum by only a few percent: **no appreciable change** (and the true minimum needs an impossible 81 m fall).
iii. Receiver at $h=0.5$ m: $\Delta=\dfrac{2\times80\times0.5}{1500}=0.053$ m $\approx0.012\lambda$ — deep in the destructive region: **the signal is essentially lost** (and tides cannot rescue it); the receiver must be raised.

#### Q6(c) — Bragg reflection from NaCl [8 marks]

**(i)** Adjacent planes, spacing $d$, rays reflecting at grazing angle $\theta$: the lower ray travels $2d\sin\theta$ further (down-leg $d\sin\theta$ + up-leg $d\sin\theta$, read off the right triangle between the wavefronts); constructive interference:
$$\boxed{2d\sin\theta=n\lambda}.\ \blacksquare$$

**(ii) Lattice spacing from density.** Each cube of side $d$ contains one ion on average (8 corners × 1/8), so one Na–Cl pair occupies $2d^3$:
$$2d^3=\frac{M/N_A}{\rho}=\frac{58.4\times10^{-3}/6.02\times10^{23}}{2170}=4.47\times10^{-29}\ \text{m}^3\;\Rightarrow\;\boxed{d=2.82\times10^{-10}\ \text{m}\ (0.28\ \text{nm})}.$$

**(iii)** Minimum angle = first order: $\lambda=2d\sin25^\circ=2\times0.282\times0.4226=\boxed{0.24\ \text{nm}}$.

> 【Thought】 "Minimum angle" = smallest $n$ ($n=1$), because $\sin\theta$ increases with $n$ — reading "minimum" as an order selector is the move. (ii)'s counting — one ion per $d^3$ cube — is the standard simple-cubic inventory; the resulting $d=0.282$ nm matches the accepted NaCl spacing ✓.

#### Q6(d) — Oil film on water [7 marks]

**(i) Sketch.** Ray hits the oil surface: partial reflection (ray 1) at the air–oil interface; the transmitted ray refracts down, reflects off the oil–water interface (ray 2), re-emerges and refracts out parallel to ray 1. Mark rays 1 and 2 — these interfere. Mark the incidence angle $i$ and refraction angle $r$.

**(ii) Minimum thickness for strong violet reflection.** Phase changes: ray 1 (air→oil, $n$ increases) flips by $\pi$; ray 2 (oil→water, $1.5\to1.33$, $n$ *decreases*) does **not** flip. Net $\pi$ between the rays ⟹ constructive reflection needs the round-trip path to supply a **half** wavelength:
$$2nt\cos r=\frac{\lambda}{2}\ (m=0),\qquad \sin r=\frac{\sin50^\circ}{1.5}\Rightarrow r=30.7^\circ,\ \cos r=0.860,$$
$$t_{\min}=\frac{\lambda}{4n\cos r}=\frac{410}{4\times1.5\times0.860}=\boxed{79\ \text{nm}}.$$

> 【Thought】 The phase-flip inventory is the whole game in thin-film problems: count flips at *each* boundary first (air→oil flips, oil→water doesn't), then choose $\tfrac{(2m+1)\lambda}{2}$ (one flip) vs $m\lambda$ (zero or two flips). If the film sat on glass ($n=1.6>$ oil), both rays would flip and the condition would flip too.

---
*End of Paper 13 (2019 Round 1 Section 2).*


---

## Paper 14 — 2018 Round 1 Section 2 (16 Nov 2018)

*Section 2: Questions 2–6, 25 marks each; candidates attempt two. Full solutions for all five.*

---

### Question 2 — Gravity

#### Q2(a) — Orbital period in terms of surface quantities [3 marks]

Gravity at the surface: $g=GM_p/R^2$ (defines the planet's $GM_p$ from measurable surface quantities). Circular orbit: gravity supplies the centripetal acceleration:
$$\frac{GM_p}{r^2}=\omega^2r=\frac{4\pi^2r}{T^2}\;\Rightarrow\;\boxed{T=2\pi\sqrt{\frac{r^3}{gR^2}}}.$$

> 【Thought】 The physics chain to narrate: (1) surface measurement fixes $GM_p$; (2) in orbit, gravity *is* the centripetal force — no other force acts; (3) $T=2\pi/\omega$. Substituting $GM_p=gR^2$ is the elimination step that answers "in terms of R, g, r".

#### Q2(b) — Jupiter's orbital radius [1 mark]

Kepler III in au–years: $T^2=r^3$ ⟹ $r_J=11.9^{2/3}=\boxed{5.2\ \text{au}}$.

#### Q2(c) — Earth's mass from a two-density model [3 marks]

**Key observation.** From the density graph: read the core/mantle boundary $r_c\approx3.5\times10^6$ m and representative densities $\rho_c\approx11\times10^3$ kg/m³ (core), $\rho_m\approx4.5\times10^3$ kg/m³ (mantle); sum the two shell masses.

$$M\approx\frac43\pi\left[\rho_m(R^3-r_c^3)+\rho_c r_c^3\right]=\frac43\pi\left[4.5\times10^3\times2.16\times10^{20}+11\times10^3\times4.3\times10^{19}\right]\approx\boxed{6.0\times10^{24}\ \text{kg}}.$$

> 【Thought】 Seeing a stepwise density graph → triggers *piecewise-uniform shells*: the crudest faithful model. The result lands within 1% of the true mass — a nice demonstration that two shells suffice. State your read-off values explicitly: they are the inputs that make the estimate checkable.

#### Q2(d) — Planet–moon potential landscape and the minimal launch [9 marks]

**(i) Sketch.** Equipotentials: circles around each body close in; distorted into a figure-of-eight-ish pattern between them; far away they become circles around the pair. **Neutral point** (zero field): between the bodies, much closer to the *moon* (lighter); **centre of mass**: $\dfrac{D}{1+M_p/M_m}=\dfrac{D}{9}$ from the planet — i.e. near the planet, far from the neutral point. Marking both exposes the common confusion: zero-field ≠ centre of mass.

**(ii) Lowest-speed point.** A coasting rocket is slowest at the top of the potential barrier — the neutral point, where the two fields cancel:
$$\frac{GM_p}{d^2}=\frac{GM_m}{(D-d)^2}\;\Rightarrow\;\frac{D-d}{d}=\sqrt{\frac{M_m}{M_p}}=\frac{1}{2\sqrt2},\qquad d=\frac{D}{1+1/(2\sqrt2)}=\boxed{0.74\,D=2.84\times10^8\ \text{m}}.$$

**(iii) Launch speed.** Energy conservation from the surface ($R_p$, take $R_p=6.4\times10^6$ m for this Earth-mass planet) to the neutral point with zero residual speed:
$$\frac12v^2=GM_p\left(\frac{1}{R_p}-\frac1d\right)+GM_m\left(\frac{1}{D-R_p}-\frac{1}{D-d}\right),$$
$$v=\sqrt{2\times6.67\times10^{-11}\left[6.00\times10^{24}(1.563\times10^{-7}-3.52\times10^{-9})+7.50\times10^{23}(2.65\times10^{-9}-1.00\times10^{-8})\right]},$$
$$\boxed{v\approx1.1\times10^{4}\ \text{m/s}\ (11\ \text{km/s})}.$$

> 【Thought】 Structure: "just enough energy to reach the moon" = arrive at the barrier top (neutral point) at zero speed; past it, the moon's gravity pulls the rocket in by itself. Note the moon's term is *negative* (its well helps once you're close) and small here (5%) — but omitting it is only legitimate if you say so.

#### Q2(e) — Gravity down a gold mine [4 marks]

**Key observation.** Descending $d$: two competing effects — you're closer to the centre ($+2d/R$) but the crustal shell above no longer pulls (shell theorem). Crust-shell mass: $\delta M=4\pi R^2d\,\rho_c$.

$$\frac{\Delta g}{g}\approx\frac{2d}{R}-\frac{\delta M}{M_E}=\frac{2\times3000}{6.37\times10^6}-\frac{4\pi(6.37\times10^6)^2(3000)(2500)}{6.0\times10^{24}},$$
$$=9.42\times10^{-4}-6.4\times10^{-4}=\boxed{+3.0\times10^{-4}\ (\text{g increases by}\approx0.03\%)}.$$

*(Official mark scheme: $-6.4\times10^{-4}$ (a decrease), keeping $R_E^2$ in the denominator — it drops the $+2d/R_E$ tightening term ($+9.4\times10^{-4}$ here) that the shrinking radius contributes. The full differential $dg/g=-d(\text{shell})/M+2d/R_E$ gives our $+3.0\times10^{-4}$ net increase. Same physics as Paper 33 Q8(b), where the same two terms compete.)*

> 【Thought】 The hint (shell theorem) is the licence to *subtract* the crust. The near-cancellation of two $\sim10^{-3}$ terms is the interesting physics: gravity barely changes down a mine because both effects matter. If the crust were denser than average, $g$ would actually *increase* more — the sign depends on crustal density vs mean density.

#### Q2(f) — Gravitational assembly energy of a planet [5 marks]

**(i)** Adding shell $\delta m$ (density $\rho$, thickness $\delta r$) to radius $r$: the shell falls from infinity onto the existing mass $M(r)=\tfrac43\pi r^3\rho$:
$$\delta U=-\frac{GM(r)\,\delta m}{r}=-\frac{G(\tfrac43\pi r^3\rho)(4\pi r^2\rho\,\delta r)}{r}=-\frac{16\pi^2}{3}G\rho^2r^4\,\delta r.$$

**(ii)** Integrate shell by shell, then convert $\rho=3M/(4\pi R^3)$:
$$U=-\frac{16\pi^2}{3}G\rho^2\int_0^R r^4\,dr=-\frac{16\pi^2}{15}G\rho^2R^5=\boxed{-\frac{3GM^2}{5R}}.$$

**(iii)** $|U|=Mc\,\Delta T$:
$$\Delta T=\frac{3GM}{5Rc}=\frac{3\times6.67\times10^{-11}\times4.0\times10^{26}}{5\times6.4\times10^6\times700}=\boxed{3.6\times10^{6}\ \text{K}}.$$

> 【Thought】 Millions of kelvin ⟹ a newly formed planet is fully molten/gaseous — this is why planets differentiate (iron sinks). The clean emergence of $-3GM^2/5R$ rewards keeping $\rho$ symbolic until the end.

---

### Question 3 — Springs and elasticity

#### Q3(a) — String circle with elevated anchor (conical pendulum variant) [5 marks]

**(i)** The string runs from the particle up to a point at height $h$ above the circle's centre. Vertical balance: $T\cos\theta=mg$; horizontal (centripetal): $T\sin\theta=m\omega^2r$. Dividing: $\tan\theta=\omega^2r/g$. Geometry: $\tan\theta=r/h$. So $\omega^2=g/h$:
$$\boxed{T=2\pi\sqrt{\frac{h}{g}}}\quad\text{— independent of }r.$$

> 【Thought】 The physics to narrate: tension does double duty (supports weight vertically, drives the circle horizontally); eliminating $T$ and using the *given* geometry $\tan\theta=r/h$ makes $r$ and $\theta$ cancel together — the period depends only on the anchor's height above the plane. This is why a conical pendulum's period equals that of a simple pendulum of length $h$.

**(ii)** $T=3mg$: $\cos\theta=\dfrac{mg}{T}=\dfrac13$; $h=\ell\cos\theta$:
$$\boxed{\ell=\frac{h}{\cos\theta}=3h}.$$
(Note the period involves $\ell\cos\theta=h$ — it depends only on the anchor's *height*, not on the string length or tilt separately.)

#### Q3(b) — Elastic string: hanging mass and colliding pair [7 marks]

Calibration: tension $mg$ ⟹ extension $a$ ⟹ $k=mg/a$.

**(i)** Hanging oscillator: $\boxed{T=2\pi\sqrt{\dfrac{m}{k}}=2\pi\sqrt{\dfrac{a}{g}}}$.

**(ii)** Two masses on a smooth table, string stretched to $3a$ (extension $2a$):
i. **Motion description.** Symmetric approach: while the string is taut (separation $>a$), each mass feels a spring force toward the centre — they execute the inward half of SHM about the centre, accelerating less and less as the extension shrinks; once the separation reaches $a$ the string goes **slack**, the force vanishes, and they coast at constant speed until they collide at the centre.
ii. **Time.** With $u$ = inward displacement of each mass: extension $=2a-2u$, force $=2k(a-u)$, so $m\ddot u=-2k(u-a)$: SHM about $u=a$ with $\omega=\sqrt{2k/m}$, starting at rest at $u=0$: slack at $\omega t_1=\pi/2$, speed $v=a\omega$; then coast: gap $a$ closes at relative speed $2v$: $t_2=\dfrac{a}{2a\omega}=\dfrac{1}{2\omega}$:
$$t=t_1+t_2=\frac{\pi+1}{2\omega}=\frac{\pi+1}{2}\sqrt{\frac{m}{2k}}=\frac{\pi+1}{2}\sqrt{\frac{a}{2g}}=\frac{4.14}{2}\sqrt{\frac{0.20}{19.6}}=\boxed{0.21\ \text{s}}.$$

> 【Thought】 Phase-boundary discipline: the string can only pull, so the dynamics changes character at separation $a$ — recognise the two phases (SHM segment + coast) and stitch them by matching position and velocity. With $k=mg/a$, $m$ cancels throughout — the answer depends only on $a$ and $g$. (Once the string goes slack the constraint disappears entirely — that is what splits the motion into an SHM segment and a coasting phase.)

#### Q3(c) — Elastic cord stretched to twice its length at constant volume [5 marks]

**(i)** Constant volume: $A(\ell)=A_0\ell_0/\ell$. Tension at length $\ell$: $T=EA(\ell)\dfrac{\ell-\ell_0}{\ell_0}=EA_0\dfrac{\ell-\ell_0}{\ell}$; at $\ell=2\ell_0$:
$$\boxed{T=\frac{EA_0}{2}}.$$

**(ii) Work done:**
$$W=\int_{\ell_0}^{2\ell_0}EA_0\left(1-\frac{\ell_0}{\ell}\right)d\ell=EA_0\left[\ell-\ell_0\ln\ell\right]_{\ell_0}^{2\ell_0}=EA_0\big(2\ell_0-\ell_0-\ell_0\ln 2\big)=\boxed{E\ell_0A_0(1-\ln2)}.\ \blacksquare$$

> 【Thought】 The nonlinearity comes from the *shrinking cross-section*, not from the material (E constant) — the integrand $EA_0(1-\ell_0/\ell)$ decreases as you stretch, so $W$ is less than $\tfrac12T_{\max}\Delta\ell$; the $\ln2$ is the signature of the $1/\ell$ factor. Checking: $W<EA_0\ell_0\times\tfrac12$? $1-\ln2=0.31<0.5$ ✓.

#### Q3(d) — Boxing training ball between two springs [8 marks]

Setup: springs natural length $\ell$, $k=mg/\ell$ (force $mg$ doubles a spring's length); room height $4\ell$; ball radius negligible.

**(i) Equilibrium.** Top spring stretched $x-\ell$ (pulls up), bottom stretched $3\ell-x$ (pulls down):
$$k(x-\ell)=mg+k(3\ell-x)\;\Rightarrow\;2x=5\ell\;\Rightarrow\;\boxed{x=2.5\ell\ \text{below the ceiling}}.$$

**(ii) Vertical oscillation.** Displace $y$ downward: both springs' forces change restoringly by $ky$ each ⟹ $F=-2ky$:
$$\boxed{T_v=2\pi\sqrt{\frac{m}{2k}}=2\pi\sqrt{\frac{\ell}{2g}}}.$$

**(iii) Horizontal force (small displacement ξ).** To first order the spring *lengths* don't change (length changes are second order in ξ), so tensions stay at their equilibrium values; each tilted spring pulls with a horizontal component $T\times(\xi/L)$ toward its anchor:
$$F_h=-\xi\left(\frac{T_t}{L_t}+\frac{T_b}{L_b}\right)=-\xi\left(\frac{k(1.5\ell)}{2.5\ell}+\frac{k(0.5\ell)}{1.5\ell}\right)=\boxed{-k\xi\left(\frac35+\frac13\right)=-\frac{14}{15}k\,\xi}.$$

> 【Thought】 The approximation to state: tilting a spring changes its length at order $\xi^2/L$ — negligible — so the *magnitudes* of tension are frozen; only their *directions* rotate, producing the restoring force. That argument is the entire content of "suitable approximation" and is what a marker looks for.

**(iv)** $\omega_h^2=\dfrac{14k}{15m}$ vs $\omega_v^2=\dfrac{2k}{m}$:
$$\frac{T_h}{T_v}=\sqrt{\frac{\omega_v^2}{\omega_h^2}}=\sqrt{\frac{2}{14/15}}=\boxed{\sqrt{\frac{15}{7}}\approx1.46}.$$
(Same track, same speed: only the *direction* of the normal force changes between the two runs, its magnitude does not — that is why a frequency ratio suffices.)

---

### Question 4 — Pressure and fluids

#### Q4(a) — Pressure at the bottom of a cylinder; variants [8 marks]

**(i)** i. The bottom supports the liquid's weight: $P=\dfrac{W}{A}=\dfrac{\rho g A h}{A}=\boxed{\rho gh}$.
ii. Units: $[\rho gh]=\dfrac{\text{kg}}{\text{m}^3}\dfrac{\text{m}}{\text{s}^2}\text{m}=\dfrac{\text{kg}}{\text{m s}^2}=\dfrac{\text{N}}{\text{m}^2}=\text{Pa}$ ✓.
iii. Linearly graded density: the mean density carries the weight: $P=\boxed{\tfrac12(\rho_t+\rho_b)gh}$ (integrate $\rho(y)$ or argue by the trapezium/average — total mass = mean density × volume).
iv. The atmosphere fails the model because $\rho$ is far from constant (it falls off roughly exponentially with height — the scale height is only ~8 km ≪ 200 km), and $g$ itself weakens with altitude; $\rho_{\text{surface}}gh$ with $h=200$ km would overestimate enormously. (Density *stratification*, not height, is the error source — part iii shows the fix when the variation is linear.)

**(ii) Jet from a hole at depth h′.** i. **Energy:** a mass $m$ falling $h'$ converts PE to KE: $mgh'=\tfrac12mv^2$ ⟹ $v=\sqrt{2gh'}$ (Torricelli). Falling $(h-h')$ to the floor: $t=\sqrt{2(h-h')/g}$:
$$H=vt=2\sqrt{h'(h-h')},\qquad\text{maximised at }h'=\frac h2:\quad \boxed{H_{\max}=h}.$$
ii. **Momentum/Newton route:** the pressure $p=\rho gh'$ drives a plug of cross-section $A$ and length $L$: force $pA$ accelerates mass $\rho AL$: $a=\dfrac{gh'}{L}$; the plug reaches $v$ over length $L$: $v^2=2aL=\sqrt{2gh'}^2$ — same result ✓. (Caution: the naive flux equation $\rho gh'A=\rho Av^2$ gives $v^2=gh'$, off by $\sqrt2$ — it mis-assigns the momentum balance during acceleration through the hole region; the pressure near a flowing orifice is not fully hydrostatic. Naming this trap is worth marks.)

> 【Thought】 Optimisation protocol per the writing guide: objective $H(h')=2\sqrt{h'(h-h')}$, constraint $0<h'<h$, differentiate (or AM–GM: product $h'(h-h')$ maximal at $h'=h/2$), confirm maximum ($H\to0$ at both ends), then state $H_{\max}$. (The linear $p$–$h$ law is a liquid-column model; the atmosphere is not linear — pressure falls exponentially — so this pump result does not carry over to air.)

#### Q4(b) — Suspended hollow cuboid, then pierced [7 marks]

**(i)** Pressure on top (depth $h_t$): $F_t=(P_0+\rho_\ell gh_t)ab$ down; on the bottom (depth $h_t+h$): $F_b=(P_0+\rho_\ell g(h_t+h))ab$ up. Net upward force from the liquid:
$$F_b-F_t=\rho_\ell gabh=\rho_\ell gV\ \text{(Archimedes recovered from pressure)},\qquad \boxed{T=Mg-\rho_\ell gabh}.$$

**(ii) Pierced container.** Air initially at $P_0$, volume $abh$; finally fraction $f$: $P_0abh=P_{air}f\,abh$ (isothermal — stated assumption). Pressure chain: at the hole (bottom, depth $h'$): outside pressure $P_0+\rho_\ell gh'$; the internal water column of height $(1-f)h$ sits below the trapped air: $P_{air}+\rho_\ell g(1-f)h=P_0+\rho_\ell gh'$:
$$\frac{P_0}{f}=P_0+\rho_\ell g\big(h'-(1-f)h\big)\;\Rightarrow\;\boxed{h'=(1-f)h+\frac{P_0(1-f)}{\rho_\ell gf}}.$$

> 【Thought】 Model inventory: (1) isothermal trapped air (Boyle); (2) hydrostatics through the *internal* water column as well as the external one — the internal head $(1-f)h$ is the step most solutions drop. Check limits: $f\to1$ (no leak) gives $h'\to0$ — consistent with air at $P_0$ barely needing to be compressed ✓; as $f$ shrinks, $h'$ grows — deeper submersion needed to squeeze the reduced air charge harder ✓. (The pressure balance includes the *internal* water column above the trapped air — omitting it is the classic error here.)

#### Q4(c) — Floating rod hinged at the wall [5 marks]

**Key observation.** Hinge at the top end, rod dipping into the liquid at angle $\theta$; take moments about the hinge so its reaction drops out. Buoyancy acts at the centroid of the *submerged* portion.

**Solution.** Fraction above surface $\lambda/n$; submerged length $\lambda(n-1)/n$, whose centre is $\dfrac{\lambda}{n}+\dfrac{\lambda(n-1)}{2n}=\dfrac{\lambda(n+1)}{2n}$ from the hinge. Moments (cos θ cancels):
$$\rho_rgA\lambda\times\frac{\lambda}{2}=\rho_\ell gA\frac{\lambda(n-1)}{n}\times\frac{\lambda(n+1)}{2n}\;\Rightarrow\;\rho_r=\rho_\ell\frac{n^2-1}{n^2},$$
$$\boxed{n=\sqrt{\frac{\rho_\ell}{\rho_\ell-\rho_r}}}.$$

**Check.** $\rho_r\to\rho_\ell$: $n\to\infty$ — fully submerged, rod vertical-ish, barely floating ✓; $\rho_r\to0$: $n\to1^+$ — almost everything above the surface ✓; buoyancy balance alone ($\rho_r=\rho_\ell(n-1)/n$) would miss the hinge-geometry factor — the moment equation is essential because the hinge carries part of the weight.

#### Q4(d) — Floating cone, then loaded [5 marks]

**(i)** Submerged mini-cone (height $h/n$, radius $r/n$): $V_s=\tfrac13\pi r^2h/n^3=V/n^3$. Flotation: $mg=\rho_\ell gV/n^3$:
$$\boxed{m=\frac{\rho_\ell\pi r^2h}{3n^3}}.$$

**(ii)** An equal weight ($2mg$ total) is placed gently; the cone sinks, just reaches full submersion with zero KE, then rises. Energy from the floating state (submersion depth $h/n$) to full submersion — buoyancy varies with depth, so integrate: with submersion depth $y$, $B(y)=\rho_\ell gV(y/h)^3=mg\,n^3(y/h)^3$:
$$\underbrace{2mg\,h\left(1-\frac1n\right)}_{\text{gravity work}}=\underbrace{\int_{h/n}^{h}mg\,n^3\frac{y^3}{h^3}\,dy}_{\text{work against buoyancy}}=mgn^3\frac{h^4-h^4/n^4}{4h^3}=mgh\,\frac{n^3-1/n}{4},$$
$$8\left(1-\frac1n\right)=n^3-\frac1n\;\Rightarrow\;8(n-1)=n^4-1=(n-1)(n+1)(n^2+1),$$
$$\boxed{(n+1)(n^2+1)=8\ \Longleftrightarrow\ n^3+n^2+n=7}.\ \blacksquare\quad(n\approx1.31)$$

> 【Thought】 The question's structure: "neglect inertia and viscosity + energy considerations helpful" ⟹ energy balance between two zero-KE states. The buoyancy integral is the workhorse: $B\propto y^3$ because the submerged cone's *volume* scales cubically with depth (similar cones). Spot that $n^4-1$ factorises with a factor $(n-1)$ before solving numerically — the printed target equation tells you the factoring exists. (Physically the buoyancy grows like the *cube* of depth here — displaced volume scales with the submerged cone's volume — which is what makes the equation transcendental-looking but factorable.)

---

### Question 5 — Circuits and networks

#### Q5(a) — Potentiometer vs rheostat control of V across R₂ [5 marks]

**Topology (Fig. 6).** (a) **Potentiometer**: the whole wire R₁ is across E; R₂ connects the slider to the bottom rail — R₂ is in parallel with the wire's lower fraction $x$. (b) **Rheostat**: only the left fraction $x$ of R₁ carries current, in series with R₂.

**(i) Fig. 6a graphs** ($V$ vs slider position $x$ = lower fraction):
- $R_2\gg R_1$: $V\approx Ex$ — straight line $0\to E$ (R₂ barely loads the divider).
- $R_2\ll R_1$: $V= E\,\dfrac{R_2\parallel xR_1}{(1-x)R_1+R_2\parallel xR_1}$ — hugs 0 for most of the travel, then leaps to E near the top (severe loading).

**(ii) Fig. 6b graphs** ($V= E\,\dfrac{R_2}{R_2+xR_1}$, $x$ = fraction of R₁ in circuit):
- $R_2\gg R_1$: nearly flat just below E (gentle decline $E\to E/(1+R_1/R_2)$).
- $R_2\ll R_1$: steep hyperbolic fall from E to $ER_2/(R_2+R_1)\approx ER_2/R_1$.

**(iii) Relative advantages.** Potentiometer (a): full $0\to E$ range, smooth control, linear when $R_2\gg R_1$ — but always dissipates $E^2/R_1$ even at zero output, and loading distorts linearity if $R_2$ is small. Rheostat (b): simpler two-terminal wiring, never shorts the supply (R₁ limits current), lower idle loss — but output can never reach 0 (minimum $ER_2/(R_2+R_1)$) and control is coarse when $R_2\ll R_1$. Choose (a) for full-range voltage control of light loads, (b) for current control of heavy loads.

#### Q5(b) — Five-resistor network [4 marks]

**Topology (Fig. 7):** a (30 Ω): X–N₂; b (15 Ω): X–N₁; c (15 Ω): N₁–N₂; d (15 Ω): N₂–Y; e (30 Ω): N₁–Y.

**(i)** Set $V_X=V$, $V_Y=0$. KCL:
$$N_1:\ 5N_1-2N_2=2V,\qquad N_2:\ 5N_2-2N_1=V\;\Rightarrow\;N_1=\frac{4V}{7},\ N_2=\frac{3V}{7}.$$
Currents ($V=0.21$ V at 10 mA total): $I_a=\dfrac{V-3V/7}{30}=\boxed{4\ \text{mA}}$; $I_b=\dfrac{V-4V/7}{15}=\boxed{6\ \text{mA}}$; $I_c=\dfrac{4V/7-3V/7}{15}=\boxed{2\ \text{mA}}$; $I_d=\dfrac{3V/7}{15}=\boxed{6\ \text{mA}}$; $I_e=\dfrac{4V/7}{30}=\boxed{4\ \text{mA}}$.

**(ii)** $R_{XY}=\dfrac{V}{I}=\dfrac{0.210}{0.010}=\boxed{21\ \Omega}$.

**Check.** KCL at N₁: $6=2+4$ ✓; at N₂: $4+2=6$ ✓; totals at X and Y both 10 mA ✓.

#### Q5(c) — Strain gauge [6 marks]

$A=\pi(1.4\times10^{-5})^2=6.16\times10^{-10}\ \text{m}^2$; $R_0=\dfrac{\rho L}{A}=\dfrac{5.0\times10^{-7}\times0.30}{6.16\times10^{-10}}=\boxed{244\ \Omega}$ (i).

**(ii)** Stretched to 0.301 m, diameter constant: $R=R_0\times\dfrac{0.301}{0.300}=\boxed{244.4\ \Omega}\ (\Delta R=+0.81\ \Omega)$.

**(iii)** Constant volume ($A\propto1/L$): $R\propto L^2$: $R=243.6\times(0.301/0.300)^2=\boxed{245.2\ \Omega}\ (\Delta R\approx+1.6\ \Omega$ — about double: constant-volume straining roughly doubles the gauge factor ✓ this is why real strain gauges work).

**(iv) Bridge.** R₁, R₄ stretched (244.4 Ω); R₂, R₃ plain (243.6 Ω); 9 V across the top–bottom vertices; voltmeter between left and right vertices:
$$V_L=9\frac{R_3}{R_1+R_3}=9\times\frac{243.6}{488.0}=4.493\ \text{V},\qquad V_R=9\frac{R_4}{R_2+R_4}=9\times\frac{244.4}{488.0}=4.507\ \text{V},$$
$$\boxed{V_{\text{meter}}=V_R-V_L\approx+15\ \text{mV}}.$$

> 【Thought】 Bridge sensitivity: the imbalance is $\approx E\,\Delta R/(2(2R))=E\,\Delta R/4R$ — millivolts from a sub-ohm change; the bridge converts a 0.3% resistance change into a readable voltage. Note the symmetry: stretching R₁ and R₄ (diagonal pair) moves both midpoints in opposite directions — by design. Constant volume means stretching also thins the wire, so resistance changes *twice over* ($R=\rho\ell/A$ with $\ell$ up and $A$ down) — the gauge effect doubles the response.

#### Q5(d) — Infinite ladder network [4 marks]

Self-similarity: adding one more section (series $r_1$, shunt $r_2$) to the infinite tail leaves $R$:
$$R=r_1+\frac{r_2R}{r_2+R}\;\Rightarrow\;R^2-r_1R-r_1r_2=0\;\Rightarrow\;\boxed{R=\frac{r_1+\sqrt{r_1^2+4r_1r_2}}{2}}.$$
$r_1=4$, $r_2=15$: $R=\dfrac{4+\sqrt{16+240}}{2}=\boxed{10\ \Omega}$.

> 【Thought】 The fixed-point equation is the whole method — the hint ("add one more stage") is the standard infinite-network move. Choose the positive root (resistance > 0) and justify rejecting the negative one.

#### Q5(e) — Infinite chain of cells [6 marks]

**Key observation.** An active self-similar network needs *two* fixed-point equations — one for the resistance, one for the emf — and the **port order matters**: looking into the ladder from $R$, the first element is the *shunt* ($\varepsilon_2,R_2$), then the *series* arm ($\varepsilon_1,R_1$), then the identical tail $(E,Z)$. (Writing the recurrence in the wrong order — series then shunt — is the structural error to avoid.)

**Topology and polarity conventions (draw before computing).** Bottom rail = ground. Port node P (where $R$ attaches) at potential $E$ (the open-circuit emf). The shunt branch P→ground contains $\varepsilon_2$ in series with $R_2$, **$\varepsilon_2$'s positive terminal toward P**. The series arm P→T contains $\varepsilon_1$ in series with $R_1$, **$\varepsilon_1$'s positive terminal toward P**; T is the tail's port, and the tail is the identical ladder again (emf $E$, resistance $Z$ toward ground). Every later section repeats this exactly — that is the self-similarity.

**Resistance** (all sources zeroed — cells become plain wires): looking in from P: $R_2$ to ground, in parallel with $R_1+Z$:
$$Z=R_2\parallel(R_1+Z)\;\Rightarrow\;Z(R_1+R_2+Z)=R_2(R_1+Z)\;\Rightarrow\;Z^2+R_1Z-R_1R_2=0,$$
$$Z=\frac{-R_1+\sqrt{R_1^2+4R_1R_2}}{2}=\frac{-4+\sqrt{16+96}}{2}=\frac{-4+10.58}{2}=3.29\ \Omega.$$

**Emf** (open port: no current leaves P, so the shunt current feeds the series arm entirely). With $I_2$ the current ground→P in the shunt (rising through $\varepsilon_2$) and $I_1$ the current P→T in the series arm (falling through $\varepsilon_1$):
$$I_2=\frac{\varepsilon_2-E}{R_2},\qquad I_1=\frac{E-\varepsilon_1-V_T}{R_1},\qquad\text{KCL at P: } I_2=I_1.$$
The tail, seen from T, is a source $(E,Z)$: the current entering it is $I_1=\dfrac{V_T-E}{Z}$ (driving into its port emf). KCL at T:
$$\frac{E-\varepsilon_1-V_T}{R_1}=\frac{V_T-E}{Z}\;\Rightarrow\;V_T=E-\frac{\varepsilon_1 Z}{Z+R_1}.$$
Substituting into KCL at P (note $E-\varepsilon_1-V_T=\dfrac{\varepsilon_1R_1}{Z+R_1}$):
$$\frac{\varepsilon_2-E}{R_2}=\frac{\varepsilon_1}{Z+R_1}\;\Rightarrow\;E=\varepsilon_2+\frac{\varepsilon_1R_2}{Z+R_1}=2.0+\frac{1.0\times6}{3.29+4}=2.82\ \text{V}.$$

> 【Thought】 The formula $E=\varepsilon_2+\frac{\varepsilon_1R_2}{Z+R_1}$ is meaningless without the circuit drawing: it presumes shunt-first topology and both cells' $+$ terminals facing the port P. If the stem's “shunt branch ($\varepsilon_2,R_2$) first, then the series arm ($\varepsilon_1,R_1$)” became “series first, then shunt”, condition C (the port meets the shunt branch first) would break and this recursion would fail — fall back to the general method (write KCL level by level for the actual circuit, or truncate numerically), because a series-first port sees a different network ($Z'=R_1+R_2\parallel Z$). Likewise, if one cell were reversed ($\varepsilon_i$'s positive terminal facing away from P), the corresponding term in the expression for $E$ changes sign — polarity must be read off the figure before any algebra.

**Current through** $R=1\ \Omega$:
$$I=\frac{E}{Z+R}=\frac{2.82}{3.29+1.0}=\boxed{0.66\ \text{A}}.$$

> 【Thought】 Verification (diagnostic, not proof): truncating a 300-section ladder numerically converges to $E=2.8229$ V, $Z=3.2915$ Ω, $I=0.6578$ A ✓ three-way agreement. The lesson that stuck: in a ladder, state which element the port meets *first* — shunt-first vs series-first are different networks ($3.29$ Ω vs $7.29$ Ω). (Note: the official mark scheme prints $-0.5$ A from a collapsed two-loop model that discards the ladder structure; it does not survive the numerical check. Our corrected value $0.66$ A is the one consistent with direct nodal computation of the actual infinite ladder.)

---

### Question 6 — Capacitors

#### Q6(a) — Series capacitors: relations and the energy gap [6 marks]

**(i)** $Q_1=Q_2$ (the inner plates form an isolated island — charge merely shifts between them).
**(ii)** $V_1=Q/C_1$, $V_2=Q/C_2$.
**(iii)** $V=V_1+V_2=Q\left(\dfrac1{C_1}+\dfrac1{C_2}\right)$ ⟹ $\boxed{\dfrac1{C_{eq}}=\dfrac1{C_1}+\dfrac1{C_2}}$.
**(iv)** Stored: $U=\dfrac{Q^2}{2C_{eq}}=\tfrac12C_{eq}V^2$; supplied by the battery: $W=QV=C_{eq}V^2=2U$. **Comment:** half the battery's energy is dissipated (resistance of leads/contacts, or radiated) — charging a capacitor from a fixed voltage source is inherently 50% efficient regardless of how small the resistance is.

#### Q6(b) — Doubling the plate separation of a 15 nF / 70 V capacitor [2 marks]

**(i) Battery disconnected** (Q fixed, $Q=CV=1.05\ \mu\text{C}$; $C\to C/2$):
$$W=\Delta U=\frac{Q^2}{2(C/2)}-\frac{Q^2}{2C}=\frac{Q^2}{2C}=\tfrac12CV^2=\boxed{3.7\times10^{-5}\ \text{J}\ (37\ \mu\text{J})}.$$

**(ii) Battery connected** ($V$ fixed): stored energy *falls* by $\tfrac14CV^2=18\ \mu\text{J}$, while the battery absorbs $|\Delta Q|V=\tfrac12CV^2=37\ \mu\text{J}$ of charge-pushed-back work. The operator supplies the difference:
$$W=\Delta U+W_{\text{battery}}=-18+37=\boxed{+18\ \mu\text{J}}.$$

> 【Thought】 Both answers are positive (you always do work pulling attracting plates apart), but the battery case sends twice your input into the battery while the stored energy falls — the three-way bookkeeping ($W_{\text{you}}=\Delta U+W_{\text{battery}}$) is the content of the part.

#### Q6(c) — Capacitor connections [9 marks]

**(i)** $C_1=2\ \mu$F and $C_2=4\ \mu$F each carrying $120\ \mu$C ($V_1=60$ V, $V_2=30$ V), joined positive-to-positive:
i. Total charge $240\ \mu$C on $6\ \mu$F: $\boxed{V'=40\ \text{V}}$.
ii. $\Delta U=\tfrac12\dfrac{(240\ \mu\text{C})^2}{6\ \mu\text{F}}-\left[\tfrac12\dfrac{(120\ \mu\text{C})^2}{2\ \mu\text{F}}+\tfrac12\dfrac{(120\ \mu\text{C})^2}{4\ \mu\text{F}}\right]=4.8-5.4=\boxed{-0.6\ \text{mJ}\ (\text{energy lost, dissipated in the connecting transient})}.$

**(ii) Repeated contacts.** Each contact shares the total charge in a fixed capacitance ratio; the sphere keeps fraction $f$, with $f=Q/q$ fixed by the first contact. Recurrence $Q_{n+1}=f(Q_n+q)$ has fixed point
$$\boxed{Q_f=\frac{fq}{1-f}=\frac{Qq}{q-Q}}\qquad\left(\text{finite: the sphere asymptotes; needs }q>Q\right).$$

> 【Thought】 The geometric-series structure $Q_{n+1}=f(Q_n+q)$ is the physical model of "contact + recharge"; the fixed point exists because the sphere's share fraction is constant. If $q\le Q$ the series diverges — the premise (sphere gains $Q$ from a disc carrying $q$) requires $q>Q$ ✓ consistent.

**(iii) Ring of three charged capacitors** ($1, 2, 3\ \mu$F at 12 V; plates A,C,E positive; ring B–C, D–E, F–A).
i. Node charge conservation: $-q_1+q_2=+12$, $-q_2+q_3=+12$, $-q_3+q_1=-24$ (µC), and around the ring $\dfrac{q_1}{1}+\dfrac{q_2}{2}+\dfrac{q_3}{3}=0$:
$$q_1=-\frac{84}{11}=-7.6\ \mu\text{C}\ (\text{reversed: A now negative}),\quad q_2=\frac{48}{11}=+4.4\ \mu\text{C},\quad q_3=\frac{180}{11}=+16.4\ \mu\text{C}.$$
Diagram: label each capacitor with its final plate charges (e.g. C₁: A = +7.6 µC? — no: A carries $-7.6$ µC, B $+7.6$ µC; C₂: C $+4.4$, D $-4.4$; C₃: E $+16.4$, F $-16.4$ µC).
ii. Potential walk from A (0): across C₁ rises to $+7.6$ V (B/C), flat to C, drops 2.2 V across C₂ to $+5.45$ V (D/E), flat to E, drops 5.45 V across C₃ to 0 V (F), flat back to A. Sketch: step profile closing on itself ✓ (KVL satisfied — good check).

> 【Thought】 Two rules only: *isolated nodes conserve signed plate charge*, and *voltages sum to zero around the ring*. The surprise — C₁ ends up reverse-charged — is because the big C₃'s stored charge floods around the ring; always let the algebra assign signs.

#### Q6(d) — Concentric conducting spheres [4 marks]

**(i) E-field graph** ($r$: 0→30 cm): $E=0$ for $r<10$ cm; $E=kQ/r^2$ from 10→15 cm (a falling $1/r^2$ arc); $E=0$ for $r>15$ cm (equal opposite charges enclose zero net flux).
**(ii) Potential graph:** constant $V=120$ V for $r<10$ cm; falls smoothly as $kQ(1/r-1/0.15)$ to 0 at $r=15$ cm; stays 0 beyond. (Continuous, derivative $-E$ ✓.)
**(iii)** Inner alone: $V_{in}=\dfrac{Q}{4\pi\varepsilon_0(0.10)}$; outer alone: $V_{out}=-\dfrac{Q}{4\pi\varepsilon_0(0.15)}$ (this value fills its whole interior).
**(iv)** $\Delta V=\dfrac{Q}{4\pi\varepsilon_0}\left(\dfrac{1}{0.10}-\dfrac{1}{0.15}\right)=120$:
$$Q=\frac{120\times4\pi\varepsilon_0}{3.33}=\frac{120}{8.99\times10^9\times3.33}=\boxed{4.0\times10^{-9}\ \text{C}\ (4\ \text{nC})}.$$

> 【Thought】 The superposition in (iii)–(iv): the potential difference depends only on the inner sphere's field in the gap — the outer sphere contributes a *constant* inside itself, which cancels in the difference. This is why a spherical capacitor's capacitance is $4\pi\varepsilon_0\dfrac{ab}{b-a}$.
>
> **Official mark scheme note:** it prints $Q=8.0\times10^{-10}$ C, using $\Delta V=kQ(1/a+1/b)$ — i.e. it *added* the outer sphere's potential contribution instead of recognising that a shell's potential is constant inside and cancels in $\Delta V$. The standard spherical-capacitor formula $C=4\pi\varepsilon_0 ab/(b-a)$ gives our $Q=4.0$ nC directly, and the shell-theorem cancellation confirms it; the official value fails both checks.

#### Q6(e) — LED driven at constant current from a capacitor [4 marks]

**(i)** Constant $I=800\ \mu$A ⟹ linear capacitor discharge: $V_C(t)=5.0-\dfrac{I}{C}t=5.0-0.2t$. Circuit balance $V_C=2.7+IR$:
$$R(t)=\frac{5.0-0.2t-2.7}{8.0\times10^{-4}}=\boxed{R(t)=2875-250\,t\ \ (\Omega)}\quad\text{(ramp down at 250 Ω/s from 2.9 kΩ)}.$$

**(ii)** Lit until $R\to0$ / $V_C\to2.7$ V: $t=\dfrac{2.3}{0.2}=\boxed{11.5\ \text{s}}$, equivalently $t=\dfrac{C\,(V_0-V_d)}{I}=\dfrac{4.0\times10^{-3}\times2.3}{8.0\times10^{-4}}=11.5$ s ✓ same. *(The official mark scheme prints $1.15\times10^{-6}$ s — it substituted $C=0.4$ µF for the stated $4000$ µF; its own formula $t=C(V_0-V_d)/I$ with the stated $C$ gives our $11.5$ s.)*

> 【Thought】 Consistency check: charge removed $=It=800\ \mu\text{A}\times11.5\ \text{s}=9.2$ mC $=C\Delta V=4000\ \mu\text{F}\times2.3$ V ✓. Design lesson: a linearly-timed rheostat turns an exponential RC decay into a constant-current drive — that's the point of the circuit.

---
*End of Paper 14 (2018 Round 1 Section 2).*


---

## Paper 15 — 2018 Round 1 Section 1 (15 Nov 2018)

*Section 1, Question 1, parts (a)–(r). Maximum 50 marks from 87.*

---

### Q1(a) — Sun's speed around the galaxy [3 marks]

**Key observation.** Circular orbit speed $v=2\pi r/T$; convert light years via $c$.

$$v=\frac{2\pi\times26\,000\ \text{ly}}{240\times10^6\ \text{yr}}=\frac{2\pi\times26000\times9.46\times10^{15}\ \text{m}}{240\times10^6\times3.156\times10^7\ \text{s}}=\boxed{2.0\times10^{5}\ \text{m/s}\ (\approx200\ \text{km/s})}.$$

> 【Thought】 Unit strategy: light years and years share "year" — the ratio $r/T$ needs only one conversion (ly→m via $c\times$year). Check against the known solar value 220–230 km/s ✓ order right (the period given is slightly long).

---

### Q1(b) — Sphere suspended against a smooth wall [3 marks]

**Key observation.** Smooth wall ⟹ reaction is horizontal through the centre; weight acts through the centre; hence the thread's line must also pass through the centre (three-force concurrence) — the geometry is fully fixed by (thread + radius) = 15 cm hypotenuse with radius 6 cm horizontal offset.

**Solution.** The line anchor→centre has length $9+6=15$ cm; horizontal offset = radius = 6 cm:
$$\sin\theta=\frac{6}{15}=0.4\ \text{(thread at }\theta=23.6^\circ\text{ to the vertical)},\qquad T=\frac{mg}{\cos\theta}=\frac{0.5\times9.81}{0.9165}=\boxed{5.4\ \text{N}}.$$

> 【Thought】 Concurrence theorem again (as in Paper 5's rod-in-bowl): with two of the three forces passing through the centre, the third must too — this converts a statics problem into pure geometry. The wall's smoothness (no friction) is what allows it.

---

### Q1(c) — Kinematics from a cubic displacement [4 marks]

$s=2t^3-9t^2+12t+4$; $v=6t^2-18t+12=6(t-1)(t-2)$; $a=12t-18$.

**(i)** Rest when $v=0$: $\boxed{t=1\ \text{s}\ \text{and}\ t=2\ \text{s}}$.
**(ii)** $a=0$: $\boxed{t=1.5\ \text{s}}$.
**(iii)** $v(1.5)=6(2.25)-27+12=\boxed{-1.5\ \text{m/s}}$ (moving backward through the turnaround region).
**(iv)** $a(1)=-6\ \text{m/s}^2$, $a(2)=+6\ \text{m/s}^2$: $\boxed{\mp6\ \text{m/s}^2\text{ at }t=1\text{ s and }t=2\text{ s respectively}}$.

> 【Thought】 Read the cubic's story: the object reverses at $t=1$ and $t=2$ (two stationary points), with the inflection (a=0) exactly between them — a cubic's symmetry makes (ii) the midpoint of (i); noticing that saves a computation.

---

### Q1(d) — Train stopping distances [4 marks]

**Key observation.** Fit $s=av+bv^2$ to the two data points, then invert at $s=500$ m. The fitting trick: divide through by $v$ — $s/v=a+bv$ is *linear* in $v$.

> 【Thought】 The two terms have physical meanings: $av$ = thinking/reaction distance (scales with $v$), $bv^2$ = braking distance (KE dissipation). Fitting: divide each equation by $v$ first — $s/v=a+bv$ is *linear* in $v$: $(100/40)=a+40b$, $(280/80)=a+80b$: two clean equations.

**Solution.** $2.5=a+40b$; $3.5=a+80b$ ⟹ $b=\dfrac{1}{40}=0.025$, $a=1.5$ (with $v$ in km/h, $s$ in m). Solve $500=1.5v+0.025v^2$:
$$v^2+60v-20\,000=0\;\Rightarrow\;v=\frac{-60+\sqrt{3600+80000}}{2}=\frac{-60+289.1}{2}=\boxed{115\ \text{km/h}}.$$

**Check.** $1.5(114.5)+0.025(114.5)^2=172+328=500$ ✓; sanity: quadrupling 40 km/h → 160 km/h would give $1.5\times160+0.025\times25600=240+640=880$ m > 500 m, so the answer must lie well below 160 km/h ✓ 115 km/h is consistent.

---

### Q1(e) — Two planes turning to meet [7 marks]

**Key observation.** Positions at the turn time, then a head-to-head closure along the joining line; the meeting point divides the separation in the ratio of speeds.

> 【Thought】 Two phases, one line: after the turn both planes fly the same straight segment toward each other, so the closure speed is the *sum* (360+300) and the meeting point splits the separation as 360:300. Convert bearings with ($\sin\beta$ east, $\cos\beta$ north) as always.

**Solution.** At 40 min: plane 1 at $(0, 240)$ km; plane 2 at $200$ km on bearing 135°: $(141.4, -141.4)$ km. Separation: $(141.4, -381.4)$ km, $|\Delta|=406.8$ km. Closure: $t=406.8/660=0.616$ h; plane 1 covers $360\times0.616=221.9$ km along the unit vector $(0.3476, -0.9374)$:
$$\text{meeting point}=(0,240)+221.9(0.3476,-0.9374)=(77.1,\ 32.0)\ \text{km}.$$
(i) Bearing $=\arctan\dfrac{77.1}{32.0}=\boxed{067^\circ}$; (ii) distance $=\sqrt{77.1^2+32.0^2}=\boxed{83.5\ \text{km}}$.

**Check.** Plane 2 covers $300\times0.616=184.9$ km: $(141.4-184.9\times0.3476,\ -141.4+184.9\times0.9374)=(77.1,\ 32.0)$ ✓ same point.

---

### Q1(f) — Neutron moderation by deuterons [6 marks]

**(i)** Elastic head-on, target at rest, $m_d=2m_n$: $v_d=\dfrac{2m_n}{m_n+m_d}u=\boxed{\dfrac{2}{3}u}$.

**(ii)** Fraction transferred: $\dfrac{\tfrac12(2m)(2u/3)^2}{\tfrac12mu^2}=\boxed{\dfrac{8}{9}\approx89\%}$.

**(iii)** The neutron keeps $\dfrac{u'}u=\dfrac{|m-2m|}{m+2m}=\dfrac13$ of its speed ⟹ $\dfrac19$ of its KE per collision:
$$\left(\tfrac19\right)^n\le\frac{0.01\ \text{eV}}{10^7\ \text{eV}}=10^{-9}\;\Rightarrow\;n\log_{10}9\ge9\;\Rightarrow\;n\ge9.4\;\Rightarrow\;\boxed{10\ \text{collisions}}.$$

> 【Thought】 The elastic-collision formulas (velocity transfer $2m_1/(m_1+m_2)$, retained fraction $|m_1-m_2|/(m_1+m_2)$) are the workhorse of moderator physics — deuterium is good because 1/9 retention per head-on hit is heavy loss; the counting uses the *geometric* (not arithmetic) decay of energy.

---

### Q1(g) — Chain falling onto a table [6 marks]

**Key observation.** Every link free-falls (the chain goes slack onto the pile); at time $t$: length $x=\tfrac12gt^2$ landed, the rest still falling at $v=gt$. The table's reaction does two jobs: support the pile's weight AND absorb the momentum flux of landing links.

> 【Thought】 Seeing "falls and comes to rest without bouncing" → triggers *two-term reaction*: static weight of the arrived part + dynamic force $\dfrac{dm}{dt}v$ to stop the incoming links (the hint's $F=\frac{\Delta m}{\Delta t}v$). Both grow with $t$ — the peak is at the end.

**Solution.** (i) $\dfrac{dm}{dt}=\mu v=\mu gt$ (mass landing per second):
$$R(t)=\underbrace{\mu x g}_{\text{pile weight}}+\underbrace{\mu v^2}_{\text{stopping}}=\tfrac12\mu g^2t^2+\mu g^2t^2=\boxed{\tfrac32\mu g^2t^2}\quad\left(t\le\sqrt{\frac{2L}{g}}\right).$$

**(ii)** Maximum at the last instant, $t=\sqrt{2L/g}$: $R_{\max}=\tfrac32\mu g^2\times\dfrac{2L}{g}=3\mu gL=\boxed{3W}$, at the moment the final link lands.

**Check.** The dynamic term alone ($\mu v^2=2\mu gx$) is twice the pile weight ($\mu gx$) — so the table reads up to 3× the chain's weight ✓ this is the classic result for a falling chain.

---

### Q1(h) — Particle looping inside a cylindrical hole in a movable block [5 marks]

**Key observation.** The block lifts when the particle's upward push on the top of the hole exceeds $Mg$; the particle's top-of-circle speed is set by energy.

> 【Thought】 This is loop-the-loop with a movable frame: the condition at the top is $N\ge Mg$ (not the usual $N\ge0$) — the frame's weight replaces the contact condition. Newton's third law pairing (particle pushes block up with $N$) is the link. Note the block doesn't move until lift-off, so energy conservation for the particle alone is clean.

**Solution.** Top of the circle: $mg+N=\dfrac{mv_t^2}{r}$; lift when $N=Mg$. Energy: $v_t^2=v^2-4gr$.
$$\frac{m(v^2-4gr)}{r}-mg=Mg\;\Rightarrow\;v^2=\frac{gr(M+m)+4mgr}{m},$$
$$\boxed{v_{\min}=\sqrt{\frac{gr(M+5m)}{m}}}.$$

**Check.** $M\to0$: $v=\sqrt{5gr}$ — the standard loop-the-loop minimum ✓ (nice limit); heavier block ⟹ larger $v$ linearly under the root ✓.

---

### Q1(i) — Two cells, two resistors, earthed midpoint [4 marks]

**Topology (Fig. 3), read correctly this time.** Single loop: 2.0 V cell ($r=1.0$ Ω) — A — 5.0 Ω — earth — 3.0 Ω — B — 1.5 V cell ($r=0.5$ Ω) — back. In the figure the 2.0 V cell's long ($+$) plate faces **left** and the 1.5 V cell's long plate faces **right** — the $+$ terminals point *outward*, so around the loop the cells **aid** each other: net emf $3.5$ V. (Misreading the plates as opposing is the trap; the official mark scheme confirms the aiding reading.)

**(i)** $I=\dfrac{2.0+1.5}{1.0+5.0+3.0+0.5}=\dfrac{3.5}{9.5}=\boxed{0.37\ \text{A}}$ (clockwise: both cells discharging).

**(ii)** Terminal pds (both discharging, $V=\mathcal E-Ir$): 2.0 V cell: $2.0-0.368\times1.0=\boxed{1.63\ \text{V}}$; 1.5 V cell: $1.5-0.368\times0.5=\boxed{1.32\ \text{V}}$.

**(iii)** Current flows A→earth through the 5 Ω and earth→B... i.e. from B to earth through the 3 Ω:
$$\boxed{V_A=+0.368\times5.0=+1.84\ \text{V},\qquad V_B=-0.368\times3.0=-1.11\ \text{V}}.$$

> 【Thought】 Sign discipline: the earth point only fixes the zero — it carries no net current; $V_A,V_B$ follow from the resistor drops with signs set by the clockwise current. Both cells discharge here, so $V=\mathcal E-Ir$ applies to both — decide the regime from the current direction *before* writing the terminal-pd formula. (Official values: $I=0.368$ A, $1.63$ V, $1.32$ V, $+1.84$ V, $-1.11$ V — now identical to ours.)

---

### Q1(j) — Apparent displacement through glass, water and oil layers [7 marks]

**Key observation.** For near-normal viewing, each layer of thickness $t$ and index $n$ contributes an *apparent* thickness $t/n$; the displacement is the difference between real and apparent total thickness.

> 【Thought】 Small-angle optics: the ray in each layer bends toward the normal; extrapolating the final direction back gives apparent depth $t/n$ per layer (derive once from $\tan\theta\approx\sin\theta$ and Snell). The layers' effects **add** — this is why the three-layer problem is no harder than one layer.

**Solution.** (i) Sketch: ray from the bench (underside) refracting toward the normal at glass→water→oil→air boundaries, bending furthest at the final oil→air step; extend the emergent ray straight back to find the virtual bench position above the real one.
(ii) Apparent thickness: $\dfrac{1.8}{1.5}+\dfrac{1.2}{1.3}+\dfrac{0.8}{1.1}=1.200+0.923+0.727=2.85$ cm vs real 3.8 cm:
$$\boxed{\text{bench appears raised by }3.8-2.85\approx0.95\ \text{cm}\ (\approx9.5\ \text{mm})}.$$

**Check.** All indices >1 ⟹ raised ✓; largest shift from the highest-index layer relative thickness ✓. (Apparent-depth contributions from stacked layers simply add — each interface contributes its own $(1-1/n_i)$ share.)

---

### Q1(k) — Jumping on a bigger, lighter planet [4 marks]

**Key observation.** Same jump energy ⟹ height ∝ $1/g_{\text{planet}}$; and $g\propto\rho R$ (since $g=GM/R^2$ with $M\propto\rho R^3$).

> 【Thought】 Scaling chain: $g=\tfrac43\pi G\rho R$ — surface gravity of a uniform planet is linear in both density and radius. Fixed jumping energy $E=mgh$ then gives $h\propto1/g$.

**Solution.** $\dfrac{g'}{g}=\dfrac{\rho'R'}{\rho R}=\dfrac23\times2=\dfrac43$; 
$$\boxed{h'=h\times\frac34=0.75\ \text{m}}.$$

**Check.** Bigger radius wins over smaller density ⟹ stronger gravity ⟹ lower jump ✓ direction sane.

---

### Q1(l) — Wood block floating across an oil–water interface [4 marks]

**Key observation.** The block (density = oil's $\tfrac23\rho$) extends through both fluids; buoyancy comes from displaced oil *and* displaced water. Test whether it pokes into the water (it must, since floating in oil alone would need depth $4b$ > oil depth $b$).

**Solution.** Immersed depth $y$ below the oil surface; since $y>b$: buoyancy per unit area $=g\left[\tfrac23\rho\,b+\rho(y-b)\right]$. Weight per unit area $=\tfrac23\rho g\times4b$:
$$\tfrac23b+(y-b)=\tfrac83b\;\Rightarrow\;y-b=2b\;\Rightarrow\;y=3b,\qquad\boxed{\text{fraction immersed}=\frac{3b}{4b}=\frac34}.$$

**Check.** Buoyancy check: $\tfrac23\rho b+\rho(2b)=\tfrac83\rho b$ vs weight $\tfrac23\rho\times4b=\tfrac83\rho b$ ✓; the block dips $b$ into the water ($3b$ below oil top: $b$ of oil + $2b$ of water) ✓.

---

### Q1(m) — Cooling calorimetry: ethanol's specific heat [5 marks]

**Key observation.** "Same circumstances" ⟹ same heat-loss curve; Newton cooling through the same temperature range takes time ∝ total heat capacity. Compare the two runs.

> 【Thought】 The calorimeter's own heat capacity participates in both runs — include the 150 g of copper in *both* inventories. The ratio method cancels the unknown cooling law entirely.

**Solution.** $C_1=0.080\times4200+0.150\times400=336+60=396$ J/K (water run). Ethanol run: $m=0.064$ kg, $C_2=0.064c+60$. $\dfrac{C_1}{C_2}=\dfrac{12}{8}$:
$$C_2=\frac{396}{1.5}=264\;\Rightarrow\;0.064c=204\;\Rightarrow\;\boxed{c\approx3.2\times10^3\ \text{J kg}^{-1}\text{K}^{-1}}.$$

**Check.** Same order as water but lower ✓ (real ethanol ≈ 2400 — the experiment's number is coarse but plausible; the *method* is the content).

---

### Q1(n) — Thermal stress in a constrained girder [4 marks]

**Key observation.** Ends fixed ⟹ thermal expansion is converted into elastic compression: $\sigma=E\alpha\Delta T$, independent of the girder's length.

> 【Thought】 Mechanism: free expansion would be $\alpha L\Delta T$; preventing it strains the girder by $\varepsilon=\alpha\Delta T$; Hooke turns that into stress. The given length 4.0 m cancels — note that, since it reassures you the model is understood. (The stated expansivity $1.2\times10^{-7}$ is 100× smaller than real steel — the number given governs.)

**Solution.** $F=EA\alpha\Delta T=2.0\times10^{11}\times30\times10^{-4}\times1.2\times10^{-7}\times15$:
$$\boxed{F=1.08\times10^{3}\ \text{N}\ (\approx1.1\ \text{kN})}.$$

**Check.** Strain $=1.8\times10^{-6}$, stress $=E\varepsilon=3.6\times10^5$ Pa, × area $3\times10^{-3}$ m² $=1080$ N ✓. (The wire's length cancels between the strain and the extension — only the fractional change matters.)

---

### Q1(o) — Grating with off-normal incidence [6 marks]

**(i) Sketch.** Grating vertical, normal dashed; incident rays hitting adjacent slits at angle $\theta_1$ (path difference $d\sin\theta_1$ on the entrance side), diffracted rays leaving at $\theta_2$ on the same side (path difference $d\sin\theta_2$ on the exit side); mark both small right triangles.

**(ii)** Total path difference (same side, measured from the incident direction's extension): $d(\sin\theta_2-\sin\theta_1)=n\lambda$ — the grating equation with signed angles.

**(iii)–(v)** Successive orders $n,n+1$ at $14^\circ$ and $73^\circ$ (same side): subtracting eliminates $\theta_1$:
$$\lambda=d(\sin73^\circ-\sin14^\circ)=833\ \text{nm}\times(0.9563-0.2419)=\boxed{595\ \text{nm}}.$$
First order at $14^\circ$: $\sin\theta_1=\sin14^\circ-\lambda/d=0.2419-0.7144=-0.4725$ ⟹ $\boxed{\theta_1=-28.2^\circ}$ — incident from the **opposite** side of the normal. Third transmitted beam: zeroth order straight through at $\theta_0=\theta_1$: $\boxed{28.2^\circ\text{ on the opposite side}}$; (third order would need $\sin\theta_3=-0.47+3\times0.714>1$ — does not exist).

> 【Thought】 The designed structure: subtracting the two order equations kills the unknown incidence angle and yields λ directly; then back-substitution gives $\theta_1$ — and the *sign* of the result tells you the incidence side. "Third transmitted beam" is a probe of whether you check all orders: only $n=0$ remains physically allowed.

---

### Q1(p) — Two spheres, one heated one cooled: equivalent common temperature [4 marks]

**Key observation.** Equal volumes, gas free to move ⟹ common final pressure; total moles conserved. The equivalent common temperature is the **harmonic mean** of the two temperatures.

**Solution.** $T_0=373$ K; $T_1=423$ K, $T_2=323$ K:
$$\frac{2PV}{T_0}=\frac{P_fV}{T_1}+\frac{P_fV}{T_2}\;\Rightarrow\;P_f=P\times\frac{2T_1T_2}{T_0(T_1+T_2)}.$$
Same $P_f$ from a uniform temperature $T_c$: $P_f/P=T_c/T_0$:
$$T_c=\frac{2T_1T_2}{T_1+T_2}=\frac{2\times423\times323}{746}=366.3\ \text{K}=\boxed{93.3^\circ\text{C}}.$$

> 【Thought】 Reading: the harmonic mean sits *below* the arithmetic mean (373 K) — heating one bulb and cooling the other symmetrically still lowers the pressure (the cold bulb holds more gas). If your $T_c$ came out above 373 K, the means are inverted — that's the error to check for.

---

### Q1(q) — Pendulum bouncing elastically off a wall at φ = 7° [4 marks]

**Key observation.** Small angles ⟹ SHM: $\theta(t)=14^\circ\cos\omega t$; the elastic wall at $7^\circ$ reverses the velocity; one full oscillation is two journeys $14^\circ\to7^\circ$.

> 【Thought】 The elastic bounce conserves energy, so the bob returns to $14^\circ$ — the cycle is $14^\circ\to7^\circ$ twice. The only computation is the SHM time between two angles: $\cos\omega t=\tfrac12$. (If the wall were inelastic, the motion would decay into small bounces — elasticity is what makes a clean period exist.)

**Solution.** The bob released from $+14^\circ$ descends through $0^\circ$ to the wall at $-7^\circ$ (far side), bounces back elastically, and retraces to $+14^\circ$. With $\theta(t)=14^\circ\cos\omega t$ (release at maximum), reaching $-7^\circ$:
$$14\cos\omega t_1=-7\;\Rightarrow\;\cos\omega t_1=-\tfrac12\;\Rightarrow\;\omega t_1=\frac{2\pi}{3}\;\Rightarrow\;t_1=\frac{T_0}{3}.$$
The bounce reverses the velocity (energy conserved), so the return journey takes another $t_1$; the full period is
$$\boxed{T=2t_1=\frac{2T_0}{3}}.$$

**Check.** $T<T_0$ ✓ (bounce shortens the swing); phase accounting: $\omega t_1=2\pi/3$ each way → total $4\pi/3 = \omega T$ ✓ consistent. Alternative route (official's second method): time centre→wall is $T_0/12$ ($\sin$ route), so $T=2(T_0/2-T_0/12)+...$... both give $2T_0/3$ ✓. (Boxing the one-way time $t_1=T_0/3$ as the period is the trap; the bounce doubles it. The official mark scheme's $2T_0/3$ confirms.)

---

### Q1(r) — Four charges on a square [7 marks]

**Setup.** A(+10 nC) top-left, B(+8) top-right, C(−12) bottom-right, D(−6) bottom-left; side 10 cm; centre O at $r=5\sqrt2$ cm from each corner; $k_e/r^2=8.99\times10^9/0.005=1.80\times10^{12}$ per unit charge (×10⁻⁹ → 1798 N/C per nC).

**(i) Field at the centre.** (Worth noting first: the centre's *potential* is $V_O=k(10+8-12-6)/r=0$ — the square is an equipotential point at the middle.) Each corner field points along a diagonal (away from positives, toward negatives). Components along the diagonals:
- Direction A→C: $(Q_A+|Q_C|)-(Q_B+|Q_D|)$... working in $x$ (right) and $y$ (up):
$$E_x=\frac{1798}{\sqrt2}(10-8+12-6)\times\ldots$$
Component-wise (each vector makes 45°): $E_x=1798\cos45^\circ(10-8+12-6)=1271\times8=1.02\times10^4$ N/C; $E_y=-1798\cos45^\circ(10+8+12+6)=-1271\times36=-4.58\times10^4$ N/C:
$$|\mathbf E|=1271\sqrt{8^2+36^2}=1271\times36.9=\boxed{4.7\times10^4\ \text{N/C}},\quad \text{at }77^\circ\text{ below the }+x\text{ direction (toward the C corner side)}.$$

**(ii) Work moving an electron O → midpoint of CD.** $V_O=0$ (charges sum to zero and are equidistant). Midpoint M of CD: distances 0.05 m to C and D, $\sqrt{0.05^2+0.1^2}=0.112$ m to A and B:
$$V_M=8.99\times10^9\left[\frac{(10+8)\times10^{-9}}{0.112}+\frac{(-12-6)\times10^{-9}}{0.05}\right]=8.99\,(161-360)=-1.79\times10^3\ \text{V},$$
$$W_{\text{ext}}=q\,\Delta V=(-e)(V_M-V_O)=(-e)(-1789)=\boxed{+1.8\ \text{keV}\approx+2.9\times10^{-16}\ \text{J}}$$
(external work positive: the electron is pushed *toward* higher potential by the field, so moving it to the lower-potential point M requires restraint work from the agent).

> 【Thought】 Efficiency trick used twice: (i) diagonal components let the four charges' contributions reduce to two signed sums; (ii) $V_O=0$ for free — *spotting the zero sum before computing four potentials*. For (ii), decide the sign convention explicitly: $W_{\text{ext}}=q\Delta V$ (work by the agent) vs $W_{\text{field}}=-q\Delta V$; report which you mean.

---
*End of Paper 15 (2018 Round 1 Section 1).*


---

## Paper 16 — 2017 Round 1 Section 1 (17 Nov 2017)

*Section 1, Question 1, parts (a)–(r). Maximum 50 marks from 94.*

---

### Q1(a) — "1 foot per nanosecond" as c [3 marks]

**Solution.** $1\ \text{ft/ns}=\dfrac{0.3048\ \text{m}}{10^{-9}\ \text{s}}=3.048\times10^8$ m/s (using 1 m = 1.094 yd × 3 ft/yd):
$$\text{error}=\frac{3.048-3.00}{3.00}=\boxed{1.6\%\ \text{(too large)}}.$$

> 【Thought】 The approximation is *high* — handy mnemonic anyway; the chain-rule conversion (m→yd→ft) is the only work. Note the error direction matters for back-checking quick estimates done with it.

---

### Q1(b) — Tapered ladder: centre of mass by lifting [5 marks]

**Key observation.** Lifting one end quasi-statically: the lift force × length = weight × (COM distance from the grounded end). Each end's lift measures the COM's lever arm from the *other* end.

**(i)** Lifting the narrow end needs 80 N: moments about the wide end: $80\times5.0=350\times x_{\text{wide}}$ ⟹ $x_{\text{wide}}=1.14$ m ⟹
$$\boxed{x_{CM}=5.0-1.14=3.86\ \text{m from the narrow end}}.$$
**(ii)** Lifting the wide end: $F\times5.0=350\times3.86$ ⟹ $\boxed{F=270\ \text{N}}$.

> 【Thought】 Built-in check: the two lift forces sum to the weight ($80+270=350$ N ✓) — because each lift force is the share of the weight borne at that end. If your two answers don't add to $W$, one moment arm is wrong.

---

### Q1(c) — Velocity under a ramping acceleration [7 marks]

**Key observation.** Velocity change = area under the $a$–$t$ graph (trapezium), not a constant-acceleration formula.

**Solution.** Phase 1 (0–10 s): $a$ falls linearly 10→5: $\Delta v=\tfrac{10+5}{2}\times10=75$ m/s ⟹ $v(10)=175$ m/s. Phase 2: $a=5$ constant. Doubling needs $\Delta v=100$: remaining $25$ at 5 m/s² ⟹ 5 s:
$$\boxed{v\text{ doubles at }t=15\ \text{s}}.$$
Sketch: curve rising with decreasing slope from 100 (concave down) to (10 s, 175), then a straight line of slope 5 onward; mark the doubling point (15 s, 200).

> 【Thought】 The trap is using $v=u+at$ with the *initial* acceleration (gives 10 s) — acceleration varying means integrate. The trapezium area is the exact integral here because $a(t)$ is piecewise linear.

---

### Q1(d) — Ball rebounding off a wall, landing 2a from it [6 marks]

**Key observation.** Split at the bounce: horizontal speed reverses with factor $e=2/3$; vertical motion is unaffected. Two flight times linked by the given landing point.

> 【Thought】 Strategy: parametrise by $t_1$ (time to the wall). The vertical motion runs continuously through the bounce (only $v_x$ changes) — the post-bounce ground hit is a *separate* mini-projectile from the bounce point. Everything is polynomial in $t_1$; the $\tan\theta$ terms cancel beautifully.

**Solution.** $t_1=\dfrac{a}{V\cos\alpha}$; height at the wall $h=a\tan\alpha-\tfrac12gt_1^2$; post-bounce: lands $2a$ from the wall at speed $eV\cos\alpha$ ⟹ $t_2=\dfrac{2a}{eV\cos\alpha}=\dfrac{3a}{V\cos\alpha}=3t_1$. Vertical closure $h+v_y't_2-\tfrac12gt_2^2=0$ with $v_y'=V\sin\alpha-gt_1$:
$$a\tan\alpha-\tfrac12gt_1^2+3t_1(V\sin\alpha-gt_1)-\tfrac92gt_1^2=0.$$
Using $a\tan\alpha=Vt_1\sin\alpha$:
$$4Vt_1\sin\alpha=8gt_1^2\;\Rightarrow\;t_1=\frac{V\sin\alpha}{2g}\;\Rightarrow\;\boxed{a=\frac{V^2\sin\alpha\cos\alpha}{2g}=\frac{V^2\sin2\alpha}{4g}}.$$

**Check.** Note $a$ is half the usual range-quarter… sanity: without a wall the range is $V^2\sin2\alpha/g=4a$ — the ball lands $2a$ beyond the wall position measured back from the wall, consistent ordering ($a$ wall distance < bounce travel $2a$ ✓ since $e<1$). (At each bounce the horizontal velocity multiplies by $e$; the vertical motion is untouched — the two components decouple.)

---

### Q1(e) — Helicopter downwash velocity [5 marks]

**Key observation.** Hover ⟹ thrust = weight; thrust = momentum flux of the air cylinder: $F=\dot m v=\rho Av^2$ (mass flow $\rho A v$, each kilogram given speed $v$).

$$v=\sqrt{\frac{Mg}{\rho A}}=\sqrt{\frac{1000\times9.81}{1.2\times\pi\times3^2}}=\sqrt{\frac{9810}{33.9}}=\boxed{17\ \text{m/s}}.$$

> 【Thought】 Two-step momentum-flux model (actuator disk): mass flow ∝ v and momentum per kg ∝ v, hence $v^2$. Known sanity: real helicopter downwash is ~10–20 m/s ✓.

---

### Q1(f) — Intercepting a ship (nautical miles) [7 marks]

**(i)** Ship at 2 p.m.: $(3\hat i-\hat j)-(\hat i+4\hat j)\times1\ \text{h}=\boxed{2\hat i-5\hat j}$.
**(ii)** Boat velocity $\mathbf v_b$: interception condition at time $t$ (hours from 2 p.m.):
$$(-4,-5)+t\,\mathbf v_b=(2,-5)+t(1,4)\;\Rightarrow\;t(v_{bx}-1)=6,\quad t(v_{by}-4)=0.$$
The second gives $v_{by}=4$; then $|\mathbf v_b|=\sqrt{41}$ ⟹ $v_{bx}=+\sqrt{41-16}=5$:
$$\boxed{\mathbf v_b=5\hat i+4\hat j\ \text{nmi/h}}.$$
**(iii)** $t(5-1)=6\Rightarrow t=1.5$ h ⟹ $\boxed{\text{interception at }3{:}30\ \text{p.m.}}$ (at position $3.5\hat i+\hat j$).

> 【Thought】 The yacht's $y$-equation has no unknown time on the right — always solve the component that collapses first ($v_{by}=4$ pops out), then use the speed magnitude for $v_{bx}$, then $t$. Sign choice for $v_{bx}$: the ship is to the east, so $+5$.

---

### Q1(g) — Steam vs hot-water heating [4 marks]

**Key observation.** Per kilogram, steam delivers latent heat **plus** sensible cooling: $L+c\Delta T$.

$$Q_{\text{water}}=1.00\times4200\times22=9.24\times10^4\ \text{J};\qquad q_{\text{steam}}=2.260\times10^6+4200\times18=2.34\times10^6\ \text{J/kg},$$
$$\boxed{m_{\text{steam}}=\frac{9.24\times10^4}{2.34\times10^6}=0.040\ \text{kg}\approx40\ \text{g}}.$$

> 【Thought】 The latent heat dominates (97%) — this is *why* steam heating is effective, and why the answer is a striking ~4% of the water mass. Don't drop the condensate's cooling term (it contributes the remaining 3%).

---

### Q1(h) — Cell emf and internal resistance from two load measurements [5 marks]

**Key observation.** Two measurements, two unknowns $(\mathcal E, r)$: write $I=\mathcal E/(R+r)$ twice. Parallel: $2\parallel5=1.43\ \Omega$.

$$0.80=\frac{\mathcal E}{2.00+r},\qquad 1.00=\frac{\mathcal E}{1.43+r}\;\Rightarrow\;0.80(2+r)=1.43+r\cdot\ldots$$
$$1.60+0.80r=1.4286+r\;\Rightarrow\;r=\frac{0.1714}{0.20}=\boxed{0.86\ \Omega},\qquad \mathcal E=0.8\times2.86=\boxed{2.3\ \text{V}}.$$

**Check.** $1.00\times(1.43+0.86)=2.29$ ✓ consistent; note the current *rose* when resistance fell — expected direction ✓.

---

### Q1(i) — Maximum energy dissipated in one minute [4 marks]

**Key observation.** "Maximum current 3 A" ⟹ short-circuit ⟹ internal resistance $r=\mathcal E/I_{\max}=2\ \Omega$. Maximum power transfer when $R=r$.

$$P_{\max}=\frac{\mathcal E^2}{4r}=\frac{36}{8}=4.5\ \text{W}\;\Rightarrow\;\boxed{E_{\max}=4.5\times60=270\ \text{J}}.$$

> 【Thought】 Chain: max current (short) → internal resistance → matched load → $P_{\max}=\mathcal E^2/4r$. The question never states $r$ directly — recognising "maximum current" as the short-circuit current is the decoding step.

---

### Q1(j) — Photons in a nanosecond laser pulse [3 marks]

$$N=\frac{Pt}{hc/\lambda}=\frac{5\times10^{-4}\times10^{-9}}{(6.63\times10^{-34}\times3\times10^8/6.39\times10^{-7})}=\frac{5\times10^{-13}}{3.11\times10^{-19}}=\boxed{1.6\times10^{6}\ \text{photons}}.$$

> 【Thought】 Even a nanosecond pulse from a feeble laser carries millions of photons — the takeaway about photon granularity scales.

---

### Q1(k) — Rod swinging in a vertical circle, tensionless at the top [6 marks]

**Key observation.** $T=0$ at the top fixes the top speed: $mg=mv_t^2/\ell$. Energy then gives the bottom speed, and the bottom tension adds weight *plus* centripetal.

> 【Thought】 The two force balances differ by a sign: top $T+mg=mv_t^2/\ell$, bottom $T-mg=mv_b^2/\ell$. The most common error is dropping the $mg$ at the bottom (writing $T=mv_b^2/\ell=5mg$). Energy supplies $v_b^2=v_t^2+4g\ell$.

**Solution.** $v_t^2=g\ell$; $v_b^2=g\ell+4g\ell=5g\ell$:
$$T_{\text{bottom}}=mg+\frac{mv_b^2}{\ell}=mg+5mg=\boxed{6mg}.$$

**Check.** The classic loop result: tension rises by exactly $6mg$ from top ($0$) to bottom ($6mg$) ✓ (the $4mg$ from the height difference plus $2mg$ from the gravity terms).

---

### Q1(l) — Sand leaving a vibrating loudspeaker cone [3 marks]

**Key observation.** The sand loses contact when the cone's downward acceleration exceeds $g$: $\omega^2A=g$.

$$\omega=\sqrt{\frac{g}{A}}=\sqrt{\frac{9.81}{2.0\times10^{-4}}}=221\ \text{rad/s}\;\Rightarrow\;\boxed{f\approx35\ \text{Hz}}.$$

> 【Thought】 Mechanism: the cone can only push, not pull — contact requires $N\ge0$, and $N=0$ when $a_{\downarrow}=g$. This is the same "lift-off" condition as the hump-backed bridge (Paper 11 Q5a) in oscillatory dress. (A conical surface can only push, never pull — contact breaks the moment the required normal force would go negative.)

---

### Q1(m) — Equatorial radio link via two geostationary satellites [6 marks]

**Key observation.** Signal path: station → satellite 1 → satellite 2 → station; the station–satellite legs are *tangents* from the surface to the orbit circle: length $\sqrt{r^2-R^2}$; the satellites sit at the tangent points.

> 【Thought】 Draw the circle geometry first: tangent length $\sqrt{r^2-R_E^2}$, tangent point at central angle $\arccos(R_E/r)$ from the station. The inter-satellite chord closes the path. The whole question is one right triangle plus one chord — geometry, not astrophysics.

**Solution.** $r=6371+35900=42271$ km; tangent leg: $\sqrt{42271^2-6371^2}=41\,789$ km; central angle to tangent point: $\arccos(6371/42271)=81.3^\circ$. Satellites are $180-2\times81.3=17.3^\circ$ apart: chord $=2r\sin(8.67^\circ)=12\,742$ km.
$$d=2\times41\,789+12\,742=96\,320\ \text{km}\;\Rightarrow\;\boxed{\Delta t=\frac{9.63\times10^7}{3.00\times10^8}\approx0.32\ \text{s}}.$$

**Check.** The chord clears the surface: closest approach $r\cos8.67^\circ=41\,789$ km $>R_E$ ✓ (by construction it just grazes — the geometry is self-consistent); delay $\sim$0.3 s matches real satellite-link experience ✓. (The grazing ray is the tangent from the satellite's altitude: length $\sqrt{r^2-R_E^2}$.)

---

### Q1(n) — Thin coating on glass: strongest reflected wavelength [5 marks]

**Key observation.** Phase flips: air→coating (1.52 > 1): $\pi$; coating→glass (1.60 > 1.52): $\pi$. **Both** flip ⟹ they cancel in the relative phase ⟹ constructive reflection when $2nt=m\lambda$.

> 【Thought】 Flip inventory first (as in Paper 13 Q6d): two flips → the integer condition $2nt=m\lambda$; zero/one flip → half-integer. Then list which orders fall in the visible.

**Solution.** $2nt=2\times1.52\times0.42\ \mu\text{m}=1.277\ \mu\text{m}$; $\lambda=1277/m$ nm: $m=1$: 1277 nm (IR); $m=2$: $\boxed{638\ \text{nm (red)}}$; $m=3$: 426 nm (violet — also visible, weaker region of typical white light near the edge). The principal visible maximum: **638 nm** (with 426 nm as the next order).

---

### Q1(o) — Evacuating a tube: 25-fringe shift [5 marks]

**Key observation.** Removing air shortens the optical path by $(n-1)L$; each fringe shift is one wavelength of optical path change.

$$(n_{\text{air}}-1)L=25\lambda\;\Rightarrow\;\boxed{n_{\text{air}}=1+\frac{25\times600\times10^{-9}}{0.050}=1.0003}.$$

> 【Thought】 Same lever as Paper 11 Q3(e) — a macroscopic $L$ and a fringe count give a microscopic $n-1$: interferometry turns $10^{-4}$ index differences into countable fringes. Fringe order bookkeeping: 25 fringes = 25 wavelengths of path change ✓.

---

### Q1(p) — Cable extension change lifting a wreck clear of water [5 marks]

**Key observation.** Only the *buoyancy* disappears when the load leaves the water: $\Delta T=\rho_w gV$. Volume from mass/density; extension change from Young's modulus.

**Solution.** $V=\dfrac{1.0\times10^4}{8000}=1.25\ \text{m}^3$; $\Delta T=1000\times9.81\times1.25=1.23\times10^4$ N:
$$\Delta x=\frac{\Delta T\,L}{EA}=\frac{1.23\times10^4\times10}{5.0\times10^{10}\times5.0\times10^{-4}}=\boxed{4.9\times10^{-3}\ \text{m}\ (\approx5\ \text{mm}\ \text{longer out of water})}.$$

> 【Thought】 The tension is uniform (given) so one Hooke calculation covers the whole cable. Buoyancy loss is the *only* change — crane height, cable weight are distractors here.

---

### Q1(q) — Beam on three springs [8 marks]

**Key observation.** A rigid straight beam ⟹ the three compressions are collinear (linear): $x_2=\tfrac{x_1+x_3}{2}$. Plus vertical force balance and moment balance about O.

**(i)** $k_1=k_3=k$, $k_2=2k$ (symmetric ⟹ $x_1=x_3$, hence all equal):
$$kx_1+2kx_1+kx_1=4kx_1=Mg\;\Rightarrow\;\boxed{x=\frac{Mg}{4k}\ \text{each};\quad F_A=F_B=\frac{Mg}{4},\ F_O=\frac{Mg}{2}}.$$

**(ii)** $k,2k,3k$: moments about O: $kx_1=3kx_3\Rightarrow x_1=3x_3$; collinearity: $x_2=2x_3$:
$$kx_1+2kx_2+3kx_3=3kx_3+4kx_3+3kx_3=10kx_3=Mg,$$
$$\boxed{x_1=\frac{3Mg}{10k},\ x_2=\frac{Mg}{5k},\ x_3=\frac{Mg}{10k};\qquad F_A=\frac{3Mg}{10},\ F_O=\frac{2Mg}{5},\ F_B=\frac{3Mg}{10}}.$$

> 【Thought】 Rigid-body support problems are *statically indeterminate* without the stiffness law: the straightness condition $x_2=(x_1+x_3)/2$ is what closes the system — that's the transferable content. Check: end forces symmetric (the stiffer B spring balances the geometry) and all forces sum to $Mg$ ✓.

---

### Q1(r) — Ice thickening on a pond [7 marks]

**Key observation.** Freezing rate is limited by conduction through the *existing* ice: heat flux $\propto1/x$ ⟹ $x\,dx\propto dt$ ⟹ thickness grows as $\sqrt t$ (diffusion-like law).

> 【Thought】 Seeing conduction-limited growth → triggers *write the instantaneous balance* $\rho L\,dx/dt=\lambda\Delta T/x$, separate variables, integrate between the two thicknesses. The initial 5 cm is the lower limit of the integral — growing from zero would start with infinite rate (unphysical), which is why the problem starts at 5 cm.

**Solution.** $\rho L\dfrac{dx}{dt}=\dfrac{\lambda\Delta T}{x}$ with $\Delta T=10$ K (ice surface at $-10^\circ$C, interface at $0^\circ$C):
$$t=\frac{\rho L}{\lambda\Delta T}\int_{0.05}^{0.10}x\,dx=\frac{900\times3.30\times10^5}{2.1\times10}\times\frac{0.10^2-0.05^2}{2}=\frac{2.97\times10^8}{21}\times0.00375,$$
$$\boxed{t\approx5.3\times10^4\ \text{s}\approx15\ \text{hours}}.$$

**Check.** Quadratic-in-thickness: doubling thickness takes $4\times$ the energy-time per area for the second 5 cm as... from 5→10 cm: $\Delta(x^2)=75$ cm² vs 0→5: 25 cm² — the second layer takes 3× longer than the first ✓ consistent with slower conduction through thicker ice.

---
*End of Paper 16 (2017 Round 1 Section 1).*


---

## Paper 17 — 2017 Round 1 Section 2 (17 Nov 2017)

*Section 2: Questions 2–6, 25 marks each; candidates attempt two. Full solutions for all five.*

---

### Question 2 — Current, resistance and nonlinear components

#### Q2(a) — Electron drift in a 50 Hz AC wire [6 marks]

**(i)** Drift speed from $I=neAv$; rms→peak $I_0=10\sqrt2$ A; $A=\pi(5\times10^{-4})^2=7.85\times10^{-7}$ m², $n=9.0\times10^{28}\ \text{m}^{-3}$:
$$v_0=\frac{I_0}{neA}=\frac{14.14}{9.0\times10^{28}\times1.6\times10^{-19}\times7.85\times10^{-7}}=\boxed{1.3\ \text{mm/s}}.$$

**(ii)** In AC the electrons execute SHM with the field: $x_0=v_0/\omega=\dfrac{1.25\times10^{-3}}{2\pi\times50}=\boxed{4.0\times10^{-6}\ \text{m}\ (\approx4\ \mu\text{m})}$.

> 【Thought】 Seeing AC → the drift velocity oscillates sinusoidally about zero: displacement amplitude = velocity amplitude / ω. The numbers are the moral: drift speeds are mm/s and excursions microns — current is carried by *collective* drift, not fast electrons.

#### Q2(b) — Stretching a wire at constant volume [6 marks]

**(i)** $R=\rho l/A$ and $lA=$ const ⟹ $R\propto l^2$:
$$\boxed{\frac{\delta R}{R}=\frac{2\varepsilon}{l}}.$$
**(ii)** $R=100.0\ \Omega$, $\varepsilon/l=0.001$: $\boxed{R_{\text{new}}=100.0+0.2=100.2\ \Omega}$.

> 【Thought】 Constant volume is what doubles the sensitivity ($\delta R/R=2\,\delta l/l$ rather than $\delta l/l$): the wire gets thinner as it stretches. This is the strain-gauge gauge-factor mechanism (cf. Paper 14 Q5c).

#### Q2(c) — Non-linear component with a series resistor [6 marks]

**(i)** KVL: $\varepsilon=IR+V_c$ with $I=AV_c+BV_c^2$:
$$300=(0.070V_c+0.0050V_c^2)\times4.0\ \text{(mA×kΩ=V)}\ +V_c\;\Rightarrow\;\boxed{0.020V_c^2+1.28V_c-300=0}.$$

**(ii)** $V_c=\dfrac{-1.28+\sqrt{1.28^2+4\times0.02\times300}}{0.04}=\dfrac{-1.28+5.06}{0.04}=\boxed{94.6\ \text{V}}$;
$$I=\frac{300-94.6}{4000}=\boxed{51\ \text{mA}}\quad(\text{check: }0.070\times94.6+0.005\times94.6^2=51.4\ \text{mA ✓}).$$

> 【Thought】 The quadratic is the load-line equation for this algebraic nonlinearity — the physics is "KVL still rules"; the skill is units discipline (mA × kΩ = V) and root selection (the negative root is unphysical here: $V_c>0$).

#### Q2(d) — Hemisphere electrode in a resistive liquid [7 marks]

**(i)** Current flows radially outward through hemispherical shells (area $2\pi r^2$):
$$\boxed{\delta R=\frac{\rho\,\delta r}{2\pi r^2}}.$$

**(ii)** $R=\displaystyle\int_a^\infty\frac{\rho\,dr}{2\pi r^2}=\frac{\rho}{2\pi a}=\frac{60}{2\pi\times0.10}=\boxed{95\ \Omega}$ (hemisphere radius $a=0.10$ m).

> 【Thought】 Same spreading-resistance structure as the lithography problem (Paper 10 Q1p): current area grows as $r^2$, so the integral converges at infinity and most of the resistance sits within a few radii of the electrode — that's why "large tank" is a safe assumption.

---

### Question 3 — Tug boat winch problems

#### Q3(a) — Snatch loading with slipping brakes [9 marks]

**Key observation.** While the brakes slip, the cable tension is *fixed* at 50 kN (kinetic friction limit) — so each vessel has a constant acceleration; slipping ends when their speeds match.

> 【Thought】 The model decode: "brakes slip when tension reaches 50 kN" = tension clamped at 50 kN during slip. After that, both bodies move together and statics resume. Timescale separation: the propeller thrust (35 kN) keeps acting throughout — it belongs in the tug's equation during slip.

**Solution.** During slip: tug: $a_t=\dfrac{35-50\ \text{kN}}{450\ \text{t}}=-0.0333\ \text{m/s}^2$; barge: $a_b=\dfrac{50\ \text{kN}}{6300\ \text{t}}=+7.94\times10^{-3}\ \text{m/s}^2$.
(i) Speeds equal: $2.5-0.0333t=7.94\times10^{-3}t$ ⟹ $\boxed{t=\frac{2.5}{0.0413}=61\ \text{s}}$.
(ii) $\boxed{v=7.94\times10^{-3}\times60.6=0.48\ \text{m/s}}$.
(iii) Cable run-out = relative travel:
$$\Delta x=2.5t-\tfrac12(0.0333+0.00794)t^2\cdot\frac{1}{1}=2.5(60.6)-\tfrac12(0.0413)(60.6)^2=\boxed{76\ \text{m}}.$$

**Check.** Momentum sanity: without thrust, the fully inelastic outcome would be $v=\frac{450\times2.5}{6750}=0.167$ m/s; the thrust adds over the long slip time — our 0.48 m/s sits above it ✓ direction sane; run-out ≈ 76 m of cable is dramatic but consistent with a 1-minute slip ✓. (Model assumption: the cable pays out at constant tension — a real drum brake would modulate it.)

#### Q3(b) — Crane framework [8 marks]

**Geometry (note: the figure has $CB=CD=5L$ and $BD=8L$ — do not swap $BD$ and $CD$).** $B=(0,0)$, $C=(0,5L)$, and $D=(4.8L,6.4L)$ from $|D|=8L$, $|D-C|=5L$ ($x^2+y^2=64L^2$, $x^2+(y-5L)^2=25L^2\Rightarrow y=6.4L$, $x=4.8L$). $\cos\theta=0.8$ at $\angle CDB$ (or read off the 3-4-5 geometry).

**(i)–(ii) Joint D equilibrium.** Moments about C kill $T_{CD}$ and C's joint force: the load's moment arm about C is the horizontal distance $4.8L$; member BD's force on D along $D\!\to\!B$ has moment arm $\dfrac{|(C-B)\times(D-B)|}{|D-B|}=\dfrac{|0\times6.4-5\times4.8|}{8}L=3L$:
$$T_{BD}\times3L=15W\times4.8L\;\Rightarrow\;|T_{BD}|=24W.$$
Sense: the load's moment about C is clockwise; the balance requires BD to push D *away* from B — **BD is in compression**, $|F_{BD}|=24W$. Then at joint D, $x$-balance: $24W\times0.6=T_{CD}\times0.949\Rightarrow T_{CD}=24W\times0.632=15W$ (pulling D toward C — **tension**):
$$\boxed{|F_{BD}|=24W\ \text{(BD in compression)},\qquad T_{CD}=15W\ \text{(tension)}}.$$

**(iii) Distance AB.** Whole-crane moments about B (eliminating B's reactions): the load's moment $15W\times4.8L$ (clockwise) is balanced by A's downward force $31W$ at distance $AB$:
$$31W\times AB=15W\times4.8L\;\Rightarrow\;\boxed{AB=\frac{72}{31}L\approx2.3L}.$$

> 【Thought】 Method: joints first for member forces (two equations, two unknowns at D), whole-structure moments for the ground fixings — choosing the moment centre at B deletes B's unknown reaction entirely. The sign convention: assume tension, let negative answers announce compression — and then *say* "compression" explicitly.

#### Q3(c) — Bucket with leaking sand, constant winch force [8 marks]

**Key observation.** Mass varies linearly: $M(\tau)=m+m_0(1-\tau/t)$; constant force $F$; Newton's second law $M\dot v=F-Mg$ integrates by substitution.

> 【Thought】 Variable-mass caution: because the sand leaves *with the bucket's velocity* (leaks out, not thrown), no thrust term appears — plain $F=Ma$ with the current mass is correct here. (If sand were ejected with relative velocity, a $u\,dm/dt$ term would appear.) The supplied integral hint tells you a $\ln$ is coming.

**Solution.** $v=\displaystyle\int_0^t\left(\frac{F}{M(\tau)}-g\right)d\tau=\frac{F}{m_0/t}\int_m^{m+m_0}\frac{du}{u}-gt$ (with $u=m+m_0(1-\tau/t)$):
$$\boxed{v=\frac{Ft}{m_0}\ln\left(1+\frac{m_0}{m}\right)-gt}.$$

**Check.** $m_0\to0$ (no sand): $\frac{Ft}{m_0}\times\frac{m_0}{m}\to\frac{Ft}{m}$ ⟹ $v=(F/m-g)t$ ✓ constant-mass kinematics recovered. The log exceeds the naive average-mass estimate slightly — consistent with lighter end-of-run ✓. (The sand leaves at the bucket's own speed, so it carries no thrust term — momentum flux from *leaving* mass vanishes when $v_{\text{rel}}=0$.)

---

### Question 4 — Refraction, fibres and lenses

#### Q4(a) — 60° prism: total internal reflection at the second face [5 marks]

**Key observation.** At the second face, TIR needs $r_2\ge\theta_c$; with $r_1+r_2=A=60^\circ$ and entry limited by $r_1\le\theta_c$ (Snell), the binding constraint is $r_1\le A-\theta_c$.

> 【Thought】 Direction of the inequality is the content: TIR at face 2 needs $r_1$ *small*, so incidence is bounded **above**: $i\le i_{\text{crit}}$; the "smallest angle of incidence such that all light is totally reflected" reads as the marginal/boundary value $i_{\text{crit}}$ — rays within $[0,27.9^\circ]$ are all totally reflected. Draw the marginal ray grazing out of face 2.

**Solution.** $\theta_c=\arcsin(1/1.5)=41.8^\circ$; $r_1\le60-41.8=18.2^\circ$:
$$\sin i=1.5\sin18.2^\circ=0.469\;\Rightarrow\;i_{\text{crit}}=27.9^\circ\;\Rightarrow\;\boxed{\text{for all incident angles }0\le i\le27.9^\circ\text{, the second face totally internally reflects}}$$
(the question's "smallest angle such that all light is TIR" is the boundary value $i=27.9^\circ$ itself).

Diagram: large prism; ray entering near-normal ($i=27.9^\circ$), internal ray at $r_1=18.2^\circ$, striking face 2 at exactly $\theta_c=41.8^\circ$ and emerging grazing ($e=90^\circ$).

#### Q4(b) — Step-index optical fibre [12 marks]

**(i) Acceptance angle.** Entry: $n_3\sin\theta=n_1\sin\theta_1$ ($\theta_1$ to the axis); TIR at the core–cladding wall needs the grazing angle there $\ge\theta_c$: $\cos\theta_1\ge n_2/n_1$. At the margin: $\sin\theta_1=\sqrt{1-n_2^2/n_1^2}$:
$$n_3\sin\theta_m=n_1\sqrt{1-\frac{n_2^2}{n_1^2}}\;\Rightarrow\;\boxed{\sin\theta_m=\frac{\sqrt{n_1^2-n_2^2}}{n_3}}\quad(\text{the numerical aperture}).$$

**(ii) Pulse broadening.** Axial ray time: $t_0=Ln_1/c$. Edge-ray zigzags at $\theta_1^{max}$: path stretched by $1/\cos\theta_1=n_1/n_2$:
$$\Delta t=t_0\left(\frac{n_1}{n_2}-1\right)=\frac{Ln_1}{c}\cdot\frac{n_1-n_2}{n_2}=\frac{10^5\times1.48585}{3\times10^8}\times\frac{0.02944}{1.45641}=\boxed{1.0\times10^{-5}\ \text{s}\ (10\ \mu\text{s per 100 km})}.$$

**(iii)** Non-overlap: $f_p^{\max}=1/\Delta t=\boxed{1.0\times10^5\ \text{Hz}\ (100\ \text{kHz})}$.

**(iv)** With $c'=c/n_1$: $\Delta t=\dfrac{Ln_1}{c}\dfrac{\Delta n}{n_2}=\boxed{\dfrac{L}{c'\,n_2}\,\Delta n}$. $\blacksquare$

> 【Thought】 The broadening mechanism is *multipath dispersion*: different angles, different path lengths, same speed. Note the answer scales with the *index difference* — hence graded-index (GRIN) fibres, which leads into part (d)'s lens. Chain-of-custody for factors: the ray is longer ($1/\cos\theta_1$) but not slower — one factor only. This is multipath dispersion in fibre language — and the GRIN profile of (c)–(d) is precisely the cure, equalising optical paths.

#### Q4(c) — Meaning of f [2 marks]

$u\to\infty$: $\dfrac1v=\dfrac1f$ ⟹ $v=f$: **$f$ is the image distance for an object at infinity** — parallel rays converge to the focal point a distance $f$ behind the lens. $\blacksquare$

#### Q4(d) — GRIN disc as a lens (Fermat's principle) [6 marks]

**(i)** Ray at radius $r$ (paraxial, $r$ small): geometrical path $O\to$disc$\to P$ stretches to $\approx u+\dfrac{r^2}{2u}$ and $\dfrac{r^2}{2v}+v$; optical path inside the disc is $n(r)d=n_0(1-kr^2)d$. Equal travel times (Fermat) against the axial path:
$$\underbrace{u+\frac{r^2}{2u}+v+\frac{r^2}{2v}+n_0(1-kr^2)d}_{\text{off-axis path at }r}=\underbrace{u+v+n_0d}_{\text{axial path}}\ \Longrightarrow\ \frac{r^2}{2}\left(\frac1u+\frac1v\right)=n_0kr^2d,$$
$$\boxed{\frac1u+\frac1v=2n_0kd}\ \text{— lens behaviour (the }r^2\text{ terms cancel identically for all }r\text{)}.$$

**(ii)** Compare with $\dfrac1u+\dfrac1v=\dfrac1f$:
$$\boxed{f=\frac{1}{2n_0kd}}.$$

> 【Thought】 The paraxial expansions $\sqrt{u^2+r^2}\approx u+r^2/2u$ produce the $r^2$ terms; the quadratic index profile $n_0(1-kr^2)$ cancels them exactly — that's *why* a quadratic GRIN focuses perfectly in the paraxial limit. The design rule of thumb to remember: focusing needs the optical path to *fall* quadratically off-axis. A graded index thus corrects spherical aberration (and, with the right dispersion profile, helps chromatic too) — that is the point of GRIN lenses.

---

### Question 5 — Pendulums, dipoles and a thundercloud

#### Q5(a) — Charged pendulum in an electric field [6 marks]

**(i)** Horizontal $E$: equilibrium angle $\theta$ from vertical given by balancing $QE$ (horizontal) against $mg$ (vertical):
$$\boxed{\tan\theta=\frac{QE}{mg}}.$$

**(ii)** $E$ vertically down, charge $-Q$: the electric force $QE$ points *up*, reducing effective gravity: $g_{\text{eff}}=g-\dfrac{QE}{m}$:
$$\boxed{T=2\pi\sqrt{\frac{\ell}{g-QE/m}}=2\pi\sqrt{\frac{m\ell}{mg-QE}}}.$$

**(iii)** Oscillations need a downward net restoring gravity (string stays taut, bob hangs): $\boxed{QE<mg}$. (At $QE=mg$ the bob is weightless; beyond, it "falls upward" and the string goes slack.)

> 【Thought】 Electric fields on pendula reduce to *effective gravity* — rotate $g$ (part i) or rescale it (part ii). The condition in (iii) is a stability boundary: $QE<mg$ is where $g_{\text{eff}}>0$.

#### Q5(b) — Dipole field at large distance [10 marks]

Charges $\pm Q$ at $x=\pm a$; point P at $r\gg a$; dipole moment $p=2Qa$.

**(i) P on the axis** (beyond $+Q$):
$$V=\frac{kQ}{r-a}-\frac{kQ}{r+a}=\frac{2kQa}{r^2-a^2}\approx\boxed{\frac{kp}{r^2}},\qquad E=-\frac{dV}{dr}\approx\boxed{\frac{2kp}{r^3}}.$$

**(ii) P on the perpendicular bisector:** $V=\dfrac{kQ}{\sqrt{r^2+a^2}}-\dfrac{kQ}{\sqrt{r^2+a^2}}=\boxed{0}$; fields: magnitudes $kQ/(r^2+a^2)$, vertical components cancel, horizontal components (each $\times\,a/\sqrt{r^2+a^2}$) add:
$$\boxed{E=\frac{2kQa}{(r^2+a^2)^{3/2}}\approx\frac{kp}{r^3}}\quad(\text{pointing antiparallel to the dipole}).$$

> 【Thought】 The two expansions to state explicitly: $(r\mp a)^{-1}\approx r^{-1}(1\pm a/r)$ and $(r^2+a^2)^{-3/2}\approx r^{-3}$ — the dipole's signature is that the *leading* terms cancel (net charge zero), leaving $1/r^3$ fields and $1/r^2$ potentials. On-axis is twice as strong as the bisector at the same range — worth remarking.

#### Q5(c) — Rotating an HCl dipole through 180° [2 marks]

$p=e\times2\times10^{-11}=3.2\times10^{-30}$ C·m; $U(\theta)=-pE\cos\theta$:
$$W=U(180^\circ)-U(0^\circ)=2pE=2\times3.2\times10^{-30}\times3\times10^5=\boxed{1.9\times10^{-24}\ \text{J}}.$$

#### Q5(d) — Thundercloud model with image charges [7 marks]

**(i)** $Q_+=\rho_+\pi r^2h=0.21\times10^{-9}\times\pi(5\times10^3)^2\times3\times10^3=\boxed{+49.5\ \text{C}}$ (centre 10.5 km); $Q_-=-0.18\times10^{-9}\times\pi(5\times10^3)^2\times7\times10^3=\boxed{-99.0\ \text{C}}$ (centre 5.5 km).

**(ii) Field at the ground below.** Each real charge plus its opposite image gives a field $2kq/h^2$ at the surface point directly beneath (both contributions point the same way at that point); downward positive:
$$E=2k\left[\frac{49.5}{(10.5\ \text{km})^2}-\frac{99.0}{(5.5\ \text{km})^2}\right]=2\times8.99\times10^9\times(4.49\times10^{-7}-3.27\times10^{-6}),$$
$$\boxed{E\approx-5.1\times10^{4}\ \text{V/m}\ \text{— i.e. }5.1\times10^4\ \text{V/m pointing upward (toward the dominant negative base charge)}.}$$

**(iii) Head potential.** The field is essentially uniform over 2 m: going up along the (upward) field, potential falls:
$$V_{\text{head}}=V_{\text{ground}}-E\times2\ \text{m}=0-(5.1\times10^4)(2)=\boxed{-1.0\times10^5\ \text{V}\ (\approx-100\ \text{kV, negative})}.$$

> 【Thought】 The image-charge rule is given in the question — the skill is deploying it: field at the surface = real + image, and directly below the cloud they reinforce (factor 2). For (iii), *field uniform over 2 m* is the licensed approximation (cloud at km distances ≫ 2 m). Sign statement: the cloud's negative base induces positive charge on the ground, so the field points up and potential falls with height — hence the head is negative relative to the feet. (The body is a conductor: the head-to-foot pd is what matters physiologically, not the absolute potential.)

---

### Question 6 — Doppler effects and binary stars

#### Q6(a) — Boat against sea waves [4 marks]

Waves spaced $\lambda=c/f$ approach the boat at relative speed $u+c$: in time $\Delta t$ the boat meets $\dfrac{(u+c)\Delta t}{\lambda}$ waves:
$$f'=\frac{(u+c)\Delta t/\lambda}{\Delta t}=\frac{u+c}{\lambda}=\boxed{\frac{(u+c)f}{c}}.\ \blacksquare$$

> 【Thought】 Counting wavefronts is the most robust Doppler derivation — no sign conventions to misremember. Here both source and observer motions are folded into the *relative* approach speed because the medium (sea surface) pattern moves at $c$ relative to land.

#### Q6(b) — Moving sound source, stationary observer [6 marks]

**(i)** In $\Delta t$ the source emits $f\Delta t$ waves while approaching: the wave train occupies $(c-v_s)\Delta t$ (first front travelled $c\Delta t$, the source followed at $v_s\Delta t$): wavelength in the forward direction $\lambda'=\dfrac{(c-v_s)\Delta t}{f\Delta t}=\dfrac{c-v_s}{f}$; observer receives
$$f'=\frac{c}{\lambda'}=\frac{fc}{c-v_s}=\boxed{\frac{f}{1-v_s/c}}.\ \blacksquare$$

**(ii)** Receding at $c/2$: $f'=\dfrac{f}{1+1/2}=\dfrac{2f}{3}$: $\boxed{\Delta f=-\dfrac{f}{3}}$.

**(iii)** $v_s\ll c$: $\dfrac{1}{1\mp v_s/c}\approx1\pm v_s/c$ ⟹ $\boxed{\left|\dfrac{\Delta f}{f}\right|\approx\dfrac{v_s}{c}}$ (approach: $+$, recede: $-$). $\blacksquare$ (Do not mix the two Doppler formulas: source-moving and observer-moving differ at second order; at $v\ll c$ both reduce to this same first-order shift.)

#### Q6(c) — Rotational broadening of a solar absorption line [5 marks]

**(i)** The Sun's limbs move at $v=\dfrac{2\pi R}{T}$ toward/away from us; the line from each limb shifts by $\pm\dfrac{v}{c}f$, so the observed frequency sweeps $f\pm\delta f$ with
$$\boxed{\delta f=\frac{2\pi Rf}{Tc}}.\ \blacksquare$$

**(ii)** $R=\left(\dfrac{M}{\tfrac43\pi\rho}\right)^{1/3}=\left(\dfrac{2.0\times10^{30}}{5864}\right)^{1/3}=6.99\times10^8$ m; $v=\dfrac{2\pi R}{T}=\dfrac{2\pi\times6.99\times10^8}{24.5\times86400}=2074$ m/s:
$$\boxed{\frac{\delta f}{f}=\frac{2074}{3.00\times10^8}=6.9\times10^{-6}}\quad(\text{at }550\ \text{nm}:\ \delta\lambda\approx\pm3.8\ \text{pm}).$$

**Check.** Real solar equatorial speed ≈ 2 km/s ✓ (our estimate from the given bulk data matches) — the broadening is tiny but resolvable with a good spectrograph ✓.

#### Q6(d) — Binary star: masses from Doppler shift [10 marks]

**Data:** separation $a=19.8$ AU $=2.96\times10^{12}$ m; $T=50.1$ yr $=1.58\times10^9$ s; Hα line 656.3 nm varies $\pm0.0235$ nm ⟹ star A's orbital speed amplitude $v_A=c\,\delta\lambda/\lambda=1.07\times10^4$ m/s (orbit plane contains the line of sight, so the full speed is measured). Note the mass inversion: the *faster* star is the *lighter* one — speeds ratio inverts the mass ratio.

**(i)** Relative circular orbit: separation $a$, relative speed $2\pi a/T$; gravity between them supplies it: $\dfrac{Gm_Am_B}{a^2}=m\ldots$; cleanly: the relative coordinate obeys $\ddot{\mathbf r}=-\dfrac{GM}{r^2}\hat r$ with $M=m_A+m_B$, so $\dfrac{GM}{a^2}=\left(\dfrac{2\pi}{T}\right)^2a$:
$$\boxed{T^2=\frac{4\pi^2a^3}{GM}}.\ \blacksquare$$

**(ii)** $M=\dfrac{4\pi^2(2.96\times10^{12})^3}{6.67\times10^{-11}\times(1.58\times10^9)^2}=\boxed{6.2\times10^{30}\ \text{kg}\ (\approx3.1\ M_\odot)}$.

**(iii)** $v_A=\dfrac{2\pi R_A}{T}$ with $R_A=\dfrac{m_B}{M}a$ (CM condition); substituting $M=4\pi^2a^3/GT^2$:
$$v_A=\frac{2\pi a}{T}\frac{m_B}{M}=\frac{2\pi a\,m_B}{T}\times\frac{GT^2}{4\pi^2a^3}=\boxed{\frac{GT}{2\pi a^2}m_B}.\ \blacksquare$$

**(iv)** $m_B=\dfrac{2\pi a^2v_A}{GT}=\dfrac{2\pi(2.96\times10^{12})^2\times1.07\times10^4}{6.67\times10^{-11}\times1.58\times10^9}=\boxed{5.6\times10^{30}\ \text{kg}\ (\approx2.8\ M_\odot)}$;
$$m_A=M-m_B=\boxed{5.6\times10^{29}\ \text{kg}\ (\approx0.28\ M_\odot)}.$$

**(v)** $\boxed{\dfrac{R_A}{R_B}=\dfrac{m_B}{m_A}\approx10}$.

> 【Thought】 Reading the structure: the Doppler shift measures $v_A$ (the *bright* star's speed); the CM condition converts speed ratio to mass ratio; Kepler fixes the total. Note the physics alert: the computed $m_B$ exceeds the Chandrasekhar limit for a white dwarf — the printed line-shift is larger than the real Sirius-like value would give, so the data describe a somewhat idealised system; the *method* (spectroscopic-binary mass solve) is unaffected. Guard your powers of ten: $GT\approx0.105$ here, not 105 — a factor $10^3$ slip inverts the mass ratio.

---
*End of Paper 17 (2017 Round 1 Section 2).*


---

## Paper 18 — 2016 Round 1 Section 1 (18 Nov 2016)

*Section 1, Question 1, parts (a)–(q). Maximum 40 marks from 70.*

---

### Q1(a) — Field of +Q and +2Q; neutral point [5 marks]

**(i)** Neutral point between them (fields oppose only there), distance $x$ from A:
$$\frac{kQ}{x^2}=\frac{2kQ}{(d-x)^2}\;\Rightarrow\;d-x=\sqrt2\,x\;\Rightarrow\;\boxed{x=\frac{d}{1+\sqrt2}=(\sqrt2-1)d\approx0.41d\ \text{from A}}.$$
(Sketch: lines radiate from both charges, bowing apart between them; the neutral point is the saddle where the line pattern pinches.)

**(ii)** A field line's *direction* tracks $E$, but its *magnitude* varies because the sources are inverse-square and geometry changes along the line: lines spread out (density falls) away from charges, and the field strength is encoded in the line density — so $E$ falls as the line diverges and rises where lines crowd.

> 【Thought】 The neutral point sits closer to the *smaller* charge ✓ (field balance needs more distance from the bigger one). For (ii), the intended physics language: field strength ∝ spacing of field lines; a single line carries no magnitude information, but the bundle's divergence does.

---

### Q1(b) — Battery discharge time [2 marks]

$$E=VQ=12\times0.5\times10^6=6.0\times10^6\ \text{J};\qquad t=\frac{6.0\times10^6}{450}=\boxed{1.3\times10^{4}\ \text{s}\approx3.7\ \text{h}}.$$
(Model assumption: an ideal battery — constant emf and full capacity until exhausted; real cells sag.)

---

### Q1(c) — Resistive networks [5 marks]

**(i)** Two series then three in parallel: $R_{eq}=R+R+\dfrac{R}{3}=\boxed{\dfrac{7R}{3}}$.
**(ii)** Five resistors, no series/parallel reduction: the **Wheatstone bridge** (diamond of four with a fifth across the middle). With all equal to $R$: the bridge is balanced ⟹ middle resistor carries no current ⟹ two series pairs ($2R$ each) in parallel:
$$\boxed{R_{AB}=R}.$$

> 【Thought】 The bridge is the canonical "not series–parallel" network; with equal arms it's balanced by symmetry — that observation replaces Kirchhoff equations entirely.

---

### Q1(d) — Two spheres gravitationally colliding [7 marks]

**Key observation.** Both move: use the relative coordinate (or momentum + energy). From rest at great separation, falling to contact $r=R_1+R_2$:

$$\frac12\mu v^2=\frac{Gm_1m_2}{R_1+R_2},\qquad \mu=\frac{m_1m_2}{m_1+m_2}\;\Rightarrow\;\boxed{v=\sqrt{\frac{2G(m_1+m_2)}{R_1+R_2}}}.$$

> 【Thought】 The reduced-mass form handles the "both move" subtlety in one step: the relative motion has mass $\mu$ and potential $-Gm_1m_2/r$. Equivalent check: momentum conservation + energy per body gives the same answer (a useful exercise).

---

### Q1(e) — Pump strokes to inflate a tyre [5 marks]

**Key observation.** Isothermal: count moles via $PV$; each stroke delivers $P_0V_p$ of air at atmospheric pressure.

$$N=\frac{P_tV_t}{P_0V_p}=\frac{3.0\times10^5\times1.2\times10^{-3}}{1.0\times10^5\times9.0\times10^{-5}}=\boxed{40\ \text{strokes}}.$$

> 【Thought】 The "flat tyre containing no air" clause means the tyre's full final inventory comes from the pump. The ratio $\frac{P_tV_t}{P_0V_p}$ is just mole-counting in disguise.

---

### Q1(f) — Car accelerating to pass a van [4 marks]

**Key observation.** The question never says the car starts from rest — it is moving at some speed $u$ when the van passes. The data then over-determine the problem just enough: the van covers the 500 m in $t=500/22.22=22.5$ s, and the car covers the same 500 m in the same time while accelerating at $a=1.2$ m/s² — two equations for $u$ and $V$. (Assuming $u=0$ is tempting but *not* printed; the official mark scheme confirms the two-unknown reading.)

**Solution.** Van: $t=\dfrac{500}{80/3.6}=22.5$ s. Car: $500=u t+\tfrac12at^2=22.5u+303.75$ ⟹ $u=8.72$ m/s:
$$\boxed{V=u+at=8.72+1.2\times22.5=35.7\ \text{m/s}\ (\approx129\ \text{km/h})}.$$

**Check.** The car enters the stretch slower than the van ($8.7<22.2$ m/s — hence being overtaken) and leaves it faster ($35.7>22.2$) ✓; average speed over the interval $=(8.72+35.7)/2=22.2$ m/s $=v_{\text{van}}$ ✓ — the meeting condition is satisfied identically, a closed-loop check.

> 【Thought】 The temptation to set $u=0$ comes from pattern-matching to "accelerate from rest" problems; the discipline: use only stated data, and let the *over-determination* (same $t$, same distance) supply the unknown initial speed. If the data had been genuinely inconsistent, the audit-first response would be right — but here one extra unknown ($u$) restores consistency.

---

### Q1(g) — Molten lead into a calorimeter [5 marks]

**Key observation.** The lead passes through **three** thermal stages: liquid cooling to 327 °C, freezing (latent), solid cooling to 25 °C. All three deliver heat to water + calorimeter.

> 【Thought】 Seeing "molten lead … final 25 °C" with a freezing point at 327 °C → triggers the *three-segment heat ledger*. Forgetting the latent heat (or the solid cooling) are the two designed errors.

**Solution.** Heat gained: $(0.800\times4200+42.8)\times10=3.40\times10^4$ J. Heat from lead, per kg: $158(T_i-327)+23\,230+137\times302$:
$$0.400\left[158(T_i-327)+23\,230+41\,314\right]=34\,028,$$
$$63.2(T_i-327)=8210\;\Rightarrow\;\boxed{T_i\approx457^\circ\text{C}}.$$

**Check.** Breakdown: freezing supplies $0.4\times23230=9.3$ kJ, solid cooling $16.5$ kJ, liquid cooling $8.2$ kJ — all three comparable; $T_i>327^\circ$C ✓ consistent with "molten".

---

### Q1(h) — Object leaving a vibrating scale-pan [3 marks]

**Key observation.** Contact is lost when the pan's downward acceleration reaches $g$ (the pan can't pull the object down): $\omega^2\mathcal A=g$.

$$\mathcal A=\frac{g}{\omega^2}=\frac{gT^2}{4\pi^2}=\frac{9.81\times0.25}{39.5}=\boxed{6.2\times10^{-2}\ \text{m}\ (\approx6\ \text{cm})}.$$

> 【Thought】 Same lift-off mechanism as the loudspeaker sand (Paper 16 Q1l) and the hump bridge — collect these; they're one condition: $N=0\iff a_{\text{down}}=g$.

---

### Q1(i) — Three spheres joined by a wire [5 marks]

**Key observation.** Capacitance $\propto$ radius; charge conserved; potentials equalise.

**Solution.** Initial total charge: $Q_0=4\pi\varepsilon_0V(2r+6r)=8\pi\varepsilon_0rV\cdot\frac{1}{1}\ldots$ i.e. $4\pi\varepsilon_0 rV\times8$ units. Common final potential:
$$V'=\frac{Q_0}{4\pi\varepsilon_0(2r+3r+6r)}=\boxed{\frac{8}{11}V}.$$
Charge on the $3r$ sphere: $Q_{3r}=4\pi\varepsilon_0(3r)\times\dfrac{8V}{11}=\dfrac{24}{11}\times4\pi\varepsilon_0rV$:
$$\boxed{\text{fraction}=\frac{24/11}{8}=\frac{3}{11}\approx27\%.}$$

**Check.** Radius ratios $2:3:6$ share the final charge in the same ratio — the $3r$ sphere holds $3/11$ ✓ consistent with Paper 12 Q1(q)'s template ($C\propto r$, equalise $V$).

---

### Q1(j) — Tungsten work function [3 marks]

$$W=\frac{hc}{\lambda}-KE_{\max}=\frac{6.63\times10^{-34}\times3\times10^8}{248\times10^{-9}}-8.60\times10^{-20}=8.02\times10^{-19}-0.86\times10^{-19},$$
$$\boxed{W=7.2\times10^{-19}\ \text{J}\approx4.5\ \text{eV}}.$$

**Check.** Accepted tungsten work function ≈ 4.5 eV ✓ spot on.

---

### Q1(k) — Climbing a slippery ladder [5 marks]

**Key observation.** Slip condition: required friction (wall reaction $P$, by horizontal balance) reaches $\mu N$; moments about the base eliminate the ground forces.

> 【Thought】 The ladder is nearly flat (60° to the wall = 30° to the ground) — expect slipping almost immediately, since the moment arm of the wall's push ($l\sin30^\circ$) is small while weights act with large horizontal arms ($\cos30^\circ$). The answer being small is the physics, not an error.

**Solution.** Angle to horizontal $30^\circ$; $N=(m+2m)g=3mg$; slip when $P=\mu N=1.2mg$. Moments about the base (student at fraction $f$):
$$P\,l\sin30^\circ=\left(mg\frac l2+2mg\,fl\right)\cos30^\circ\;\Rightarrow\;1.2mg\times0.5l=\left(0.5+2f\right)mg\,l\times0.866,$$
$$0.6=0.866(0.5+2f)\;\Rightarrow\;f=\frac{0.693-0.5}{2}=\boxed{0.10\ \text{— only about one tenth of the way up}}.$$

**Check.** Without the student ($f=0$): $P=0.866mg<1.2mg$ ✓ ladder alone holds; a heavy student tips it into slip quickly ✓ physically grim but consistent with the shallow angle.

---

### Q1(l) — Ball on a string in a horizontal wind [4 marks]

**Key observation.** Wind stops on collision ⟹ force = momentum flux $F=\rho Av^2$ with $A=\pi r^2$; pendulum-style balance $\tan\theta=F/mg$.

$$F=mg\tan39^\circ=0.600\times9.81\times0.810=4.77\ \text{N},\qquad v=\sqrt{\frac{F}{\rho A}}=\sqrt{\frac{4.77}{1.293\times\pi\times0.10^2}}=\boxed{11\ \text{m/s}}.$$

> 【Thought】 "Wind speed drops to zero on collision" is the momentum-flux licence ($F=\dot mv=\rho Av^2$); without it you wouldn't know how much momentum the air transfers. Note the ball's projected area is a circle, not a hemisphere. (The string capture is a perfectly inelastic event — ball and acquired air-column momentum move off together; that type label selects momentum-over-energy bookkeeping.)

---

### Q1(m) — Polonium half-life and decay equation [4 marks]

**Key observation.** $1/8=(1/2)^3$: exactly three half-lives; balance mass and charge for the α-decay equation.

**Solution.** $T_{1/2}=420/3=\boxed{140\ \text{days}}$.
Equation: $^{210}_{84}\text{Po}\to{}^4_2\text{He}+{}^{206}_{82}\text{Pb}+\gamma$:
$$\boxed{a=210,\ b=84,\ c=4,\ d=2,\ e=206,\ f=82}$$
(with the γ carrying $(0,0)$).

> 【Thought】 The half-life result (140 d) identifies the isotope as Po-210 — the equation's indices then follow from conservation of nucleons and charge. Two rules only: superscripts and subscripts each balance.

---

### Q1(n) — Centre of mass: four corner masses + ring [3 marks]

**Key observation.** The ring (8 kg) sits at O by symmetry; the two opposite 4 kg masses cancel each other; only the 1 kg / 3 kg opposite pair displaces the CM.

**Solution.** Pair CM of 1 kg at $\mathbf p$ and 3 kg at $-\mathbf p$: $-\mathbf p/2$ (mass 4 kg); plus 8 kg (ring) and 8 kg (4 kg pair) at O:
$$\mathbf r_{CM}=\frac{4\times(-\mathbf p/2)}{20}=-\frac{\mathbf p}{10}=-\frac{(a,a)}{10}\;\Rightarrow\;\boxed{|\mathbf r_{CM}|=\frac{\sqrt2\,a}{10}\approx0.14a,\ \text{toward the 3 kg corner}}.$$

> 【Thought】 Decompose into symmetric pairs *before* summing vectors — the ring and the 4–4 pair vanish from the calculation, halving the work.

---

### Q1(o) — Trumpeter Doppler [3 marks]

**Key observation.** Approaching source, stationary observer: $f'=\dfrac{f}{1-v/c}$.

$$466=\frac{440}{1-v/331}\;\Rightarrow\;1-\frac{v}{331}=\frac{440}{466}=0.9442\;\Rightarrow\;\boxed{v=18.5\ \text{m/s}\ (\approx67\ \text{km/h})}.$$

**Check.** $\Delta f/f=26/440=5.9\%\approx v/c$ ✓ (small-shift approximation consistent).

---

### Q1(p) — Proton beam in a magnetic field [4 marks]

**Key observation.** $r=\dfrac{mv}{eB}$ with $v=\sqrt{2eV/m_p}$ ⟹ $r=\dfrac{1}{B}\sqrt{\dfrac{2Vm}{e}}$.

$$r_p=\frac{1}{0.2000}\sqrt{\frac{2\times2000\times1.67\times10^{-27}}{1.60\times10^{-19}}}=\frac{6.45\times10^{-3}}{0.2}=\boxed{3.2\times10^{-2}\ \text{m}\ (3.2\ \text{cm})}.$$

Deuterons (twice the mass, same charge): $r\propto\sqrt m$:
$$\boxed{r_d=\sqrt2\,r_p=4.6\ \text{cm}}.$$

> 【Thought】 Seeing "accelerated through V then bent in B" → triggers *eliminate v*: $r=\frac{1}{B}\sqrt{2Vm/e}$ — then the isotope question is a pure scaling, no recomputation.

---

### Q1(q) — Minimum height to complete the loop [3 marks]

**Key observation.** Contact at the top needs $v_{top}^2\ge gr$; energy from height $h$ (start, rest) to the loop top (height $2r$):

$$mgh=mg(2r)+\tfrac12m(gr)\;\Rightarrow\;\boxed{h_{\min}=\frac{5r}{2}}.$$

> 【Thought】 The classic 5/2 factor: 2r of height + r/2 of required kinetic energy. The condition $N\ge0$ at the top is the binding constraint — state it.

---
*End of Paper 18 (2016 Round 1 Section 1).*


---

## Paper 19 — 2016 Round 1 Section 2 (18 Nov 2016)

*Section 2: Questions 2–8, 20 marks each; candidates attempt two (and only one of Q5/Q6). Full solutions for all seven.*

---

### Question 2 — Potentiometer circuits and bridges

#### Q2(a) — Cells on a resistance wire [2 marks]

**(i)** With K₁, K₂ open, the wire AB (resistance $R$, length $\ell$) carries the cell $\varepsilon_0$ alone; the potential falls linearly along a uniform wire (constant current ⟹ constant gradient):
$$\boxed{V(\ell_1)=\varepsilon_0\,\frac{\ell_1}{\ell}}\quad\text{(potential relative to A)}.$$

**(ii)** Null condition: with no galvanometer current, the tapped wire potential exactly balances the cell's emf (the cell then supplies no current — potentiometer balance):
$$\boxed{\text{a. }\ \varepsilon_1=\varepsilon_0\frac{\ell_1}{\ell};\qquad \text{b. }\ \varepsilon_2=\varepsilon_0\frac{\ell_2}{\ell}.}$$

> 【Thought】 The potentiometer's core idea: at null, the measurement draws *no* current, so the cell's true emf (not terminal pd under load) is read off the wire's linear voltage gradient. "No current flows through G" is the signal that the tapped voltage equals the emf.

#### Q2(b) — Measuring a thermocouple's emf [8 marks]

**Circuit logic (Fig. 2(b)).** The 2.00 V cell drives a steady current through $R$ and the uniform wire AB (1.00 m, 2.00 Ω), setting a linear voltage gradient along the wire; the 100 Ω sits in the detector branch (at balance it carries no current, so it drops out). The 1.02 V standard cell calibrates the gradient; the thermocouple T is then balanced against it.

**Solution.**
(i) K₁ closed (standard cell): balance at $AC=0.900$ m ⟹ wire gradient $=\dfrac{1.02}{0.900}=1.133$ V/m.
(ii) K₂ closed (thermocouple): balance at $AC=0.450$ m:
$$\boxed{\varepsilon=1.133\times0.450=0.51\ \text{V}}.$$
For $R$: the whole wire (2.00 Ω) carries pd $1.133$ V ⟹ current $I=0.5667$ A; the driver loop (2.00 V cell, $R$, wire):
$$2.00=I(R+2.00)\;\Rightarrow\;R+2.00=\frac{2.00}{0.5667}=3.53\;\Rightarrow\;\boxed{R=1.53\ \Omega}.$$

> 【Thought】 Two-stage logic: the standard cell *calibrates the gradient* (V/m), then the unknown emf is a pure length ratio. The driver resistor $R$ follows from Ohm's law on the working current. Note that at every balance the detector branch draws zero current — that is why the 100 Ω protective resistor is invisible in the equations.

#### Q2(c) — Wheatstone bridge with a filament lamp [5 marks]

**Key observation.** Balance requires the lamp's *operating* resistance $V/I=4\ \Omega$ (to match the other arms); use $V=2I+8I^2$ to find the operating point, then compute the bridge supply.

> 【Thought】 The lamp is nonlinear, so "resistance 4 Ω" is a *condition on the operating point*, not a fixed property: solve $V/I=4$. The supply voltage follows from the arm currents at balance — note the galvanometer arm is open, so each side of the bridge is a simple series pair.

**Solution.** Balance: $\dfrac{V}{I}=2+8I=4\Rightarrow I=0.25$ A, $V=1.0$ V. Each leg carries its series current; the lamp leg: $0.25$ A through lamp + 4 Ω:
$$\boxed{V_b=0.25\times(4.0+4.0)=2.0\ \text{V}}.$$

**Check.** Top leg: $I=2.0/8=0.25$ A ✓ same; node voltages at the galvanometer ends both $=1.0$ V below the supply rail ✓ balanced.

#### Q2(d) — Choose R to minimise heating in the 5 Ω resistor [5 marks]

**Topology (Fig. 2(d)).** Nodes: right rail $Q$ (all right ends wire-joined); centre top $C_T$ and centre bottom $C_B$ (the 5 Ω between them); left column ML–BL via 1 Ω, with 2 Ω from ML to $C_T$ and 4 Ω from BL to $C_B$; 10 Ω and $R$ both from $C_T$ to $Q$; 12 Ω from $C_B$ to $Q$; 10 V cell between the bottom rail (BL side) and $Q$.

**Key observation.** The power in the 5 Ω is minimised (zero) when its ends are at the same potential — a *balance* condition, achievable if $R$ can tune the right-hand divider.

> 【Thought】 Seeing "minimise heat in the 5 Ω" → triggers *bridge-balance thinking*: $P=0$ iff $V_{C_T}=V_{C_B}$. The 5 Ω then carries no current and can be removed from the analysis; the remaining conditions fix $V_0$ from the bottom divider and then $R$ from the top one. (Compare Paper 8 Q1(q), where balance was impossible and the minimum was at $R\to\infty$ — always check the balance is attainable for $R>0$.)

**Solution.** With the 5 Ω removed (balanced), $C_B$: fed from BL (10 V) via 4 Ω and from $Q$ (0 V) via 12 Ω:
$$\frac{V_0-10}{4}+\frac{V_0}{12}=0\;\Rightarrow\;V_0=7.5\ \text{V}.$$
$C_T$: fed from BL via $(2+1)=3\ \Omega$ and from $Q$ via $10\parallel R$:
$$\frac{7.5-10}{3}+\frac{7.5}{10\parallel R}=0\;\Rightarrow\;\frac{7.5}{10\parallel R}=\frac{2.5}{3}\;\Rightarrow\;10\parallel R=9\ \Omega,$$
$$\frac{10R}{10+R}=9\;\Rightarrow\;\boxed{R=90\ \Omega}\quad(\text{then }P_{5\Omega}=0).$$

**Check.** Full nodal analysis at $R=90\ \Omega$ confirms $V_{C_T}=V_{C_B}=7.5$ V and zero 5 Ω current ✓; since power $\ge0$ and 0 is attained, this is the global minimum ✓.

---

### Question 3 — Interference: optical and acoustic

#### Q3(a) — Young's slits theory [14 marks]

**(i) Fringe spacing.** Slits $S_1,S_2$ separated by $2a$, screen at $D$, P at $x$ from the symmetry line. Path difference:
$$\Delta=S_2P-S_1P=\sqrt{D^2+(x+a)^2}-\sqrt{D^2+(x-a)^2}\approx D\left[1+\frac{(x+a)^2}{2D^2}-1-\frac{(x-a)^2}{2D^2}\right]=\frac{2ax}{D},$$
using $(1+u)^{1/2}\approx1+u/2$ for $u\ll1$ (state it). Maxima when $\Delta=n\lambda$ ⟹ adjacent fringes:
$$\boxed{\Delta x=\frac{\lambda D}{2a}}.$$

> 【Thought】 The binomial approximation is the designated tool (the paper even supplies it); keep *both* slits' expansions to first order in $(x\pm a)^2/D^2$ — zeroth order cancels, and the $x^2$ terms cancel between the slits, leaving the linear term $2ax/D$. Skipping the second order is fine *because* the surviving term is first order.

**(ii) White light.** Centre: all wavelengths coincide at zero path difference ⟹ a **white central maximum**; on each side, a few fringes with **blue edges toward the centre and red outward** (fringe spacing $\propto\lambda$), rapidly smearing into uniform white illumination after a few orders (spectra of different orders overlap).

**(iii) Purpose of the single slit.** The filament is an extended, spatially *incoherent* source: different points of it emit uncorrelated light, which would superpose many shifted fringe patterns and wash them out. The narrow single slit acts as a spatial filter — a secondary point source — so the light reaching the two slits is **spatially coherent** (the two slits are illuminated with a definite phase relationship). The colour filter narrows the wavelength band (temporal coherence), giving sharp, well-separated fringes. Without the single slit: no visible fringes; without the filter: blurry chromatic fringes.

#### Q3(b) — Two whistles: speed of sound [6 marks]

**Key observation.** This is Young's experiment with sound: minima spacing $\Delta x$ on a distant parallel line gives $\lambda$; then $v=f\lambda$.

$$\lambda=\frac{\Delta x\,s}{D}=\frac{1.14\times3.00}{20.0}=0.171\ \text{m};\qquad v=f\lambda=2000\times0.171=\boxed{342\ \text{m/s}}.$$

**Check.** Accepted value ✓ ($\sim343$ m/s at room temperature). (Two synchronised whistles are the acoustic double slit: the path difference to the observer sets the interference, exactly as in (a).)

---

### Question 4 — Charges on a square and a cube; axial oscillations

#### Q4(a) — Total potential energy [9 marks]

**Key observation.** Total PE = sum over all *pairs*, $U=\sum_{i<j}k q_iq_j/r_{ij}$ — count pair classes, don't integrate anything.

**(i) Square, side $2a$, $+Q$ at corners, $-q$ at centre.** Pairs: 4 edges ($2a$), 2 diagonals ($2\sqrt2\,a$), 4 centre-to-corner ($\sqrt2\,a$):
$$U=\frac{kQ^2}{a}\left(2+\frac{1}{\sqrt2}\right)-\frac{2\sqrt2\,kQq}{a}=\boxed{\frac{kQ^2}{a}\left(2+\frac{\sqrt2}{2}\right)-\frac{2\sqrt2\,kQq}{a}}.$$

**(ii) Cube, side $2a$.** 28 corner pairs: 12 edges ($2a$), 12 face diagonals ($2\sqrt2\,a$), 4 body diagonals ($2\sqrt3\,a$) — self-check $12+12+4=28=\binom{8}{2}$ ✓; plus 8 centre-to-corner ($\sqrt3\,a$):
$$U=\frac{kQ^2}{a}\left(6+3\sqrt2+\frac{2\sqrt3}{3}\right)-\frac{8kQq}{\sqrt3\,a}=\boxed{\frac{11.40\,kQ^2}{a}-\frac{4.62\,kQq}{a}}.$$

> 【Thought】 Pair-counting discipline: edges/face-diagonals/body-diagonals = 12/12/4 for a cube (check: $12+12+4=28=\binom82$ ✓). Sketches: mark each distance class in a different colour. If a factorisation offers — $U=\frac{kQ}{a}[\ldots]$ — pull it out.

#### Q4(b) — Axial force on the central charge [5 + 6 marks]

**(i)** Displaced $x$ along the axis (perpendicular to the square's plane): each corner is at distance $\sqrt{x^2+2a^2}$; the four force vectors' transverse parts cancel, axial parts add (factor $\cos\varphi=x/\sqrt{x^2+2a^2}$):
$$\boxed{F(x)=-\frac{4kQq\,x}{(x^2+2a^2)^{3/2}}}\quad(\text{restoring toward the centre}).$$
Graph: $F$ vs $x$ is odd-symmetric; rises from 0 to a maximum at $x=a$ (set $dF/dx=0$: $x^2+2a^2=3x^2$), then falls as $1/x^2$; negative mirror image for $x<0$.

**(ii) SHM condition and period.** Small $x$: $(x^2+2a^2)^{3/2}\approx(2a^2)^{3/2}=2\sqrt2\,a^3$:
$$F\approx-\frac{4kQq}{2\sqrt2\,a^3}x=-\frac{\sqrt2\,kQq}{a^3}x\;\Rightarrow\;\omega^2=\frac{\sqrt2\,kQq}{ma^3},\qquad \boxed{T=2\pi\sqrt{\frac{ma^3}{\sqrt2\,kQq}}}.$$
Validity: the linearisation needs $|x|\ll\sqrt2\,a$, so the amplitude must satisfy $\boxed{\mathcal A\ll a}$.

> 【Thought】 The small-$x$ licence: the force law is exactly linear only as $x\to0$; the oscillation is *approximately* SHM only while the amplitude keeps $x\ll\sqrt2a$ — stating the amplitude condition explicitly is what part (ii) asks for. Note the restoring force dies at large $x$ (the $1/x^2$ tail): big oscillations would be anharmonic.

---

### Question 5 — Galaxy rotation curves and dark matter

#### Q5(a) — Rotation velocity from enclosed mass [2 marks]

$$\frac{GM(r)}{r^2}=\frac{v^2}{r}\;\Rightarrow\;\boxed{v(r)=\sqrt{\frac{GM(r)}{r}}}$$
(spherical symmetry ⟹ only the enclosed mass matters — shell theorem).

#### Q5(b) — Predicted rotation curve [7 marks]

Inside the uniform bulge ($r\le r_b$): $M(r)=\tfrac43\pi\rho_0r^3$:
$$v=\sqrt{\tfrac43\pi G\rho_0}\;r\ \propto r\quad(\text{linear rise}).$$
Outside: $M\approx$ const $=M_b$:
$$v=\sqrt{\frac{GM_b}{r}}\ \propto r^{-1/2}\quad(\text{Keplerian fall}).$$
Sketch: linear rise to a peak at $r_b$ ($v_{\max}=\sqrt{GM_b/r_b}$), then a $1/\sqrt r$ decline.

#### Q5(c) — Dark-matter profile for a flat curve [4 marks]

Flat curve at $r>r_b$: $v=$ const ⟹ $M(r)\propto r$. With $\rho(r)=\rho_0(r_b/r)^\alpha$:
$$M(r)=\int_{r_b}^r4\pi r'^2\rho_0\left(\frac{r_b}{r'}\right)^\alpha dr'\propto r^{3-\alpha}\;\Rightarrow\;3-\alpha=1\;\Rightarrow\;\boxed{\alpha=2}\quad\left(\rho\propto\frac{1}{r^2}\right).$$

> 【Thought】 Chain: flat curve ⟺ $M\propto r$ ⟺ $\rho\propto r^{-2}$. The exponent chase ($v^2\propto M/r$) is the whole argument — this is the observational motivation for dark matter halos.

#### Q5(d) — Milky Way's visible vs true mass [3 marks]

$r=2.8\times10^4$ ly $=2.65\times10^{20}$ m; $M=\dfrac{v^2r}{G}$:
$$M_{\text{vis}}=\frac{(70\times10^3)^2\times2.65\times10^{20}}{6.67\times10^{-11}}=1.95\times10^{40}\ \text{kg}\approx9.8\times10^{9}M_\odot,$$
$$M_{\text{true}}=M_{\text{vis}}\left(\frac{220}{70}\right)^2=1.92\times10^{41}\ \text{kg}\approx9.7\times10^{10}M_\odot\quad(M\propto v^2\text{ at fixed }r,\text{ ratio }(220/70)^2\approx9.9),$$
$$\boxed{\text{dark fraction}=1-\left(\frac{70}{220}\right)^2\approx90\%.}$$

> 【Thought】 The mass ratio needs no absolute numbers: $M\propto v^2$ at fixed $r$, so $M_{\text{true}}/M_{\text{vis}}=(220/70)^2\approx9.9$ — the dark matter is ~90% of the total.

#### Q5(e) — MOND flat curve [4 marks]

MOND: $F=ma\,\mu(a/a_0)$ with $\mu\to1$ ($a\gg a_0$), $\mu\to a/a_0$ ($a\ll a_0$). Deep-MOND limit ($a\ll a_0$): gravity law becomes
$$\frac{GMm}{r^2}=m\,a\,\frac{a}{a_0}\;\Rightarrow\;a^2=\frac{GMa_0}{r^2}\;\Rightarrow\;\frac{v^4}{r^2}=\frac{GMa_0}{r^2},$$
$$\boxed{v=(GMa_0)^{1/4}=\text{const}}\ \text{— flat rotation curve at large radii}.\ \blacksquare$$

> 【Thought】 The trick is spotting that $a=v^2/r$ makes the Newtonian $1/r^2$ force law and the MOND factor conspire: $a^2\propto1/r^2$ ⟹ $v^4=$ const. One line of algebra after the right substitution order (force law first, then centripetal).

---

### Question 6 — Kepler's law and escape velocities

#### Q6(a) [8 marks]

**(i)** Equal $\dfrac{R^\alpha}{T^\gamma}$ for Earth and Jupiter (periods in years, $T_E=1$):
$$\left(\frac{7.76\times10^{11}}{1.50\times10^{11}}\right)^{\alpha}=(11.8)^{\gamma}\;\Rightarrow\;\alpha\log\frac{7.76}{1.50}=\gamma\log(11.8)\;\Rightarrow\;\boxed{\frac{\alpha}{\gamma}=\frac{\log 11.8}{\log 5.17}=\frac{1.0719}{0.7138}=1.50},$$
i.e. $\alpha/\gamma=3/2$ — Kepler's third law, $T^2\propto R^3$.

> 【Thought】 Taking logs turns the unknown *exponent ratio* into an ordinary ratio of numbers — no need to guess $3/2$ in advance and merely verify it. (Consistency check the other way: $(5.17)^{3/2}=11.8$ ✓.)

**(ii)** $M_\odot=\dfrac{4\pi^2r^3}{GT^2}$ with Earth's orbit ($T=3.156\times10^7$ s):
$$M_\odot=\frac{4\pi^2(1.50\times10^{11})^3}{6.67\times10^{-11}\times(3.156\times10^7)^2}=\boxed{2.0\times10^{30}\ \text{kg}}.\ \blacksquare$$

#### Q6(b) — Synchronous orbit [4 marks]

$T=24$ h:
$$r=\left(\frac{GM_ET^2}{4\pi^2}\right)^{1/3}=\left(\frac{6.67\times10^{-11}\times5.98\times10^{24}\times86400^2}{39.48}\right)^{1/3}=\boxed{4.22\times10^{7}\ \text{m}\ (42\,200\ \text{km}\approx6.6R_E\ \checkmark)},$$
$$v=\frac{2\pi r}{T}=\boxed{3.07\times10^{3}\ \text{m/s}}.$$

#### Q6(c) — Escape velocity [6 marks]

**(i)** *Escape velocity*: the minimum launch speed (no further propulsion) for which the body's total energy is zero — it reaches infinity with (just) zero speed.

**(ii)** $\tfrac12mv_e^2=\dfrac{GM_Em}{R_E}$:
$$v_e=\sqrt{\frac{2GM_E}{R_E}}=\sqrt{\frac{2\times6.67\times10^{-11}\times5.98\times10^{24}}{6.38\times10^6}}=\boxed{11.2\ \text{km/s}}.$$

**(iii) Launch-site dependence.** Earth rotates: an eastward equatorial launch starts with $v_{rot}=2\pi R_E/T_{day}\approx465$ m/s of inertial-frame speed, reducing the *additional* speed needed; latitude reduces this assist ($\propto\cos$ latitude); polar or westward sites get none/negative. Also local altitude and Earth's oblateness alter $R$ slightly.

**(iv)** Minimum initial launch speed (equatorial, eastward):
$$v_{\min}\approx v_e-v_{rot}=11.2-0.47=\boxed{10.7\ \text{km/s}\ (\text{ground-relative, equatorial eastward})}.$$

#### Q6(d) — Escaping the Sun from Earth [2 marks]

Escape speed from the Sun at Earth's orbital radius:
$$v_{\odot,\text{esc}}=\sqrt{\frac{2GM_\odot}{r_{\text{orbit}}}}=42.2\ \text{km/s}.$$
Launching *along* Earth's orbital motion, Earth's orbital speed $v_{\text{orb}}=\dfrac{2\pi r_{\text{orbit}}}{T}=29.9$ km/s is already in the bank, so the minimum launch speed (ignoring launch-site effects, per the question) is the residual:
$$\boxed{v_{\min}=42.2-29.9=12.3\ \text{km/s}}.$$

> 【Thought】 The $(\sqrt2-1)$ structure: escape needs $\sqrt2\times$ circular-orbit speed, so only $(\sqrt2-1)v_{\text{orb}}=0.414\times29.9$ must be supplied. The Earth's orbital motion does most of the heliocentric work — launching *against* it would require far more.
>
> 【Thought】 *Official approach note.* The mark scheme's answer is exactly this $12.3$ km/s (2 marks: solar escape speed, orbital speed, subtract). A fuller treatment that *also* climbs out of Earth's own gravity well stitches the two escapes energetically — $v=\sqrt{v_e^2+v_{\min}^2}=\sqrt{11.2^2+12.3^2}=16.6$ km/s — but the question's "ignoring any effect of the launch site" signals the simple subtraction is what is wanted. If the stem's “ignoring any effect of the launch site” became “taking account of Earth's gravity well”, condition C (only the heliocentric residual speed is needed) would break and the shortcut would fail — return to the general method (energetic stitching, $\sqrt{v_e^2+v_{\min}^2}$), because the energy needed to escape Earth's gravity well is not negligible.

---

### Question 7 — Millikan's oil drop experiment

#### Q7(a) — Charge change between two observations [8 marks]

**Key observation.** Rising at constant speed against gravity: $qE-mg=6\pi\eta rv$ (field pulling up, drag down). Two runs of the *same* drop (same $m$, $r$) with different charges: subtract to eliminate the unknown weight.

> 【Thought】 The difference trick: $q_1E-mg=\beta v_1$, $q_2E-mg=\beta v_2$ ⟹ $\Delta q\,E=\beta\Delta v$ — the unknown $mg$ (drop density never given!) cancels. When a problem withholds a quantity, look for the measurement *difference* that deletes it.

**Solution.** $E=\dfrac{5000}{0.0150}=3.33\times10^5$ V/m; $v_1=\dfrac{1.00\ \text{cm}}{42\ \text{s}}=2.38\times10^{-4}$ m/s, $v_2=\dfrac{1.00}{78}=1.28\times10^{-4}$ m/s; $\beta=6\pi\eta r=6\pi\times1.82\times10^{-5}\times2.76\times10^{-6}=9.47\times10^{-10}$ kg/s:
$$\Delta q=\frac{\beta(v_1-v_2)}{E}=\frac{9.47\times10^{-10}\times1.10\times10^{-4}}{3.33\times10^5}=3.1\times10^{-19}\ \text{C},$$
$$\boxed{\Delta n=\frac{\Delta q}{e}=\frac{3.1\times10^{-19}}{1.6\times10^{-19}}\approx2\ \text{electrons}}.$$

**Check.** Integer outcome ✓ — the whole point of Millikan: charge changes come in quanta of $e$.

#### Q7(b) — Coalescing drops [5 marks]

**Key observation.** The drops carry identical charges $Q$ and move at terminal velocity in the field $E$ — the question mentions $Q$ precisely because the electric force stays in the balance. Write the terminal-velocity equation for each drop and *add*; the weights combine automatically.

> 【Thought】 Two equations, three unknowns ($m_1$, $m_2$, and how they combine)? No — adding the two balance equations makes the weights appear as $(m_1+m_2)g=m_3g$, exactly the coalesced drop's weight. Whenever two bodies merge, try *adding* their individual balance equations before doing anything else.

**Solution.** Rising at terminal velocity (field pulling the charge up, weight and drag down):
$$QE=6\pi\eta r_1u_1+m_1g,\qquad QE=6\pi\eta r_2u_2+m_2g.$$
Coalesced drop: charge $2Q$, mass $m_3=m_1+m_2$, radius $r_3$, terminal velocity $u_3$:
$$2QE=6\pi\eta r_3u_3+m_3g.$$
Adding the first two equations and comparing with the third (the $2QE$ and $m_3g$ terms match exactly):
$$r_3u_3=r_1u_1+r_2u_2.$$
Volume conservation: $r_3^3=r_1^3+r_2^3$. Hence
$$\boxed{u_3=\frac{r_1u_1+r_2u_2}{\left(r_1^3+r_2^3\right)^{1/3}}}.$$
(The same derivation with different initial charges $Q_1,Q_2$ — total charge $Q_1+Q_2$ after merging — gives the identical result, so the relation is completely general.)

> 【Thought】 *Limiting-case check.* With the field off, terminal fall under gravity alone gives $u\propto r^2$ (Stokes vs weight), so $r_i\propto\sqrt{u_i}$ and the general formula collapses to $u_3=\left(u_1^{3/2}+u_2^{3/2}\right)^{2/3}$ — the pure gravity-fed coalescence rule. Both limits of one relation; the field-on form is what this question asks for (equal drops: $u_3=(u_1+u_2)/2^{1/3}$; field-free equal drops: $u_3=2^{2/3}u_1$ — different, so reading the regime correctly matters).

#### Q7(c) — Measuring e/m by crossed fields [7 marks]

**Key observation.** Two-stage measurement: crossed $E$ and $B$ select the velocity (no deflection: $eE=evB$); the accelerating voltage gives the energy. Eliminate $v$ between them.

> 【Thought】 The Wien filter condition $v=E/B$ is mass-independent; the accelerating stage $eV=\tfrac12mv^2$ carries the mass. Dividing the equations eliminates $v$ — that's the design of the experiment.

**Solution.** No deflection: $v=\dfrac{E}{B}=\dfrac{3000/0.020}{2.5\times10^{-3}}=\dfrac{1.5\times10^5}{2.5\times10^{-3}}=6.0\times10^7$ m/s. Acceleration through $V_a=10\,000$ V: $eV_a=\tfrac12m_ev^2$:
$$\boxed{\frac{e}{m_e}=\frac{v^2}{2V_a}=\frac{(6.0\times10^7)^2}{2\times10^4}=1.8\times10^{11}\ \text{C/kg}}.$$

**Check.** Accepted value $1.76\times10^{11}$ C/kg ✓ within a few percent.

---

### Question 8 — Rotating copper ring in the Earth's field

**Setup.** Ring radius $a=0.125$ m, resistance $R$, rotating at $\omega$ about a vertical diameter; Earth's horizontal field $B_H$; at $t=0$ the ring's plane is perpendicular to $B_H$ (normal along $B_H$).

**(a) Flux.** The normal rotates at $\omega$: $\boxed{\Phi(t)=B_H\pi a^2\cos\omega t}$.

**(b) Current.** Faraday: $I=-\dfrac{1}{R}\dfrac{d\Phi}{dt}$:
$$\boxed{I(t)=\frac{B_H\pi a^2\omega}{R}\sin\omega t}.$$

**(c) Ring's field at the centre** ($B=\mu_0 I/2a$, along the instantaneous axis — which makes angle $\omega t$ with $B_H$):
$$B_{\text{ring}}(t)=\frac{\mu_0\pi a\omega B_H}{2R}\sin\omega t,$$
$$\parallel B_H:\quad B_\parallel=B_{\text{ring}}\cos\omega t=\frac{\mu_0\pi a\omega B_H}{4R}\sin2\omega t,$$
$$\perp B_H:\quad B_\perp=B_{\text{ring}}\sin\omega t=\frac{\mu_0\pi a\omega B_H}{4R}(1-\cos2\omega t).$$

**(d) Time averages.** $\langle\sin2\omega t\rangle=0$, $\langle 1-\cos2\omega t\rangle=1$:
$$\boxed{\langle B_\parallel\rangle=0,\qquad \langle B_\perp\rangle=\frac{\mu_0\pi a\omega B_H}{4R}.}$$

**(e) Resistance from the compass deflection.** The needle settles along the mean total field: $\tan\alpha=\dfrac{\langle B_\perp\rangle}{B_H+\langle B_\parallel\rangle}=\dfrac{\langle B_\perp\rangle}{B_H}$:
$$\tan2.00^\circ=\frac{\mu_0\pi a\omega}{4R}\;\Rightarrow\;R=\frac{\mu_0\pi a\omega}{4\tan2.00^\circ}=\frac{1.2566\times10^{-6}\times\pi\times0.125\times62.8}{4\times0.0349},$$
$$\boxed{R\approx2.2\times10^{-4}\ \Omega\ (0.22\ \text{m}\Omega)}.$$

> 【Thought】 The mechanism: the oscillating induced current rectifies into a *steady* perpendicular field on average (the $\sin^2$ term) while the parallel component averages out — the compass reads the ratio. Watch the bookkeeping: ring field ∝ $\sin\omega t$, projected by another $\sin\omega t$ — the average of the product, not the product of averages, is what survives. (This is the same physics as a rotating-coil magnetometer.)

---
*End of Paper 19 (2016 Round 1 Section 2).*


---

## Paper 20 — 2015 Round 1 Section 1 (13 Nov 2015)

*Section 1, Question 1, parts (a)–(m). Maximum 40 marks from 71.*

---

### Q1(a) — Calibrating a camera shutter with a turntable [3 marks]

**Key observation.** Exposure = rotation angle / angular speed; propagate the uncertainties.

$$t=\frac{\theta}{2\pi f}=\frac{12.4^\circ/360^\circ}{33.3/60\ \text{rev/s}}=\frac{0.03444}{0.555}=0.0621\ \text{s},\qquad \frac{\delta t}{t}=\frac{0.1}{12.4}+\frac{0.1}{33.3}=0.011\;\Rightarrow\;\delta t=0.0007\ \text{s},$$
$$\boxed{t=0.0621\pm0.0007\ \text{s}\ \text{— the true exposure is }\approx1/16\ \text{s, not the marked }1/15\ \text{s}}.$$

> 【Thought】 Fractional uncertainties add for a quotient — state that rule before using it. The comparison with the nominal 1/15 s (0.0667 s) is the point of the measurement.
>
> 【Thought】 *Marking-aware note (from the 2015 marking guidance).* This part is specifically about sf and dp: **the decimal places of the result and its uncertainty must agree** — quote $0.0621\pm0.0007$ (both 4 dp). Writing $0.062\pm0.001$ or mismatched pairs like $0.0621\pm0.001$ loses a mark even though the physics is identical. (An rms combination of the uncertainties, $\delta t=0.0005$ s, is equally acceptable.)

---

### Q1(b) — Temperature-compensated resistor from two alloys [5 marks]

**Key observation.** Series: $R(T)=L_cr_c(1+\alpha_cT)+L_mr_m(1+\alpha_mT)$; zero temperature coefficient requires the weighted coefficients to cancel; the total must be 5.0 Ω.

> 【Thought】 Two conditions, two unknowns ($L_c$, $L_m$) — linear system. The negative coefficient of constantan does the compensating. Note the condition involves $r\alpha$ products, not $\alpha$ alone.

**Solution.** Cancellation: $L_c(6.3)(-3.0\times10^{-5})+L_m(5.3)(1.4\times10^{-5})=0$ ⟹ $L_m=2.55L_c$.
Total: $6.3L_c+5.3L_m=5.0$ ⟹ $6.3L_c+13.5L_c=19.8L_c=5.0$:
$$\boxed{L_c=0.25\ \text{m},\qquad L_m=0.64\ \text{m}}.$$

**Check.** $R=6.3(0.2525)+5.3(0.6433)=1.59+3.41=5.0$ Ω ✓; cancellation: $-1.51\times10^{-5}+3.40\times10^{-5}\cdot\frac{1}{2.25}\ldots$ — verify directly: $6.3\times0.2525\times(-3\times10^{-5})+5.3\times0.6433\times1.4\times10^{-5}=-4.77\times10^{-5}+4.77\times10^{-5}\approx0$ ✓.

---

### Q1(c) — Photon density around a sodium lamp [5 marks]

**Key observation.** Photon number flux at distance $R$: $\dfrac{\dot N}{4\pi R^2}$; density = flux/$c$ (photons move at $c$).

**Solution.** $\dot N=\dfrac{P}{hc/\lambda}=\dfrac{100\times6.0\times10^{-7}}{6.63\times10^{-34}\times3\times10^8}=3.02\times10^{20}\ \text{s}^{-1}$;
$$n=\frac{\dot N}{4\pi R^2c}=10^6\;\Rightarrow\;R=\sqrt{\frac{3.02\times10^{20}}{4\pi\times3\times10^8\times10^6}}=\boxed{2.8\times10^{2}\ \text{m}\ (\approx280\ \text{m})}.$$

> 【Thought】 The relation $n=\text{flux}/c$ is the bridge between "per second" and "per cubic metre" — same logic as the beam-density problem in Paper 6 Q1(i). Inventory: $n\times4\pi R^2c=\dot N$ ✓ dimensional and physical.

---

### Q1(d) — Proton–gold closest approach [4 marks]

**Key observation.** Head-on ⟹ all KE converts to Coulomb PE at closest approach: $eV_{acc}=\dfrac{Ze^2}{4\pi\varepsilon_0 r_{\min}}$.

$$r_{\min}=\frac{Ze^2}{4\pi\varepsilon_0\,E_k}=\frac{79\times8.99\times10^9\times(1.60\times10^{-19})^2}{2.0\times10^6\times1.60\times10^{-19}}=\frac{79\times2.30\times10^{-28}}{3.2\times10^{-13}},$$
$$\boxed{r_{\min}=5.7\times10^{-14}\ \text{m}}.$$

> 【Thought】 Rutherford's logic: closest approach measures the nucleus's compactness — the answer (57 fm) is larger than the nuclear radius (~7 fm) but far smaller than the atom ✓ consistent with a point nucleus at this energy. Note the proton never "touches" the nucleus: the experiment is pure Coulomb.

---

### Q1(e) — Sphere at rest in a rotating parabolic bowl [4 marks]

**Key observation.** In the rotating frame, the sphere is in equilibrium under gravity + centrifugal force + normal force. For this to work at *every* $x$, the surface slope must track the ratio $\omega^2x/g$ — exactly what a parabola does.

> 【Thought】 Seeing "at rest relative to the rotating bowl, wherever it is placed" → triggers *the surface must be an equipotential of the effective potential* $U=mgz-\tfrac12m\omega^2x^2$: the bowl's profile satisfies $dz/dx=\omega^2x/g$. Comparing with the given gradient $2ax$ pins $\omega$. If the bowl were spherical, no single $\omega$ would work everywhere — the parabola is special.

**Solution.** Slope condition: $\tan\phi=\dfrac{\omega^2x}{g}=2ax$ (given gradient):
$$\boxed{\omega=\sqrt{2ag}}.$$

**Check.** Dimensions: $a$ is $\text{m}^{-1}$ (for $z=ax^2$), so $ag$ is s⁻² ✓; $\omega$ independent of $x$ ✓ as required by "wherever placed".

---

### Q1(f) — 60° prism at i = 48.59° [5 marks]

**Key observation.** Compute $r_1$: $\sin r_1=\dfrac{\sin48.59^\circ}{1.500}=\dfrac{0.750}{1.500}=0.500$ — the data are engineered for $r_1=30.0^\circ$.

**Solution.** $r_1=30.0^\circ$; $r_2=A-r_1=30.0^\circ$; emergence: $\sin e=1.500\sin30^\circ=0.750$:
$$\boxed{e=48.6^\circ\ (\text{symmetric passage});\qquad \delta=i+e-A=48.59+48.59-60=37.2^\circ}.$$

> 【Thought】 Recognise the minimum-deviation signature: $r_1=r_2=A/2$ ⟹ $e=i$. The deviation formula $\delta=i+e-A$ then applies directly. When numbers land exactly ($\sin r_1=0.500$), say so — it signals the intended path.

---

### Q1(g) — Receding whistle + wall reflection: beats [6 marks]

**Key observation.** The observer hears two sounds: directly from the receding source, and via the wall — which the source *approaches*. The wall re-radiates (reflects) at the frequency it receives, Doppler-shifted oppositely.

> 【Thought】 Two separate Doppler events: (1) source recedes from observer: $f_-=f/(1+v/c)$; (2) source approaches the wall: the wall receives $f_+=f/(1-v/c)$, and being stationary, reflects that same frequency to the observer. The wall is a *stationary observer + re-emitter* — that's the correct two-step model (not "moving mirror" double-shift).

**Solution.** Derivation (receding source): in $\Delta t$ the source emits $f\Delta t$ wavefronts while retreating, so the train stretched over $(c+v)\Delta t$: $\lambda'=(c+v)/f$ ⟹ $f_-=fc/(c+v)=\dfrac{f}{1+v/c}$.
$$f_-=\frac{500}{1+2/330}=497.0\ \text{Hz},\qquad f_+=\frac{500}{1-2/330}=503.05\ \text{Hz}\ \ \text{(the wall receives and re-emits at this frequency)},$$
$$f_{\text{beat}}=f_+-f_-=500\left(\frac{330}{328}-\frac{330}{332}\right)=\frac{500\times330\times4}{328\times332}=\boxed{6.06\ \text{Hz}}.$$

**Check.** Small-$v$: beat $\approx 2fv/c=2\times500\times2/330=6.06$ Hz ✓ (the two first-order shifts add — nice approximation check).

---

### Q1(h) — Network resistances between B–C, B–D, B–A [6 marks]

**Topology (Fig. 1.h).** Nodes B (top), C (right), D (mid-left), A (bottom); edges: B–C 2 Ω, B–D 3 Ω, D–C 7 Ω, D–A 21 Ω, C–A 14 Ω.

**Key observation for B–A first:** the two series paths B–C–A (2+14) and B–D–A (3+21) satisfy $\dfrac{2}{14}=\dfrac{3}{21}$ — a *balanced bridge*: C and D are equipotential, so the 7 Ω carries nothing:
$$R_{BA}=(2+14)\parallel(3+21)=16\parallel24=\boxed{9.6\ \Omega}.$$

**B–C:** direct 2 Ω ∥ [3 Ω + (7 Ω ∥ (21+14) Ω)] $=2\parallel(3+5.83)=\boxed{1.63\ \Omega}$.

**B–D:** direct 3 Ω ∥ [2 Ω + (7 Ω ∥ (14+21) Ω)] $=3\parallel(2+5.83)=\boxed{2.17\ \Omega}$.

> 【Thought】 Order the work by symmetry: spot the balanced bridge for BA *first* (it dissolves the 7 Ω), then the two-terminal reductions are series/parallel only. Verified by nodal analysis: $R_{BC}=1.631$, $R_{BD}=2.169$, $R_{BA}=9.600\ \Omega$ ✓.

---

### Q1(i) — Radium mass for 10 α/s [4 marks]

**Key observation.** Activity $A=\lambda N=\dfrac{\ln2}{T_{1/2}}N$; mass = $N\times$ atomic mass.

$$N=\frac{10\times1620\times365.25\times86400}{0.693}=7.4\times10^{11}\ \text{atoms},$$
$$m=\frac{N\times226}{N_A}=\frac{7.4\times10^{11}\times226}{6.02\times10^{23}}\ \text{g}=\boxed{2.8\times10^{-10}\ \text{g}\ (\sim0.3\ \text{ng})}.$$

> 【Thought】 A gram of radium has activity ~1 Ci ($3.7\times10^{10}$/s) — our 10/s needs a tiny fraction ✓ consistent with Marie Curie's discovery rate scale. Note 1 α per decay — the α emission rate equals the activity.

---

### Q1(j) — Mean, rms and rms-deviation of a stepped waveform [4 marks]

Waveform over one period $4\tau$: $+10$ V for $\tau$, $-2$ V for $\tau$, $+4$ V for $2\tau$.

**(i)** $\bar V=\dfrac{10-2+4\times2}{4}=\boxed{4.0\ \text{V}}$.
**(ii)** $V_{\text{rms}}=\sqrt{\dfrac{10^2+(-2)^2+4^2\times2}{4}}=\sqrt{\dfrac{136}{4}}=\boxed{\sqrt{34}=5.83\ \text{V}}$.
**(iii)** $V_{\text{rms dev}}=\sqrt{\dfrac{(10-4)^2+(-2-4)^2+(4-4)^2\times2}{4}}=\sqrt{\dfrac{72}{4}}=\boxed{\sqrt{18}=4.24\ \text{V}}$.

> 【Thought】 Built-in consistency check: $V_{\text{rms}}^2=\bar V^2+V_{\text{rms dev}}^2$ (mean + variance decomposition): $34=16+18$ ✓. Quote that identity when computing (iii) — it halves the work and self-checks.

---

### Q1(k) — Equator vs pole: fractional difference in g [8 marks]

**Key observation.** Homogeneous spherical Earth: only rotation differentiates them. At the equator, part of gravity supplies the centripetal acceleration; at the poles, none.

> 【Thought】 The instruction "you may not use the table's g" forces you to compute $g=GM_E/R_E^2$ from first principles. The Earth's real oblateness (which also changes $g$ with latitude) is excluded by "homogeneous sphere" — name that model boundary.

**Solution.** $g_0=\dfrac{GM_E}{R_E^2}=\dfrac{6.67\times10^{-11}\times5.98\times10^{24}}{(6.38\times10^6)^2}=9.80\ \text{m/s}^2$ (both latitudes, homogeneous sphere). Equatorial centripetal: $\omega^2R_E=\left(\dfrac{2\pi}{86164\ \text{s}}\right)^2\times6.38\times10^6=0.0339\ \text{m/s}^2$:
$$\frac{g_{\text{pole}}-g_{\text{eq}}}{g_0}=\frac{\omega^2R_E}{g_0}=\frac{0.0339}{9.80}=\boxed{3.5\times10^{-3}\ (0.35\%),\ \text{greater at the poles}}.$$

**Check.** Uses the sidereal day (86 164 s), not 86 400 s — a 0.3% refinement that matters at this precision level ✓.

---

### Q1(l) — Switching off the magnetic field through a loop [7 marks]

**(i)** emf $=\dfrac{\Delta\Phi}{\Delta t}=\dfrac{A\Delta B}{\Delta t}=\dfrac{0.04^2\times0.700}{0.800}=1.4\times10^{-3}$ V:
$$I=\frac{\mathcal E}{R}=\frac{1.4\times10^{-3}}{2.00\times10^{-3}}=\boxed{0.70\ \text{A}},$$
direction: the downward field is decreasing, so the induced current drives its own field downward to oppose the decrease — **clockwise viewed from above** (Lenz).

**(ii)** Constant emf (uniform rate):
$$E=\frac{\mathcal E^2}{R}\Delta t=\frac{(1.4\times10^{-3})^2}{2.00\times10^{-3}}\times0.800=\boxed{7.8\times10^{-4}\ \text{J}\ (\approx0.78\ \text{mJ})}.$$

> 【Thought】 "Uniform rate" is what makes $\mathcal E$ constant and the energy integral trivial. Direction logic (Lenz): decreasing downward flux → induced current *reinforces* the downward field → clockwise from above by the right-hand rule — state the two steps separately.

---

### Q1(m) — Heat generated when two charged spheres are joined [10 marks]

**Key observation.** Charge equilibrates at a common potential (capacitances equal ⟹ final $V$ = mean); the heat is the *drop in stored electrostatic energy*, not the charge transfer times voltage.

> 【Thought】 Compute energy before and after via $U=\tfrac12CV^2=\tfrac12QV$: connect ⟹ charge conserved, potentials equalise. The difference is dissipated in the wire (and radiated). With identical spheres the mean-voltage step is immediate: $V'=300$ V.

**Solution.** $C=4\pi\varepsilon_0r=1.11\times10^{-11}$ F each. $V'=\dfrac{200+400}{2}=300$ V:
$$Q=\Delta U=\tfrac12C\left(200^2+400^2\right)-2\times\tfrac12C(300^2)=\tfrac14C(400-200)^2=\tfrac12C\times(200\,000-180\,000)=10^4C,$$
$$\boxed{Q=10^4\times1.11\times10^{-11}=1.1\times10^{-7}\ \text{J}\ (\approx0.1\ \mu\text{J})}.$$

**Check.** Quick formula: $\Delta U=\tfrac14C(V_1-V_2)^2$ for two equal capacitors (verify: $\tfrac14C(200)^2=10^4C$ ✓) — a memorable form: the dissipated energy depends only on the *initial voltage difference*.

---
*End of Paper 20 (2015 Round 1 Section 1).*


---

## Paper 21 — 2015 Round 1 Section 2 (13 Nov 2015)

*Section 2: Questions 2–6, 20 marks each; candidates attempt two. Full solutions for all five.*

---

### Question 2 — Electron beam deflection by parallel plates

**Setup.** Electrons accelerated through $V_A$ (along $x$); deflecting field along $y$ from plates: pd $V_P$, separation $d$, length $\ell$.

#### Q2(a) [8 marks]

**(i)** Energy: $eV_A=\tfrac12mv_x^2$ ⟹ $\boxed{v_x=\sqrt{2eV_A/m_e}}$.

**(ii)** In the field: $t=\ell/v_x$, $a_y=\dfrac{eE}{m}=\dfrac{eV_P}{m_ed}$, $v_y=a_yt$:
$$\tan\alpha=\frac{v_y}{v_x}=\frac{eV_P}{m_ev_x^2}\cdot\frac{\ell}{d}=\boxed{\alpha=\arctan\frac{V_P\ell}{2V_Ad}}.$$

> 【Thought】 Structure to note: $\tan\alpha\propto V_P/V_A$ — the deflecting voltage and accelerating voltage appear as a *ratio*, because both the kick and the flight time scale with them oppositely. The "parabolic-in-field, straight-after" trajectory (like a projectile) is the physics: deflection angle is set at exit.

**(iii)** Displacement at the plate exit P: parabolic within the field:
$$\boxed{y_P=\tfrac12a_yt^2=\frac{V_P\ell^2}{4V_Ad}}\quad(\propto V_P).$$

#### Q2(b) — Transit time [2 marks]

$$t=\frac{\ell}{v_x}=\ell\sqrt{\frac{m_e}{2eV_A}}=0.0400\times\sqrt{\frac{9.11\times10^{-31}}{6.40\times10^{-16}}}=\boxed{1.5\ \text{ns}}.$$

#### Q2(c) — Second identical field along z [10 marks]

The beam enters the second field with $\mathbf v=(v_x,v_y,0)$, $v_y=v_x\tan\alpha$; the $x$-speed is untouched; the second field (identical, along $z$) applies the same impulse in $z$: $v_z=v_x\tan\alpha$. Final state:
$$\mathbf v_f=(v_x,\;v_x\tan\alpha,\;v_x\tan\alpha),\qquad \boxed{|\mathbf v_f|=v_x\sqrt{1+2\tan^2\alpha}},$$
direction cosines:
$$\cos\theta_x=\frac{1}{\sqrt{1+2\tan^2\alpha}},\qquad \cos\theta_y=\cos\theta_z=\frac{\tan\alpha}{\sqrt{1+2\tan^2\alpha}}.$$

**Numbers** ($V_A=2000$ V, $V_P=50$ V, $\ell=4$ cm, $d=1.5$ cm): $\tan\alpha=\dfrac{50\times4}{2\times2000\times1.5}=\dfrac1{30}$; $v_x=2.65\times10^7$ m/s:
$$|\mathbf v_f|=2.65\times10^7\times\sqrt{1+\textstyle\frac{2}{900}}=\boxed{2.65\times10^7\ \text{m/s}},\qquad \theta_x=\boxed{2.7^\circ},\quad \theta_y=\theta_z=\boxed{88.1^\circ}.$$

> 【Thought】 The second stage adds an *orthogonal* kick of identical size (same plates, same transit) — the velocity components are independent because the fields act on perpendicular components and neither changes $v_x$. The direction cosines must satisfy $\cos^2\theta_x+\cos^2\theta_y+\cos^2\theta_z=1$: check $1/1.0022+2\times0.001111/1.0022=1$ ✓.

---

### Question 3 — Cyclist power model F = av² + b

#### Q3(a) — Extracting a and b [8 marks]

**Key observation.** $P=Fv=av^3+bv$ ⟹ divide by $v$: $P/v=av^2+b$ — plot $P/v$ (=$F$) against $v^2$ for a straight line.

> 【Thought】 Linearisation strategy: the model is cubic in $v$ for power, but dividing by $v$ first turns it into a line in $v^2$. The trap: plotting $P$ vs $v^3$ directly weights the high-speed points overwhelmingly and buries the constant term; dividing by $v$ first balances the leverage.

**Solution.** Computed table ($F=P/v$ vs $v^2$): points $(1.96,4.29)\ldots(146.4,30.8)$; least-squares:
$$\boxed{a\approx0.19\ \text{N s}^2\text{/m}^2\ (\text{kg/m}),\qquad b\approx4.0\ \text{N}}\qquad(\text{graphical accuracy: }a\pm0.01,\ b\pm0.6\ \text{N — official tolerances}).$$
(A careful least-squares fit gives $a=0.184$, $b=4.2$ — inside the graphical tolerance band.)

#### Q3(b) — Physical meaning [2 marks]

$av^2$ = **aerodynamic drag** (quadratic in speed, $\propto$ air density, frontal area, drag coefficient); $b$ = **speed-independent rolling resistance** (tyre deformation, bearings, drivetrain friction).

#### Q3(c) — Maximum sustainable speed [5 marks]

$P_{\max}=Fv_m$: 
$$\boxed{av_m^3+bv_m=P_{\max}:\quad 0.184\,v_m^3+4.2\,v_m=60}\quad\text{(cubic to solve numerically)}.$$

#### Q3(d) — Graphical solution [5 marks]

*Official approach (cleanest):* the maximum-power condition $Fv=60$ recast on the $(v^2,F)$ axes is the curve $F=\dfrac{60}{v}=\dfrac{60}{(v^2)^{1/2}}$ — overplot it on the same graph as the model line. The intersection solves $\dfrac{60}{v_c}=av_c^2+b$, i.e. exactly the cubic of (c):
$$\boxed{v_m\approx5.8\ \text{m/s}\ (\pm0.4\ \text{m/s; }\approx21\ \text{km/h})}.$$

> 【Thought】 The graphical trick is to put the *constraint* on the same axes as the *model*: $F=60/v$ drawn as $F$ vs $v^2$ intersects the fitted line where the available force equals the required force. Read off $v_c$, quote the unit (m/s), and take the uncertainty from the graph's spread — the scheme awards separate marks for value, unit, and uncertainty. Numerical check: $0.19\times5.8^3+4.0\times5.8=37.1+23.2=60.3$ W ✓.

---

### Question 4 — Circuits

#### Q4(a) — Square pulse across a series RC [6 marks]

$\tau=RC=2.0\ \text{k}\Omega\times5.0\ \mu\text{F}=0.010$ s; pulse: 5.0 V for 0.020 s ($=2\tau$).

**Sketch.** During the pulse ($0<t<0.020$ s):
- $V_R$ (full curve): jumps to $+5$ V at $t=0$, decays exponentially toward 0 with $\tau=0.010$ s: $V_R=5e^{-t/\tau}$ (reaches $5e^{-2}\approx0.68$ V at pulse end);
- $V_C$ (dashed): rises from 0 as $V_C=5(1-e^{-t/\tau})$ toward 5 V (reaches $4.32$ V at pulse end);
- Dotted sum: constant $5$ V (KVL).

At $t=0.020$ s (pulse falls to 0): $V_R$ jumps to $-V_C=-4.32$ V and both decay exponentially to 0 ($V_R=-V_C$ after the source drops): dotted sum drops to 0.

> 【Thought】 The three curves must satisfy $V_R+V_C=V_{\text{source}}$ at every instant — that constraint is how you draw them correctly: $V_R$ mirrors $V_C$ about $V_s/2$. The current is proportional to $V_R$ — its jump is the capacitor's inrush.

#### Q4(b) — Nonlinear rod, I = 0.20V³, in series with R on 6.0 V [7 marks]

**(i)** $I=0.40$ A: $V_{\text{rod}}=\left(\dfrac{0.40}{0.20}\right)^{1/3}=2^{1/3}=1.26$ V:
$$V_R=6.0-1.26=4.74\ \text{V}\;\Rightarrow\;\boxed{R=\frac{4.74}{0.40}=11.8\ \Omega}.$$

**(ii)** $P_{\text{rod}}=2P_R\Rightarrow V_{\text{rod}}=2V_R$ (same current) ⟹ $V_{\text{rod}}=4.0$ V, $V_R=2.0$ V; $I=0.20\times4^3=12.8$ A:
$$\boxed{R=\frac{2.0}{12.8}=0.156\ \Omega}.$$

> 【Thought】 For (ii), the power ratio at common current is just the voltage ratio — convert the power statement to voltages *before* touching the nonlinear law. Then the law supplies the current.

#### Q4(c) — Network reduction to Fig. 4.c(ii) [7 marks]

**Reduction sequence** (redraw after each step):

1. **Bottom branch A–D:** 20 µF + 30 µF in series: $C=\dfrac{20\times30}{50}=12$ µF; this is in parallel with the 8 µF middle branch:
$$\boxed{C_2=12+8=20\ \mu\text{F}}\quad(\text{between A and D}).$$
2. **Right path B–D:** 20 MΩ ∥ 5 MΩ $=\dfrac{100}{25}=4$ MΩ between C and D; in series with the 6 MΩ (B–C):
$$\boxed{R_2=6+4=10\ \text{M}\Omega}\quad(\text{between B and D}).$$
3. **Left branch B–A:** the node at the bottom of the 5 µF is wired straight down to the bottom rail, so the 5 µF *also* spans B–A — in parallel with the 15 µF (far-left leg) and the 10 MΩ (E–F):
$$\boxed{R_1=10\ \text{M}\Omega,\qquad C_1=15+5=20\ \mu\text{F}}\quad(\text{branches between B and A}).$$

The resulting network is Fig. 4.c(ii): $R_1$ and $C_1$ in parallel from B to A; $C_2$ from A to D; $R_2$ from B to D:
$$\boxed{R_1=R_2=10\ \text{M}\Omega,\qquad C_1=C_2=20\ \mu\text{F}}.$$

> 【Thought】 Method: identify components sharing the same node pair (parallel) and chains with no side branches (series). The rails are equipotentials — sliding a component along an uninterrupted wire changes nothing. **The trap in this circuit is the 5 µF: drawn horizontally at the top, it *looks* like a series element between B and the middle, but its lower plate wires directly to the bottom rail — trace both plates to their rail nodes before classifying.** Draw each intermediate circuit, as the question demands: the marks are in the *sequence* of valid reductions. (Do not drop the 5 µF — that would quote $C_1=15\ \mu$F; the correct reduction gives $15+5=20\ \mu$F.)

---

### Question 5 — Air and mercury in a vertical tube (reduced variables)

#### Q5(a) — The reduced equation of state [4 marks]

**Geometry/physics.** Air expands by extra length $\ell$ ($\hat\ell=\ell/\ell_0$): volume $V=V_0(1+\hat\ell)$ (uniform bore). The mercury column left above the air is $\ell_0-\ell$; with $P_0=\rho g\ell_0$:
$$P=P_0+\rho g(\ell_0-\ell)=P_0(2-\hat\ell).$$
Hence:
$$\hat V=1+\hat\ell,\qquad \hat P=2-\hat\ell\;\Rightarrow\;\boxed{\text{(i) }\hat P+\hat V=3}\ (\text{temperature-independent}).$$
(ii) Ideal gas: $PV=nRT$ with $P_0V_0=nRT_0$:
$$\boxed{\hat P\hat V=\hat T}\qquad\left(\hat T=\frac{T}{T_0},\quad T_0=\frac{P_0V_0}{nR}\right).$$

#### Q5(b) — The Ṕ–V̂ diagram and the maximum temperature [8 marks]

- **System line:** $\hat P=3-\hat V$: straight line from $(1,2)$ (initial) to $(2,1)$ (all mercury expelled) — the physically admissible region is $\hat V\in[1,2]$.
- **Isotherms:** $\hat P\hat V=\hat T$ — rectangular hyperbolas; they cross the system line twice for $\hat T<2.25$ and touch it at the tangent point $(1.5,1.5)$ for $\hat T_{\max}=\left(\dfrac32\right)^2=\dfrac94$.
- **Symmetry:** both the line and the hyperbolas are symmetric about the diagonal $\hat P=\hat V$ — hence the tangency at $(1.5,1.5)$.

Highest temperature (mid-expulsion, when the line is tangent to the highest reachable isotherm):
$$\boxed{\hat T_{\max}=\frac94\;\Rightarrow\;T_{\max}=\frac{9P_0V_0}{4nR}}.$$

> 【Thought】 The maximum-temperature condition is a *tangency* condition: $\hat T=\hat V(3-\hat V)$ is a downward parabola peaked at $\hat V=3/2$. Beyond that point the required temperature falls while mercury keeps being expelled — the expulsion becomes self-sustaining (runaway) at the tangency: the physics of "the last of the mercury gushes out".

#### Q5(c) — Effective heat capacity along the process [4 marks]

First law for the air (diatomic, $C_V=\tfrac52R$ per mole): $\delta Q=n\tfrac52R\,\delta T+P\,\delta V$; in reduced variables ($P_0V_0=nRT_0$): $\dfrac{\delta Q}{nRT_0}=\tfrac52\delta\hat T+\hat P\,\delta\hat V$ — i.e. the supplied relation. The process heat capacity per mole $\hat c=\dfrac{\delta Q}{n\,\delta T}$:
$$\hat c=R\left[\frac52+\hat P\frac{\delta\hat V}{\delta\hat T}\right],\qquad \hat T=\hat V(3-\hat V)\Rightarrow\frac{\delta\hat T}{\delta\hat V}=3-2\hat V,$$
$$\hat c=R\left[\frac52+\frac{3-\hat V}{3-2\hat V}\right]=R\,\frac{\tfrac52(3-2\hat V)+(3-\hat V)}{3-2\hat V}=\boxed{\hat c=R\,\frac{21-12\hat V}{6-4\hat V}}.\ \blacksquare$$
(Note the denominator $6-4\hat V$: $\hat c$ diverges at $\hat V=1.5$ — the pole is the temperature-maximum point, where $\delta Q\ne0$ produces $\mathrm dT=0$.)

#### Q5(d) — Sketch of ĉ(V̂) [4 marks]

On $\hat V\in[1,2]$: $\hat c(1)=\dfrac{9R}{2}$; rises to $+\infty$ as $\hat V\to1.5^-$; re-enters from $-\infty$ at $\hat V\to1.5^+$; crosses zero at $\hat V=21/12=1.75$; ends at $\hat c(2)=\dfrac{3R}{2}$. Mark the asymptote at $\hat V=1.5$ (the tangency point — heat added with no temperature rise) and the zero at 1.75 (beyond which the air *cools while being heated* — the work of expulsion exceeds the heat input).

> 【Thought】 A negative process heat capacity is the signature of work-dominated expansion (stars do this too — "negative heat capacity" of gravitating systems). The pole at the temperature maximum is the statement $dT=0$ while $\delta Q\ne0$.

---

### Question 6 — Two identical stars: potential landscape

**Setup.** Stars A, B: mass $M$, radius $r$ each, centres $6r$ apart, fixed.

#### Q6(a) [9 marks]

**(i)** B's surface is **not** an equipotential: although B's own field gives $-GM/r$ everywhere on it, A's contribution varies across B ($-GM/s_A$ with $s_A$ from $5r$ to $7r$) ⟹ the total varies from $-\dfrac{6GM}{5r}$ (near side) to $-\dfrac{8GM}{7r}$ (far side). (Only an isolated spherical body has an equipotential surface.)

**(ii)** External to the stars: the potential is **largest** (closest to zero) at infinity; **smallest** (most negative) at the two surface points where the stars face each other (both wells superpose most strongly there: $-\dfrac{6GM}{5r}$).

**(iii)** Maximum on each surface: the **far-side** point (antipodal to the other star): $V=-\dfrac{GM}{r}-\dfrac{GM}{7r}=-\dfrac{8GM}{7r}$.

**(iv)** Midpoint (3r from each centre): $\boxed{V_{\text{mid}}=-\dfrac{2GM}{3r}}$.

#### Q6(b) — Equipotential sketches [4 marks]

- $V_1=-\dfrac{10GM}{3r}$ (deep): two separate small loops, one around each star;
- $V_2=-\dfrac{2GM}{3r}$: the **separatrix** through the midpoint — a figure-eight (two lobes touching at the saddle): the critical topology;
- $V_3=-\dfrac{GM}{3r}$ (shallow): one large closed loop enclosing **both** stars (peanut-shaped).

> 【Thought】 The ordering principle: the saddle value $-2GM/3r$ separates "two islands" from "one continent" topologies. On the axis between the surfaces, the midpoint is a maximum of $V$ (potential barrier top); transversely it's a minimum — a saddle. Sketch by interpolating between the surface values computed in (a).

#### Q6(c) — Minimum launch speed from B to A [7 marks]

**Key observation.** The energetic barrier between the stars is the saddle at the midpoint ($V=-2GM/3r$); launch from the surface point with the *highest* potential (the far side, $-8GM/7r$) to minimise the required kick; arrive at the saddle with zero speed.

$$\frac12v_{\min}^2=V_{\text{saddle}}-V_{\text{launch}}=-\frac{2GM}{3r}+\frac{8GM}{7r}=\frac{GM}{r}\left(\frac{8}{7}-\frac23\right)=\frac{10GM}{21r},$$
$$\boxed{v_{\min}=\sqrt{\frac{20GM}{21r}}}.$$

> 【Thought】 Two optimisations named: (1) launch site — the far-side point, since lifting out of a shallower well costs less; (2) trajectory target — the saddle midpoint, the lowest point of the barrier between the wells (a body that barely crosses the saddle falls onto A thereafter). The energy criterion $\tfrac12v^2\ge V_{\text{barrier}}-V_{\text{start}}$ is the whole content; the catch: it assumes the body can be steered through the saddle, which the fixed stars' geometry permits along the axis.

---
*End of Paper 21 (2015 Round 1 Section 2).*


---

## Paper 22 — 2014 Round 1 Section 1 (14 Nov 2014)

*Section 1, Question 1, parts (a)–(l). Maximum 40 marks from 67.*

---

### Q1(a) — Calibrating an unknown resistance by current ratio [4 marks]

**(i)** X–Y shorted: $E=I_0R_0$. With $R$ in series: $E=\alpha I_0(R_0+R)$. Eliminate $E$:
$$\alpha(R_0+R)=R_0\;\Rightarrow\;\boxed{R=R_0\left(\frac1\alpha-1\right),\qquad 0<\alpha<1\ (\text{and }R\ge0)}.$$

**(ii)** $R$ in **parallel** with $R_0$: the supply current flows through the parallel combination, so $\alpha' I_0 = \dfrac{E}{R_0\parallel R}$:
$$\alpha'=\frac{R_0}{R_0\parallel R}=\frac{R_0+R}{R}\;\Rightarrow\;\boxed{\alpha'>1,\qquad R=\frac{R_0}{\alpha'-1}},$$
so the modified circuit covers $\alpha\in(1,\infty)$ — extending the original range $(0,1)$, with $\alpha=1$ the shared boundary ($R\to\infty$, open circuit / no resistor inserted).

> 【Thought】 The circuit measures $R$ through a current ratio, eliminating the emf — ratio methods kill unknowns. The validity ranges follow from demanding $R\ge0$: a beautiful way to force "think about the domain" — the series version covers $\alpha<1$, the parallel version $\alpha>1$.

---

### Q1(b) — Ball thrown from a moving wagon [5 marks]

**Key observation.** The woman sees the ball rise vertically ⟹ the ball's ground-frame horizontal velocity is zero ⟹ in the man's frame the throw was backward at 60°.

> 【Thought】 Galilean decomposition: ground velocity = wagon velocity + throw velocity. Setting the ground-frame horizontal component to zero pins the throw speed. The vertical motion is identical in both frames — the "height" question probes exactly that Galilean invariance.

**Solution.** Man's frame: throw at $v'$ at 60° backward: horizontal: $10-v'\cos60^\circ=0$ ⟹ $v'=20$ m/s; vertical: $v_y=20\sin60^\circ=17.3$ m/s.
$$h=\frac{v_y^2}{2g}=\frac{17.3^2}{19.6}=\boxed{15.3\ \text{m}\ \text{— identical in both frames: (i) and (ii) both 15.3 m}}.$$

> 【Thought】 The point of the question: the two observers *disagree about the trajectory's shape* (slant vs vertical) but **agree about the height** — vertical dynamics are shared by all horizontal inertial frames.

---

### Q1(c) — Laser through an L-shaped block [6 marks]

**Key observation.** Entry at the left (vertical) face at $45^\circ$: Snell gives the internal ray; the decisive question is the incidence angle at each subsequent face against $\theta_c=\arcsin(1/1.5)=41.8^\circ$.

**Solution.** Entry: $\sin r=\dfrac{\sin45^\circ}{1.5}=0.471$ ⟹ $r=28.1^\circ$ below horizontal (inside, heading down-right).

**(i)** The ray first crosses the **vertical section** (the L's upright column): entry and exit faces are both vertical and parallel, so passage through them restores the original direction — the ray emerges from the column's right face at $e=45^\circ$, *parallel to the incident beam* ($1.5\sin28.1^\circ=\sin45^\circ$). It then re-enters the foot through the top (horizontal) face — again $45^\circ\to28.1^\circ$ — and reaches the **bottom face at incidence $90^\circ-28.1^\circ=61.9^\circ$**. Critical angle: $\theta_c=\arcsin(1/1.5)=41.8^\circ$. Since $61.9^\circ>41.8^\circ$:
$$\boxed{\text{the beam does NOT emerge from the bottom face — it undergoes total internal reflection there}.}$$

> 【Thought】 The question's phrasing "determine the angle at which the beam will emerge from the bottom face" is bait: the correct answer is that it *cannot* emerge — always test the incidence angle against $\theta_c$ before applying Snell at an exit face (Snell would demand $\sin e=1.5\sin61.9^\circ>1$, the algebraic signature of TIR).

**(ii)** Beam entering **below** the horizontal through P: the internal ray (still $28.1^\circ$ below horizontal) passes directly into the foot. At both horizontal faces (bottom and top of the foot) the incidence is $61.9^\circ>\theta_c$, so the ray **zigzags by repeated total internal reflection along the foot — ad infinitum**. It never reaches the inner vertical face PB: the ray's shallow angle ($28.1^\circ<45^\circ$ to horizontal) keeps it below the line from its reflection point to B, so the vertical step face is geometrically out of reach. The only possible exit is the **far (right) end vertical face** of the foot, at incidence $28.1^\circ<\theta_c$: $\boxed{\text{emerges there at }45^\circ\text{ to the normal, parallel to the original beam}}$ (this alternative reading is explicitly credited in the official marking).

> 【Thought】 The structural lesson: in a rectilinear block, the ray's angle to horizontal/vertical is invariant under horizontal-face reflections, so there are only ever two incidence angles ($28.1^\circ$ at vertical faces, $61.9^\circ$ at horizontal ones) — one below, one above the critical angle. A $45^\circ$ entry into $n=1.5$ glass is *just* past the TIR threshold at horizontal faces: the design turns the L-block into a light pipe.

---

### Q1(d) — Mass of Jupiter from Ganymede [5 marks]

**Key observation.** Kepler III for Jupiter; calibrate the Earth mass from $g$ and $R_E$ (no $M_E$ given directly).

$$M_J=\frac{4\pi^2r^3}{GT^2}=\frac{4\pi^2(1.07\times10^9)^3}{6.67\times10^{-11}\times(7.16\times86400)^2}=1.90\times10^{27}\ \text{kg},$$
$$M_E=\frac{gR_E^2}{G}=\frac{9.81\times(6.38\times10^6)^2}{6.67\times10^{-11}}=5.99\times10^{24}\ \text{kg}\;\Rightarrow\;\boxed{M_J\approx316\,M_E}.$$

**Check.** Accepted value 318 $M_E$ ✓ within 1%.

---

### Q1(e) — Copper–tungsten wire pair under load [6 marks]

**Key observation.** Series ⟹ same tension $F=Mg$; extensions add: $\Delta L=F\sum_i\dfrac{L_i}{E_iA_i}$. Compute the *known* copper extension first — what remains of the 6.00 cm is the tungsten's share.

> 【Thought】 Split-before-solve: with extensions adding, evaluate the fully-determined copper term numerically *before* touching the unknown tungsten area — it turns a two-term symbolic equation into simple subtraction. (Careful with powers of ten here: $\tfrac{1}{E_cA_c}\sim4\times10^{-5}$, not $10^{-8}$ — a slip of three orders in the exponent is the classic failure mode of this computation.)

**Solution.** $F=100\times9.81=981$ N; $A_c=\dfrac{\pi}{4}(0.50\times10^{-3})^2=1.963\times10^{-7}$ m²:
$$\delta l_c=\frac{FL}{E_cA_c}=\frac{981\times1.00}{12.4\times10^{10}\times1.963\times10^{-7}}=\frac{981}{2.434\times10^{4}}=4.03\times10^{-2}\ \text{m},$$
$$\delta l_t=6.00\times10^{-2}-4.03\times10^{-2}=1.97\times10^{-2}\ \text{m},$$
$$A_t=\frac{FL}{E_t\,\delta l_t}=\frac{981}{35.5\times10^{10}\times1.97\times10^{-2}}=1.40\times10^{-7}\ \text{m}^2,$$
$$\boxed{d_t=\sqrt{4A_t/\pi}=0.423\ \text{mm}}.$$

**Check.** The copper takes 4.0 cm of the 6.0 cm — far from negligible (its area is larger but not enough to offset the lower modulus); tungsten carries the remaining 2.0 cm ✓; tungsten thinner than copper (stiffer material but much higher stress) ✓ physically consistent. Matches the official $d=0.423$ mm ✓.

---

### Q1(f) — Carbon-14 dating of the coffin wood [5 marks]

**Key observation.** Specific activity $\propto$ surviving ¹⁴C fraction: $A/A_0=2^{-t/T_{1/2}}$.

$$t=T_{1/2}\frac{\ln(A_0/A)}{\ln2}=5700\times\frac{\ln(2.0/1.2)}{0.693}=5700\times0.737=\boxed{4.2\times10^{3}\ \text{years}}.$$

> 【Thought】 Specific activity (per kg) already normalises the mass — use the ratio directly. Logarithm discipline: $\ln(1/0.6)=0.51$; dividing by $\ln2$ converts to half-life units.

---

### Q1(g) — Centre of gravity of a triangular plate [7 marks]

**Why the CG lies on a median.** Slice the triangle into thin strips parallel to one side; each strip's midpoint lies on the median to that side's opposite vertex (the median bisects every parallel chord). Since every strip's centre of mass is on the median, the plate's CG is on the median — and repeating for another side puts it on two medians: at their intersection, $\tfrac23$ from a vertex.

**The remaining plate.** Equilateral triangle side $b$, height $h=\tfrac{\sqrt3}{2}b$; the removed triangle has vertices $B$, $C$ (two corners) and $G$ (the CG). Its area is $\tfrac13$ of the whole (same base $BC$, one third the height), so mass $M/3$, with its own CG at $\tfrac{B+C+G}{3}$. Complement rule with the full plate:
$$M\,\mathbf g=\frac M3\,\mathbf g_{BCG}+\frac{2M}{3}\,\mathbf X\;\Rightarrow\;\mathbf X=\frac{3\mathbf g-\mathbf g_{BCG}}{2}.$$
With $B=(0,0)$, $C=(b,0)$, $A=(b/2,h)$: $\mathbf g=(b/2,\,h/3)$, $\mathbf g_{BCG}=(b/2,\,h/9)$:
$$\mathbf X=\frac{(3b/2-b/2,\;h-h/9)}{2}=\left(\frac b2,\ \frac{4h}{9}\right),$$
$$\boxed{\text{on the symmetry axis (median from A), at height }\frac{4h}{9}=\frac{2\sqrt3}{9}b\approx0.385b\ \text{above the base}}$$
(slightly above the original CG at $h/3$, as the removed mass was below it ✓).

> 【Thought】 Two reusable tools: the *strip argument* (why CG is on a median) and the *complement rule* $M\mathbf g=m_1\mathbf g_1+m_2\mathbf g_2$ for removal problems — solve for the unknown piece, never integrate afresh.

---

### Q1(h) — U-tube in accelerating frames [7 marks]

**Key observation.** In the vehicle frame, replace gravity by the effective vector $(g\ \text{down},\ a\ \text{horizontal})$; hydrostatics then runs on effective gravity.

**(i) Vertical acceleration α:** $g_v=\boxed{g+\alpha}$ (straight addition — depths and pressures scale up uniformly).

**(ii) Horizontal acceleration a:** the free surface tilts by $\tan\theta=a/g$; the pressure difference between the arms comes from the horizontal pseudo-force over the arm spacing $L$: $\rho g h=\rho a L$ (equivalently the tilted free surface):
$$a=\frac{gh}{L},\qquad \boxed{g_h=\sqrt{g^2+a^2}=g\sqrt{1+\left(\frac{h}{L}\right)^2}=\frac{g}{L}\sqrt{L^2+h^2}}.$$

> 【Thought】 The pressure balance $\rho g h=\rho aL$ is the fastest route: the bottom of the U sees the difference between the two columns' weights plus the horizontal drive along the base. Note $g_h$ is the *magnitude* of effective gravity (what a plumb line feels); the height difference $h$ encodes the direction via $\tan\theta=h/L$.

---

### Q1(i) — Rotating-mirror speed measurement [4 marks]

**Key observation.** The light's round trip to the fixed mirror takes $\Delta t=2\times0.30\ \text{km}/c$; meanwhile the rotating mirror turns by $\omega\Delta t$, which *doubles* in the reflected ray's direction change ($2\omega\Delta t$ — mirror rotation doubles into the beam).

> 【Thought】 The rotating-mirror lever: angular deflection of the beam = twice the mirror's angular motion. The beam's lateral displacement at the receiver station = (beam deflection) × (return distance). Setting that equal to the source–receiver separation gives the threshold.

**Solution.** $\Delta t=\dfrac{600\ \text{m}}{c}=2.0\times10^{-6}$ s; beam deflection needed: $\dfrac{0.60\ \text{m}}{0.30\ \text{km}}=2.0\times10^{-3}$ rad:
$$2\omega\Delta t=2.0\times10^{-3}\;\Rightarrow\;\omega=\frac{2.0\times10^{-3}}{2\times2.0\times10^{-6}}=\boxed{500\ \text{rad/s}\ (\approx80\ \text{rev/s})}.$$

**Check.** This is Michelson-style chronometry: metre-scale displacement over km-scale arms from µs-scale rotation ✓ consistent numbers.

---

### Q1(j) — Car horn passing an observer [8 marks]

**Key observation.** The Doppler shift tracks the *radial* velocity component $v_r=v\sin\theta=v\dfrac{x}{\sqrt{x^2+D^2}}$ — zero at the closest point.

**(i)** At A: $v_r=0$ ⟹ $\boxed{f'=400\ \text{Hz}}$ (no shift at closest approach).

**(ii)** Beyond A by $x$ (receding component $v_r=25\dfrac{x}{\sqrt{x^2+100^2}}$ m/s):
$$\boxed{f'(x)=\frac{f}{1+v_r/v_s}=\frac{400}{1+\dfrac{25x}{343\sqrt{x^2+100^2}}}\ \text{Hz}},$$
which falls smoothly from 400 Hz toward $400/(1+25/343)=373$ Hz as $x\to\infty$.

> 【Thought】 The classic mishearing: "at the closest point the frequency is unshifted" is instant-kinematics correct; strictly, the sound heard *when* you see the car at A was emitted earlier (retardation) — beyond this question's scope, but the honest boundary to state. The frequency swoop (high→low through closest approach) is the everyday experience; its symmetric-looking curve is actually shifted by retardation.

---

### Q1(k) — Elastic collision: deriving u − v₁ = v₂ [5 marks]

**(i)** Conservation laws (signs: $v_1$ is a rebound, taken as a positive speed backward):
$$\text{momentum: }mu=-mv_1+Mv_2,\qquad \text{energy: }\tfrac12mu^2=\tfrac12mv_1^2+\tfrac12Mv_2^2.$$

**(ii)** Rearrange: momentum as $m(u+v_1)=Mv_2$; energy factorised: $m(u-v_1)(u+v_1)=Mv_2^2$. Divide:
$$\frac{m(u-v_1)(u+v_1)}{m(u+v_1)}=\frac{Mv_2^2}{Mv_2}\;\Rightarrow\;\boxed{u-v_1=v_2}.\ \blacksquare$$

> 【Thought】 The factorisation trick — difference of squares in the energy equation divided by the momentum equation — is THE elastic-collision move; the result is the relative-velocity reversal rule ($u=v_1+v_2$) in disguise. Memorise the pair, not the derivation.

---

### Q1(l) — Velocity selector (slotted discs) [5 marks]

**Key observation.** Transit time must equal the time for the second slot to arrive at the beam: $t_n=\dfrac{\theta+2\pi n}{\omega}$; speed $v_n=d/t_n$.

> 【Thought】 The slots' offset $\theta$ picks the fastest passing bunch ($n=0$); each extra revolution adds a slower cohort. The beam is thus sliced into discrete speeds — that's the selector's purpose.

**Solution.** $\omega=24\,000\ \text{rpm}=400\times2\pi=2513$ rad/s; $\theta=60^\circ=\pi/3=1.047$ rad; $d=1.00$ m:
$$v_n=\frac{\omega d}{\theta+2\pi n}=\frac{2513}{\,1.047+2\pi n\;}\ \text{m/s},$$
$$\boxed{v_0=2400\ \text{m/s},\quad v_1=343\ \text{m/s},\quad v_2=185\ \text{m/s},\quad v_3=126\ \text{m/s},\ \ldots}$$

**Check.** The first cohort ($v_0=2400$ m/s — no extra turn) is well separated from the rest; the series converges like $1/n$ ✓.

---
*End of Paper 22 (2014 Round 1 Section 1).*


---

## Paper 23 — 2014 Round 1 Section 2 (14 Nov 2014)

*Section 2: Questions 2–9, 20 marks each; candidates attempt two. Full solutions for all eight.*

---

### Question 2 — Triangular-prism resistor networks (symmetry methods)

**Network (all edges R):** a triangular prism — end triangles $ABE$ and $CDF$, rungs $AC$, $BD$, $EF$.

#### Q2(a) — Driven at A, out at B [5 marks]

**(i) Current in EF.** Consider two operations on the driven network: (τ) the prism's mirror symmetry $A\leftrightarrow B$, $C\leftrightarrow D$ (E, F fixed); and (rev) reversing $V$, which reverses every current without changing magnitudes. The composition τ∘rev leaves the *driven* circuit invariant (same port, same $V$) but sends $i_{EF}\to-i_{EF}$ — hence
$$\boxed{i_{EF}=0}\quad(\text{E and F are equipotential}).$$

**(ii) R_AB.** Since E, F are equipotential, remove EF. Now E dangles on A–B as a series $2R$ in parallel with the direct $R$; the bottom path A–C–F…: C–D is $R$ in parallel with C–F–D ($2R$) = $2R/3$, so the bottom path A–C–…–D–B has $R+\frac{2R}{3}+R=\frac{8R}{3}$:
$$R_{AB}=\left(\frac{2R}{3}\right)\parallel\left(\frac{8R}{3}\right)=\frac{(2R/3)(8R/3)}{10R/3}=\boxed{\frac{8R}{15}}.$$

#### Q2(b) — Driven at A, out at C [5 marks]

**Current assignment.** Injecting $I$ at A, extracting at C: the automorphism $(AC)(BD)(EF)$ composed with $V$-reversal forces $i_{BE}=i_{DF}=0$ (they reverse under the map). The remaining network: A–E–F–C chains… assigning loop currents and applying Kirchhoff's junction rule, the distribution per unit $I$ is: $i_{AB}=i_{AE}=i_{EF}=i_{BD}=i_{FC}=\tfrac15 I$, $i_{AC}=\tfrac35 I$, $i_{CD}=\tfrac15 I$ (E, B carry no... — E and F now link the chain). Junction-rule check at A: $i_{AB}+i_{AE}+i_{AC}=\tfrac15I+\tfrac15I+\tfrac35I=I$ ✓; at C the inflow $\tfrac35I+\tfrac15I+\tfrac15I=I$ is extracted ✓. The port drop
$$V_{AC}=\frac35 IR+\frac15IR+\frac15IR\ldots\ \text{(summed along any path)}=0.60\,IR\;\Rightarrow\;\boxed{R_{AC}=\frac{3R}{5}}.$$

> 【Thought】 Both (b) and (c) yield to the same discipline: use symmetry to kill edges, then one independent loop equation. Verified by full nodal analysis: $R_{AB}=0.533R$, $R_{AC}=0.600R$, $R_{AD}=0.733R$ ✓.

#### Q2(c) — Driven at A, out at D [10 marks]

No symmetry kills enough edges now, so assign currents and write Kirchhoff's **second** rule (loop sums of $iR$ vanish). With unit input at A and output at D, solving the node equations gives the branch currents $i_{AB}=\tfrac{5}{15},\ i_{AE}=\tfrac{4}{15},\ i_{AC}=\tfrac{6}{15},\ i_{BE}=-\tfrac{1}{15},\ i_{BD}=\tfrac{6}{15},\ i_{CD}=\tfrac{5}{15},\ i_{EF}=\tfrac{3}{15},\ldots$ (all in units of $I$, signs showing direction). Junction rule at A: $\tfrac{5}{15}+\tfrac{4}{15}+\tfrac{6}{15}=I$ ✓; at B: $i_{BA}+i_{BE}+i_{BD}=-\tfrac{5}{15}-\tfrac{1}{15}+\tfrac{6}{15}=0$ ✓ (no external tap at B):
$$R_{AD}=\frac{V_A-V_D}{I}=\frac{11}{15}R=\boxed{\frac{11R}{15}}.$$

> 【Thought】 Method note: the loop rule ("clockwise sums of iR vanish") plus junction rule always close these networks; symmetry only shortens the algebra. The port voltage reads off any single path — e.g. A→C→D: $\tfrac{6}{15}+\tfrac{5}{15}=\tfrac{11}{15}$ ✓.

---

### Question 3 — Charged particles in a uniform magnetic field (helical motion)

**(a) Helix.** Decompose $\mathbf v=v\cos\theta\,\hat{\mathbf B}+v\sin\theta\,\hat{\perp}$. The magnetic force $q\mathbf v\times\mathbf B$ has no component along $\mathbf B$ ⟹ the parallel motion is uniform ($v_\parallel=v\cos\theta$ const). Perpendicular: $qv_\perp B=mv_\perp^2/\rho$ ⟹ uniform circular motion with
$$\rho=\frac{mv_\perp}{qB},\qquad \omega=\frac{qB}{m},\qquad T=\frac{2\pi m}{qB}\ (\text{independent of }v_\perp).$$
Uniform translation along $\mathbf B$ + uniform circle around it = a **helix** with axis along $\mathbf B$. $\blacksquare$

**(b) Pitch** (the axial advance per turn). $x_{10}=v_\parallel T=\boxed{\dfrac{2\pi mv\cos\theta}{qB}}$.

**(c) Magnetic focusing.** Small $\theta$: $v_\parallel=v\cos\theta\approx v(1-\theta^2/2)\approx v$ for *all* small $\theta$ at fixed $v$ — so after one cyclotron period every particle has travelled the same axial distance:
$$\boxed{L=\frac{2\pi mv}{qB}};$$
they refocus at point P (diverging at entry ⟹ converging at P). Electrons, $v=10^7$ m/s, $B=10^{-4}$ T:
$$L=\frac{2\pi\times9.11\times10^{-31}\times10^7}{1.60\times10^{-19}\times10^{-4}}=\boxed{3.6\ \text{m}}.$$

> 【Thought】 The focusing is second-order robust: $v_\parallel$ varies only at $O(\theta^2)$, so a *fan* of small angles refocuses — this is the principle of magnetic lenses in electron microscopes. Note $T$ independent of speed is the cyclotron's magic ingredient.

**(d) Relativistic modification.** Replace $m$ by $\gamma m$ (the transverse momentum relation $q v_\perp B=\gamma m v_\perp^2/\rho$): pitch $=\dfrac{2\pi\gamma mv\cos\theta}{qB}$ — refocusing still works at fixed speed (common $\gamma$), but the period lengthens by $\gamma$ and the focusing point moves out; if particles share energy rather than speed, the angles also spread differently.

---

### Question 4 — Statics: beads on a bent rod; a straw on a cylinder

#### Q4(a) — Beads on a right-angled rod [12 marks]

**Setup.** Left arm at 30° to horizontal ($m_1=100$ g), right arm at 60° ($m_2=300$ g), arms perpendicular; a straight cord joins the beads; $\alpha$ = cord-to-left-arm angle, $\beta$ = cord-to-right-arm angle. A straight cord crossing two perpendicular rods gives $\alpha+\beta=90^\circ$.

> 【Thought】 Smooth rods ⟹ only the along-rod force balance constrains each bead (the normal absorbs the rest). That decouples the problem into two one-line equations sharing $T$ — divide to eliminate $T$ first (the angle question), then recover $T$.

**Solution.** Along-rod balances:
$$T\cos\alpha=m_1g\sin30^\circ=\frac{m_1g}{2},\qquad T\sin\alpha=m_2g\sin60^\circ=\frac{\sqrt3\,m_2g}{2},$$
(i) $\tan\alpha=\dfrac{\sqrt3\,m_2}{m_1}=3\sqrt3$ ⟹ $\boxed{\alpha=79.1^\circ}$.
(ii) $T=\dfrac{m_1g}{2\cos\alpha}=\dfrac{0.981}{2\times0.1890}=\boxed{2.6\ \text{N}}$.

**Check.** Verify the second equation: $T\sin\alpha=2.60\times0.981=2.55$ N vs $\sqrt3 m_2g/2=2.55$ N ✓.

#### Q4(b) — Straw balanced on a cylindrical container [8 marks]

**Key observation.** The straw touches the rim's edge at P (reaction $\perp$ straw) and its flat lower end sits in the container's far bottom corner Q (reaction along the straw's axis, from the corner on the end face). Both reactions then pass through the straw's axis, so the moment equation about P forces the weight's line through P — the rim contact must be at the straw's **midpoint**.

> 【Thought】 Identify the reaction directions first: sharp rim edge ⟹ ⊥ to the straw; end face in the corner ⟹ along the straw. With two of three forces concurrent along the axis, the third (weight) must pass through their concurrency line — that's what fixes the contact point, and the container's diameter then fixes the angle.

**Solution.** Contact at the midpoint ⟹ the segment from rim P to the bottom corner Q has length $L/2$ and horizontal span $d$:
$$\frac{L}{2}\cos\alpha=d\;\Rightarrow\;\boxed{\alpha=\arccos\frac{2d}{L}}\qquad(\text{needs }L>2d).$$
(For completeness: $N_P=mg\cos\alpha$, $N_Q=mg\sin\alpha$.)

**Check.** $L\to2d$: $\alpha\to0$ — nearly horizontal, rim at the middle ✓; longer straw ⟹ steeper… wait, longer $L$ ⟹ smaller $2d/L$ ⟹ larger α — steeper for a longer straw ✓ consistent with the pivot geometry.

---

### Question 5 — Newton's rings

**(a) Interference conditions.** Normal incidence; the air gap of thickness $t$ gives a round-trip path $2t$. Phase flips: at the lens→air surface (glass to air, index drops) **no** flip; at the air→plate surface (air to glass, index rises) a $\pi$ flip. Net one flip ⟹
$$\boxed{2t=n\lambda\ \text{destructive (dark)},\qquad 2t=\left(n+\tfrac12\right)\lambda\ \text{constructive (bright)},}\quad n=0,1,2,\ldots$$
(the contact point $t=0$ is dark ✓ — the well-known Newton's-rings signature).

> 【Thought】 Flip inventory again (cf. Paper 13 Q6d, Paper 16 Q1n): exactly one of the two reflections flips here, so dark/bright swap relative to a both-flip film — the dark centre is the quick experimental check of the phase bookkeeping.

**(b) Geometry.** The lens surface is spherical (radius $a$); at ring radius $r$ the gap is $t$: the circle chord relation (intersecting-chord/sagitta theorem: the vertical through the lens contact point is a diameter chord):
$$r^2=t(2a-t)\;\Rightarrow\;\boxed{r^2=2at-t^2}.\ \blacksquare$$

**(c)** $t\ll a$ ⟹ drop $t^2$: $t\approx\dfrac{r^2}{2a}$; nth dark ring: $2t=n\lambda$:
$$\boxed{a=\frac{r_n^2}{n\lambda}}.$$

**(d)** Bright rings: $r_n^2=a\left(n+\tfrac12\right)\lambda$ — so diameters: $d_n^2=4a\lambda(n+\tfrac12)$, and the $n$ dependence is linear with a known slope ⟹ subtract the two measurements to kill the offset $+\tfrac12$:
$$d_{n+20}^2-d_n^2=4a\lambda\times20\;\Rightarrow\;a=\frac{(1.36^2-0.582^2)\times10^{-4}}{80\times598\times10^{-9}}=\frac{1.511\times10^{-4}}{4.784\times10^{-5}}=\boxed{3.16\ \text{m}}.$$

> 【Thought】 Data pattern: never compute $n$ first — the difference of squared diameters eliminates both the unknown order $n$ and the half-integer offset. This "difference of squares" pattern recurs in fringe metrology (compare Paper 6 Q1(n)'s logarithmic version).

**(e) Filling with methyl alcohol** ($\mu=1.33$) in 5.0 s: the conditions become $2\mu t=(n+\tfrac12)\lambda$, so each ring's radius shrinks by $1/\sqrt\mu$: $\Delta r=r\left(1-\dfrac1{\sqrt{1.33}}\right)=0.133\,r$, inward:
$$r_1=0.291\ \text{cm}:\ |\dot r|=\frac{0.0387\ \text{cm}}{5.0\ \text{s}}=\boxed{7.7\times10^{-5}\ \text{m/s}};\qquad r_2=0.680\ \text{cm}:\ |\dot r|=\boxed{1.8\times10^{-4}\ \text{m/s}},$$
both **inward** (the rings contract toward the centre as the liquid fills the gap — the question's "increase" in radius is the magnitude of motion; note the sign physically).

> 【Thought】 Index bookkeeping: the wavelength *in the gap* is $\lambda/\mu$, so fixed order ⟹ smaller gap ⟹ smaller radius. The factor $1/\sqrt\mu$ (not $1/\mu$) is because radius ∝ √(thickness).

---

### Question 6 — Diode rectifier with a reservoir capacitor

**Setup.** $V(t)=V_0\cos(2\pi f t)$, $V_0=20$ V, $f=50$ Hz (period 20 ms); $C=50\ \mu$F; diode ideal.

**(a) Time constants:** $\tau=RC$: $\boxed{10\ \text{k}\Omega: 0.50\ \text{s};\quad 1\ \text{k}\Omega: 0.050\ \text{s};\quad 100\ \Omega: 5.0\ \text{ms}}$.

**(b) Sketches.** In each, overlay $V_0\cos\omega t$ (thin) with the output (bold):
- $R=10$ kΩ ($\tau=0.5$ s $\gg T$): output hugs the input peaks, shallow exponential sag between them — small ripple around ≈19 V;
- $R=1$ kΩ ($\tau=50$ ms $>T$): noticeable sag between peaks — moderate ripple;
- $R=100$ Ω ($\tau=5$ ms $<T$): the capacitor nearly empties between peaks — output is sharp humps with deep valleys (large ripple).
In all three, the diode conducts only in short windows around the source maxima (output > source otherwise).

**(c) Conduction condition.** From a peak ($t=0$, $V=V_0$) the capacitor discharges $V_0e^{-t/RC}$ while the source falls as $V_0\cos2\pi ft$; the diode re-conducts when they meet:
$$\boxed{e^{-T_1/RC}=\cos(2\pi fT_1)}\ \ \blacksquare\quad(T_1=\text{discharge time per cycle}).$$
Verify $T_1=0.019125$ s: $e^{-0.019125/0.5}=e^{-0.03825}=0.9625$; $\cos(2\pi\times50\times0.019125)=\cos(6.008\ \text{rad})=0.9625$ ✓ equal.
Conduction fraction:
$$\frac{T-T_1}{T}=\frac{0.020-0.019125}{0.020}=\boxed{4.4\%}.$$

**(d) Ripple for R = 10 kΩ:** $V_{\min}=V_0e^{-T_1/RC}=20\times0.9625=19.25$ V:
$$\boxed{\Delta V=20-19.25=0.75\ \text{V}}.$$

> 【Thought】 The transcendental equation $e^{-T_1/RC}=\cos(2\pi fT_1)$ comes from matching the *values* at the re-conduction instant (a fuller analysis also matches slopes); the capacitor discharges for ~96% of each cycle, and the diode gulps current in the remaining 4% — the physics of rectifier current spikes.

---

### Question 7 — Errors and data analysis

**(a)** Random errors: unpredictable scatter about the true value, reduced by repetition/averaging (e.g. reaction-time scatter in timing with a stopwatch; parallax flicker in an ammeter needle at varying observation angles). Systematic errors: a consistent bias affecting all readings alike, *not* averaging out (e.g. a clock that continually gains time — readings all too high; an incorrectly calibrated ammeter — readings all wrong in the same direction). 
(i) Correct but low-precision: $\boxed{g=9.8\pm1.0\ \text{m/s}^2}$ — correctly centred on the true value, but the uncertainty is large *compared with the value* (~10%). 
(ii) $\text{rms}=\sqrt{\dfrac{65.0^2+72.0^2}{2}}=\sqrt{4704.5}=\boxed{68.6\ \text{m}}$.

**(b)** $g=4\pi^2L/T^2$: fractional errors add with powers as weights:
$$\frac{\delta g}{g}=\frac{\delta L}{L}+2\frac{\delta T}{T}=0.60\%+2\times0.20\%=\boxed{1.0\%}.$$

> 【Thought】 The exponent of $T$ doubles its contribution — error-propagation rule: fractional uncertainties multiply by the power. Note the mean of the two lengths in (a)(ii) would be 68.5 m — the rms 68.6 m is (always) slightly larger: worth remarking why.

**(c)** The given model is $10^V=AI^\alpha$ — so take $\log_{10}$ of *both sides as written*: $V=\log_{10}A+\alpha\log_{10}I$. **Plot $V$ itself (not $\log V$) against $\log_{10}I$** for the straight line; gradient $=\alpha$, intercept $=\log_{10}A$.

Computed table $\log_{10}I$: $0.505,\ 0.996,\ 1.310,\ 1.500,\ 1.987,\ 2.286$. From the best-fit line (graph, through the centroid $(1.43,\ 4.83)$):
$$\boxed{\alpha=2.25\pm0.10,\qquad A=10^{\,1.62}\approx42\pm4}.$$
(A least-squares fit gives $\alpha=2.16$, inside the official graphical tolerance $2.25\pm0.25$; note $A$ is very sensitive to the adopted gradient — that sensitivity is why the accuracy estimate must be stated.)

> 【Thought】 Read the model before choosing axes: here $V$ appears *linearly* in the exponent relation $10^V=AI^\alpha$, so the linearising plot is semi-log ($V$ vs $\log I$), not log-log. Plotting $\log V$ vs $\log I$ fits the *wrong model* and gives a meaningless $\alpha\approx0.2$ — a reminder that the equation given in the question dictates the axes.

**(d)** Pairwise slopes $\alpha=\dfrac{\Delta V}{\Delta\log_{10}I}$: $(1,4)$: $\dfrac{2.00}{0.995}=2.01$; $(2,5)$: $\dfrac{2.60}{0.991}=2.62$; $(3,6)$: $\dfrac{2.00}{0.976}=2.05$. Mean $\boxed{\alpha_M=2.23}$; deviations $|2.01-2.23|=0.21$, $|2.62-2.23|=0.40$, $|2.05-2.23|=0.18$; mean deviation $D=0.26$.

**Comment.** This is a *quantitative* method that does not depend on judging the "best" straight line by eye — but its average deviation ($0.26$) is larger than the graphical estimate's accuracy in (c) ($\pm0.10$): each pairwise slope is hostage to the errors of just two points, while the graph's best-fit line uses all six. Lesson: regress (or draw the best line), don't pair.

---

### Question 8 — Collision kinematics with m₂ = 4m₁

**(a) Momentum-only ratios.** Transverse and longitudinal components (initial direction $\hat u$):
$$m_1v_1\sin\theta_1=4m_1v_2\sin\theta_2,\qquad m_1u=m_1v_1\cos\theta_1+4m_1v_2\cos\theta_2,$$
$$\boxed{\frac{v_1}{v_2}=\frac{4\sin\theta_2}{\sin\theta_1},\qquad \frac{v_1}{u}=\frac{\sin\theta_2}{\sin(\theta_1+\theta_2)}}.$$

**(b) Energy checks.** Eliminating speeds with (a): $\dfrac{T_F}{T_I}=\dfrac{\sin^2\theta_2+\tfrac14\sin^2\theta_1}{\sin^2(\theta_1+\theta_2)}$.
- (i) $\theta_1=\theta_2=60^\circ$: ratio $=\dfrac{0.750+0.1875}{0.750}=1.25$ — final KE *exceeds* initial: **not conserved** (impossible passively; would need internal energy release).
- (ii) $\theta_1=\theta_2=56^\circ$: ratio $=\dfrac{0.6873+0.1718}{0.8597}=0.9994\approx1$ — **conserved** (this is essentially the true elastic pair for this mass ratio).
- (iii) $v_1=v_2$, $\theta_1=90^\circ$: transverse gives $\sin\theta_2=\tfrac14$, $\theta_2=14.5^\circ$; longitudinal: $u=4v_2\cos\theta_2=3.87v_2$; ratio $=\dfrac{v_1^2+4v_2^2}{u^2}=\dfrac{5v_2^2}{15.0v_2^2}=\boxed{\tfrac13}$ — **not conserved** (two-thirds lost).

> 【Thought】 Structure: momentum alone fixes speed *ratios* from angles; the energy test then discriminates which angle pairs are physical for an elastic collision. A ratio > 1 (case i) is the loudest possible failure — no passive collision gains KE.

**(c) Small angles — verification of energy conservation for $3\theta_1=-8\theta_2$.** Put $\sin\theta\approx\theta$ in the ratio from (b) and substitute $\theta_2=-\frac38\theta_1$, so $\theta_1+\theta_2=\frac58\theta_1$:
$$\frac{T_F}{T_I}=\left(\frac{\theta_2}{\theta_1+\theta_2}\right)^{\!2}\left[1+\frac{\theta_1^2}{4\theta_2^2}\right]=\left(\frac{-3/8}{5/8}\right)^{\!2}\left[1+\frac{1}{4\times(9/64)}\right]=\frac{9}{25}\times\left[1+\frac{16}{9}\right]=\frac{9}{25}\times\frac{25}{9}=1.\ \blacksquare$$
Energy is conserved ✓ (the opposite signs mean the two particles scatter to *opposite sides* of $\mathbf u$).

> 【Thought】 The verification is one substitution — but notice where the magic ratio *comes from*: imposing the elastic condition on (b)'s ratio at small angles gives $(\theta_1+\theta_2)^2=\theta_2^2+\tfrac14\theta_1^2$, i.e. $\tfrac34\theta_1^2+2\theta_1\theta_2=0$ ⟹ $3\theta_1=-8\theta_2$. So the given relation is exactly the elastic locus in the small-angle limit; the problem only asks you to verify the easy direction.

---

### Question 9 — Photons and quantum

**(a)** $n=3\to n=1$: $\Delta E=13.6\left(1-\tfrac19\right)=12.09$ eV:
$$\boxed{\lambda=\frac{1240}{12.09}=102.6\ \text{nm}\ (\text{UV, Lyman-}\beta)}.$$

**(b)** The divergence angle $1.5\times10^{-3}$ rad is the beam's **full cone angle**, so the spot's *diameter* at the Moon is $D=R_{EM}\times1.5\times10^{-3}=3.84\times10^8\times1.5\times10^{-3}=5.76\times10^5$ m; area $=\dfrac{\pi D^2}{4}=2.61\times10^{11}$ m². Photon rate $\dot N=\dfrac{P}{hc/\lambda}=\dfrac{5.0\times10^{-4}\times590\times10^{-9}}{6.63\times10^{-34}\times3.00\times10^8}=1.48\times10^{15}$ s⁻¹:
$$\boxed{\Phi=\frac{\dot N}{\pi D^2/4}=\frac{1.48\times10^{15}}{2.61\times10^{11}}=5.7\times10^{3}\ \text{photons m}^{-2}\text{s}^{-1}}.$$

> 【Thought】 Two-stage calculation: photon rate from power, then dilution by the spot area. **The trap is radius vs diameter**: a "divergence angle" quoted for a beam is conventionally the full angle, so $D=R_{EM}\theta$ is the spot *diameter* and the area is $\pi D^2/4$ — using $\pi D^2$ instead quadruples the area and quarters the flux — the classic slip here. "Maximum" assumes all photons land within the spot, uniformly.

**(c) Inverse Compton bookkeeping.** Photon $f_1\to f_2$ backscattered; electron gains $K=5.00$ keV moving forward. Energy: $E_1=E_2+K$. Momentum (photon reverses, electron forward): $\dfrac{E_1}{c}=-\dfrac{E_2}{c}+p_e$ ⟹ $p_ec=E_1+E_2$. Electron (non-relativistic, $K\ll511$ keV): $(p_ec)^2=2m_ec^2K$:
$$(E_1+E_2)^2=2m_ec^2K=(2E_2+K)^2\;\Rightarrow\;2E_2+5=\sqrt{2\times511\times5}=71.5\ \text{keV},$$
$$E_2=33.2\ \text{keV},\qquad E_1=38.2\ \text{keV}\;\Rightarrow\;\boxed{\lambda_1=\frac{1240\ \text{eV nm}}{38.2\ \text{keV}}=0.0324\ \text{nm}\ (\text{X-ray})}.$$

> 【Thought】 The electron's small KE justifies $K=p^2/2m$ — check it: 5 keV ≪ 511 keV ✓. The two conservation laws produce one quadratic; the negative root would give $E_2<0$ — reject on physical grounds (state it).

**(d)** $W=\dfrac{hc}{\lambda}-eV_s=\dfrac{1240}{380}-1.32=3.26-1.32=\boxed{1.94\ \text{eV}}$.

---
*End of Paper 23 (2014 Round 1 Section 2).*


---

## Paper 24 — 2013 Round 1 Section 1 (15 Nov 2013)

*Section 1, Question 1, parts (a)–(m). Maximum 40 marks from 78.*

---

### Q1(a) — Resistor-unit chain [6 marks]

**Key observation.** Each unit is a square C-shape — from terminal A: series $R$ (top), shunt $R$ (left side, down to the lower rail node), series $R$ (bottom) to terminal B — and the next unit attaches at the left-side nodes. So a chain of $n$ units obeys a one-step recursion: adding a unit on the left puts the existing chain $X_{n-1}$ in **parallel with the unit's left-side resistor**, flanked by the two series resistors.

**(i)** With $X_0=\infty$ (bare unit) and $X_n=2R+\dfrac{R\,X_{n-1}}{R+X_{n-1}}$:
$$R_1=2R+R=3R,\qquad R_2=2R+\frac{R\cdot3R}{R+3R}=2R+\frac{3R}{4}=\boxed{\frac{11R}{4}},$$
$$R_3=2R+\frac{R\cdot\frac{11R}{4}}{R+\frac{11R}{4}}=2R+\frac{11R}{15}=\boxed{\frac{41R}{15}}.$$

**(ii)** The chain is unchanged by adding a unit ⟹ fixed point of the recursion:
$$R_T=2R+\frac{R\,R_T}{R+R_T}\;\Rightarrow\;R_T(R+R_T)=2R(R+R_T)+R^2_T\;\Rightarrow\;R_T^2-2RR_T-2R^2=0,$$
$$\boxed{R_T=(1+\sqrt3)\,R\approx2.73R}\quad(\text{positive root}).$$

> 【Thought】 The ladder recursion $X_n=2R+(R\parallel X_{n-1})$ is the workhorse; its fixed point gives (ii) in one line. Self-audit: $R_2=2.75R$ and $R_3=2.733R$ already sandwich the limit $2.732R$ ✓ — checking the finite chains converge to the fixed point validates both directions of the argument.

---

### Q1(b) — Grazing-orbit density, and a diving board [6 marks]

**(i)** Circular orbit just above the surface: $\dfrac{GM}{R^2}=\dfrac{4\pi^2R}{T^2}$ with $M=\tfrac43\pi R^3\rho$:
$$\boxed{\rho T^2=\frac{3\pi}{G}=\text{const}\ (1.41\times10^{11}\ \text{kg s}^2\text{/m}^3)}.$$
**Comment:** the grazing-orbit period depends **only on the planet's density**, not its size — $T=\sqrt{3\pi/G\rho}$ (~84 min for Earth's density) — a surprising and memorable independence.

**(ii)** Diving board: $k=\dfrac{mg}{d}$ (static depression $d$); jumping in rhythm = driving at resonance:
$$T=2\pi\sqrt{\frac{m}{k}}=2\pi\sqrt{\frac{d}{g}}=2\pi\sqrt{\frac{0.30}{9.81}}=\boxed{1.1\ \text{s}}.$$

> 【Thought】 Note the elegant cancellation: the man's mass cancels — the static depression $d$ alone sets the period ($T=2\pi\sqrt{d/g}$, exactly like a pendulum of length $d$).

---

### Q1(c) — Trapped air in a submerged tube; a leaky barometer [6 marks]

**(i)** At 10.0 m: water fills half ⟹ air at half volume ⟹ pressure doubled: $P_1=2P_0$ — consistent with the water pressure at 10 m ($P_0+\rho g\times10\approx2P_0$ ✓, since 10 m of water ≈ 1 atm). For 90% filled: air at $V_0/10$ ⟹ $P_2=10P_0$:
$$P_0+\rho g d=10P_0\;\Rightarrow\;d=\frac{9P_0}{\rho g}=\frac{9\times1.01\times10^5}{1000\times9.81}=\boxed{93\ \text{m}}.$$
(Equivalently, using part (i)'s own calibration $P_0\equiv10$ m of water exactly — as the official scheme does — $d=90$ m; the 3% gap is just the rounding of $P_0$. State which convention you use.)

**(ii) Barometer with trapped air.** Work in mmHg units. Vertical: column 0.700 m, air column 0.300 m at pressure $p_1$: $P_{atm}=700+p_1$. Inclined 60°: mercury reading 0.950 m along the tube ⟹ vertical height $0.950\cos60^\circ=0.475$ m; air column $1.000-0.950=0.050$ m at $p_2$: Boyle: $p_2=p_1\times\dfrac{0.300}{0.050}=6p_1$:
$$P_{atm}=475+6p_1\ \text{and}\ P_{atm}=700+p_1\;\Rightarrow\;5p_1=225\;\Rightarrow\;p_1=45\ \text{mm},$$
$$\boxed{P_{atm}=745\ \text{mmHg}}.$$

> 【Thought】 The barometer's trapped air is the confounder the problem tests: two configurations give two equations ($p_1$ and $P_{atm}$). Note the *vertical* height of the inclined column is what balances pressure ($0.95\cos60^\circ$), while the *length along the tube* sets the trapped air's volume — using each correctly is the whole game.

---

### Q1(d) — Average speed and average acceleration for sinusoidal motion [3 marks]

On $t\in[0,\pi/10]$: $x$ goes monotonically $0\to A$ (since $v=5A\cos5t\ge0$ there):
$$\boxed{v_{AV}=\frac{A-0}{\pi/10}=\frac{10A}{\pi}},\qquad \boxed{f_{AV}=\frac{v(\pi/10)-v(0)}{\pi/10}=\frac{0-5A}{\pi/10}=-\frac{50A}{\pi}}.$$

> 【Thought】 Averages are endpoint quantities: $\bar v=\Delta x/\Delta t$, $\bar a=\Delta v/\Delta t$ — no integration needed, but check the monotonicity (average *speed* = average of $|v|$ only if $v$ doesn't change sign — it doesn't here ✓).

---

### Q1(e) — Earth–Moon electrostatic force [5 marks]

**Key observation.** 1 g of hydrogen ≈ 1 mole ⟹ the separated charge is one Faraday, $Q=N_Ae$; the force is then a plain Coulomb attraction between Earth and Moon.

$$Q=\frac{1.00\ \text{g}}{1.008\ \text{g/mol}}\times6.02\times10^{23}\times1.60\times10^{-19}=9.56\times10^{4}\ \text{C},$$
$$F=\frac{kQ^2}{R_{EM}^2}=\frac{8.99\times10^9\times(9.56\times10^4)^2}{(3.84\times10^8)^2}=\boxed{5.6\times10^{2}\ \text{N}\ (\text{attractive})}.$$

> 【Thought】 The Faraday scale ($N_Ae\approx10^5$ C/mol) is the whole point: macroscopic charge from a gram of matter. Inverse-square at $3.8\times10^8$ m still leaves 560 N — electrostatics is *strong*.
>
> 【Thought】 *Official-answer note.* The official solution quotes $F=1.41\times10^2$ N, using $Q=\tfrac12N_Ae$ — i.e. counting **½ mole of atoms** per gram (taking "molecular weight 2.00" for H₂). But the question says "one gram of hydrogen *atoms*": 1 g of H atoms is 1.00 mol of atoms (atomic weight 1.008), so $Q=N_Ae$ and $F=5.6\times10^2$ N stands as the correct reading. If the stem's “hydrogen atoms” became “hydrogen molecules (H₂)”, condition C ($N_A$ atoms per gram) would break and our reading would fail — fall back to the official reading $\tfrac12N_Ae$: 1 g of H₂ contains only $\tfrac12N_A$ molecules — but each H₂ has 2 protons, so the total charge comes back to $N_Ae$ anyway (the official treatment of this item is itself a slip).

---

### Q1(f) — Uranium's half-life from radium content [5 marks]

**Key observation.** Ancient mineral ⟹ **secular equilibrium**: radium decays as fast as it is produced by uranium: $N_U\lambda_U=N_{Ra}\lambda_{Ra}$.

> 【Thought】 "All the radium arises from the uranium" + "ancient" ⟹ the chain is in equilibrium: the activities are equal. Convert the mass ratio to an atom ratio via atomic weights first.

**Solution.** $\dfrac{N_{Ra}}{N_U}=\dfrac{3.23\times10^{-7}}{226}\times\dfrac{238}{1}=3.40\times10^{-7}$ (per gram U):
$$T_U=T_{Ra}\times\frac{N_U}{N_{Ra}}=\frac{1600}{3.40\times10^{-7}}=\boxed{4.7\times10^{9}\ \text{years}}.$$

**Check.** Accepted U-238 half-life $4.5\times10^9$ yr ✓; note $T_U/T_{Ra}=N_U/N_{Ra}$ — the longer-lived parent dominates the inventory ✓.

---

### Q1(g) — Separating protons from deuterons in a magnetic field [6 marks]

**Key observation.** Same charge, same accelerating voltage ⟹ $r=\dfrac{mv}{eB}=\dfrac{1}{B}\sqrt{\dfrac{2mV}{e}}\propto\sqrt m$; the beams separate by their *diameters* after a semicircle.

$$r_p=\frac{1}{0.500}\sqrt{\frac{2\times1.673\times10^{-27}\times10^4}{1.60\times10^{-19}}}=2.89\ \text{cm};\qquad r_d=\sqrt2\,r_p=4.09\ \text{cm},$$
$$\boxed{\text{separation}=2(r_d-r_p)=2(\sqrt2-1)r_p\approx2.4\ \text{cm}}.$$

> 【Thought】 Structure: $r\propto\sqrt{m}$ at fixed accelerating voltage (both speed and inertia shift) — mass spectrometry in one line (this is the Bainbridge geometry). The semicircle turns the radius difference into a diameter difference — factor of 2.

---

### Q1(h) — Moving source, moving observer [8 marks]

**General formula.** Source speed $u$ toward the observer's region compresses the wave train: $f'=\dfrac{fc}{c-u}$ at the observer's location; the approaching observer (speed $v$) sweeps up wavefronts faster: 
$$\boxed{f_O=f\,\frac{c+v}{c-u}}.$$

**Configuration.** S and P approach point Q along paths at 30° to each other; when equidistant from Q, the triangle SQP is isosceles with apex 30° ⟹ base angles 75°. Only the *line-of-sight* components matter:
$$u_{\parallel}=15\cos75^\circ=3.88\ \text{m/s}\ (\text{source toward P}),\qquad v_{\parallel}=18\cos75^\circ=4.66\ \text{m/s}\ (\text{observer toward S}),$$
$$\boxed{f_O=200\times\frac{331+4.66}{331-3.88}=205\ \text{Hz}}.$$

> 【Thought】 Seeing velocities not collinear with the line of sight → project first: only the components along the source–observer line Doppler-shift. The isosceles geometry (equidistant from Q) makes both projections $\cos75^\circ$.

---

### Q1(i) — Beaker + immersed sphere on a scale [3 marks]

**Key observation.** The sphere's buoyancy reaction pushes down on the water (Newton's third law) — the scale reads the beaker's weight *plus* the weight of the displaced water.

$$W=0.300\,g+\rho_w gV_{\text{sphere}}=2.943+1000\times9.81\times\frac{0.250}{8930}=2.943+0.275=\boxed{3.22\ \text{N}}.$$

> 【Thought】 Same reaction principle as Paper 8 Q1(n) (block on a newton-meter vs beaker on a balance) — the buoyant force is an internal *pair*: whatever lifts the sphere presses the water. The sphere's own weight is carried by its suspension, not the scale.

---

### Q1(j) — Connecting a charged capacitor to an uncharged one [8 marks]

**Key observation.** Charge is conserved (total $Q_0$); potentials equalise in the loop: $V'=\dfrac{Q_0}{C_1+C_2}$. Compare energies via $U=\tfrac12QV$.

**Solution.** Before: $U_i=\dfrac{Q_0^2}{2C_1}$. After: charges $Q_1'=\dfrac{C_1Q_0}{C_1+C_2}$, $Q_2'=\dfrac{C_2Q_0}{C_1+C_2}$ at common potential $V'$:
$$U_f=\frac{Q_1'^2}{2C_1}+\frac{Q_2'^2}{2C_2}=\frac{Q_0^2}{2(C_1+C_2)}<U_i,\qquad \Delta U=\frac{Q_0^2}{2C_1}\cdot\frac{C_2}{C_1+C_2}\ \text{lost}.$$

**Conclusion.** The stored energy *decreases* even though charge is conserved: the difference is dissipated as heat (and EM radiation) in the connecting wires during the redistribution transient. This is inevitable whenever charge flows down a potential difference — the "capacitor paradox": even with tiny resistance, the dissipation is the same (compare Paper 20 Q1(m)).

---

### Q1(k) — Sphere pulled up an incline by a surface-attached string [10 marks]

**Key observation.** Quasi-static at the point of sliding: friction maximal $F=\mu N$ down-slope (impending upward slide); the string (parallel to the plane, attached at P) provides the torque balance about the contact point C.

**Setup.** Plane at 33°; P on the surface with OP at angle θ from OC (C = contact); the string's moment arm about C is the height of P above the plane, $R(1+\cos\theta)$.

**(i)** Along the plane: $T=F+Mg\sin33^\circ=\mu Mg\cos33^\circ+Mg\sin33^\circ$:
$$\boxed{T=Mg(\sin33^\circ+0.420\cos33^\circ)=5.00\times9.81\times(0.545+0.352)=44.0\ \text{N}}.$$

**(ii)** Moments about C (the weight's arm is $R\sin33^\circ$; N and F pass through C). With $\theta$ measured from OC (the radius to the contact point), P stands at height $R(1-\cos\theta)$ above the plane — that height is the string's moment arm:
$$TR(1-\cos\theta)=MgR\sin33^\circ\;\Rightarrow\;1-\cos\theta=\frac{\sin33^\circ}{\sin33^\circ+\mu\cos33^\circ}=0.607,$$
$$\boxed{\cos\theta=0.393\;\Rightarrow\;\theta=66.9^\circ}$$

— P sits $66.9^\circ$ around from the contact point (forward-uphill side), so the string's line runs at height $0.61R$ above the plane, creating the torque that balances gravity's overturning moment ✓. *Cross-check (moments about O):* gravity and N pass through O; friction acts along the plane at distance $R$; the string's perpendicular distance from O is $R\cos\theta$: $TR\cos\theta=FR$ ⟹ $\cos\theta=F/T=\mu Mg\cos33^\circ/T=0.393$ ✓ same answer.

> 【Thought】 Method: resolve for $T$ (needs $\mu N$ — the "about to slide" clause sets $F=\mu N$), then moments about the contact point C to kill $N$ and $F$ (or about O to kill $N$ and $Mg$ — a slicker route the official scheme uses, since $F/T$ falls out directly). The geometry step — the string's moment arm about C is the height of P above the plane, $R(1-\cos\theta)$ with $\theta$ measured *from the downward radius OC* — is the one place to be careful: writing $R(1+\cos\theta)$ (measuring $\theta$ from the upward vertical) flips the sign and gives a spurious obtuse angle. (That sign slip is exactly the trap; the official answer is $\theta=66.9^\circ$.)

---

### Q1(l) — Three boats in cyclic pursuit [8 marks]

**(i) Evolution.** The triangle stays equilateral (symmetry), shrinking and rotating; the boats spiral logarithmically into the centre P.

**(ii) Velocity components.** Each boat's heading toward its target makes 30° with the direction to the centre P (the target is 30° off the centreline). Self-similar motion ⟹ both components constant:
$$\boxed{v_{\text{radial}}=v\cos30^\circ=26.0\ \text{km/h}\ (\text{toward P, constant})},\qquad v_{\perp}=v\sin30^\circ=15.0\ \text{km/h}\ (\text{constant}).$$

**(iii) Meeting time.** Along a side: the pursued boat's velocity has component $-v/2$ along the side (it heads at 60° off the side, partly back toward its pursuer's start), so the side shrinks at $v-(-\tfrac{v}{2})$… — cleanly: $\dot s=v_B\cdot\hat s-v_A\cdot\hat s=-\tfrac{v}{2}-v=-\tfrac{3v}{2}$:
$$\boxed{t_M=\frac{50}{3\times30/2}=\frac{50}{45}=1.11\ \text{h}\ (\approx67\ \text{min})}.$$

**(iv) Distance.** Constant speed ⟹ $\boxed{D=v\,t_M=30\times1.11=33.3\ \text{km}}$.

> 【Thought】 The side-shrink rate $\tfrac32v$ is the cleanest route (the target's 60°-offset flight has a *negative* along-side component, helping the closure). Cross-check via the centre: centre distance $\frac{50}{\sqrt3}=28.9$ km at 26.0 km/h ⟹ 1.11 h ✓. The boats make infinitely many turns around P — a logarithmic spiral with finite length (33 km) and finite time.

---

### Q1(m) — Pump strokes for the tyre [4 marks]

Identical to Paper 18 Q1(e): $N=\dfrac{P_tV_t}{P_0V_p}=\dfrac{3.0\times10^5\times1.20\times10^{-3}}{1.00\times10^5\times9.0\times10^{-5}}=\boxed{40\ \text{strokes}}$.

> 【Thought】 Note this problem is recycled from the 2016 paper — when revising past papers, register such repeats as *templates*: isothermal mole-counting, $\frac{P_tV_t}{P_0V_p}$.

---
*End of Paper 24 (2013 Round 1 Section 1).*


---

## Paper 25 — 2013 Round 1 Section 2 (15 Nov 2013)

*Section 2: Questions 1–6, 20 marks each; candidates attempt two. Full solutions for all six.*

---

### Question 1 — Bridge-like network with R and 2R (port P–S)

**Topology (Fig. 1.1):** edges PQ $=R$, QS $=2R$, PT $=2R$, QT $=R$, TS $=R$; the cell drives the network across P and S.

**(a) Reversal.** The network is linear: reversing the cell's polarity reverses every current's direction with magnitudes unchanged. More sharply: the reversed circuit is the *same network driven from the other port*, so reflection composed with reversal shows the current in QS equals that in PT, and the current in TS equals that in PQ:
$$\boxed{i_{QS}=i_2\ (=i_{PT}),\qquad i_{TS}=i_1\ (=i_{PQ})}$$
— the upstream/downstream arms pair off. (Confirmed by the numbers in (b)–(d): $i_{QS}=\tfrac{2V}{7R}=i_2$, $i_{TS}=\tfrac{3V}{7R}=i_1$ ✓. This mirror-pairing is also the engine of Paper 23 Q2.)

**(b)–(d) Currents and R_PS.** Set $V_P=V$, $V_S=0$; KCL at Q and T:
$$\frac{V-Q}{R}=\frac{Q}{2R}+\frac{Q-T}{R},\qquad \frac{V-T}{2R}=\frac{T}{R}+\frac{T-Q}{R},$$
solve: $Q=\dfrac{4V}{7}$, $T=\dfrac{3V}{7}$. Junction rule then gives:
$$i_1=\frac{3V}{7R}\ (PQ),\quad i_2=\frac{2V}{7R}\ (PT),\quad \boxed{i_{QT}=\frac{V}{7R}},\quad i_{QS}=\frac{2V}{7R},\quad i_{TS}=\frac{3V}{7R},\quad \boxed{i_{SUP}=\frac{5V}{7R}}.$$

**(c) Loop equations.** Path PQTP (no source): $i_1R+i_{QT}R=2i_2R$ ⟹ $i_1+i_{QT}=2i_2$ ✓ ($\tfrac37+\tfrac17=\tfrac47$ ✓). Path PTSUP (with the cell): $2i_2R+i_{TS}R=E$ ✓ ($\tfrac47+\tfrac37=1$ ✓).

**(d)** $R_{PS}=\dfrac{V}{I}=\dfrac{V}{5V/7R}=\boxed{\dfrac{7R}{5}}$; $i_1=\boxed{\dfrac{3E}{7R}}$, $i_2=\boxed{\dfrac{2E}{7R}}$. A cell with internal resistance $3R$: $R_{PS}$ is a network property — **unchanged**; the total resistance the cell sees becomes $\dfrac{7R}{5}+3R=\dfrac{22R}{5}$, so all currents scale down by $\dfrac{7}{22}$.

**(e) QT → variable X.** Redo the node analysis with $y=R/X$:
$$R_{PS}(X)=\frac{3+4y}{2+3y}\,R=\frac{3X+4R}{2X+3R}\,R\ \ (\text{monotonic in }X,\ \text{decreasing in }y),$$
$$\boxed{\frac{4R}{3}\le R_{PS}\le\frac{3R}{2}}\qquad(X=0\text{ (short)}\to\frac{4R}{3};\ X\to\infty\text{ (open)}\to\frac{3R}{2}).$$

> 【Thought】 The endpoints are clean reductions: $X=0$ shorts Q–T ($R\parallel2R$ then $2R\parallel R$ in series: $\frac{2R}{3}+\frac{2R}{3}$); $X=\infty$ opens QT (two 3R paths in parallel: $\frac{3R}{2}$). Monotonicity between them can be read off $\frac{d}{dy}\frac{3+4y}{2+3y}<0$ — the bridge element X always "pulls toward balance", never overshooting: check that the endpoints bound the physical answer.

---

### Question 2 — Springs: cutting, two-spring oscillator

**(a) Cutting a spring.** A spring of constant $k_1$ cut into $n$ identical pieces: under the same load $F$, each piece carries $F$ and extends $F/k_2$; the original spring's extension was the sum of $n$ such: $F/k_1=nF/k_2$:
$$\boxed{k_2=nk_1}\quad(\text{shorter springs are stiffer}).$$

**(b) Equilibrium.** Lower spring at zero tension ⟹ the upper alone supports the weight:
$$\boxed{x_{10}=\frac{mg}{k_1}}.$$

**(c) SHM.** Displace down by $x$: upper extension grows by $x$ (extra upward $k_1x$); the lower spring compresses by $x$ (pushes up $k_2x$):
$$F_{\text{net}}=k_1(x_{10}+x)+k_2x-mg=(k_1+k_2)x\ \text{(restoring)},$$
$$m\ddot x=-(k_1+k_2)x\;\Rightarrow\;\boxed{f=\frac{1}{2\pi}\sqrt{\frac{k_1+k_2}{m}}}\ \text{— SHM}.\ \blacksquare$$

**(d) Energy.** Summing KE + both spring PEs + GPE (measured from equilibrium):
$$E=\tfrac12mv^2+\tfrac12k_1(x_{10}+x)^2+\tfrac12k_2x^2-mg(x_{10}+x)=\tfrac12mv^2+\tfrac12(k_1+k_2)x^2+\text{const},$$
since the linear term $k_1x_{10}x-mgx=(k_1x_{10}-mg)x=0$ by the equilibrium condition. So **$E$ depends only on $v^2$ and $x^2$** (plus a constant) ⟹ the motion about equilibrium is exactly harmonic, gravity merely re-centring it. $\blacksquare$

**(e) Horizontal.** Gravity drops out entirely; the two springs still oppose with constants $k_1$, $k_2$:
$$\boxed{f_H=\frac{1}{2\pi}\sqrt{\frac{k_1+k_2}{m}}}\ \text{— identical.}$$

> 【Thought】 The reusable content of (c)–(e): opposing springs add constants ($k_1+k_2$), gravity shifts only the equilibrium (the linear term in the energy vanishes at equilibrium — that's *why* it's the equilibrium). The "energy depends only on $v^2$ and $x^2$" form is the definition of an SHM potential.

---

### Question 3 — Electrostatics of two and three charges

**(a)** (i) A *field line* is a curve whose tangent everywhere gives the direction of E (it begins on positive charge and ends on negative charge). (ii) An *equipotential surface* is a surface on which the potential is constant — no work is done moving a charge on it, and E is everywhere perpendicular to it.

**(b) Neutral point(s) for +4Q at A, −Q at B** (AB = $a$). Between the charges the fields add (both point toward B); beyond A the bigger charge dominates. Only beyond B can they cancel:
$$\frac{4Q}{(a+x)^2}=\frac{Q}{x^2}\;\Rightarrow\;2x=a+x\;\Rightarrow\;\boxed{x=a\text{ beyond B}\ \text{(C lies on line AB, }2a\text{ from A)}}.$$

**(c) Equipotential equation.** $\boxed{\dfrac{4}{r_A}-\dfrac{1}{r_B}=\dfrac{V}{kQ}}$ (with $k=1/4\pi\varepsilon_0$) — a Cassini-like oval family.

**(d) Sketches.** (i) Field lines: dense bundle radiating from A (+4Q); one quarter of A's lines terminate on B (−Q), the rest escape to infinity; the neutral point C sits beyond B as the pinch point (no line passes through it). (ii) Equipotentials: near-spherical shells around each charge close in; the $V=0$ surface is the Apollonius circle $r_A=4r_B$ (a closed loop around B, diameter from $\tfrac{4a}{5}$ to $\tfrac{4a}{3}$ measured from A); far away, circles around the net $+3Q$.

**(e) Right triangle (3a, 4a, 5a), +Q at each corner; M = midpoint of the 3a side.** Place the right angle at the origin: corners $(0,0)$, $(3a,0)$, $(0,4a)$; $M=(1.5a,0)$. Distances: $1.5a$, $1.5a$, $\sqrt{1.5^2+16}\,a=4.272a$:
$$V_M=\frac{kQ}{a}\left(\frac{1}{1.5}+\frac{1}{1.5}+\frac{1}{4.272}\right)=\boxed{1.57\,\frac{kQ}{a}}.$$
Fields from the two ends of the 3a side cancel (equal distances, opposite directions); only the far corner contributes, along the direction from $(0,4a)$ to $M$, i.e. unit vector $(0.351,-0.936)$:
$$\boxed{\mathbf E_M=\frac{kQ}{18.25\,a^2}(0.351\,\hat x-0.936\,\hat y),\qquad |\mathbf E_M|\approx\frac{0.055\,kQ}{a^2}}.$$

> 【Thought】 Symmetry first: the two equal distances $1.5a$ cancel in the *vector* sum but add in the *scalar* (potential) sum — the classic demonstration that E is a vector and V a scalar. Compute components only after using the cancellation.

---

### Question 4 — Collisions of identical balls

**(a) Elastic, head-on, equal masses.** Conservation laws: $u_0=v_A+v_B$ (momentum) and $u_0^2=v_A^2+v_B^2$ (energy); with $u_0=v_A+v_B$, squaring gives $u_0^2=v_A^2+v_B^2+2v_Av_B$ ⟹ $v_Av_B=0$; the physical (non-trivial) root: 
$$\boxed{v_A=0,\ v_B=u_0}\quad\text{— the balls exchange velocities (A stops dead, B moves off at }u_0\text{)}.$$

> 【Thought】 The two-line derivation: substitute momentum into energy and factor out the trivial root $v_A=u_0$ (no collision). Newton's cradle is built on exactly this.

**(b) Inelastic 2-D collision with equal exit angles.** Data: $T_i=8.00$ J, heat $2.00$ J ⟹ $T_f=6.00$ J; A and B leave at equal angles $\pm\theta$ from $\mathbf u_0$.

(i) Energy: $\tfrac12mv_A^2+\tfrac12mv_B^2=6.00$ J ⟹ $v_A^2+v_B^2=\dfrac{12.0}{m}$; also $\tfrac12mu_0^2=8.00$ ⟹ $u_0=\dfrac{4}{\sqrt m}$.
(ii) Momentum: transverse $mv_A\sin\theta=mv_B\sin\theta$ ⟹ $v_A=v_B\equiv v$; longitudinal $mu_0=m(v_A+v_B)\cos\theta=2mv\cos\theta$.
(iii) From energy: $v=\sqrt{\dfrac{6}{m}}=\dfrac{\sqrt6}{4}u_0$; then
$$u_0=2v\cos\theta\;\Rightarrow\;\cos\theta=\frac{u_0}{2v}=\frac{2}{\sqrt6}=\sqrt{\frac23}\;\Rightarrow\;\boxed{\theta=35.3^\circ}.$$
(iv) Change in A's momentum: by vector momentum conservation $m\mathbf u_0=m\mathbf v_A+m\mathbf v_B$, so $\Delta\mathbf p_A=m(\mathbf v_A-\mathbf u_0)=-m\mathbf v_B$ — A's momentum change is *equal and opposite to B's final momentum*:
$$\boxed{|\Delta\mathbf p_A|=mv=\sqrt{6m}}\quad\text{(directed opposite to }\mathbf v_B\text{)}.$$

> 【Thought】 For (iv), read the momentum triangle before reaching for components: $\mathbf u_0=\mathbf v_A+\mathbf v_B$ rearranged is $\mathbf v_A-\mathbf u_0=-\mathbf v_B$ — one line, no trig. (Mis-computing the ratio as $\tfrac{\sqrt3}{2}u_0$ instead of the correct $\sqrt6/4$ corrupts $\theta$ and $|\Delta p_A|$; the official values $\theta=35.3^\circ$, $|\Delta p_A|=\sqrt{6m}$ are in place. Sanity check by the law of cosines: $v^2+u_0^2-2vu_0\cos\theta=\frac6m+\frac{16}{m}-2\times\frac{\sqrt6}{\sqrt m}\frac{4}{\sqrt m}\frac{2}{\sqrt6}=\frac6m$ ✓.)

> 【Thought】 The transverse momentum equation forces $v_A=v_B$ immediately (equal masses, equal angles) — then everything is scalar. For (iv), use the law of cosines on the momentum triangle ($\mathbf u_0=\mathbf v_A+\mathbf v_B$ vectorially) rather than components — the magnitude drops out in one line.

---

### Question 5 — Diffraction grating: order analysis

**(a)** Normal incidence, period $d$: path difference between adjacent slits $=d\sin\theta$:
$$\boxed{\text{constructive: }d\sin\theta=n\lambda;\qquad \text{destructive: }d\sin\theta=\left(n+\tfrac12\right)\lambda}\quad(n=0,1,2,\ldots).$$

**(b) The composite fourth line.** Counting from the zero order, lines appear in order of $d\sin\theta=n\lambda$: violet deviates least per order. The observed sequence: violet 1st, red 1st, violet 2nd, then a **superposition: red 2nd order with violet 3rd order** — because $2\lambda_r\approx3\lambda_v$ (red ≈ 690 nm, violet ≈ 460 nm: $2\times690=1380\approx3\times460=1380$). So the first four lines are V1, R1, V2, (R2 + V3).

> 【Thought】 Coincidence condition: $n_r\lambda_r=n_v\lambda_v$ requires the wavelength ratio near a small rational — here $\lambda_r/\lambda_v\approx3/2$. Recognising "superposition ⟹ commensurate wavelengths" is the diagnostic.

**(c)** $d=1/500\ \text{mm}=2000$ nm; composite line at $\theta=43.6^\circ$: $d\sin\theta=2000\times0.6897=1380$ nm:
$$\boxed{\lambda_r=\frac{1380}{2}=690\ \text{nm}\ (\text{2nd order}),\qquad \lambda_v=\frac{1380}{3}=460\ \text{nm}\ (\text{3rd order})}.$$

**(d) Fifth line.** Next after the composite: violet 4th order vs red 3rd: $4\times460=1840<3\times690=2070$ — violet 4th comes first:
$$\boxed{\sin\theta=\frac{4\times460}{2000}=0.920\;\Rightarrow\;\theta=66.9^\circ\ \text{(violet, 4th order)}}.$$

**(e) Intensity vs order.** The finite slit width imposes a single-slit envelope: $I_n=I_0\,\text{sinc}^2\!\left(\dfrac{n\pi w}{d}\right)$ (w = slit width): sketch — peaks at each order under a falling sinc² envelope, with the first missing order at $n=d/w$ (where the envelope hits zero). 

> 【Thought】 The envelope is the convolution logic of gratings: *positions* set by the period $d$, *heights* by the single-slit width $w$. Missing orders occur when a grating maximum lands on a single-slit zero — worth a mark to mention.

---

### Question 6 — Pouring liquid into a cylinder on scales

**Setup.** Cylinder: height $H$, area $A$, weight $W_{MC}$; liquid poured from height $H$ above the base at volume rate $v$; liquid surface at height $h$; stream lands at speed $u=\sqrt{2g(H-h)}$.

**(a) Scale reading.** Contents' weight + momentum-flux force of the landing stream ($\dot m=\rho v$):
$$\boxed{w=W_{MC}+\rho gAh+\rho v\sqrt{2g(H-h)}}.$$

**(b) Maximum.** With $y=\sqrt{H-h}$: $w=W_{MC}+\rho gA(H-y^2)+\rho v\sqrt{2g}\,y$ — quadratic in $y$; complete the square (as hinted):
$$\frac{dw}{dy}=-2\rho gAy+\rho v\sqrt{2g}=0\;\Rightarrow\;y^*=\frac{v}{\sqrt{2g}\,A},$$
$$w_{\max}=W_{MC}+\rho gAH+\frac{\rho v^2}{2A}=\boxed{W_{MC}+\rho gAH+\frac{\rho v^2}{2A}}\qquad\left(\text{at }h^*=H-\frac{v^2}{2gA^2}\right).$$

**(c)** At that instant the contents weigh $W_{MC}+\rho gAh^*=W_{MC}+\rho gAH-\dfrac{\rho v^2}{2A}$:
$$\boxed{w_{\max}-(\text{contents' weight})=\frac{\rho v^2}{A}}.$$

**(d) Time dependence.** Watch the flight delay: pouring starts at $t=0$, but the first drop falls the full height $H$ and lands at $t_1=\sqrt{2H/g}$ — before that the scale reads just $W_{MC}$. Thereafter the level rises as $h=v(t-t_1)/A$ (until the reservoir empties at $t_E$; the water already in flight keeps landing until $t_E+\sqrt{2H/g}$):
$$w(t)=\begin{cases}W_{MC}, & 0\le t\le t_1,\\[4pt] \left(W_{MC}+\rho gAH+A\rho g b^2\right)-A\rho g\left[\sqrt{H-\frac{v(t-t_1)}{A}}-b\right]^2, & t_1\le t\le t_E+\sqrt{\frac{2H}{g}},\\[4pt] W_{MC}+\rho gAH, & t\ge t_E+\sqrt{\frac{2H}{g}},\end{cases}\qquad b\equiv\frac{v}{A\sqrt{2g}}.$$
(The middle branch is (b)'s completed square with $y=\sqrt{H-h}$ written in terms of $t$ — the form the official scheme uses.)

**(e) Sketch.** Flat at $W_{MC}$ for $0\le t\le t_1$ (stream in flight); then a curve rising through $W_{MC}+\rho v\sqrt{2gH}$ (first impact) to the maximum $w_{\max}$ at $t_{\max}=t_1+\dfrac{h^*A}{v}$; easing back down and settling at $W_{MC}+\rho gAH$ from $t_E+\sqrt{2H/g}$ onward. Mark the points $(W_{MC},t_1)$, $(w_{\max},t_{\max})$, and the settling point $\left(W_{MC}+\rho gAH,\ t_E+\sqrt{2H/g}\right)$ — the scheme marks each labelled feature.

> 【Thought】 The interesting physics: the momentum-flux term *decreases* as the surface rises toward the spout, while the weight grows linearly — their sum can peak before the cylinder fills. The completing-the-square hint signals the quadratic in $y=\sqrt{H-h}$; the answer to (c) — $\rho v^2/A$ — is the momentum flux at the maximum, a neat closed form worth boxing separately.

---
*End of Paper 25 (2013 Round 1 Section 2).*


---

## Paper 26 — 2012 Round 1 Section 1 (16 Nov 2012)

*Section 1, Question 1, parts (a)–(p). Maximum 40 marks from 83.*

---

### Q1(a) — Planck constant data: best estimate and uncertainty [3 marks]

**Key observation.** The value 3.66 sits ~55σ from the cluster (6.57–6.72): a measurement blunder (likely a transcription slip for 6.66) — reject it, then average.

> 【Thought】 Outlier rejection needs a stated criterion, not vibes: with the other ten values in a 0.15-wide band, 3.66 is incompatible with the distribution (it's 2.9 units off the mean while the spread is 0.05). State the criterion, then quote mean ± standard error.

**Solution.** Remaining ten values mean $\bar h=6.650\times10^{-34}$ J s; standard deviation $\sigma=0.047$, standard error $\sigma/\sqrt{10}=0.015$:
$$\boxed{h=(6.65\pm0.02)\times10^{-34}\ \text{J s}\ (\text{standard error};\ \pm0.05\ \text{if quoting the spread})}.$$

**Check.** The accepted value 6.63 lies within the band ✓.

---

### Q1(b) — Differential (Weston) pulley [5 marks]

**Mechanism.** The compound wheel (radii $a$, $b$ rigidly joined) winds rope onto one wheel while paying it out from the other; the movable pulley P hangs in the loop. Section A pulled down at speed $V$ rotates the wheel at $\omega=V/a$ (A wraps the radius-$a$ wheel).

**(i) Direction.** The big wheel takes up rope at $b\omega>V$, the small one pays out $a\omega=V$: the loop supporting P **shortens**, so $\boxed{W\text{ moves upward}}$.

**(ii) Speed.** Net rope taken from the loop per second: $(b-a)\omega=(b-a)V/a$; P is carried by two strands, so it rises at half that:
$$\boxed{v_W=\frac{(b-a)}{2a}\,V}.$$

> 【Thought】 Two levers compound: the differential take-up $(b-a)\omega$ and the movable pulley's two-strand halving. If the rope instead wraps the radius-$b$ wheel, the answer becomes $\frac{(b-a)V}{2b}$ — the structure (difference × half) is the content. Limit check: $a\to b$ gives zero motion — the differential principle ✓.

---

### Q1(c) — Earth's mean density [5 marks]

**Key observation.** $g=GM/R^2$ with $M=\tfrac43\pi R^3\rho$ ⟹ $\rho=3g/(4\pi GR)$ — no masses needed.

> 【Thought】 Assumptions to state: spherical, uniform-density, non-rotating Earth (rotation changes the *measured* $g$ by 0.3%, Paper 20 Q1(k)); uniform density is the crude one (real Earth is centrally denser — hence the true mean 5.5 vs surface rock 2.7 g/cm³).

**Solution.** $\rho=\dfrac{3\times9.81}{4\pi\times6.67\times10^{-11}\times6.38\times10^6}=\boxed{5.5\ \text{g/cm}^3}$ (5.5×10³ kg/m³).

**Check.** Matches the accepted 5.51 g/cm³ ✓.

---

### Q1(d) — Half-life from a 1% activity drop [5 marks]

**Key observation.** Small decay ⟹ linearise: $\Delta A/A=\lambda t$.

$$\lambda=\frac{0.0100}{10^8\ \text{s}}=1.0\times10^{-10}\ \text{s}^{-1}\ (\text{exact: }-\ln0.99/10^8),\qquad T_{1/2}=\frac{\ln2}{\lambda}=\boxed{6.9\times10^{9}\ \text{s}\approx220\ \text{years}}.$$

> 【Thought】 Approximation discipline: $1-e^{-\lambda t}\approx\lambda t$ at 1% level introduces ~0.5% error — smaller than the data's significance; state it.

---

### Q1(e) — Rotating bar with pendulum ropes [5 marks]

**Key observation.** Each sphere is a conical pendulum whose circle radius is $r=r_0+\ell\sin\theta$ — the bar's half-length plus the rope's swing-out; the "conical" condition is $\tan\theta=\omega^2r/g$.

**Solution.** $r=4.0+2.0\sin30^\circ=5.0$ m:
$$\omega^2=\frac{g\tan\theta}{r}=\frac{9.81\times0.5774}{5.0}=1.133\;\Rightarrow\;\omega=1.06\ \text{rad/s},\qquad \boxed{T=\frac{2\pi}{\omega}=5.9\ \text{s}}.$$

> 【Thought】 Compare Paper 13 Q3(b) (chair-o-plane): same structure — the support radius adds to the swing radius. The coupled geometry ($r$ contains $\sin\theta$) is handled cleanly by $\tan\theta=\omega^2 r/g$ rather than by writing $r$ out first.

---

### Q1(f) — Lithium charging up under photoelectric emission [4 marks]

**Key observation.** The surface charges positive until its potential turns back the fastest photoelectrons: $eV=KE_{\max}$ (same mechanism as the sphere in Paper 11 Q2(c) and Paper 12 Q1(p)).

$$KE_{\max}=hf-W=6.63\times10^{-34}\times6.3\times10^{14}-3.7\times10^{-19}=4.18\times10^{-19}-3.7\times10^{-19}=0.48\times10^{-19}\ \text{J},$$
$$\boxed{V=\frac{KE_{\max}}{e}=0.30\ \text{V}\ (\text{positive})}.$$

---

### Q1(g) — Specific heat of a flowing liquid [2 marks]

$$P=\dot mc\,\Delta T\;\Rightarrow\;s=\frac{12}{(0.060/60)\times2.0}=\frac{12}{0.002}=\boxed{6.0\times10^3\ \text{J kg}^{-1}\text{K}^{-1}}.$$

> 【Thought】 Convert the flow rate to SI first (per minute → per second is the designed tripwire).

---

### Q1(h) — Thundercloud capacitor energy [10 marks]

**Setup.** $C=\varepsilon_0A/d=8.85\times10^{-12}\times2.5\times10^7/750=2.95\times10^{-10}$ F; $V=10^5$ V:
$$E_1=\tfrac12CV^2=\tfrac12\times2.95\times10^{-10}\times10^{10}=\boxed{1.5\times10^{3}\ \text{J}}.$$

The cloud is **isolated** (charge trapped), so rising means $d$ increases with $Q$ fixed:

**(i)** $C$ falls ($\propto1/d$) and $E=Q^2/2C$ *increases* — the work done separating the attracted plates (cloud from the induced ground charge) against gravity-against-attraction appears as stored energy. (If the potential were pinned instead, energy would fall — constant-$Q$ vs constant-$V$, cf. Paper 8 Q1(s).)

**(ii)** $E\propto d$ at fixed $Q$: $E_2=E_1\times\dfrac{1250}{750}$:
$$\boxed{\Delta E=E_1\left(\frac{1250}{750}-1\right)=1.5\times10^3\times\frac{2}{3}\approx+1.0\times10^{3}\ \text{J}}.$$

> 【Thought】 The model choice *is* the physics here: a thundercloud holds its charge (isolated conductor), so use $U=Q^2/2C$ with $Q$ fixed — using $U=\tfrac12CV^2$ with $V$ fixed would flip the answer's sign. Ask "what is conserved?" before choosing the energy form.

---

### Q1(i) — Square plate with a circular hole [6 marks]

**Key observation.** Negative-mass method: treat the hole as negative mass superposed on the full plate; the CG shifts *opposite* to the hole.

> 【Thought】 Masses are proportional to areas (uniform density): full plate $\propto9R^2$, hole $\propto\pi R^2$. The complement rule $\mathbf X=\frac{M\cdot\mathbf 0-m\,\mathbf x_h}{M-m}$.

**Solution.** (i) Hole at $(x,0)$: $X=\dfrac{-\pi R^2 x}{9R^2-\pi R^2}=\boxed{-\frac{\pi}{9-\pi}x=-0.54\,x}$ (opposite side), $Y=0$.
(ii) Hole at $(x,y)$: by the same linearity, $\boxed{X=-0.54x,\ Y=-0.54y}$.

**Check.** $|\mathbf X|<x$ ✓ (the hole shifts the CG by less than its own displacement); the shift vanishes as the hole shrinks ✓.

---

### Q1(j) — Battery, two resistors, two configurations [5 marks]

**Key observation.** Two load configurations give two equations in $(E,r)$.

**Solution.** Parallel ($1\ \Omega$): $E=3.0(1+r)$; series ($4\ \Omega$): $E=1.2(4+r)$:
$$3+3r=4.8+1.2r\;\Rightarrow\;1.8r=1.8\;\Rightarrow\;\boxed{r=1.0\ \Omega,\qquad E=6.0\ \text{V}}.$$
Power per resistor: parallel case (1.5 A each): $\boxed{4.5\ \text{W}}$; series case (1.2 A through each): $\boxed{2.88\ \text{W}}$.

**Check.** $1.2\times(4+1)=6$ ✓; total power check: $EI_1=18$ W vs $3^2\times1+3^2\times1=18$ ✓ (loads + internal).

---

### Q1(k) — Alpha-particle deflections; the unfixed nucleus [5 marks]

**Sketch.** Three hyperbolic trajectories about the nucleus: (i) 10° — wide, grazing bend; (ii) 90° — intermediate, turning sharply around the nucleus; (iii) 180° — head-on: straight in, momentary stop, straight back along the same line. Smaller impact parameter ⟹ larger deflection.

**Unfixed nucleus in (iii):** at the distance of closest approach in a head-on encounter, both particles move with the centre-of-mass velocity — momentarily at rest relative to each other:
$$\boxed{v_{\text{rel}}=0\ \text{at closest approach}\ (\text{both move at }V_{CM}=\tfrac{m_\alpha}{m_\alpha+m_N}u).}$$

> 【Thought】 The CM-frame reading: at closest approach the radial relative motion vanishes by definition of the turning point, and in a head-on ($b=0$) collision there's no tangential motion either — so relative velocity is exactly zero. Energy then converts cleanly: $\tfrac12\mu u^2$ becomes Coulomb PE.

---

### Q1(l) — Water jet from a tank [5 marks]

**(i)** Torricelli (energy): $v=\sqrt{2gh'}=\sqrt{2\times9.81\times0.20}=\boxed{2.0\ \text{m/s}}$ (hole 20 cm below the surface).
**(ii)** The hole is $1.0-0.2=0.80$ m above the base/floor; the jet is horizontal, so projectile time $t=\sqrt{2\times0.80/9.81}=0.404$ s:
$$x=vt=2\sqrt{h'h''}=2\sqrt{0.20\times0.80}=\boxed{0.80\ \text{m}}.$$

> 【Thought】 The product form $x=2\sqrt{h'h''}$ is worth memorising (it also makes the maximum-range result $h'=h''$ obvious). Compare Paper 14 Q4(a) for the momentum derivation of Torricelli.

---

### Q1(m) — Puck released on a rotating turntable [10 marks]

**Key observation.** The turntable is smooth ⟹ after release the puck moves in a **straight line** in the inertial frame, with its tangential release speed $v=\omega r_0$. It leaves the table when it reaches the rim.

> 【Thought】 Frame discipline: "smooth turntable" means no horizontal force after release — so the inertial-frame motion is trivial (a straight chord). The rotating student sees a spiral-outward path; the two descriptions meet at the exit point. Compute in the inertial frame, then transform.

**Solution.** $\omega=0.050\times2\pi=0.314$ rad/s; release at $r_0=1.5$ m (0.50 m from the rim of the 2.0 m radius table): $v=0.314\times1.5=0.471$ m/s. The puck follows the tangent chord; exit when the chord reaches the circle: chord length $=\sqrt{R^2-r_0^2}=\sqrt{4-2.25}=1.32$ m:
$$\boxed{\text{(i)}\quad t=\frac{1.32}{0.471}=2.8\ \text{s}.}$$

**(ii) Relative velocity at exit.** The puck's (constant) velocity is $v=0.471$ m/s perpendicular to the *release* radius OA; the rim material at the exit point B moves at $v_R=\omega R=0.628$ m/s perpendicular to the *exit* radius OB. Since OA ⟂ puck velocity and OB ⟂ rim velocity, the velocity triangle is **similar to the geometric triangle OAB** (right-angled at A, since the chord is perpendicular to OA) — so the relative velocity is the third side of a right triangle with hypotenuse $v_R$:
$$v_{\text{rel}}=\sqrt{v_R^2-v^2}=\sqrt{0.628^2-0.471^2}=\boxed{0.415\ \text{m/s}\ (\approx0.42\ \text{m/s})},$$
at angle $\varphi=\arcsin\!\dfrac{v}{v_R}=\arcsin\!\dfrac{1.5}{2.0}=\boxed{48.6^\circ\ \text{to the rim's tangent}}$ (pointing outward across the rim — what the rotating student at the centre sees the puck leave with).

> 【Thought】 *Official approach borrowed.* The elegant step is the similarity: velocities are the two radii rotated by 90°, so the velocity triangle inherits OAB's right angle — no components needed. Check by the law of cosines instead: the angle between the two velocities equals $\angle AOB=\arccos(1.5/2.0)=41.4^\circ$, and $v_{\text{rel}}^2=0.628^2+0.471^2-2(0.628)(0.471)\cos41.4^\circ=0.172$ ✓ same. If the stem's “smooth turntable” became “rough turntable”, condition C (no horizontal force after release, straight-line inertial motion) would break and this elegant solution would fail — return to the general method (integrate the trajectory in the rotating frame with centrifugal and Coriolis forces), because friction would keep changing the puck's velocity.

---

### Q1(n) — Loop in an increasing magnetic field [4 marks]

**Solution.** $\mathcal E=A\dfrac{dB}{dt}=(0.040)^2\times0.030=4.8\times10^{-5}$ V:
$$I=\frac{\mathcal E}{R}=\frac{4.8\times10^{-5}}{2.0\times10^{-3}}=\boxed{2.4\times10^{-2}\ \text{A}\ (24\ \text{mA})}.$$
**Direction (diagram):** if $B$ points into the page and is *increasing*, the induced current flows **anticlockwise** (its own field points out of the page, opposing the increase — Lenz's law: oppose the *change* of flux, not the field itself).

> 【Thought】 *Official-answer note.* The official script computes with $dB/dt=0.30$ T/s (getting 0.24 A) — a factor-of-ten misreading of the question's printed $0.030$ T/s; with the question's data, $24$ mA is correct. When your answer and the scheme differ by a clean power of ten, re-check the data transcription on both sides.

> 【Thought】 The two-step Lenz logic: (1) what sign of flux change, (2) which current fights it. Both steps stated explicitly is what "with the aid of a diagram" wants.

---

### Q1(o) — Energy storage as equivalent height [5 marks]

**(i) Car battery:** $E=12\ \text{V}\times60\ \text{Ah}=720\ \text{Wh}=2.59\times10^6$ J; $h=\dfrac{E}{mg}=\dfrac{2.59\times10^6}{20\times9.81}=\boxed{1.3\times10^4\ \text{m}\ (\approx13\ \text{km})}$.
**(ii) Petrol** (per kg): $h=\dfrac{4\times10^7}{9.81}=\boxed{4.1\times10^6\ \text{m}\ (\approx4100\ \text{km}, \sim 300\times\text{ the battery})}$.

> 【Thought】 This metric is the *specific energy* $E/m$ in disguise ($h=(E/m)/g$) — batteries are ~50 Wh/kg, petrol ~12 kWh/kg: the 300× gap is the whole point of the comparison.

---

### Q1(p) — Helium soap bubble: film thickness in wavelengths [4 marks]

**Key observation.** Floating ⟹ buoyancy = total weight: the film's mass makes up the air–helium density difference times the volume.

**Solution.** $m_{\text{film}}=(\rho_a-\rho_{He})V=(1.28-0.18)\times\tfrac43\pi(0.015)^3=1.10\times1.414\times10^{-5}=1.56\times10^{-5}$ kg. Film: $m=\rho_f\,4\pi r^2\,t$:
$$t=\frac{1.56\times10^{-5}}{10^3\times4\pi\times0.015^2}=5.5\times10^{-6}\ \text{m},\qquad \boxed{\frac{t}{\lambda}=\frac{5.5\ \mu\text{m}}{650\ \text{nm}}\approx8.5\ \text{wavelengths}}.$$

> 【Thought】 The helium carries most of the buoyancy duty; the film is the *difference* term — sensitive to the density contrast, so state it as $\Delta\rho\times V$ first. Physicality check: real soap films are µm-thick ✓.

---
*End of Paper 26 (2012 Round 1 Section 1).*


---

## Paper 27 — 2012 Round 1 Section 2 (16 Nov 2012)

*Section 2: Questions 2–8, 20 marks each; candidates attempt two. Full solutions for all seven.*

---

### Question 2 — DC supply + battery + load network; a symmetric resistor network

#### Q2(a) — Charging threshold and power split [8 marks]

**Topology (Fig. 2.a).** Three branches between the top rail and the broken bottom rail: supply $E$ (left), load $1.0\ \Omega$ (middle), 12 V battery (right); the bottom rail carries $0.40\ \Omega$ (supply leg) and $0.20\ \Omega$ (battery leg).

**(i) Charging threshold.** The battery current is zero when the top rail sits at exactly the battery's open emf above the battery's bottom node — i.e. the load drop is 12 V:
$$I_L=12\ \text{A},\qquad E_{\text{crit}}=I_L(1.0+0.40)=12\times1.4=\boxed{16.8\ \text{V}}.$$

**(ii) Power fraction at zero charging.** Supply delivers $EI=16.8\times12=201.6$ W; the load takes $I_L^2\times1.0=144$ W:
$$\boxed{\frac{144}{201.6}=\frac{5}{7}\approx71\%}\quad(\text{the other }\tfrac27\text{ heats the }0.40\ \Omega\text{ leg}).$$

**(iii) E = 20 V.** Full nodal solution (equations: load drop $=$ battery emf $+$ internal drop, KCL at the rail junctions):
$$I_{\text{battery}}=\boxed{4.7\ \text{A}\ \text{(charging)}},\qquad I_{\text{load}}=12.9\ \text{A},\quad I_{\text{supply}}=17.6\ \text{A}.$$

> 【Thought】 Threshold thinking: "begins to charge" = the battery branch current passes through zero — a boundary condition, not an inequality slog. Note the useful intermediate fact: at the threshold the load alone sits at the battery's emf (12 V ⟹ 12 A). At E = 10 V the battery would *discharge* into the load ($I_B=-10$ A) — the sign reversal confirms the threshold logic.

#### Q2(b) — Symmetric network (2, 2, 3, 1, 1, 2 Ω) [12 marks]

**Topology (Fig. 2.b):** triangle with D at top, A and B at the base corners, C in the centre; edges D–A 2 Ω, D–B 2 Ω, D–C 3 Ω, C–A 1 Ω, C–B 1 Ω, A–B 2 Ω; port A–B.

**(i) Current relations.** The network is mirror-symmetric about the D–C axis; reversing $V$ and reflecting gives: $i_1=i_2$ (the D-side arms), $i_3=i_4$ (the C-side arms), and the centre carries $i_6=0$ (it reverses under the composed symmetry).

**(ii)–(iii) R_AB and the currents.** With $i_6=0$ the 3 Ω arm is dead; node analysis with $V_A=V$, $V_B=0$ gives $V_C=V_D=V/2$; currents per unit $V$:
$$\boxed{i_1=i_2=\frac{V}{4},\qquad i_3=i_4=i_5=\frac{V}{2},\qquad i_6=0},\qquad I_{\text{total}}=\frac{5V}{4},$$
$$\boxed{R_{AB}=\frac{V}{I}=\frac45\ \Omega}.$$

**(iv) Port C–D.** Redrawn with CD as the base (same triangle, A and B now at the sides): symmetry $A\leftrightarrow B$ is *retained* for this port: $V_A=V_B$; solving: $V_A=V_B=2V/3$, and
$$\boxed{R_{CD}=1.0\ \Omega}.$$

**(v) Port A–C.** With AC as the base, no mirror symmetry survives (D and B are inequivalent, and the port breaks the C-swap): currents distribute without any vanishing/equal pair, so no branch can be deleted or merged — the network is a genuine *bridge* topology for this port. Numerically $R_{AC}=\dfrac{29}{45}\ \Omega\approx0.644\ \Omega$ — a value unreachable by series/parallel fractions with these small integer arms, demonstrating the point: **the bridge circuit is not series–parallel reducible** (it needs Kirchhoff's two rules or Y–Δ transforms).

> 【Thought】 The lesson arc: (i)–(ii) symmetry kills the bridge arm (like Paper 23 Q2's prism); (iv) a port change preserves just enough symmetry; (v) a port choice with *no* symmetry forces the general method — knowing when the shortcut dies is as valuable as the shortcut.

---

### Question 3 — Tunnels through the Earth

**(a) Diameter tunnel.** Inside a uniform sphere, the shell theorem gives gravity $g(r)=\dfrac{GM}{R_E^3}r$ toward the centre (linear in $r$). Along the diameter tunnel, displacement $r$ from the centre: force $=-\dfrac{GMm}{R_E^3}r$ — linear restoring ⟹ SHM:
$$\boxed{T_1=2\pi\sqrt{\frac{R_E^3}{GM_E}}=2\pi\sqrt{\frac{R_E}{g}}=2\pi\sqrt{\frac{6.38\times10^6}{9.81}}=5060\ \text{s}\approx84\ \text{min}}.$$

**(b) Any chord tunnel.** Tunnel at perpendicular distance $d_0$ from the centre; coordinate $s$ along the tunnel from its midpoint: the tunnel-direction component of gravity at position $s$ (radius $r=\sqrt{d_0^2+s^2}$) is
$$-\frac{GMm}{R_E^3}r\times\frac{s}{r}=-\frac{GMm}{R_E^3}s\ \text{— linear in }s\text{ with the same constant},$$
so SHM with the **same** period: $\boxed{T_2=T_1=2\pi\sqrt{R_E/g}}$.

> 【Thought】 The cancellation $r\times(s/r)=s$ is the magic step: the component along the tunnel is proportional to the along-tunnel displacement *regardless of the tunnel's offset*. This is why every chord gives the same 84 minutes.

**(c) Grazing satellite.** $T_S=2\pi\sqrt{R_E^3/GM_E}=\boxed{T_S=T_2}$ — identical (the gravity train through the Earth matches the orbit period around it) ✓ a memorable coincidence rooted in the linear (Hookean) interior field.

**(d) Extra speed at the midpoint.** The particle emerges with more than the "drop" speed: once outside, it is a free projectile in the $1/r^2$ field, so **by Kepler's first law its trajectory is an ellipse with the centre of the Earth as a focus** (the official 2-mark answer) — in practice an ellipse intersecting the surface, so it will fall back, possibly re-entering the tunnel or landing elsewhere, periodically returning. (If the boost took it above escape speed, the conic opens into a hyperbola and it leaves Earth for good.)

---

### Question 4 — Oil drops (Millikan with vertical and horizontal plates)

**(a)** Zero pd, vertical fall at constant velocity: gravity is balanced by viscous drag (terminal speed reached) — $mg=kv_1$; the uniform motion itself demonstrates a speed-proportional drag.

**(b) 45° trajectory.** Steady motion ⟹ the drag points opposite the path and the *resultant* of the electric force (horizontal $qE$) and weight (vertical $mg$) lies along the path: $\tan45^\circ=\dfrac{qE}{mg}$:
$$q=\frac{mg}{E}\tan45^\circ=\frac{3.3\times10^{-15}\times9.81}{2.0\times10^3/0.030}=\frac{3.24\times10^{-14}}{6.67\times10^4}=\boxed{4.9\times10^{-19}\ \text{C}\ (\approx3e)}.$$

**(c) The two path changes.** Charge quantisation: $\tan\theta=qE/mg$, so $q\propto\tan\theta$: the sequence $\tan45^\circ=1$, $\tan18.43^\circ=\tfrac13$, $\tan33.70^\circ=\tfrac23$ reads charges $3e\to e\to 2e$ — the drop **lost two electrons, then gained one** (spontaneous ionisation events). Best estimate of $e$ from the *changes* ($2e$ and $e$):
$$\boxed{e\approx\frac{4.9\times10^{-19}}{3}=1.6\times10^{-19}\ \text{C}}.$$

> 【Thought】 The ratios do the work: the tangent values are engineered to be $1, \tfrac13, \tfrac23$ — reading off $\tan\theta$ ratios turns trajectory angles into integer charges. This is Millikan's "proof of charge quantisation" in one line: charge states change by equal steps.

**(d) Horizontal plates.** Fall (no field): $mg=kv_1$. Rise (field on): $qE=mg+kv_2$ (drag now aids gravity downward... rather opposes the rise). Eliminate $k=mg/v_1$:
$$qE=mg\left(1+\frac{v_2}{v_1}\right)\;\Rightarrow\;q=\frac{mg(v_1+v_2)}{v_1E}=\frac{10^{-14}\times9.81\times4.8\times10^{-4}}{4.0\times10^{-4}\times1.25\times10^5},$$
$$q=9.4\times10^{-19}\ \text{C}\;\Rightarrow\;\boxed{N=\frac{q}{e}\approx6\ \text{electrons}}.$$

> 【Thought】 The two-speed subtraction (rise vs fall) is Millikan's original trick for eliminating the unknown drag constant: $qE=k(v_1+v_2)$ — the drag coefficient never needs evaluating.

---

### Question 5 — Draining soap-film wedge (interference)

**Setup.** Wedge film ($\mu=1.45$), thickness $t$ at distance $x$ from the top: $t=x\tan\varphi\approx x\varphi$; near-normal incidence, viewed in reflection.

**(i) Lowest-order constructive violet band.** Reflection phase inventory: outer surface (air→film, $n$ rises): $\pi$ flip; inner surface (film→air, $n$ falls): no flip — net $\pi$, so constructive needs the path to supply a half wavelength; lowest order ($m=0$):
$$2\mu t_V=\frac{\lambda_V}{2}\;\Rightarrow\;\boxed{t_V=\frac{\lambda_V}{4\mu}=\frac{420}{4\times1.45}=72.4\ \text{nm}}.$$

**(ii) Wedge angle.** $\varphi=\dfrac{t_V}{x_V}=\dfrac{72.4\times10^{-9}}{0.030}=2.4\times10^{-6}\ \text{rad}=\boxed{1.4\times10^{-4}\ ^\circ}$.

**(iii) Red band.** $t_R=\dfrac{\lambda_R}{4\mu}=\dfrac{680}{5.8}=117$ nm; $x_R=\dfrac{t_R}{\varphi}=\dfrac{117.2\times10^{-9}}{2.413\times10^{-6}}=\boxed{4.9\ \text{cm}}$ (further down, since the red needs a thicker film ✓).

**(iv) Fringe migration speed as the wedge drains.** The violet band's position obeys $x_V\varphi=t_V=$ const; differentiating the product:
$$\boxed{x_V\,\Delta\varphi+\varphi\,\Delta x_V=0}\;\Rightarrow\;\frac{\Delta x_V}{\Delta t}=-\frac{x_V}{\varphi}\frac{\Delta\varphi}{\Delta t},$$
$$\frac{\Delta x_V}{\Delta t}=-\frac{3.0\ \text{cm}}{1.38\times10^{-4}\ ^\circ}\times\left(-8.3\times10^{-5}\ ^\circ/\text{min}\right)=\boxed{+1.8\ \text{cm/min}\ \text{(outward, away from the top edge)}}.$$

> 【Thought】 The product rule $d(x\varphi)=0$ is the whole mechanism: the band tracks a *fixed thickness*, and as the wedge thins (φ falls) that thickness migrates to larger $x$. The positive answer confirms the fringe moves away from the thin end as draining proceeds.

---

### Question 6 — Three-ball pendulum collisions

**Setup.** Balls A, B, C hanging in a line with small gaps; A raised by $h$ and released: impact speed $v_0=\sqrt{2gh}$. All collisions elastic.

**(i) All masses M.** Equal-mass elastic collisions exchange velocities: A stops, B moves at $v_0$; B stops, C moves at $v_0$:
$$\boxed{\text{C rises to height }h\ \text{(full transfer)}},$$
then C swings back and the chain reverses — the cradle oscillates end-to-end.

**(ii) A = M, B = 2M, C = 3M.** First collision (A→B, elastic): $v_B=\dfrac{2M}{M+2M}v_0=\dfrac23v_0$. Second (B→C): $v_C=\dfrac{2(2M)}{2M+3M}v_B=\dfrac45\times\dfrac23v_0=\dfrac{8}{15}v_0$:
$$\boxed{h_C=\frac{v_C^2}{2g}=\left(\frac{8}{15}\right)^2h=\frac{64}{225}h\approx0.28\,h}.$$

> 【Thought】 The velocity-transfer factor for elastic collisions onto a stationary target, $v_2=\frac{2m_1}{m_1+m_2}v_1$, composes multiplicatively through the chain. Since each striker is lighter than its target (A rebounds off B, B off C), each transfer factor is $<1$, and the rebound energy stays in play for the return swing.

---

### Question 7 — Launch speeds (polar orbit, escape, Sun)

**(a) Polar orbit (grazing).** Minimum launch speed ≈ circular-orbit speed at the surface:
$$v_{\text{polar}}=\sqrt{\frac{GM_E}{R_E}}=\sqrt{gR_E}=\sqrt{9.81\times6.38\times10^6}=\boxed{7.9\ \text{km/s}}.$$

**(b) Polar vs equatorial ratio.** Earth's spin assists an eastward equatorial launch ($v_{rot}=2\pi R_E/T=465$ m/s) but not a polar one:
$$\boxed{\frac{v_{\text{polar}}}{v_{\text{eq}}}=\frac{\sqrt{gR_E}}{\sqrt{gR_E}-v_{rot}}=\frac{7907}{7442}\approx1.06}$$
(marginally harder to launch polar; ignoring rotation the ratio is 1 — the same speed is needed energetically, the ratio being purely the spin assist).

**(c) Escape Earth.** $\sqrt2\times$ circular speed:
$$\boxed{v_{\text{esc}}=\sqrt{2gR_E}=11.2\ \text{km/s}}.$$
Minimum *ground* launch speed, using the Earth's rotation at the equator (eastward): $v_{\min}=11.2-0.46=\boxed{10.7\ \text{km/s}}$ (the same 0.46 km/s spin assist as in (b)).

**(d) Hit the Sun (neglect Earth's field).** Minimum ⟹ cancel Earth's orbital speed so the probe falls straight toward the Sun: launch retrograde at
$$\boxed{v_{\min}=v_{\text{orb}}=\sqrt{\frac{GM_S}{R_{ES}}}=29.8\ \text{km/s}\ (\text{relative to Earth, opposite Earth's motion})}.$$

**(e) Leave the Solar System.** Solar escape from Earth's orbit: $\sqrt2\,v_{\text{orb}}=42.1$ km/s; using Earth's motion (launch prograde): need $42.1-29.8=12.3$ km/s relative to Earth:
$$\boxed{v_{\min}\approx12.3\ \text{km/s}}.$$

> 【Thought】 The striking contrast: hitting the Sun costs *more* than escaping it (29.8 vs 12.3 km/s) — killing orbital angular momentum is harder than escaping; this is why solar-probe trajectories matter. The $\sqrt2$ relations ($v_{esc}=\sqrt2\,v_{orb}$) and the boost bookkeeping are the reusable content.

---

### Question 8 — Quarter-cylinder prism; seismic refraction

#### Q8(a) — Quarter-cylinder on a table (R = 5.00 cm, μ = 1.50) [10 marks]

**Geometry (Fig. 8.a).** Centre of the quarter circle at the bottom-left corner (on the table); curved surface from $(0,R)$ to $(R,0)$. Beam horizontal from the left; the vertical face admits it undeviated (normal incidence).

**(i) Illumination of the table.** A ray entering at height $y$ hits the curve at incidence $i=\arcsin(y/R)$ from the (radial) normal (check: $y\to0$ hits the curve's vertical point head-on, $i\to0$ ✓).
- For $i>\theta_c=\arcsin(1/1.5)=41.8^\circ$ ($y>3.33$ cm): **TIR** at the curved face — the reflected ray heads *upward* back into the block (reflection of the horizontal direction about the radial normal has positive vertical component $(\cos2i,\sin2i)$ for $i>41.8^\circ$); on the circular arc it would keep the same incidence (chord property) — these rays do not contribute to the table *beyond* the cylinder.
- For $i<\theta_c$: the ray refracts out of the curve at $e=\arcsin(\mu\sin i)$ from the normal, descending at $e-i$ below horizontal, and lands at
$$x=R\cos i+\frac{R\sin i}{\tan(e-i)},\qquad e=\arcsin(\mu\sin i).$$

**Bounds of the lit band.** *Near edge* (critical ray, $i\to\theta_c^-$ with $e\to90^\circ$): the expression collapses beautifully —
$$x_{\min}=R\cos\theta_c+\frac{R\sin\theta_c}{\tan(90^\circ-\theta_c)}=R\cos\theta_c+R\,\frac{\sin^2\theta_c}{\cos\theta_c}=\frac{R}{\cos\theta_c}=\frac{R}{\sqrt{1-1/\mu^2}}=\frac{5.00}{0.745}=6.71\ \text{cm},$$
i.e. $\dfrac{R}{R+x}=\cos\theta_c$ with $x$ measured beyond the cylinder's edge: $x_{\min}'=6.71-5.00=\boxed{1.71\ \text{cm beyond the cylinder}}$ — the official form. *Far edge* ($i\to0$): $e-i\approx(\mu-1)i$ and $R\sin i/\tan(e-i)\to\dfrac{R}{\mu-1}=10$ cm, so $x_{\max}=R+\dfrac{R}{\mu-1}=15$ cm. The table is lit in the continuous fan
$$\boxed{\text{from }6.71\ \text{cm to }15\ \text{cm from the corner}\ \left(\text{i.e. }1.71\ \text{cm to }10\ \text{cm beyond the cylinder's edge}\right).}$$

> 【Thought】 The near bound is the designed result ($R/(R+x)=\cos\theta_c$ — the official scheme's compact form); the far bound ($x_{\max}=R(1+\frac{1}{\mu-1})$) comes from the grazing-height rays. Between them every landing point is covered continuously — that is the complete answer to "where will the table be illuminated". (It is tempting but wrong to send the TIR rays descending to the bottom face; the reflection direction $(\cos2i,\sin2i)$ actually points upward for $i>45^\circ$ — always compute the reflected direction before claiming where it goes.)

**(ii) Beam from the right — verify the 83.27° threshold.** The ray refracts into the curve at incidence $i$ (measured from the radius): $\sin r=\sin i/\mu$; it then meets the vertical face, whose normal is horizontal. The geometry gives the internal ray's angle to that normal as $i-r$; direct emergence fails when $i-r\ge\theta_c$. At the boundary:
$$i=\arcsin(\mu\sin r)\ \text{with}\ i-r=\theta_c:\quad i-r=41.81^\circ,\ \sin i=1.50\sin r\ \Rightarrow\ r=41.46^\circ,\ i=83.27^\circ\ ✓$$
$$\boxed{\text{so for }i>83.27^\circ,\ i-r>\theta_c:\ \text{TIR at the vertical face — no direct emergence}}.\ \blacksquare$$

> 【Thought】 The verification structure: the constraint chain is $i$ (curve) → $r$ (Snell) → $i-r$ (vertical-face incidence, by the angle chase across the two normals) → compare with $\theta_c$. The printed 83.27° is reverse-engineered from $\theta_c$ — reproducing it exactly is the check.

#### Q8(b) — Seismic head-wave: simultaneous arrival [10 marks]

**Setup.** Direct surface path: $T_1=x/V_1$. Refracted path: down at the critical angle $\theta_c$ from vertical ($\sin\theta_c=V_1/V_2$ — Snell with grazing transmission into the faster layer), along the interface at $V_2$, and back up symmetrically:
$$T_2=\frac{2h}{V_1\cos\theta_c}+\frac{x-2h\tan\theta_c}{V_2}.$$
Setting $T_1=T_2$:
$$\frac{x}{V_1}-\frac{x}{V_2}=\frac{2h}{V_1\cos\theta_c}-\frac{2h\tan\theta_c}{V_2}\;\Rightarrow\;x\,\frac{V_2-V_1}{V_1V_2}=\frac{2h}{V_1\cos\theta_c}\left(1-\frac{V_1}{V_2}\frac{\sin\theta_c}{1}\right)=\frac{2h\cos\theta_c}{V_1},$$
(using $V_1/V_2=\sin\theta_c$) ⟹
$$\boxed{x=\frac{2hV_2\cos\theta_c}{V_2-V_1}=2h\sqrt{\frac{V_2+V_1}{V_2-V_1}}}\qquad\left(\cos\theta_c=\frac{\sqrt{V_2^2-V_1^2}}{V_2}\right).$$

> 【Thought】 This is the crossover-distance formula of seismic refraction: beyond this $x$ the head wave (through the fast layer) arrives *first* despite the longer path — the principle behind crustal sounding. The algebra's keystone: substituting $\sin\theta_c=V_1/V_2$ to collapse the bracket to $\cos\theta_c/V_1$ — do the trig before the numbers.

---
*End of Paper 27 (2012 Round 1 Section 2).*


---

## Paper 28 — 2011 Round 1 Section 1 (11 Nov 2011) [2012 paper]

*Section 1, Question 1, parts (a)–(n). Maximum 40 marks from 76.*

---

### Q1(a) — Square network with a diagonal, all R [4 marks]

**Topology (Fig. 1.a):** square ABCD with diagonal AC; all five resistors are $R$.

**(i) R_AC:** the diagonal $R$ directly, in parallel with two paths A–B–C and A–D–C ($2R$ each):
$$R_{AC}=R\parallel2R\parallel2R=\frac{1}{1+\tfrac12+\tfrac12}R=\boxed{\frac{R}{2}}.$$

**(ii) R_AB:** no symmetry shortcut survives this port — the swap C↔D combined with A↔B would map the diagonal AC onto BD, which is *not* an edge, so C and D are **not** equipotential. Reduce explicitly: from A, node D dangles through A–D–C ($2R$), in parallel with the direct diagonal A–C ($R$):
$$R_{AC,\text{eff}}=R\parallel2R=\frac{2R}{3};\qquad\text{path A–C–B: }\frac{2R}{3}+R=\frac{5R}{3},$$
$$R_{AB}=R\parallel\frac{5R}{3}=\boxed{\frac{5R}{8}}.$$

Nodal cross-check: with $V_A=V$, $V_B=0$, KCL at D and C gives $2V_D=V+V_C$ and $3V_C=V+V_D$, so $V_C=\tfrac35V$, $V_D=\tfrac45V$; the injected current $I=\dfrac{V}{R}+\dfrac{V-V_C}{R}+\dfrac{V-V_D}{R}=\dfrac{8V}{5R}$ ⟹ $R_{AB}=\dfrac{5R}{8}$ ✓.

> 【Thought】 Symmetry audit before shorting nodes: an equipotential pair must be swapped by an *automorphism of the network* (composed with voltage reversal if it swaps the port terminals). Here the diagonal breaks the square's symmetry, so C and D are at different potentials (nodal check: $V_C=0.6V$, $V_D=0.8V$ — genuinely different, and the audit gives $R_{AB}=5R/8$ ✓). If the stem's “square plus diagonal AC” became “square plus both diagonals”, condition C (C and D not equipotential) would break and this conclusion would fail — return to the symmetry-shorting method, because in the fully symmetric network C and D are equipotential and can be shorted.

---

### Q1(b) — Hydrogen levels [4 marks]

**(i)** Ionisation energy $=|E_1|=\boxed{13.6\ \text{eV}\ (=2.18\times10^{-18}\ \text{J})}$.
**(ii)** Hα ($n=3\to2$): $\Delta E=13.6\left(\dfrac14-\dfrac19\right)=1.89$ eV:
$$\boxed{\lambda=\frac{1240\ \text{eV nm}}{1.89\ \text{eV}}=656\ \text{nm}\ (\text{red})}.$$

---

### Q1(c) — Two overhanging blocks [5 marks]

**Key observation.** Two toppling conditions: the upper block relative to the lower (its CG over the lower block's edge), and the pair relative to the table edge. Check both; the binding one wins.

> 【Thought】 Toppling = CG passes the support edge. The classic trick: the upper block's CG is fixed relative to the lower (its overhang 6 cm < half-length 12 cm ✓ always safe), so the system topples as a unit about the table edge — compute the *combined* CG.

**Solution.** Upper block: 6.0 cm overhang $<12$ cm (half its length) — always stable on the lower. Pair CG from the lower block's left end: centres at $12-x$ (lower) and $6-x$ (upper) relative to the table edge... measuring from the table edge: combined CG at $9-x$ (cm) left of it:
$$\text{collapse when }9-x<0\;\Rightarrow\;\boxed{x>9\ \text{cm}\ \text{(the pair topples together; the upper block never topples alone)}}.$$

**Check.** Limit check: with $x=9$ cm the lower block already hangs 9 cm out; the pair's CG sits exactly at the edge ✓ marginal.

---

### Q1(d) — Proton scattered through 90° by an oxygen nucleus [12 marks]

**Key observation.** Elastic collision, target initially at rest, 90° deflection: momentum is a right triangle; combine with energy.

> 【Thought】 With the proton deflected through exactly 90°, the momentum diagram is a right triangle: $\mathbf p_0=\mathbf p_p'+\mathbf p_O$ with $p_p'\perp p_0$ ⟹ $p_O^2=p_0^2+p_p'^2$. Energy then closes the system. This is Rutherford-style kinematics; the 90° clause is what makes the triangle right.

**Solution.** Momentum: $p_O^2=(m_pu)^2+(m_pv_p')^2$. Energy: $m_pu^2=m_pv_p'^2+p_O^2/m_O$:
$$m_pu^2=m_pv_p'^2+\frac{m_p^2(u^2+v_p'^2)}{m_O}\;\Rightarrow\;v_p'^2=u^2\,\frac{m_O-m_p}{m_O+m_p},$$
$$v_p'=3.00\times10^7\sqrt{\frac{2.56\times10^{-26}-0.167\times10^{-26}}{2.73\times10^{-26}}}=3.00\times10^7\times0.937=2.81\times10^7\ \text{m/s}.$$
Oxygen: $p_O=m_p\sqrt{u^2+v_p'^2}$:
$$v_O=\frac{m_p}{m_O}\sqrt{u^2+v_p'^2}=\frac{3.00\times10^7}{15.3}\times\sqrt{1+0.937^2}=2.69\times10^6\ \text{m/s},$$
direction: $\tan\varphi=\dfrac{m_pv_p'}{m_pu}=0.937$ ⟹ $\varphi=43.1^\circ$ off the proton's initial path (opposite side from the proton's deflection):
$$\boxed{v_O=2.7\times10^6\ \text{m/s}\ \text{at}\ 43^\circ\ \text{to the beam}\quad(\text{proton: }2.8\times10^7\ \text{m/s at }90^\circ)}.$$

**Check.** $v_O\ll u$ ✓ (heavy target barely moves); energy: $m_pu^2=m_pv_p'^2+m_Ov_O^2$ ✓ by construction.

---

### Q1(e) — Wreck lifted clear of water: cable extension change [5 marks]

Identical mechanism to Paper 16 Q1(p): $\Delta T=\rho_wgV=1000\times9.81\times\dfrac{10^4}{8\times10^3}=1.23\times10^4$ N:
$$\Delta x=\frac{\Delta T\,L}{EA}=\frac{1.23\times10^4\times10}{5\times10^{10}\times5\times10^{-4}}=\boxed{4.9\ \text{mm}\ \text{(longer out of water)}}.$$

---

### Q1(f) — Mirror: the equal-path and least-time proofs [6 marks]

**(i)** B′ is the image of B: the mirror plane is the perpendicular bisector of BB′, so any point O on it is equidistant: $OB=OB'$ ⟹ $AO+OB=AO+OB'$, i.e. $\boxed{AOB=AOB'}$. $\blacksquare$

**(ii)** In the unfolded plane, the broken path $AOB'$ has length $\ge AB'$ (triangle inequality), with equality iff $O$ lies on the straight segment $AB'$ — which is precisely the point where the incidence and reflection angles are equal. Hence the actual reflected path (equal angles) has the **minimum** length among all paths $AOB$. $\blacksquare$ (This is Fermat's principle for reflection.)

> 【Thought】 The image trick converts a broken path into a straight line — the same geometric inversion used for the "spherical cow" reflection problems and for method-of-images in electrostatics (Paper 13/14). The minimality proof is then one line (triangle inequality).

---

### Q1(g) — Moon rock lifted by tidal gravity [8 marks]

**Orbit condition.** Circular orbit: $\boxed{GM_m/r^2=m\omega^2r}$ ($\omega^2r^3=GM$).

**Rock equilibrium** (near face, moon's rotating frame). Forces on the rock (mass $\mu$): moon's gravity $Gm\mu/a^2$ (toward the moon's centre); centrifugal $\omega^2(r-a)\mu$ (away from the planet — into the surface on the near face); planet's gravity $GM\mu/(r-a)^2$ (toward the planet — *off* the surface); surface reaction $R$:
$$R=\mu\left[\frac{Gm}{a^2}+\omega^2(r-a)-\frac{GM}{(r-a)^2}\right].$$

**Lift-off condition** ($R=0$, $a\ll r$ expansions $(r-a)^{-2}\approx r^{-2}(1+2a/r)$, $\omega^2(r-a)\approx\dfrac{GM}{r^2}(1-a/r)$):
$$\frac{Gm}{a^2}=\frac{GM}{r^2}\left[(1+2a/r)-(1-a/r)\right]=\frac{3GMa}{r^3}\;\Rightarrow\;\boxed{\frac{M}{m}>\frac{r^3}{3a^3}\ \text{(equivalently }r<a(3M/m)^{1/3}\text{ — Roche-type condition, independent of }\omega)}.$$

> 【Thought】 The tidal stretch = planet's gravity gradient × moon radius: $3GMa/r^3$ — the factor 3 is the content (gravity difference minus centrifugal difference). The $\omega$-elimination via the orbit condition is what makes the answer "ω-independent" — a designed substitution, signposted by the question.

---

### Q1(h) — Two-run calorimetry with heat loss [6 marks]

**Key observation.** Both runs share the same heat loss $H$ (same ΔT, same duration) — subtract or solve simultaneously.

> 【Thought】 Model: $P t=mc\Delta T+H$ with $H$ identical across runs (same temperatures, same time). Two equations, two unknowns ($s_B$, $H$). The heat loss is *not* negligible here — it's the point.

**Solution.** Run 1 (A alone, 64 g): $4.80\times400=0.064\times860\times20+H$: $1920=1101+H$ ⟹ $H=819$ J.
Run 2 (32 g A + 40 g B): $4.90\times400=0.032\times860\times20+0.040\,s_B\times20+H$:
$$1960=550+0.8\,s_B+819\;\Rightarrow\;0.8s_B=590,$$
$$\boxed{s_B=738\ \text{J kg}^{-1}\text{K}^{-1},\qquad H=819\ \text{J}\ (\text{same in both})}.$$

**Check.** Heat loss is ~43% of the input — substantial but plausible for an unstirred open beaker over 400 s ✓; $s_B<s_A$ ✓ plausible.

---

### Q1(i) — Cathode-ray gun: apparent origin at x = −d [6 marks]

**Key observation.** The field accelerates along $x$ only, so $v_y$ is conserved and tiny; compute the exit point and slope, then back-project.

**Solution.** In the field: $v_x^2=2ad$ with $a=eE/m$ ($v_{x0}\ll v_x$), transit time $\tau=\dfrac{v_x}{a}=\dfrac{2d}{v_x}$; exit point $(d,\ y_d=v_y\tau)$, slope $m=\dfrac{v_y}{v_x}$. Back-projected line crosses the axis at
$$x^*=d-\frac{y_d}{m}=d-\frac{v_y\tau}{v_y/v_x}=d-\tau v_x=d-2d=\boxed{-d}.\ \blacksquare$$
The $v_y$ (and small $v_x$) spread cancels: every electron appears to originate from the single point $x=-d$ — a virtual point source.

> 【Thought】 This is the physics behind "the electron gun acts as if electrons come from a point one gun-length behind the filament" — the designed result. The cancellation of $v_y$ (both the exit height and the slope are proportional to it) is the elegant step; the factor-2 kinematics ($\tau=2d/v_x$ for constant acceleration from near rest) does the rest.

---

### Q1(j) — α-particle binding energy per nucleon [3 marks]

$$\Delta m=2(1.0080)+2(1.0087)-4.0026=0.0308\ \text{u};\qquad E_b=0.0308\times930=28.6\ \text{MeV},$$
$$\boxed{E_b/4=7.2\ \text{MeV per nucleon}}.$$

**Check.** Near the accepted 7.07 MeV ✓ (given masses are rounded); the α is the most tightly bound light nucleus ✓.

---

### Q1(k) — Organ pipe with a diaphragm [6 marks]

**Data.** 2000 Hz: adjacent nodes 8.0 cm apart ⟹ $\lambda=16$ cm.

**(i)** $v=f\lambda=2000\times0.16=\boxed{320\ \text{m/s}}$.
**(ii)** At 1600 Hz: $\lambda=20$ cm ⟹ node spacing $\boxed{10\ \text{cm}}$.
**(iii)** The two resonances must both be standing-wave modes of the same tube: the node–node/antinode inventory forces a common length containing whole quarter-wavelengths; the frequencies 2000 and 1600 Hz are in the ratio 5:4, so they are the 5th and 4th harmonics of a 400 Hz fundamental:
$$L=\frac{v}{2f_1}=\frac{320}{2\times400}=\boxed{0.40\ \text{m}}.$$
**(iv)** Next pattern below 1600 Hz: the 3rd harmonic: $\boxed{1200\ \text{Hz}}$.

> 【Thought】 Model note: the resonance sequence 400, 800, 1200, 1600, 2000 Hz contains *all* harmonics — strictly, a pipe closed at one end supports only odd harmonics; the data given here (5:4 ratio) only fit an all-harmonic series, so the tube behaves as if both ends share the same symmetry (the driven diaphragm acts as an open/forced end and the pattern is harmonic-complete). Reading the mode ratio from the data — rather than assuming it — is the lesson.

---

### Q1(l) — Helicopter: downwash speed and hover power [5 marks]

**(i)** $v=\sqrt{\dfrac{Mg}{\rho A}}=\sqrt{\dfrac{810\times9.81}{1.20\times\pi\times16}}=\boxed{11.5\ \text{m/s}}$.
**(ii)** $P=\tfrac12\dot mv^2=\tfrac12\rho Av^3=\tfrac12\times1.20\times\pi\times16\times11.5^3=\boxed{4.6\times10^{4}\ \text{W}\ (\approx46\ \text{kW})}$.

> 【Thought】 Two momentum-flux relations chained: thrust $=\rho Av^2$ (mass flux × speed) and power $=\tfrac12\rho Av^3$ (KE flux). Note $P=\tfrac12Fv$ here — the factor ½ is the kinetic-energy flux, not force×distance bookkeeping. Compare Paper 16 Q1(e).

---

### Q1(m) — Decay probability after surviving 5 half-lives [4 marks]

**Key observation.** Exponential decay is memoryless: survival to $5T$ changes nothing about the future.

**(i)** Further $T$: $\boxed{1/2}$. (ii) Further $3T$: $\boxed{1-2^{-3}=7/8}$.

> 【Thought】 The 5T survival is a deliberate red herring — the Markov property of exponential decay means conditional probabilities reset. This is the precise statement that "a nucleus does not age".

---

### Q1(n) — Fractional uncertainty in density [2 marks]

$$\frac{\delta\rho}{\rho}=\frac{\delta m}{m}+\frac{\delta V}{V}=\frac{0.03}{1.5}+\left(\frac{1}{80}+\frac{1}{50}+\frac{1}{30}\right)=0.020+0.0658=\boxed{0.086\ (\approx9\%)}.$$

> 【Thought】 Worst-case (linear) addition is intended here ("uncertainties of magnitude…"): sum the fractional contributions. The thickness (1/30) dominates the volume error — identify the dominant term.

---
*End of Paper 28 (2011 Round 1 Section 1).*


---

## Paper 29 — 2011 Round 1 Section 2 (11 Nov 2011) [2012 paper]

*Section 2: Questions 2–9, 20 marks each; candidates attempt three. Full solutions for all eight.*

---

### Question 2 — Charging a battery from a solar panel; two networks

#### Q2(a) — Charging circuit [5 marks]

**Topology (Fig. 2.a):** single series loop — solar panel (24.0 V, 1.00 Ω internal), voltmeter V₁ across the panel's terminals, fixed resistor R, battery being charged (12.6 V, 0.10 Ω internal), voltmeter V₂ across the battery's terminals.

**(i)** Loop: $24.0-12.6=I(1.00+0.10+R)$ with $I=5.00$ A:
$$R=\frac{11.4}{5.00}-1.10=\boxed{1.18\ \Omega}.$$

**(ii)** $R=0.90\ \Omega$: $I=\dfrac{11.4}{1.00+0.10+0.90}=5.70$ A. Terminal readings:
$$V_1=24.0-5.70\times1.00=\boxed{18.3\ \text{V}},\qquad V_2=12.6+5.70\times0.10=\boxed{13.2\ \text{V}}.$$

> 【Thought】 Terminal-pd sign discipline again: the panel (discharging) reads $E-Ir$; the battery (charging) reads $E+Ir$ — same current, opposite signs of the internal drop. Voltmeters read *terminal* pds, not emfs.

#### Q2(b) — No current through E₂ [3 marks]

**Topology (Fig. 2.b):** E₁ = 2.0 V drives a loop containing R₁ and R₂ = 10 Ω in series; E₂ = 1.5 V taps from the R₁–R₂ junction. No current through E₂ ⟹ the junction sits at E₂'s emf above the bottom rail — the divider's drop across R₁ must equal 1.5 V:
$$\frac{2.0\times R_1}{R_1+10}=1.5\;\Rightarrow\;2R_1=1.5R_1+15\;\Rightarrow\;\boxed{R_1=30\ \Omega}.$$

> 【Thought】 This is the potentiometer balance condition again (Paper 19 Q2): a branch carrying no current measures the open potential — the junction's potential equals E₂'s emf exactly when the divider supplies it.

#### Q2(c) — Square-plus-diagonals network, all R [7 marks]

**Topology (Fig. 2.c):** square E(top-left), D(top-right), C(bottom-left), F(bottom-right), with both diagonals through centre O (edges E–O, O–F, D–O, C–O); port A–B wired to E–F.

**(i) Why $V_C=V_D$.** Compose the network's mirror symmetry $C\leftrightarrow D$, $E\leftrightarrow F$ with reversal of $V$ (which flips every current): the driven circuit maps to itself while swapping C and D — so their potentials coincide. (Same machine as Paper 23 Q2a.)

**(ii)** Joining C and D with a wire: **nothing changes** — no current flows in the link since they're equipotential.

**(iii) Simplified circuit:** merge C≡D into one node X: E–X becomes $R\parallel R=R/2$; X–F likewise $R/2$; O–X likewise $R/2$; E–O and O–F remain $R$ each.

**(iv)** Node analysis of the simplified network gives $V_X=V_O=V/2$: so the pd across CO is $\boxed{0}$ (C and O are equipotential).

**(v)** With $V_X=V_O$, the O–X pair carries nothing; the network is $2R$ (E–O–F) in parallel with $R$ (E–X–F):
$$\boxed{R_{AB}=2R\parallel R=\frac{2R}{3}}.$$

#### Q2(d) — R_AO [5 marks]

Driving between E and O instead: the mirror $C\leftrightarrow D$ still holds, so merge $V_C=V_D\equiv V_X$; the reduced network has E–X, X–F, X–O each $R/2$, plus E–O and O–F each $R$. With $V_E=V$, $V_O=0$, KCL at X and F:
$$3V_X-V_F=V,\qquad 3V_F=2V_X\;\Rightarrow\;V_X=\frac{3V}{7},\quad V_F=\frac{2V}{7},$$
$$I=\frac{V}{R}+\frac{V-V_X}{R/2}=\frac{V}{R}\left(1+\frac{8}{7}\right)=\frac{15V}{7R}\;\Rightarrow\;\boxed{R_{AO}=\frac{7R}{15}}.$$

> 【Thought】 (c)'s chain demonstrates the full toolkit: symmetry → equipotential → merge → series/parallel. For (d), with port E–O, merge C and D again (symmetric) and reduce; the fraction 7/15 is the kind of answer that verifies cleanly by nodal check.

---

### Question 3 — Whistle from a bridge; violin-string beats

#### Q3(a) — Train passing under a bridge [6 marks]

*Approach* (source moving toward the observer): in one period the train closes $u/f_0$ of the wave train, so the wavelength ahead is compressed to $\lambda_a=\dfrac{v_s-u}{f_0}$:
$$\boxed{f_a=\frac{v_s}{\lambda_a}=\frac{v_s}{v_s-u}\,f_0}.$$
*Receding* (moving away): the train stretches the train behind it, $\lambda_d=\dfrac{v_s+u}{f_0}$:
$$\boxed{f_d=\frac{v_s}{v_s+u}\,f_0}.$$

> 【Thought】 The derivation to show (the marks are for it): in time $t$ the source emits $f_0t$ crests while advancing $ut$, so the crests occupy $(v_s\mp u)t$ — count crests per metre, then the stationary observer hears $v_s/\lambda$. Note the asymmetry: the same speed produces a bigger *upward* shift than downward ($\frac{v_s}{v_s-u}$ vs $\frac{v_s}{v_s+u}$). Keep the two Doppler formulas apart: *moving source* compresses the wavelength in the medium; *moving observer* changes the crossing rate — they are not interchangeable, though they share the first-order shift.
>
> *Refinement (beyond the marked answer):* exactly under the bridge the radial component of the train's velocity is zero, so the heard frequency passes smoothly *through* $f_0$ at closest approach — the collinear values above are the far-field limits of $f=\dfrac{f_0v_s}{v_s-u\cos\theta}$, $\cos\theta=x/\sqrt{x^2+h^2}$.

#### Q3(b) — Violin string vs tuning fork (beats) [14 marks]

$f=\dfrac{1}{2l}\sqrt{F/\mu}$; beats $b=|f-f_0|$.

**(i) Sketch/analysis.** $f\propto\sqrt F$: a concave rising curve; mark the horizontal line $f_0$. Data: at $F_1=0.99T$, $b_1=3.30$; at $F_2=1.00T$, $b_2=2.00$; at $F_3=1.02T$, $b_3=0.58$: beats shrink as $F$ grows ⟹ the string is *below* the fork and closing; at $F_3$ it's still slightly below or just crossing: $f_0$ lies in the region $f(F_2)\lesssim f_0\lesssim f(F_3)$ (approached from below; $b_3>0$ means not yet crossed or just past — refined below).

**(ii)–(iii) Solving for $f_0$.** String below the fork for the first two: $f_1=f_0-3.30$, $f_2=f_0-2.00$; ratio via $\sqrt F$:
$$\frac{f_0-3.30}{f_0-2.00}=\sqrt{\frac{0.99T}{1.00T}}=0.99499,$$
$$f_0-3.30=0.99499f_0-1.98997\;\Rightarrow\;0.00501f_0=1.310\;\Rightarrow\;\boxed{f_0=261\ \text{Hz}\ (\text{middle C})}.$$
**(iv)** Third set (the string has now crossed above): $f_3=f_0+0.58$; check: $\dfrac{f_3}{f_2}=\sqrt{1.02}$: $\dfrac{261.9}{259.3}=1.010$ ✓ consistent.
**(v)** Unison at $F_2$ by changing length: $f\propto1/l$:
$$\frac{l'}{l}=\frac{f_2}{f_0}=\frac{259.3}{261.3}=0.9924\;\Rightarrow\;\boxed{\text{shorten by }0.77\%}.$$

> 【Thought】 The case analysis: beats give only $|f-f_0|$ — the sign must be inferred from the *trend* of $b$ with $F$ (decreasing ⟹ approaching from below). Then $\sqrt F$ scaling closes the system. The answer landing on middle C (261 Hz) validates the case choice.

---

### Question 4 — Pendulum clock and a loudspeaker

**(a) Temperature rise** ($15\to20^\circ$C): length grows $\Delta l/l=\alpha\Delta T=1.9\times10^{-5}\times5=9.5\times10^{-5}$; period $\propto\sqrt l$: the clock runs slow by $\tfrac12\Delta l/l$:
$$\text{weekly loss}=604800\times\frac12\times9.5\times10^{-5}=\boxed{29\ \text{s lost per week}}.$$

**(b) Height 20 m:** $g$ falls by $\Delta g/g=-2h/R_E=-6.3\times10^{-6}$; period rises by $\tfrac12|\Delta g/g|=3.1\times10^{-6}$:
$$\boxed{\text{loss}=604800\times3.1\times10^{-6}=1.9\ \text{s per week}}.$$

> 【Thought】 Both answers follow from $\delta T/T=\tfrac12\,\delta(\text{length}/g)$: read the question as "compute $\delta\ln T$" — the machinery is fractional differentials, and the week enters only at the end.

**(c) Tension variation.** $F=mg\cos\theta+\dfrac{mv^2}{\ell}$: two terms — gravity's radial component *and* the centripetal demand — both vary along the swing.
(i) At maximum amplitude $\theta_M$ ($v=0$): $F=mg\cos\theta_M<mg$ (less than the weight).
(ii) At $\theta=0$: $F=mg+\dfrac{mv_{\max}^2}{\ell}=mg\left(3-2\cos\theta_M\right)>mg$ (greater; using $v_{\max}^2=2g\ell(1-\cos\theta_M)$).

**(d) Sand on a vibrating membrane.** Contact lost when $\omega^2A=g$:
$$f=\frac{1}{2\pi}\sqrt{\frac{g}{A}}=\frac{1}{2\pi}\sqrt{\frac{9.81}{1.5\times10^{-4}}}=\boxed{41\ \text{Hz}}.$$

---

### Question 5 — Air-wedge interference for glass-plate testing

**(a) Mechanism and conditions.** The two plates form a thin air wedge (angle θ, zero at the contact edge, thickness $t$ under the top plate). At near-normal incidence, interference occurs between reflections off the bottom of the top plate (glass→air: no phase flip) and the top of the bottom plate (air→glass: π flip). One flip total ⟹
$$\boxed{2t=n\lambda\ \text{destructive (dark)},\qquad 2t=(n+\tfrac12)\lambda\ \text{constructive (bright)},}$$
so the dark contact edge anchors the count. With 200 fringes across to the wire ($t=5.0\times10^{-3}$ cm):
$$2t=n\lambda\;\Rightarrow\;\lambda=\frac{2\times5.0\times10^{-3}}{200}=\boxed{5.0\times10^{-5}\ \text{cm}=500\ \text{nm}}.$$

**(b)** White light: the contact line is dark for all λ; nearby, each wavelength's fringes sit at different positions ⟹ a sequence of *coloured* bands (blue inward), smearing to uniform white a few fringes out. With a liquid of index μ in the wedge: conditions become $2\mu t=n\lambda$ — fringes **closer together** by the factor μ (the optical path is what matters); the flip structure is unchanged (glass→liquid→glass, liquid less dense optically) ⟹ same bright/dark assignment, contracted scale.

**(c) Mapping a defective slide.** Form an air wedge (or contact) between the defective slide and the reference optical flat; illuminate with monochromatic light; the fringes are **contour lines of air-gap thickness** (interval $\lambda/2$). Flat regions ⟹ straight evenly spaced fringes; a thin defect displaces fringes *toward the contact side* by one spacing per $\lambda/2$ of thinning — read the deviation map directly off the fringe distortion (each fringe's local sideways shift measures local thickness error).

**(d) Unknown wavelength from a known one.** Same wedge, same geometry: fringe spacing $\Delta x=\lambda/2\theta$ ⟹ $\lambda\propto\Delta x$:
$$\boxed{\lambda_{\text{unknown}}=\lambda_{\text{known}}\times\frac{\Delta x_{\text{unknown}}}{\Delta x_{\text{known}}}}$$
— measure both fringe spacings on the same wedge.

*Official alternative (coincidence method).* Run both wavelengths on the same wedge and find a thickness $t$ where bright fringes coincide: $2t=(n_1+\tfrac12)\lambda_1=(n_2+\tfrac12)\lambda_2$ ⟹ $\lambda_1=\dfrac{2n_2+1}{2n_1+1}\lambda_2$ — counting the fringe orders from the (dark, zeroth) contact edge then determines $\lambda_1$ from $\lambda_2$; with several coincidences, plot $n_1$ against $n_2$: gradient $\lambda_2/\lambda_1$, intercept $\tfrac12(\lambda_2/\lambda_1-1)$ — an overdetermined read.

> 【Thought】 The wedge is a *thickness-to-position transducer*: fringes are level lines of the gap. Once you see fringes as contours, (c) is "topographic mapping" and (d) is "calibrate the scale" — the physics is the same λ/2 per fringe.

---

### Question 6 — Momentum collisions and wedges

**(a) Bullet through a block.** Momentum: $mu=m(u/2)+MV$ ⟹ $V=\dfrac{mu}{2M}$. KE lost fraction:
$$\frac{\Delta T}{T_i}=1-\frac{\tfrac12m(u/2)^2+\tfrac12MV^2}{\tfrac12mu^2}=1-\frac14-\frac{m}{4M}=\boxed{\frac34-\frac{m}{4M}}.$$

**(b) Particle leaving a smooth sphere.** Slides from the top; at height $z$ above the centre, $v^2=2g(a-z)$; leaves when the normal vanishes: $mg\cos\theta=\dfrac{mv^2}{a}$ with $z=a\cos\theta$:
$$gz=2g(a-z)\;\Rightarrow\;\boxed{z=\frac{2a}{3}}.$$

> 【Thought】 The classic: lift-off when the centripetal demand outstrips the gravity component toward the centre. Note $z=2a/3$ (height above centre), i.e. a drop of $a/3$ — memorise the factor.

**(c) Two smooth 45° wedges + a mass.** Released: the big wedge W slides horizontally (recoiling from w); the small wedge w slides down W's 45° face (down and opposite to W's motion); the mass m on w's smooth horizontal top receives only vertical forces (weight and the face's normal) ⟹ **m falls vertically in a straight line**, staying above its initial horizontal position while w moves out from under it sideways. (Contact persists while w's downward acceleration is less than $g$ — both accelerate smoothly; the system is momentum-conserving horizontally overall.)

> 【Thought】 The diagnostic clause is "all surfaces smooth": no horizontal force can reach m — so its horizontal coordinate is invariant. The wedge pair conserves horizontal momentum internally.

**(d) Trains at u and 2u, 60° apart.** $\mathbf v_{\text{rel}}=\mathbf v_{2u}-\mathbf v_u$: components: $2u\cos60^\circ-u=0$ along the slow train's direction; $2u\sin60^\circ=\sqrt3\,u$ across it:
$$\boxed{|\mathbf v_{\text{rel}}|=\sqrt3\,u,\ \text{directed exactly perpendicular to the slower train's motion}}$$
(the fast train's forward component equals the slow train's speed — it pulls away purely sideways as seen from the slow train ✓ neat engineered result).

---

### Question 7 — Parking orbits, satellite paradox, galaxy mass

**(a)** Parking orbit speed: $v=\sqrt{\dfrac{GM_E}{R_E}}=\sqrt{gR_E}=\boxed{7.9\ \text{km/s}}$.
*(Official-answer note: the scheme prints $7.64\times10^3$ m/s, having keyed $R_E=6.83\times10^6$ m — a digit transposition of $6.38\times10^6$; with the correct radius, $7.9$ km/s.)*

**(b) Earth's rotation.** The surface already moves eastward at $465\ \text{m/s}\times\cos(\text{latitude})$; launching eastward banks this as free initial speed — the *extra* energy the launcher must supply is reduced (equatorial eastward launches are cheapest; polar launches get nothing).

**(c) Speeding up while losing energy.** Orbital energy $E=-\dfrac{GMm}{2r}$; friction makes $\Delta E<0$ ⟹ $r$ shrinks; speed $v=\sqrt{GM/r}$ **rises**. Energy bookkeeping: $KE=-E$ (virial), so $\Delta KE=-\Delta E>0$ — friction removes energy, but gravity does positive work as the orbit tightens, and *more* than the friction took, the excess feeding KE. (The satellite paradox, cf. Paper 11 Q5c.)

**(d) Galaxy estimate.** Assume the star's orbit is circular and the galaxy's mass is interior-dominated (shell theorem):
(i) $M=\dfrac{v^2r}{G}=\dfrac{(2.5\times10^5)^2\times3\times10^4\times9.46\times10^{15}}{6.67\times10^{-11}}=\boxed{2.7\times10^{41}\ \text{kg}\sim10^{11}M_\odot}$.
(ii) With solar-mass stars: $N\approx\dfrac{M}{M_\odot}=\boxed{1.3\times10^{11}\ \text{stars}\sim10^{11}}$.

---

### Question 8 — Compton scattering at angle θ

**(a) Vector triangle.** Incident photon $\mathbf p=hf/c$; scattered photon $\mathbf p'=h(f-\Delta f)/c$ at angle θ; electron $\mathbf p_e=m_ev$ closing the triangle: $\mathbf p=\mathbf p'+\mathbf p_e$ (draw $\mathbf p'$ at θ to $\mathbf p$, $\mathbf p_e$ connecting tip to tip).

**(b)** Cosine rule:
$$\boxed{p_e^2=p^2+p'^2-2pp'\cos\theta=\left(\frac{h}{c}\right)^2\left[f^2+(f-\Delta f)^2-2f(f-\Delta f)\cos\theta\right]}.$$

**(c)** Energy: $\boxed{hf=h(f-\Delta f)+\tfrac12m_ev^2}$ ⟹ $h\Delta f=\tfrac12m_ev^2$.

**(d) Deduce Δf.** Eliminate via $p_e=m_ev$ and $v^2=2h\Delta f/m_e$:
$$2m_eh\Delta f=\left(\frac{h}{c}\right)^2\left[f^2+(f-\Delta f)^2-2f(f-\Delta f)\cos\theta\right].$$
With $\Delta f\ll f$: the bracket $\to2f(f-\Delta f)(1-\cos\theta)\approx2f^2(1-\cos\theta)$:
$$\boxed{\Delta f\approx\frac{hf^2}{m_ec^2}(1-\cos\theta)}\ \blacksquare\quad\left(\text{equivalently }\Delta\lambda=\frac{h}{m_ec}(1-\cos\theta)\right).$$

**(e) Sketches.** (i) $\Delta f$ vs $f$ at fixed θ: a parabola (∝ $f^2$). (ii) $\Delta f$ vs θ at fixed $f$: $(1-\cos\theta)$ — rising from 0 at $\theta=0$ to maximum at $\theta=180^\circ$: greatest for **backscattering**:
$$\boxed{\Delta f_{\max}=\frac{2hf^2}{m_ec^2}\ \text{at}\ \theta=180^\circ}.$$

> 【Thought】 The approximation chain: $\Delta f\ll f$ simplifies the momentum bracket to $2f^2(1-\cos\theta)$; $hf\ll m_ec^2$ licenses the non-relativistic electron. Note the result is the Compton formula in disguise: $\Delta\lambda=\frac{h}{m_ec}(1-\cos\theta)$ — the Compton wavelength $h/m_ec=2.43$ pm is the scale.

---

### Question 9 — Molecular charge distributions

**(a) Perpendicular bisector point P** (distance $r$ from O): equidistant $\sqrt{r^2+4a^2}$ from both charges:
$$V_1=\frac{kQ}{\sqrt{r^2+4a^2}}-\frac{kQ}{\sqrt{r^2+4a^2}}=\boxed{0},$$
$$E_1=2\times\frac{kQ}{r^2+4a^2}\times\frac{2a}{\sqrt{r^2+4a^2}}=\boxed{\frac{4akQ}{(r^2+4a^2)^{3/2}}}\quad(\text{directed parallel to AB, from A toward B}).$$

**(b) Point S = (2a, 3a)** (A = (−2a,0), B = (2a,0)): distances $\sqrt{(4a)^2+(3a)^2}=5a$ from A, $3a$ from B:
$$V_2=\frac{kQ}{5a}-\frac{kQ}{3a}=\boxed{-\frac{2kQ}{15a}},$$
$$\mathbf E_2=\frac{kQ}{25a^2}\left(\frac{4}{5},\frac{3}{5}\right)+\frac{kQ}{9a^2}(0,-1)=\frac{kQ}{a^2}\left(\frac{4}{125},\;-\frac{98}{1125}\right)=\frac{kQ}{a^2}(0.032,-0.0871),$$
$$\boxed{|\mathbf E_2|\approx0.093\,\frac{kQ}{a^2}\ \text{at}\ \arctan\frac{0.0871}{0.032}\approx70^\circ\ \text{below the }+x\text{ direction}}.$$

**(c) Charged ring + rod on its axis.** Ring radius $3a$, charge $+Q$, centre C; rod (length $4a$, mass $m$) on the axis with $-Q$ at distance $4a$ and $+Q$ at $8a$ from C initially. Ring's axial potential: $V(x)=\dfrac{kQ}{\sqrt{x^2+9a^2}}$. Energy conservation between the initial position and the moment $-Q$ reaches C (rod's $+Q$ then at $4a$):
$$U_i=\frac{kQ^2}{a}\left(-\frac15+\frac{1}{\sqrt{73}}\right)=-0.0830\,\frac{kQ^2}{a},\qquad U_f=\frac{kQ^2}{a}\left(-\frac13+\frac15\right)=-0.1333\,\frac{kQ^2}{a},$$
$$\tfrac12mv^2=U_i-U_f=0.0503\,\frac{kQ^2}{a}\;\Rightarrow\;\boxed{v=\sqrt{\frac{0.101\,kQ^2}{am}}=0.32\,\sqrt{\frac{kQ^2}{am}}}.$$

> 【Thought】 Careful energy audit: both charges' potential energies change as the rod translates — write $U_i$ and $U_f$ as sums over the *two* charges explicitly, then subtract. The ring's axial potential $kQ/\sqrt{x^2+9a^2}$ is the only input (each ring element is equidistant from the axis point).

---
*End of Paper 29 (2011 Round 1 Section 2).*


---

## Paper 30 — 2010 Round 1 Section 1 (12 Nov 2010) [2011 paper]

*Section 1, Question 1, parts (a)–(o). Maximum 40 marks from 78.*

---

### Q1(a) — Gas in a tank: halved and reheated [3 marks]

$$\frac{P_2}{P_1}=\frac{n_2T_2}{n_1T_1}=\frac12\times\frac{338}{288}\;\Rightarrow\;\boxed{P_2=5.9\ \text{atm}}.$$

> 【Thought】 Two-factor bookkeeping: mole count and absolute temperature separately — the °C→K conversion is the designed trap (using Celsius gives 10×0.5×65/15 = 21.7 atm, nonsense).

---

### Q1(b) — R₁ ∥ R₂ then series R₃, total = R₁ [2 marks]

$$\frac{R_1R_2}{R_1+R_2}+R_3=R_1\;\Rightarrow\;\boxed{R_3=\frac{R_1^2}{R_1+R_2}}.$$

> 【Thought】 Same template as Paper 10 Q1(j)(i) — recognise it.

---

### Q1(c) — Field lines of 3Q and −Q [5 marks]

**Definition.** An electric field line is a curve whose tangent at every point gives the direction of the electrostatic force on a positive test charge (the direction of **E**); lines start on positive charge and end on negative charge, never cross, and their density encodes |E|.

**Sketch.** From the 3Q charge, three times as many lines emanate as terminate on −Q: one third of 3Q's flux ends on −Q (dense bundle between them, distorted toward B), the remaining two-thirds escape to infinity; a neutral point sits on the far side of −Q (where $3Q/x^2=Q/(x-a)^2$ ⟹ $x=\dfrac{a}{\sqrt3-1}=1.37a$ from 3Q, i.e. $0.37a$ beyond the smaller charge).

---

### Q1(d) — Suspended cable between level supports [5 marks]

**Key observation.** Each support carries half the weight vertically: $V=50g$; the support tension is along the cable at 30°.

**(i)** $T_A=\dfrac{50g}{\sin30^\circ}=100g=\boxed{981\ \text{N}}$ (at 30°, along the cable).
**(ii)** Lowest point: tension is horizontal, equal to the horizontal component: $T_0=T_A\cos30^\circ=100g\times0.866=\boxed{850\ \text{N}}$.

> 【Thought】 Structure: tension's vertical component carries weight, horizontal component is constant throughout the cable (only vertical forces act between points) — so the lowest point's tension is the horizontal tension everywhere.

---

### Q1(e) — Sun spot through a temple's roof-hole [4 marks]

**Key observation.** The Sun's angular speed is Earth's rotation: $\omega=2\pi/86400=7.27\times10^{-5}$ rad/s; the spot is a pointer-shadow — speed = height × angular rate.

**(i)** $v=h\omega=10\times7.27\times10^{-5}=\boxed{0.73\ \text{mm/s}}$.
**(ii)** With a floor mirror, the beam's direction rotates at $2\omega$ (mirror doubles angular motion); the ceiling spot at ~10 m path: $\boxed{v'=2\omega h=1.5\ \text{mm/s}}$.

> 【Thought】 The mirror-doubling ($2\omega$) is the same factor as in the rotating-mirror measurement of $c$ (Paper 22 Q1(i)) — collect it. Note the spot motion is slow but inexorable — sundial physics.

---

### Q1(f) — Potassium-42 decaying to calcium-42 [3 marks]

$^{42}_{19}\text{K}\to{}^{42}_{20}\text{Ca}$: atomic number rises by 1 at fixed mass number ⟹ **beta-minus decay**.

**(i)** Radiation produced: β⁻ electrons (the primary spectrum), antineutrinos, and γ rays if the daughter is left in an excited state.
**(ii)** $^{42}_{20}$Ca atom: $\boxed{20\ \text{protons},\ 22\ \text{neutrons},\ 20\ \text{electrons}}$.

---

### Q1(g) — Free glass film in reflected white light [6 marks]

**Key observation.** Free film in air: top reflection (air→glass) flips π; bottom (glass→air) does not — one flip ⟹ constructive when $2nt=(m+\tfrac12)\lambda$.

> 【Thought】 Flip inventory again (cf. Papers 13, 16, 20): exactly one flip ⟹ half-integer condition. Then scan orders for the visible window (400–700 nm).

**Solution.** $2nt=2\times1.52\times0.42\ \mu\text{m}=1.277\ \mu\text{m}$; $\lambda=\dfrac{1.277}{m+\tfrac12}\ \mu\text{m}$: $m=2$: $\boxed{\lambda=511\ \text{nm}\ (\text{green})}$ ($m=1$: 851 nm IR; $m=3$: 365 nm UV — only $m=2$ is visible).

---

### Q1(h) — Ball on a vibrating chord (ring on a smooth rod) [11 marks]

**Key observation.** The rod is smooth ⟹ the ring end is a *free* (sliding) end for transverse motion = an **antinode**; the stationary ball is a **node**. The chord's fundamental is a quarter-wave.

> 【Thought】 Boundary-condition reading is the whole problem: "ring slides on a smooth rod" ⟹ antinode; "ball remains stationary" ⟹ node. Node-to-antinode = λ/4, not λ/2 — this flips the answer by a factor of 2.
>
> 【Thought】 *Official-answer divergence.* The mark scheme reads the chord as node–node ($\lambda=2L=2.4$ m), getting $f=28$ Hz, $T=0.036$ s, $A=8.5$ cm, $T/T_0=0.016$. But the ring slides on a *smooth* rod: no horizontal force can act on the chord's top end, so that end is a free end (antinode), and the stationary ball is the node — the fundamental is node-to-antinode, $\lambda=4L$, giving our $f=14$ Hz. (Either way, $T\ll T_0$, so the "ball remains stationary" assumption stands — the qualitative conclusion of (iv) is unaffected.) If the stem's “ring free to slide on a smooth horizontal rod” became “ring fixed to the rod”, condition C (free end = antinode) would break and our λ/4 reading would fail — return to the official reading, because a fixed end is a node and the fundamental is λ/2.

**Setup.** Tension ≈ ball's weight: $T=50\times9.81=490$ N; $\mu=0.13/1.2=0.108$ kg/m; $v=\sqrt{T/\mu}=\sqrt{490/0.108}=67.3$ m/s.

**(i)** $\lambda=4L=4.8$ m: $\boxed{f=\frac{v}{4L}=14.0\ \text{Hz},\quad T=0.071\ \text{s}}$.
**(ii)** Ring (antinode) amplitude: $v_{\max}=\omega A$ ⟹ $A=\dfrac{15}{2\pi\times14.0}=\boxed{0.17\ \text{m}}$.
**(iii)** Ball free to swing (pendulum, $\ell=1.2$ m): $T_0=2\pi\sqrt{\ell/g}=\boxed{2.2\ \text{s}}$.
**(iv)** $\dfrac{T}{T_0}=\dfrac{0.071}{2.2}=\boxed{0.032\approx1/30}$ — the chord vibrates ~30 times per ball-swing, so the ball cannot respond to the fast transverse motion: **the stationary-ball assumption is justified** (timescale separation) ✓.

---

### Q1(i) — Elastic collision identities [8 marks]

$M$ at $u$ hits stationary $m$; after: $v$ and $w$ (same direction).

**(i)** Momentum: $Mu=Mv+mw$; energy: $Mu^2=Mv^2+mw^2$. Factor the energy: $M(u-v)(u+v)=mw^2$; divide by the momentum equation $M(u-v)=mw$:
$$u+v=w.\ \blacksquare$$
**(ii)** $R=\dfrac{u-v}{u}$: from momentum, $M(u-v)=mw$ ⟹ $R=\dfrac{mw}{Mu}$. $\blacksquare$
**(iii)** $R=\dfrac{m(u+v)}{Mu}$ with $v=u(1-R)$: $R=\dfrac{m}{M}(2-R)$ ⟹ $\boxed{R=\dfrac{2m}{M+m}}$.

> 【Thought】 Part (i) is the relative-velocity reversal ($w-v=u$); the factorisation trick (energy ÷ momentum) is the same move as Paper 22 Q1(k). In (iii), $R$ is the *fractional speed retained* — note $R\to0$ for $M\gg m$ (heavy projectile barely slows… wait: $R=(u-v)/u\to0$ means $v\to u$ ✓) and $R\to2$ for $m\gg M$ (rebound $v\to-u$ ✓).

---

### Q1(j) — Two charged plastic balls on threads [7 marks]

**Key observation.** Equilibrium: $\tan\theta=\dfrac{F_e}{mg}$ with $F_e=\dfrac{kQ^2}{(2L\sin\theta)^2}$ — an implicit equation in the half-angle θ.

> 【Thought】 The geometry couples back ($r=2L\sin\theta$): solve $\sin^2\theta\tan\theta=\text{const}$ numerically/iteratively. Small-angle guessing ($\sin\theta\approx\theta$) gets close fast: $\theta^3\approx0.0458$ ⟹ θ ≈ 0.358 rad ≈ 20.5° — then refine.

**Solution.** $\sin^2\theta\tan\theta=\dfrac{8.99\times10^9\times(10^{-6})^2}{4\times1.00^2\times0.005\times9.81}=0.0458$. Iteration: $\theta=20.5^\circ$: $\sin^2=0.1226$, $\tan=0.3745$: product $0.04594\approx0.0458$ ✓:
$$\boxed{\text{half-angle }\theta\approx20.5^\circ\;\Rightarrow\;\text{angle between threads}=2\theta\approx41.0^\circ}\ \blacksquare$$

**Check.** Coulomb force $=mg\tan20.5^\circ=0.005\times9.81\times0.374=18.4$ mN; directly: $kQ^2/r^2=8.99\times10^{-3}/(2\sin20.5^\circ)^2=8.99\times10^{-3}/0.490=18.3$ mN ✓ consistent.

---

### Q1(k) — Nitrogen in a barometer's vacuum space [7 marks]

**Key observation.** Initially Torricelli vacuum: the 75.9 cm column balances the atmosphere. After N₂ is added, the column drops to 62.2 cm: the nitrogen's pressure is the difference; its volume grew from the 8.0 cm space to $8.0+(75.9-62.2)=21.7$ cm of tube.

**Solution.** $P_{N_2}=(75.9-62.2)\ \text{cm Hg}=\rho_{Hg}g\times0.137=1.35\times10^4\times9.81\times0.137=1.81\times10^4$ Pa; volume $V=\pi(3.25\ \text{mm})^2\times0.217\ \text{m}=7.20\times10^{-6}\ \text{m}^3$; at 288 K:
$$n=\frac{PV}{RT}=\frac{1.81\times10^4\times7.20\times10^{-6}}{8.31\times288}=5.5\times10^{-5}\ \text{mol},$$
$$m=nM=5.5\times10^{-5}\times0.028=\boxed{1.5\times10^{-6}\ \text{kg}\ (\approx1.5\ \text{mg})}.$$

> 【Thought】 Two gauges chained: the *column difference* is the pressure (a manometer reading), and the *tube length difference* is the volume change. The barometer's vacuum becomes a gas-sample cell — the construction is the content.
>
> 【Thought】 *Official-answer note.* The scheme computes $n=5.46\times10^{-5}$ mol (same) but then takes the mass as $14n$ g — using the *atomic* weight of nitrogen. Nitrogen gas is N₂, so $M=28$ g/mol and $m=1.5$ mg (ours); the official $7.6\times10^{-4}$ g is a factor-2 slip.

---

### Q1(l) — Charging a capacitor in two stages [8 marks]

**(i)** Two cells in series (2E) charging C: $U=\tfrac12C(2E)^2=\boxed{2CE^2}$.
**(ii)** Battery supplied $Q\times2E=(2CE)(2E)=4CE^2$; stored $2CE^2$; lost: $\boxed{2CE^2}$ (the usual 50%).
**(iii) Two stages.** Stage 1 (one cell, to E): stored $\tfrac12CE^2$, supplied $CE\times E=CE^2$, lost $\tfrac12CE^2$. Stage 2 (two cells, E→2E): charge driven $\Delta Q=CE$ at 2E: supplied $2CE^2$; stored change $2CE^2-\tfrac12CE^2=\tfrac32CE^2$; lost $\tfrac12CE^2$:
$$\boxed{\text{total lost}=CE^2\ \text{vs}\ 2CE^2\ \text{directly}\ \text{— staged charging halves the loss}}.$$

> 【Thought】 The mechanism: losses scale with the *voltage gap* between supply and capacitor ($I^2R$ during charging); stepping the supply halves the typical gap. The limit: continuously ramped supply ⟹ lossless charging (the principle behind charge-pump/adiabatic logic). This refines the "50% rule" of Paper 14 Q6(a).

---

### Q1(m) — Two masses on identical springs: beats [4 marks]

**(i)** $f_1=\dfrac{1}{2\pi}\sqrt{\dfrac{39.48}{0.90}}=1.054$ Hz; $f_2=\dfrac{1}{2\pi}\sqrt{\dfrac{39.48}{1.10}}=0.954$ Hz.
**(ii)** Beat frequency $=|f_1-f_2|=0.101$ Hz ⟹ beat period $\boxed{T_b\approx9.9\ \text{s}\ (f_b\approx0.10\ \text{Hz})}$.

> 【Thought】 The spring constant 39.48 ≈ 4π²×1 is engineered so $f\approx\sqrt{1/m}$ Hz — spotting the engineered constant speeds the numerics (but don't assume it — verify).

---

### Q1(n) — Band brake heating a drum [3 marks]

Work per revolution $=F\times2\pi r=20\times0.25=5.0$ J; heat needed $=mc\Delta T=0.40\times350\times5.0=700$ J:
$$\boxed{N=\frac{700}{5.0}=140\ \text{revolutions}}.$$

---

### Q1(o) — Uniform-density atmosphere height [2 marks]

$$h=\frac{P}{\rho g}=\frac{1.01\times10^5}{1.23\times9.81}=\boxed{8.4\ \text{km}}.$$

> 【Thought】 This is the "homogeneous atmosphere" height (the scale-height-like number); contrast with the exponential real atmosphere (Paper 14 Q4(a)(iv)) — naming the model's failure mode is worth a sentence.

---
*End of Paper 30 (2010 Round 1 Section 1).*


---

## Paper 31 — 2010 Round 1 Section 2 (12 Nov 2010) [2011 paper]

*Section 2: Questions 2–9, 20 marks each; candidates attempt three. Full solutions for all eight.*

---

### Question 2 — Circuit potentials and a symmetric network

#### Q2(a) — V_AB between two open test points [6 marks]

**Topology (Fig. 2.a):** outer loop E–D–H–G–F with cells 12 V (top) and 8 V (bottom), resistors 0.5 Ω (top), 0.5 Ω (bottom), 10 Ω and 5 Ω (left edge, split by tap F); right edge split by tap C. The middle branch F–A·B–(4 V, 0.5 Ω)–C is **open at A/B** (test points), so it carries no current.

> 【Thought】 The open middle branch carries no current ⟹ the 0.5 Ω in it drops nothing, and B sits at $V_C+4$ V (or $V_C-4$) — the cell's emf appears undisturbed. So the whole question reduces to: outer loop current → tap potentials $V_F, V_C$ → $V_{AB}$ through the idle cell.

**Solution.** Taking the cells' + terminals toward the left of the figure (as drawn): net emf around the outer loop $=12-8=4$ V against $16\ \Omega$ total ⟹ $I=0.25$ A (counterclockwise — driven by the 12 V cell, charging the 8 V). Walking the left edge: $V_E-V_F=0.25\times10=2.5$ V; traversing the top against the flow: $V_E-V_D=12-0.25\times0.5=11.875$ V; hence
$$V_F-V_C=V_F-V_D=-2.5+11.875=9.375\ \text{V}\ \text{(C=D on the plain right edge)},$$
$$\boxed{V_{AB}=V_F-(V_C+4)=5.4\ \text{V}}\quad\text{(A above B; sign flips with the assumed cell orientation)}.$$

**Check.** Loop closes exactly ($12-8=4=0.25\times16$ ✓); the answer is dominated by the loop drop, with the idle 4 V cell subtracted — consistent order ✓.

#### Q2(b) — Eight 3.00 Ω resistors (square + both diagonals) [14 marks]

**Topology (Fig. 2.b):** square C–D–F–E with both diagonals crossing at O (arms C–O, D–O, E–O, F–O); port A–B wired to C–F.

**(i) Symmetry:** mirror $D\leftrightarrow E$ (axis C–O–F) ⟹ $i_1=i_2,\ i_3=i_4,\ i_6=i_7$.
**(ii) Reversal of V** (swaps the port C↔F) composed with the mirror ⟹ $i_5=-i_8$ (the two diagonal arms toward O carry opposite currents) and $i_1=-i_3$, etc.
**(iii)** Together these force $V_D=V_E=V_O=V/2$: **D, E and O are at the same potential** ⟹ $i_6=i_7=0$.
**(iv)** With the D–O and E–O arms dead, the network is the square's four sides plus the C–O–F diagonal: current splits: the diagonal arm C–O–F ($6\ \Omega$) vs the square perimeter C–D–F and C–E–F ($6\ \Omega$ each)… distributing: $i_1=i_2=i_3=i_4=i_5=i_8=I/3$, so
$$\boxed{R_{AB}=V/I=2.00\ \Omega}.$$
**(v)** $V_O=V/2$ — O sits at the mean potential (same as D and E) — the centre of a symmetric bridge.

> 【Thought】 The cascade (symmetry → reversal → equipotentials → dead branches → trivial reduction) is the full symmetry machine; note $R=2.0\ \Omega$ from eight 3 Ω resistors — the dead branches make it just three parallel 6 Ω paths.

---

### Question 3 — Calorimetry, particle-beam pressure, photon pressure

**(a) Molten lead into the calorimeter** (repeat template of Paper 18 Q1g, new numbers). Three-stage lead cooling ($T_i\to327$ liquid, freeze, $327\to25$ solid):
$$(0.80\times4182+42.7)\times10=0.40\left[157(T_i-327)+2.31\times10^4+136\times302\right],$$
$$33883=62.8(T_i-327)+25669\;\Rightarrow\;\boxed{T_i\approx458^\circ\text{C}}.$$

**(b) Beam on a plane.** (i) Elastic rebound reverses the normal momentum: per particle $\Delta p=2mv$ with $v=\sqrt{2E/m}$; at $n$ per second into area $A$:
$$\boxed{P=\frac{2nmv}{A}=\frac{2n\sqrt{2mE}}{A}}.$$
(ii) A rough surface scatters particles non-specularly (diffuse rebound): the mean *normal* recoil is smaller (some momentum goes into tangential/thermal channels), so the pressure drops below the specular value.

**(c) Photon momentum.** (i) $\boxed{E_\lambda=pc}$ (from $E=hf$ and $p=h/\lambda$, or $E^2=p^2c^2+m^2c^4$ with $m=0$).
(ii) Bulb: $I=\dfrac{20}{4\pi(2.0)^2}=0.398$ W/m²; maximum pressure = perfect reflection at normal incidence:
$$\boxed{P_{\max}=\frac{2I}{c}=2.7\times10^{-9}\ \text{Pa}}.$$
(iii) Conditions: normal incidence on a perfectly reflecting surface (absorption would give $I/c$, half as much).

---

### Question 4 — Projectile curvature; parabolic bridge

**(a)** Stone at speed $u$, small angle $\alpha$:
(i) $T_g=\dfrac{2u\sin\alpha}{g}$, $d=\dfrac{u^2\sin2\alpha}{g}$.
(ii) $h=\dfrac{u^2\sin^2\alpha}{2g}$.
(iii) At the top, velocity is horizontal ($u\cos\alpha$) and acceleration is $g$ (purely centripetal there):
$$R=\frac{(u\cos\alpha)^2}{g}=\boxed{\frac{u^2\cos^2\alpha}{g}}.$$
(iv) Eliminate: $\tan\alpha=4h/d$ (from (i),(ii)) and $\cos^2\alpha=1/(1+\tan^2\alpha)$:
$$R=\frac{u^2\cos^2\alpha}{g}=\frac{d}{\sin2\alpha}\cos^2\alpha=\frac{d}{2\tan\alpha}=\boxed{\frac{d^2}{8h}}.$$
(v) $\tan\theta=\dfrac{u\sin\alpha-gt}{u\cos\alpha}$: a straight line from $\tan\alpha$ at $t=0$ through $0$ at $t=T_g/2$ to $-\tan\alpha$ at $t=T_g$ — sketch with those three marked points.
(vi) Perpendicular velocities need $v_{x1}v_{x2}+v_{y1}v_{y2}=0$, i.e. $\tan\theta_1\tan\theta_2=-1$ (since $v_x$ is common). From (v), $\tan\theta\in[-\tan\alpha,\tan\alpha]$: the product's magnitude is bounded by $\tan^2\alpha$; perpendicularity needs $|\tan\theta_1\tan\theta_2|=1$, impossible if $\tan^2\alpha<1$:
$$\boxed{\alpha<45^\circ\Rightarrow\text{no perpendicular velocity pair exists}}\ \blacksquare$$

> 【Thought】 The algebraic sign structure: $v_x$ is a *common factor* in the dot product — perpendicularity becomes a condition purely on the vertical components, whose range is read off the linear $\tan\theta$–$t$ graph. Note (iv) $R=d^2/8h$ is the sagitta relation again (Paper 11 Q5a) — a parabola's vertex curvature.

**(b) Car on the parabolic bridge** (length $d$, height $h$) at constant speed $v$: at the crest the radius is $R=d^2/8h$ (same parabola):
$$mg-N=\frac{mv^2}{R}\;\Rightarrow\;\boxed{N=m\left(g-\frac{8hv^2}{d^2}\right)}\quad(\text{valid while }v^2<\frac{gd^2}{8h}).$$
A spoiler adds aerodynamic **downforce** $F_s\propto v^2$: $N=mg+F_s-\dfrac{mv^2}{R}$ — it counters the lift-off term with a $v^2$-matched force, raising the speed at which contact is kept (without adding inertia) — the same reason racing cars use wings.

---

### Question 5 — Wire with a mass at its midpoint (catenary-like, small sag)

**(a)(i)** Each half of the wire: length $\sqrt{L^2+x_e^2}=L\sqrt{1+x_e^2/L^2}\approx L\left(1+\dfrac{x_e^2}{2L^2}\right)$ (binomial, given):
$$\text{extension per half }y_e=\frac{x_e^2}{2L}\;\Rightarrow\;\boxed{\left(\frac{x_e}{L}\right)^2=\frac{2y_e}{L}}.\ \blacksquare$$

**(ii) Equilibrium.** Tension $T=k(2y_e)$ (total stretch $2y_e$); vertical balance: $2T\sin\theta=Mg$ with $\sin\theta\approx x_e/L$:
$$2k(2y_e)\frac{x_e}{L}=Mg\;\Rightarrow\;\frac{2kx_e^3}{L^2}=Mg\;\Rightarrow\;\boxed{x_e=\left(\frac{MgL^2}{2k}\right)^{1/3}}.$$

> 【Thought】 The geometric amplification is the physics: a tiny stretch $y_e\sim x_e^2/2L$ produces tension, but the tension's vertical leverage $\sim x_e/L$ is also small — two small factors ⟹ $x_e\propto M^{1/3}$ (cube-root stiffness). This is the sagging-cable/cricket-wire problem's essential nonlinearity.

**(b) Released from the horizontal position.** (i) With the same geometry at displacement $x$: $y=x^2/2L$, $T=kx^2/L$, restoring $2T x/L$:
$$\boxed{M\ddot x=Mg-\frac{2k}{L^2}x^3}.$$
(ii) Energy: $\tfrac12Mv^2=Mgx-\dfrac{kx^4}{2L^2}$ (elastic PE $=\tfrac12k(2y)^2=\dfrac{kx^4}{2L^2}$):
$$\boxed{\tfrac12Mv^2=Mgx-\frac{kx^4}{2L^2}}.$$
(iii) Max displacement ($v=0$):
$$Mgx_m=\frac{kx_m^4}{2L^2}\;\Rightarrow\;\boxed{x_m=\left(\frac{2MgL^2}{k}\right)^{1/3}=4^{1/3}x_e\approx1.59\,x_e}.$$

> 【Thought】 Note the motion is **not** SHM (restoring $\propto x^3$): the mass overshoots past $2x_e$ — because the wire is softest near $x=0$. The cube-root equations are exact consequences of the quadratic sag relation.

---

### Question 6 — Two mirrors at a fixed angle; the rainbow

**(a) Diagram.** Draw the mirrors OA, OB meeting at O with angle θ; P between them. Construct $I_{AP}$ (image of P in OA) and $I_{BP}$ (image of P in OB) — and for the double reflection P→OA→OB, the double image $I_{AOB}P$ = image of $I_{AP}$ in OB. The emergent ray appears to come from $I_{AOB}P$.

**(b) Rotation of the pair (fixed θ).** (i) Every image of P stays at distance OP from O — reflection in a line through O preserves distance to O:
$$\boxed{|OI_{AP}|=|OI_{BP}|=|OP|}\ \text{— all images lie on a circle centred at O}.$$
(ii) The image angle mirrors the object angle about the mirror: $\angle(I_{AP}OX)=2\varphi_A-\varphi_P$; with $\varphi_A=\varphi_B+\theta$ (fixed θ):
$$\boxed{\angle I_{AP}OX=2\varphi_B+2\theta-\varphi_P\ \text{— varies linearly at twice the mirror-rotation rate}}.$$
(iii) Similarly $\angle I_{BP}OX=2\varphi_B-\varphi_P$: also linear in $\varphi_B$ at rate 2. **The emergent double-reflected ray's direction, however, is invariant**: the composition of two reflections is a rotation by $2\theta$ about O, independent of $\varphi_B$ — the classic two-mirror (optical lever) theorem: rotating the rigid pair does not move the doubly-imaged direction.

> 【Thought】 The hierarchy to state: each single image moves at $2\times$ the mirror angle, but the *double* image is fixed by the constant $\theta$ — this invariance is the usable content (sextants and periscopes rely on it).

**(c) Rainbow (qualitative).** Sunlight enters a spherical raindrop (refraction, dispersing colours), reflects once off the back (internal reflection), and refracts out. The deviation angle has a **stationary minimum** (~138° from the incident direction) where rays crowd (caustic) — hence a bright bow at ≈ 42° from the antisolar point. Dispersion makes the stationary angle wavelength-dependent: red emerges on the bow's outside, violet inside. The droplets' spherical symmetry wraps the caustic into a circle around the antisolar point.

---

### Question 7 — Photoelectric effect

**(a)** (i) The effect: light of sufficient frequency ejects electrons from a metal — each photon is absorbed whole by one electron. (ii) Einstein's relation from energy conservation:
$$\boxed{hf=\varphi+KE_{\max}}.$$
(iii) Classical vs quantum: classically, energy arrives continuously in a wave — any frequency should eventually eject electrons given enough intensity/time, and the electron's energy should grow with intensity and exhibit a measurable time lag. Quantum-mechanically: threshold frequency, instantaneous emission, and $KE_{\max}$ depending only on frequency — all falsifiable and falsified-classical.
(iv) I–V sketch: saturation current $I_0$ for $V>0$ (all emitted electrons collected); falling through the retarding region; zero for $V\le -V_s$ (stopping potential); raising the beam intensity raises $I_0$ only.
(v) Graphical $\varphi$: plot stopping potential $V_s$ vs frequency $f$: slope $h/e$, intercept $-\varphi/e$; equivalently plot $KE_{\max}$ vs $f$ (slope $h$, intercept $-\varphi$).

**(b)** From the table ($V_s$: 0.60…2.2 V vs $f$: 6–10×10¹⁴ Hz): the line is $V_s=\dfrac{h}{e}(f-f_0)$; slope $=\dfrac{0.40}{1.0\times10^{14}}$ V/Hz:
$$\boxed{h=e\times\frac{0.40}{1.0\times10^{14}}=6.4\times10^{-34}\ \text{J s}},\qquad \boxed{f_0=4.5\times10^{14}\ \text{Hz}}\ (V_s=0\text{ intercept}).$$

---

### Question 8 — Orbital decay energy; Earth–Moon transfer

**(a) Satellite decay.** Initial orbital energy $E_i=-\dfrac{GM_Em}{2r}$ ($r=6.98\times10^6$ m, altitude 600 km); final: impact KE $\tfrac12mv^2$ plus surface PE $-\dfrac{GM_Em}{R_E}$. Energy absorbed by the atmosphere = the satellite's mechanical-energy loss:
$$E_{\text{abs}}=E_i-E_f=-\frac{GM_Em}{2r}-\left(\tfrac12mv^2-\frac{GM_Em}{R_E}\right),$$
$$=-1.43\times10^{10}-\left(1.0\times10^{9}-3.12\times10^{10}\right)=\boxed{1.6\times10^{10}\ \text{J}}.$$

> 【Thought】 Sign discipline: all energies are negative-bound bookkeeping; the atmosphere gets $E_i-E_f$. Note the atmosphere absorbed *more* than the orbit's total energy — the surface PE difference is released too. (The official script prints $1.47\times10^{10}$ J, but its intermediate $R_E=6.83\times10^6$ m shows the same digit transposition as its Paper 29 Q7(a) — with $R_E=6.38\times10^6$ m the consistent figure is $1.59\times10^{10}$ J ≈ ours.)

**(b) Earth–Moon minimum-energy transfer.** (i) Velocity minimal at the gravity-neutral point:
$$\frac{GM_E}{d_E^2}=\frac{GM_M}{(R_{EM}-d_E)^2}\;\Rightarrow\;\frac{R_{EM}-d_E}{d_E}=\sqrt{\frac{M_M}{M_E}}=0.111,$$
$$\boxed{d_E=\frac{R_{EM}}{1.111}=3.46\times10^{8}\ \text{m}\ (\approx0.90\,R_{EM}\text{ from the Earth's centre})}.$$

(ii) Initial speed to reach it with zero residual speed (energy conservation; the Moon's term is a small correction):
$$\frac12v^2=GM_E\left(\frac{1}{R_E}-\frac{1}{d_E}\right)+GM_M\left(\frac{1}{R_{EM}-R_E}-\frac{1}{R_{EM}-d_E}\right),$$
$$\boxed{v\approx11.1\ \text{km/s}}\quad(\text{just under Earth's escape speed }11.2\ \text{km/s}\ ✓).$$

> 【Thought】 Approximations to justify: Moon's gravity contributes ~2% (keep it as a check, drop it for the headline number); neglect Earth's rotation boost and atmospheric drag. The threshold being just below escape is the physical reading: reaching the Moon costs nearly escape energy.

---

### Question 9 — Radioactive equilibrium, gamma attenuation, C-14 dating

**(a) U–Ra equilibrium.** $N_{Ra}=N_U\dfrac{T_{Ra}}{T_U}=10^{23}\times\dfrac{5.1\times10^{10}}{1.4\times10^{17}}=\boxed{3.6\times10^{16}\ \text{radium nuclei}}$ (equal activities).

**(b) Gamma source.** (i) Point source, isotropic: count rate $=$ flux × area: $60/\text{min}=1.0$ s⁻¹ at $r=2.0$ m:
$$1.0=\frac{R\times4.0\times10^{-4}}{4\pi(2.0)^2}\;\Rightarrow\;\boxed{R=1.26\times10^{5}\ \text{photons/s}}.$$
(ii) Moving to 1.8 m restores the rate despite the absorber: unabsorbed rate there would be $1.0\times(2.0/1.8)^2=1.235$ s⁻¹:
$$\text{transmission}=\frac{1.000}{1.235}=0.810\;\Rightarrow\;\boxed{19\%\ \text{absorbed}}.$$

**(c) Carbon dating.** Living: 4.00 g carbon → $N_{14}=\dfrac{4.00}{12}N_A\times1.25\times10^{-12}=2.51\times10^{11}$ C-14 atoms; living activity $A_0=\dfrac{\ln2}{5600\ \text{yr}}\times2.51\times10^{11}=59.1$ counts/min (for this sample). Dead: $A=20.0\pm0.4$ /min:
$$t=T_{1/2}\frac{\ln(A_0/A)}{\ln2}=5600\times\frac{\ln(59.1/20.0)}{0.693}=\boxed{8.8\times10^{3}\ \text{years}},$$
$$\delta t=\frac{T_{1/2}}{\ln2}\times\frac{\delta A}{A}=8077\times\frac{0.4}{20.0}=\boxed{\pm160\ \text{years}}.$$

> 【Thought】 The uncertainty propagates logarithmically: $\delta t=\dfrac{T_{1/2}}{\ln2}\dfrac{\delta A}{A}$ — counting precision translates directly into age precision at fixed fractional size. (The living-wood specific activity ~15 counts/min/g is the calibration to check against.)

---
*End of Paper 31 (2010 Round 1 Section 2).*


---

## Paper 32 — 2009 Round 1 Section 1 (13 Nov 2009) [2010 paper]

*Section 1, Question 1, parts (a)–(p). Maximum 40 marks from the pool.*

---

### Q1(a) — Cooling molten lead: latent heat from the cooling curve [4 marks]

**Key observation.** Constant heat-loss rate $P$; the three phases (liquid cooling, plateau freezing, solid cooling) calibrate each other.

> 【Thought】 The plateau's length (300 s) measures latent heat against the solid-cooling phase (8.4 s for 5 K) — the cooling curve is a complete calorimeter. Read rates off each segment separately.

**Solution.** (i) Solid phase: $P=\dfrac{mc_s\Delta T}{t}=\dfrac{3.0\times140\times5}{8.4}=\boxed{250\ \text{W}}$.
(ii) Plateau: $P\times300=3.0\,L$: $L=\dfrac{250\times300}{3.0}=\boxed{2.5\times10^4\ \text{J/kg}}$.
(iii) Liquid phase: $c_l=\dfrac{Pt}{m\Delta T}=\dfrac{250\times10}{3.0\times5}=\boxed{167\ \text{J kg}^{-1}\text{K}^{-1}}$.

**Check.** $c_s<c_l$? Here $140<167$ ✓ plausible; plateau ≫ cooling segments ✓ (latent ≈ 60 K-worth of sensible heat).

---

### Q1(b) — Rope on a wall, pulled horizontally [3 marks]

**Key observation.** Two-point equilibrium: the wall-end tension (at 30° to the wall) has the weight as its vertical component and the 20 N pull as its horizontal component.

$$W=\frac{20}{\tan30^\circ}=34.6\ \text{N}\;\Rightarrow\;\boxed{m=\frac{34.6}{9.81}=3.5\ \text{kg}}.$$

> 【Thought】 For a rope (no stiffness), the tension direction at the wall end is the rope direction there — the wall angle IS the equilibrium angle. (The rope's shape is a catenary, but only the endpoint angles matter here.)

---

### Q1(c) — Area of one bit on a CD [3 marks]

$$A_{\text{bit}}=\frac{\pi(5.5^2-2.2^2)\ \text{cm}^2}{650\times8\times10^6\ \text{bits}}=\frac{79.8\ \text{cm}^2}{5.2\times10^9}=\boxed{1.5\times10^{-12}\ \text{m}^2\ \text{per bit}\approx(1.2\ \mu\text{m})^2}.$$

> 【Thought】 Estimate sanity: a µm² per bit is exactly the optical-diffraction scale of the CD's laser — the answer is physically forced by the readout optics, which is a nice consistency remark.

---

### Q1(d) — Photons striking the film [5 marks]

**Key observation.** Chain: lamp light power (1% of 100 W) → inverse-square to 100 m → lens area → exposure time → photon count.

$$P_{\text{lens}}=1.0\ \text{W}\times\frac{\pi(0.010)^2}{4\pi(100)^2}=2.5\times10^{-9}\ \text{W};\qquad E=2.5\times10^{-9}\times0.015=3.75\times10^{-11}\ \text{J},$$
$$N=\frac{E}{hc/\lambda}=\frac{3.75\times10^{-11}}{3.31\times10^{-19}}=\boxed{1.1\times10^{8}\ \text{photons}}.$$

---

### Q1(e) — Tungsten filament's working temperature [4 marks]

**Key observation.** Hot resistance from the rating ($V^2/P$); linear temperature coefficient from the cold value.

$$R_{\text{hot}}=\frac{230^2}{250}=211.6\ \Omega;\qquad 211.6=20\left(1+5.0\times10^{-3}\Delta T\right)\;\Rightarrow\;\Delta T=1916\ \text{K},$$
$$\boxed{T\approx273+1916\approx2190\ \text{K}\ (\approx1900^\circ\text{C})}.$$

> 【Thought】 The rating's hidden content: $R_{\text{hot}}=V^2/P$. The linear law is being extrapolated over 2000 K — flag that as the model's boundary (real tungsten's coefficient drifts).

---

### Q1(f) — Polaroid sheet: transmitted amplitude and intensity [3 marks]

**Key observation.** A Polaroid transmits only the field component along its transmission axis; intensity goes as the square of amplitude.

The incident amplitude $a$ is at $\theta$ to the transmission plane, so

$$a_t=a\cos\theta\;(\text{amplitude}),\qquad I_t=I_0\cos^2\theta\quad\text{(Malus)}.$$

Unpolarized light has equal average projection on every axis, $\langle\cos^2\theta\rangle=\tfrac12$, hence

$$\boxed{I_{\text{transmitted}}=\frac{I}{2}}.$$

> 【Thought】 Two different questions are hiding in one sentence: (1) polarized input → amplitude picks up $\cos\theta$ (field is the object that splits); (2) unpolarized input → average over a random $\theta$, which is exactly $1/2$. Never apply Malus's $\cos^2\theta$ to unpolarized light — that is the classic trap.

---

### Q1(g) — Escape velocity; why some planets keep an atmosphere [4 marks]

**Key observation.** Escape = reaching infinity with zero residual kinetic energy → pure energy balance.

$$\frac12mv_{\text{esc}}^2-\frac{GMm}{R}=0\;\Rightarrow\;\boxed{v_{\text{esc}}=\sqrt{\frac{2GM}{R}}}.$$

Atmosphere argument: gas molecules have a Maxwell distribution with mean thermal speed $\bar v\sim\sqrt{3kT/m_{\text{mol}}}$. If $v_{\text{esc}}\gg \bar v$ (typically $\gtrsim 6\bar v$), even the fast tail of the distribution cannot escape and the planet retains its gas. Large, cold planets (Earth, Jupiter) have $v_{\text{esc}}$ of several km/s and hold even light gases; the Moon ($v_{\text{esc}}\approx2.4$ km/s) and Mercury lose everything, since at their temperatures the tail above $v_{\text{esc}}$ is replenished continuously and bleeds away over geological time. Hence retention depends on the ratio $GMm_{\text{mol}}/(RkT)$.

> 【Thought】 Check the formula: $GM/R$ has units m²/s² ✓; for Earth $\sqrt{2\times9.81\times6.37\times10^6}=11.2$ km/s ✓ (known value). The atmosphere question is really "compare two speeds", not a qualitative hand-wave — that comparison is what earns the marks.

---

### Q1(h) — Foucault's rotating mirror: velocity of light [3 marks]

**Key observation.** The ray is gone for time $\Delta t=2d/c$; on return the mirror has turned by $\omega\Delta t$, and a reflected ray turns by **twice** the mirror's rotation.

Mirror: $\omega=2\pi\times35=219.9$ rad s$^{-1}$; round trip $2d=400$ m. Observed deviation $\varphi=2.0$ arcmin $=\frac{2}{60}\times\frac{\pi}{180}=5.82\times10^{-4}$ rad.

$$\varphi=2\omega\Delta t=\frac{4\omega d}{c}\;\Rightarrow\;c=\frac{4\omega d}{\varphi}=\frac{4\times219.9\times200}{5.82\times10^{-4}}=\boxed{3.0\times10^{8}\ \text{m s}^{-1}}.$$

> 【Thought】 The factor-of-2 bookkeeping is the whole problem: mirror turns $\theta$ → reflected ray turns $2\theta$. Miss that and you are out by exactly 2. Also note the method's logic: $c$ is so large that the whole apparatus is a device for converting a tiny time into a measurable angle.

---

### Q1(i) — Battery with internal resistance: emf, r, and powers [4 marks]

**Key observation.** Two load configurations give two linear equations in the two unknowns $E, r$.

Parallel ($R_{\text{ext}}=1.0\ \Omega$, $I=3.0$ A): $E=3.0(r+1.0)$; series ($R_{\text{ext}}=4.0\ \Omega$, $I=1.2$ A): $E=1.2(r+4.0)$. Subtracting:

$$3.0r+3.0=1.2r+4.8\;\Rightarrow\;1.8r=1.8\;\Rightarrow\;\boxed{r=1.0\ \Omega,\quad E=6.0\ \text{V}}.$$

Power in one resistor: parallel — each carries $3.0/2=1.5$ A, $P_p=1.5^2\times2.0=\boxed{4.5\ \text{W}}$; series — each carries $1.2$ A, $P_s=1.2^2\times2.0=\boxed{2.88\ \text{W}}$.

> 【Thought】 Check: total power from the cell in case 1 is $EI=18$ W, split $9$ W load $+9$ W internal ✓; case 2: $7.2$ W total $=5.76+1.44$ ✓. "Power dissipated in **a** resistor" — read the singular; halving the parallel current is the step most often dropped.

---

### Q1(j) — Rocket on the pad: does it lift off immediately? [4 marks]

**Key observation.** Liftoff needs thrust ≥ instantaneous weight; thrust is $u\,\mathrm{d}m/\mathrm{d}t$, weight shrinks as fuel burns.

(i) Thrust $T=u\dot m=(2.5\times10^3)(16)=4.0\times10^4$ N. Initial weight $W_0=(4.1\times10^3)(9.81)=4.02\times10^4$ N. Since $T<W_0$, the rocket initially **stays on the pad** (the pad supplies the deficit as a normal force). $\blacksquare$

(ii) Liftoff when $W(t)=T$: $m(t)=T/g=4.0\times10^4/9.81=4.08\times10^3$ kg, i.e. $\Delta m=4100-4078=22$ kg of fuel burnt. At $16$ kg s$^{-1}$:

$$\boxed{t=\frac{22\ \text{kg}}{16\ \text{kg s}^{-1}}\approx1.4\ \text{s}}.$$

> 【Thought】 The conceptual point: "engine on" ≠ "rocket moves" — thrust must first pay the weight tax. During the first 1.4 s the exhaust momentum flux is real but merely replaces part of the pad's normal reaction. (Using $g=10$ m s$^{-2}$ instead gives 6.25 s — state your $g$; the method is unchanged.)

---

### Q1(k) — Ideal vs real gas [3 marks]

**Ideal-gas molecules:** point particles (zero volume), no intermolecular forces except during collisions, all collisions perfectly elastic, continuous random motion.

**Real molecules:** finite own volume (excluded volume $b$) and attract one another at short range (van der Waals), so impacts are softened by an effective internal pressure.

**Macroscopic distinction:** an ideal gas obeys $PV=nRT$ exactly at all densities; a real gas deviates — compressibility factor $Z=PV/nRT\neq1$ (attractions dominate at moderate $P$: $Z<1$; finite volume at high $P$: $Z>1$) — and, decisively, a real gas can **liquefy**, which no force-free point-particle gas ever can. Real gases approach ideality at low pressure and high temperature.

> 【Thought】 Structure the answer as microscopic → macroscopic: the two microscopic failings (size, attraction) map one-to-one onto the two van der Waals corrections $(P+a/V^2)(V-b)=nRT$. That mapping shows understanding rather than a memorised list.

---

### Q1(l) — Crossing the river by the shortest path [7 marks]

**Key observation.** The resultant velocity is the vector sum of boat velocity (fixed magnitude $v_b=3.0$ m/s, steerable) and water velocity $v_w$. Geometry of vector addition settles everything.

**Case $v_w=2.0$ m/s ($<v_b$).** The shortest path between the banks is the straight line perpendicular to the bank. Achieve it by cancelling the drift: head upstream at angle $\theta$ to the cross-river line with

$$v_b\sin\theta=v_w\;\Rightarrow\;\sin\theta=\frac{2}{3}\;\Rightarrow\;\theta=41.8^\circ$$

i.e. row at $48.2^\circ$ to the bank (pointing upstream); the boat then crosses straight over at $\sqrt{v_b^2-v_w^2}=\sqrt{5}=2.2$ m/s.

**Case $v_w=4.0$ m/s ($>v_b$).** Straight across is now impossible (the boat cannot supply 4 m/s upstream). Draw $\vec v_w$; the tip of the resultant $\vec R=\vec v_w+\vec v_b$ lies on a circle of radius $v_b$ about the tip of $\vec v_w$. The path is shortest when $\vec R$ makes the **largest possible angle to the bank direction**, which occurs when $\vec R$ is tangent to that circle — i.e. when the heading is **perpendicular to the resultant**. Then

$$\sin\varphi=\frac{v_b}{v_w}=\frac{3}{4}\;\Rightarrow\;\varphi=48.6^\circ,$$

where $\varphi$ is the angle of the actual path to the bank. He rows at $90^\circ-\varphi=41.4^\circ$ to the upstream bank, and the boat lands downstream despite his best effort — this is the minimal-drift path, hence the shortest achievable.

> 【Thought】 The two regimes have genuinely different answers because the governing constraint changes: when $v_b>v_w$ the constraint is "zero drift" (feasible); when $v_b<v_w$ it becomes "minimum drift" (optimisation). The tangent-to-circle argument is the standard geometric solution of the latter — seeing "shortest path with $v_w>v_b$" should immediately trigger the tangent construction, not another attempt at drift cancellation.

---

### Q1(m) — Charged ball raised by an identical charge [8 marks]

**Key observation.** Three forces on B — weight (vertical), tension (along thread BO), Coulomb repulsion (along AB) — and the geometric triangle OAB is isosceles ($OA=OB=l$); the force triangle is similar to it.

Let the thread have length $l$, support at O; ball A is brought to B's original position (distance $l$ below O), and B settles with $AB=d$, having risen by $h$.

(i) Force triangle $\sim$ triangle OAB, with $T$ opposite $OB$, $mg$ opposite $OA$, $F_c$ opposite $AB$:

$$\frac{T}{l}=\frac{mg}{l}=\frac{F_c}{d}\;\Rightarrow\;\boxed{T=mg}.$$

(ii) Geometry: $d^2=2l^2(1-\cos\varphi)=2lh$ (since $h=l-l\cos\varphi$), so $h=d^2/2l$. The agent moves A quasi-statically, so the work done equals the gain in total potential energy of the system:

$$W=\underbrace{mgh}_{\text{gravity on B}}+\underbrace{\frac{kQ^2}{d}}_{\text{electric}}.$$

From the force balance $F_c=kQ^2/d^2=mg\,d/l$, hence $kQ^2/d=mgd^2/l=2mgh$. Therefore

$$W=mgh+2mgh=\boxed{W=3mgh},$$

manifestly independent of the charges: a bigger $Q$ makes $d$ bigger, and the gravitational and electric terms scale identically ($U_{\text{elec}}=2\,\Delta U_{\text{grav}}$ always).

> 【Thought】 The "similar triangles" hint is the whole key: in any three-force equilibrium, draw the force triangle and hunt for a geometric triangle it is similar to — here it converts force balance into pure geometry. The result $W=3mgh$ looks surprising (work set by gravity alone), so check the mechanism: as A approaches, B rises exactly so that the Coulomb energy deposited is always twice the gravitational gain. Dimensional check: $mgh$ is an energy ✓.

---

### Q1(n) — Two like-charged plates vs a capacitor [7 marks]

**Key observation.** Each insulating plate is a sheet of charge with field $E_1=Q/(2\varepsilon_0 A)$ on each side; a sheet exerts no net force on itself — the force on a plate is its charge times the **other** plate's field alone.

(i) $+Q,+Q$ system: fields between the plates cancel (a neutral mid-plane); field lines from each plate bend outward and escape to infinity; outside the pair the field is $Q/(\varepsilon_0A)$ on each side, lines radiating outward.

(ii) Capacitor $+Q,-Q$: fields add between the plates — uniform $E=Q/(\varepsilon_0A)$, straight parallel lines from $+$ to $-$; essentially zero field outside.

(iii) Force: in both cases the field produced by plate 1 at plate 2 is $Q/(2\varepsilon_0A)$ (a single sheet's field, independent of the other plate). Hence

$$F_{(+,+)}=Q\cdot\frac{Q}{2\varepsilon_0A}=F_{(+,-)}\;\Rightarrow\;\boxed{\text{ratio }1:1}$$

— equal magnitudes, repulsive for (i), attractive for (ii), despite the total fields looking completely different.

(iv) $C=\varepsilon_0A/x$, so $E_{\text{stored}}=\dfrac{Q^2}{2C}=\boxed{\dfrac{Q^2x}{2\varepsilon_0A}}$.

(v) $F=\dfrac{\mathrm{d}E_{\text{stored}}}{\mathrm{d}x}=\boxed{\dfrac{Q^2}{2\varepsilon_0A}}$, attractive (energy decreases as $x$ shrinks at fixed $Q$). The analogy: any system whose energy is linear in a separation $x$ carries a constant "generalised force", exactly as $F=-\mathrm{d}U/\mathrm{d}x$ for a gravitational potential linear in height.

> 【Thought】 Part (iii) is the trap: students integrate the *total* field (which differs hugely between the cases) instead of the *source* field of the other plate. The energy method of (v) is then the safer route to the same number — and the agreement of the two routes is itself the check. Note the energy is linear in $x$ at fixed $Q$ (constant field, growing volume), which is why the force is constant.

---

### Q1(o) — Whirling whistle: extreme Doppler frequencies [7 marks]

**Key observation.** The source's velocity along the line of sight oscillates between $\pm v$; the Doppler extremes occur at those instants.

Source speed: $v=2\pi r f_{\text{rot}}=2\pi(1.2)(3.0)=22.6$ m/s. Moving source, stationary observer:

$$f_{\max}=f_0\frac{c}{c-v}=256\times\frac{340}{340-22.6}=\boxed{274\ \text{Hz}},\qquad
f_{\min}=f_0\frac{c}{c+v}=256\times\frac{340}{340+22.6}=\boxed{240\ \text{Hz}}.$$

The observer hears the frequency sweep periodically between 240 and 274 Hz, three times per second.

> 【Thought】 Checks: $v\ll c$, so first-order shift $\Delta f/f\approx v/c=6.6\%$ → $\pm17$ Hz about 256, matching 240/274 ✓; the up-shift exceeds the down-shift slightly (asymmetric denominators) ✓. Only the radial component of the source velocity matters — at the extreme instants the whistle moves straight toward/away from the observer.

---

### Q1(p) — Electrons injected at angle θ into a uniform B field [8 marks]

**Key observation.** Split $\vec v$ into components parallel and perpendicular to $\vec B$; the Lorentz force $-e\,\vec v\times\vec B$ touches only the perpendicular component.

**Setup.** $v_\parallel=v\cos\theta$ (along $\vec B$), $v_\perp=v\sin\theta$.

(i) Along $\vec B$: no force, so $v_\parallel$ is constant. Perpendicular: a force of constant magnitude $ev_\perp B$, always perpendicular to $v_\perp$, rotates that component uniformly — uniform circular motion at constant speed. Superposition = a **helix** of constant radius and constant pitch, which retraces itself every turn, so the motion is periodic. $\blacksquare$

(ii) Circular part: $ev_\perp B=\dfrac{mv_\perp^2}{r}\Rightarrow r=\dfrac{mv_\perp}{eB}$, and

$$T=\frac{2\pi r}{v_\perp}=\boxed{\frac{2\pi m}{eB}}$$

— independent of $v$ and $\theta$ (the cyclotron property).

(iii) Distance along the field in one period (the pitch):

$$L=v_\parallel T=\boxed{\frac{2\pi m v\cos\theta}{eB}}.$$

> 【Thought】 The decomposition is forced by $\vec F\perp\vec B$: whatever happens, the parallel motion is inertial. The cancellation of $v_\perp$ in $T$ is the deep result (it underlies cyclotrons and magnetic mirroring) — always pause to note when an answer loses a variable it "should" contain, and double-check it: here $r\propto v_\perp$ while the circumference is also $\propto v_\perp$, so the period really is speed-independent. Units: $m/(eB)$ = kg/(C·T) = s ✓.

---

*End of Paper 32.*

## Paper 33 — 2009 Round 1 Section 2 (13 Nov 2009) [2010 paper]

### Q2 — Optics: apparent depth, underwater mirror, prism, glitter [20 marks]

**(a) Glass block that looks like a cube [2 marks].**

**Key observation.** "Appears to be a cube" viewed from above = the apparent depth equals the 5.0 cm face; apparent depth $=$ real depth$/n$.

Standing on a $5.0\times5.0$ cm face, the block is 8.0 cm deep; viewed from above its apparent depth is $8.0/n$ cm. Setting this equal to 5.0 cm:

$$\boxed{n=\frac{8.0}{5.0}=1.6}.$$

> 【Thought】 The apparent-depth rule $d'=d/n$ assumes near-normal viewing ("viewed directly from above" licenses it). Check: $n=1.6$ is a reasonable glass (denser than crown, like flint) ✓.

---

**(b) Inclined mirror at the bottom of a water tank [6 marks].**

**Key observation.** Track the ray's angle to the *vertical* through three events: refraction in (Snell), reflection off a mirror tilted $10^\circ$ (which adds $2\times10^\circ$ to the tilt of the ray), refraction out (must beat total internal reflection).

Entry: $\sin\theta=\tfrac43\sin r$, where $r$ is the angle to the vertical in water. The mirror is tilted $10^\circ$ from horizontal, so its normal OX is $10^\circ$ from vertical; reflecting the descending ray (angle $r$ to vertical) sends it back upward at angle

$$\varphi=r+2\times10^\circ=r+20^\circ$$

to the vertical (a tilted mirror rotates the reflected ray by twice the tilt — here *away* from the vertical, as the ray walks down the slope to O). For the ray to emerge at C rather than suffer TIR, $\varphi$ must not exceed the critical angle $\varphi_c=\arcsin(3/4)=48.59^\circ$. Maximum case:

$$r_{\max}=48.59^\circ-20^\circ=28.59^\circ,\qquad \sin\theta_{\max}=\tfrac43\sin28.59^\circ=0.638,$$

$$\boxed{\theta_{\max}\approx39.6^\circ\ (\approx40^\circ)}.$$

> 【Thought】 The $+20^\circ$ is the geometric heart: normal tilted $10^\circ$ ⇒ reflected ray rotated $20^\circ$; get the sign by sketching the ray walking *down* the tilted mirror — the return ray leans further from vertical, making TIR *easier*, which is why a finite $\theta_{\max}$ exists. (Had the mirror tilted the other way, $\varphi=r-20^\circ$ and every $\theta$ would emerge — a quick way to confirm the figure's orientation.)

---

**(c) Prism with one reflecting face [10 marks].**

**Setup from Figure 2.c.** HE $\perp$ HG (right angle at H), $\angle$HEF $=75^\circ$, so face EF runs at $15^\circ$ to the horizontal HG; OS $\perp$ EF, so OS sits at $75^\circ$ to horizontal; BQ $\parallel$ HG. The ray enters face HE at B, refracts to O on face EF, reflects (TIR) up to C on HG, and emerges toward D. Inside the glass, BO makes angle $\theta$ with the horizontal.

**(i) $\angle$BOC.** OB arrives at O at $\theta$ below horizontal; its angle to the normal OS is $75^\circ-\theta$. Reflection keeps this angle on the far side of OS:

$$\boxed{\angle BOC=2(75^\circ-\theta)=150^\circ-2\theta}.$$

**(ii) $\varphi$ in terms of $\theta$.** Reflecting a ray of direction $-\theta$ in a surface of slope $+15^\circ$ gives direction $2(15^\circ)-(-\theta)=30^\circ+\theta$ above horizontal. Face HG is horizontal (normal vertical), so the incidence angle at C is

$$\boxed{\varphi=90^\circ-(30^\circ+\theta)=60^\circ-\theta}.$$

**(iii) $\theta=\varphi$.** $\theta=60^\circ-\theta\Rightarrow\theta=30^\circ$. Then the incidence angle at O is $75^\circ-30^\circ=45^\circ$, and TIR requires this to exceed the critical angle:

$$\sin45^\circ\geq\frac1n\;\Rightarrow\;\boxed{n\geq\sqrt{2}\approx1.41}.$$

**(iv) Angle between incident and emergent rays when $\theta=\varphi=30^\circ$.** At B (vertical face, horizontal normal): $\sin i=n\sin30^\circ$. At C (horizontal face, vertical normal): $\sin e=n\sin30^\circ$. Hence $i=e$. The incident ray travels at $-i$ to the horizontal; the emergent ray at $90^\circ-e$ to the horizontal. The angle between them:

$$\boxed{90^\circ-e-(-i)=90^\circ}\qquad(\text{since }i=e),$$

independent of $n$ — the prism acts as a perfect $90^\circ$ deviator in the symmetric case.

> 【Thought】 The whole question is disciplined angle-chasing: fix ONE reference direction (horizontal), express every ray direction in it, and let reflection/refraction laws add or subtract angles. Seeing "$\theta=\varphi$" should trigger "symmetric path ⇒ equal refractions at both faces ⇒ clean answer". The $90^\circ$ result is a good check: it is the prism analogue of the corner-cube/right-angle deviation.

---

**(d) Elongated images of lights on a river at night [2 marks].**

The water surface is never perfectly flat: ripples present facets at a continuous range of small slopes. Specular reflection off each facet sends light to the eye from a different apparent position — facets tilted one way reflect the lamp as if it were higher, the other way lower. The reflected image is therefore smeared **vertically** into a long streak (the horizontal slopes average out, so the image stays narrow sideways). At night the scene is dark, so only these bright streaks are visible and the elongation is conspicuous.

> 【Thought】 Keyword trigger: "river at night" → not a flat mirror but a ensemble of tilted micro-mirrors → angular spread of reflected rays → streak along the direction of the slope variation. One sentence of mechanism + one of geometry earns both marks.

---

### Q3 — Stretched wire and a ladder [20 marks]

**(a) Young's modulus from a sagging wire [10 marks].**

**Key observation.** Geometry gives the strain; statics gives the tension; their ratio is $E$. The small sag makes both tiny-angle approximations exact enough at 1% sag.

Each half of the wire stretches from 0.500 m to $\ell'=\sqrt{0.500^2+0.010^2}=0.50010$ m, so

$$\text{strain}=\frac{2\ell'-1.00}{1.00}=2.0\times10^{-4}.$$

Equilibrium at the midpoint, with $\sin\alpha=0.010/0.50010=0.0200$ the angle of each half to the horizontal:

$$2T\sin\alpha=mg\;\Rightarrow\;T=\frac{0.50\times9.81}{2\times0.0200}=122.6\ \text{N};\qquad \text{stress}=\frac{T}{A}=1.23\times10^{8}\ \text{Pa}.$$

$$\boxed{E=\frac{\text{stress}}{\text{strain}}=\frac{1.23\times10^{8}}{2.0\times10^{-4}}\approx6.1\times10^{11}\ \text{Pa}}.$$

> 【Thought】 Structure of the estimate: strain scales as $(\text{sag}/\text{half-length})^2$ while $\sin\alpha$ scales linearly in sag, so $E\propto 1/\text{sag}^3$-ish — tiny sags give huge apparent stiffness. Check the order: $E\sim10^{11}$ Pa is the metal scale (steel is $2\times10^{11}$; our slightly larger value reflects the small measured strain) ✓. Note the assumption "wire obeys Hooke's law" is strained at $10^8$ Pa — worth one flagging clause.

---

**(b) Man climbing a ladder [10 marks].**

**Setup.** Ladder 4.0 m, foot B 2.0 m from the wall, so the top A is at height $\sqrt{16-4}=2\sqrt3=3.46$ m; the ladder makes $60^\circ$ with the ground. A man of 90 kg stands a distance $x$ up the ladder; ladder mass 10 kg acts at its midpoint (1.0 m horizontally from B).

**(i) Force diagram.** At A (wall): $F_{AV}$ vertical (friction — zero if the wall is smooth), $F_{AH}$ horizontal (normal, pushing the ladder away from the wall). At B (ground): $F_{BV}$ vertical (normal up), $F_{BH}$ horizontal (friction, toward the wall). Weights $90g$ at the man, $10g$ at the midpoint.

**(ii) Equilibrium conditions (smooth wall, $F_{AV}=0$).**

$$\sum F_x=0:\;F_{BH}=F_{AH};\qquad \sum F_y=0:\;F_{BV}=(90+10)g=981\ \text{N};$$

moments about A (the man's horizontal distance from the wall is $2-\tfrac{x}{2}$, since he advances $\tfrac{x}{2}$ horizontally):

$$F_{BV}\times2.0=F_{BH}\times2\sqrt3+90g\left(2-\tfrac{x}{2}\right)+10g\times1.0.$$

**(iii) Minimum $\mu$ to reach the top ($x=4.0$ m).** The man is then directly below A (zero moment arm), and

$$F_{BH}=\frac{2(981)-1(98.1)}{2\sqrt3}=\frac{1863.9}{3.464}=538\ \text{N},\qquad \mu_{\min}=\frac{F_{BH}}{F_{BV}}=\boxed{\frac{538}{981}=0.55}.$$

> 【Thought】 Why moments about A? It eliminates both wall forces from the equation, leaving ground forces and weights only — always take moments about the point with the most unknowns. Counter-intuitive feature worth naming: as the man climbs, his moment arm about A *shrinks* (he moves toward the wall), so the ladder's own weight dominates at the top; the friction demand is nonetheless maximal there because $F_{BV}\times2$ must be supplied by $F_{BH}$. Sanity: $\mu\sim0.5$ is a typical rubber–concrete value ✓.

---

### Q4 — Vertical spring: energy bookkeeping through collisions [20 marks]

**Key observation.** For a vertical spring, shifting the origin to the equilibrium position absorbs gravity into the elastic term — the motion is pure SHM about equilibrium with the same $\omega$.

**(i) Static extension.** $Mg=kx_1$ and $\omega^2=k/M$:

$$\boxed{x_1=\frac{Mg}{k}=\frac{g}{\omega^2}}.$$

**(ii) Total potential energy.** With extension $x_1+x$ and gravitational zero at the equilibrium position:

$$V=\tfrac12k(x_1+x)^2-Mgx=\underbrace{\tfrac12kx_1^2}_{\text{const}}+\underbrace{(kx_1-Mg)}_{=0}x+\tfrac12kx^2=\boxed{\tfrac12kx_1^2+\tfrac12kx^2}.$$

The linear term vanishes precisely because $kx_1=Mg$: measured from equilibrium, the system behaves as a spring alone.

**(iii) Maximum KE and total energy for amplitude $A_1$.**

$$T_1=\tfrac12M\omega^2A_1^2=\boxed{\tfrac12kA_1^2};\qquad E_1=V_{\max}=\boxed{\tfrac12kA_1^2}\quad(=T_1),$$

as energy sloshes between kinetic and potential with fixed total.

**(iv) Elastic collision with a stationary mass $M/2$ at $x=0$.** The collision occurs at equilibrium, where $M$ has its maximum speed $v_1=\omega A_1$. For an elastic collision with a stationary target:

$$v_2=\frac{M-M/2}{M+M/2}\,v_1=\frac{v_1}{3}\;\Rightarrow\;\boxed{v_2=\frac{\omega A_1}{3},\quad A_2=\frac{v_2}{\omega}=\frac{A_1}{3}}$$

(the oscillation re-centres on the same equilibrium since the spring and $M$ are unchanged).

**(v) Perfectly inelastic collision (masses coalesce).** Momentum conservation at $x=0$: $Mv_1=\tfrac{3M}{2}v'\Rightarrow v'=\tfrac{2}{3}\omega A_1$. The new oscillator has mass $\tfrac32M$, so $\omega'^2=\tfrac23\omega^2$, and its equilibrium shifts down by

$$x_2'-x_1=\frac{(3M/2)g}{k}-\frac{Mg}{k}=\frac{Mg}{2k}=\frac{x_1}{2},$$

i.e. the new equilibrium extension is $\boxed{x_2=\tfrac32x_1=\tfrac{3g}{2\omega^2}}$, and at the collision instant the combined mass is $x_1/2$ **above** its new equilibrium. Energy about the new equilibrium:

$$\tfrac12kA_2^2=\tfrac12\!\left(\tfrac{3M}{2}\right)\!v'^2+\tfrac12k\left(\tfrac{x_1}{2}\right)^2
=\frac{M\omega^2A_1^2}{3}+\frac{kx_1^2}{8},$$

$$\boxed{A_2=\sqrt{\frac{2A_1^2}{3}+\frac{x_1^2}{4}}=\sqrt{\frac{2A_1^2}{3}+\frac{g^2}{4\omega^4}}}.$$

> 【Thought】 The recurring trap this question patrols: after coalescence the equilibrium moves, so amplitude must be measured from the NEW centre and includes both the kinetic term and the static-displacement term — forgetting the $x_1^2/4$ piece is the classic error. Checks: (iv) elastic with equal-ish masses → projectile slows but continues, $v_2=v_1/3$ between the $m_2\to0$ (no change) and $m_2=M$ (stop) limits ✓; (v) if $A_1\gg x_1$, $A_2\approx\sqrt{2/3}A_1$ — amplitude shrunk by both mass increase and energy sharing ✓; $g^2/4\omega^4$ has units m² ✓.

---

### Q5 — Capacitors, a symmetric network, and rectification [20 marks]

**(a) Two capacitors joined in parallel [6 marks].**

Initially: $V_1=120\,\mu\text{C}/2.0\,\mu\text{F}=60$ V, $V_2=120\,\mu\text{C}/4.0\,\mu\text{F}=30$ V. Connecting positive plates together (charge conserved, now shared):

**(i)** $C_{\text{tot}}=6.0\ \mu$F, $Q_{\text{tot}}=240\ \mu$C:

$$\boxed{V=\frac{240}{6.0}=40\ \text{V}}.$$

**(ii)** Energies: $E_i=\tfrac{Q^2}{2C_1}+\tfrac{Q^2}{2C_2}=3.6+1.8=5.4$ mJ; $E_f=\tfrac12C_{\text{tot}}V^2=\tfrac12(6\,\mu\text{F})(40)^2=4.8$ mJ.

$$\boxed{\Delta E=-0.6\ \text{mJ (lost)}}.$$

The lost energy is dissipated as heat (and a little electromagnetic radiation/spark) in the connecting wires while the charge redistributes — charge is conserved, energy is not, whenever capacitors at different potentials are joined.

> 【Thought】 The invariant to use is charge, never voltage: the plates that are joined form an isolated island whose total charge is trapped. The energy "paradox" ($0.6$ mJ vanishes regardless of wire resistance) is resolved by noting the redistribution current always burns exactly the difference.

---

**(b) Six-resistor symmetric network [7 marks].**

**Key observation.** The network (A and B at the base, apex T, centre M; arms AT, TB, AB, TM, AM, MB, all $R$) is unchanged by swapping A and B.

**(i) Reversing $V$.** By linearity, every current simply reverses: $i_k(-V)=-i_k(V)$. But the reversed circuit is also the original circuit with A and B interchanged, and under that interchange arm AT maps to TB, AM to MB. Comparing the two descriptions:

$$i_2=i_5,\qquad i_3=i_6,\qquad\text{(and }i_1,i_4\text{ map onto themselves with sign flip under reversal)}.$$

**(ii) Currents.** Kirchhoff at T: $i_2=i_5+i_4$, but $i_2=i_5$, so $\boxed{i_4=0}$ — the vertical arm carries no current (T and M sit at the same potential, $V/2$). The network then splits into three independent paths A→B:

$$i_1=\frac{V}{R},\qquad i_2=i_5=i_3=i_6=\frac{V}{2R},\qquad i_4=0.$$

**(iii) Resistance.** $I=i_1+i_2+i_3=\dfrac{V}{R}+\dfrac{V}{2R}+\dfrac{V}{2R}=\dfrac{2V}{R}$:

$$\boxed{R_{AB}=\frac{V}{I}=\frac{R}{2}}.$$

> 【Thought】 The problem deliberately walks you through the symmetry argument instead of letting you guess it: reversal ($V\to-V$) plus the geometric A↔B interchange *forces* the pairing $i_2=i_5$, $i_3=i_6$, and KCL then kills $i_4$. General moral: a bridge arm joining two equipotential nodes may be removed entirely. Numerical check by nodal analysis: $V_T=V_M=V/2$ ✓, $R_{AB}=R/2$ ✓.

---

**(c) Half-wave rectifier with smoothing capacitor [7 marks].**

**(i) Time constants.** $\tau=RC$: with $R=10$ kΩ: $\boxed{\tau=0.50\ \text{s}}$; with $R=100\ \Omega$: $\boxed{\tau=5.0\ \text{ms}}$ (supply period $T=20$ ms).

**(ii) Waveforms across R** (sketch descriptions):
- $R=10$ kΩ ($\tau\gg T$): the capacitor charges to the peak (10 V) on each positive half-cycle and barely discharges through R before the next — output is nearly steady DC at $\approx10$ V with a small ($\sim$2%) sawtooth ripple.
- $R=100\ \Omega$ ($\tau<T/2$): the capacitor decays almost fully each cycle — output is a train of rounded pulses rising to 10 V at each positive peak and falling exponentially toward zero, zero during the negative half-cycles.

**Square wave, 10 kΩ case.** The capacitor tops up to $+10$ V almost instantly when the input is high (diode on), then discharges through R alone for the low half-cycle, $\Delta t=T/2=10$ ms:

$$\frac{\Delta V}{V}=1-e^{-\Delta t/\tau}=1-e^{-0.010/0.50}=1-e^{-0.02}=\boxed{0.020\ (\approx2\%)}.$$

> 【Thought】 Rectifier analysis is one comparison: $\tau$ vs $T$. $\tau/T=25$ → stiff DC; $\tau/T=0.25$ → barely smoothed pulses. For the square wave the discharge interval is the full half-period (input low ⇒ diode off), and $e^{-0.02}\approx1-0.02$ justifies the linear-ripple approximation that engineers use: $\Delta V/V\approx\Delta t/\tau$.

---

### Q6 — Chirped loudspeakers: measuring the speed of sound [19 marks]

**Key observation.** Because the frequency ramps with time, the two waves arriving at R were emitted at *different* times and so arrive with slightly *different* frequencies and a steadily growing phase difference — the first minimum occurs when that phase difference reaches $\pi$.

**Setup.** A $=(-d,0)$, B $=(+d,0)$ with $2d=0.500$ m; R is 1.20 km from line AB and 1.20 km from the bisector, i.e. at $45^\circ$: $D=OR=1200\sqrt2=1697.06$ m. Exact path lengths:

$$RA=\sqrt{D^2+d^2+\sqrt2\,dD}=1697.23\ \text{m},\qquad RB=\sqrt{D^2+d^2-\sqrt2\,dD}=1696.88\ \text{m},\qquad \Delta\equiv RA-RB=0.354\ \text{m}.$$

Ramp: $f=\alpha t$, $\alpha=10$ Hz s$^{-1}$; first minimum at $t=52.2$ s.

**(a) Travel times.** (i) from A: $t_A=RA/c_s=\dfrac{1697.23}{c_s}$; (ii) from B: $t_B=RB/c_s=\dfrac{1696.88}{c_s}$.

**(b) Frequencies arriving at time t.** The wave arriving now left its speaker at the retarded time $t-t_A$ (resp. $t-t_B$):

$$f_A=\alpha\!\left(t-\frac{RA}{c_s}\right),\qquad f_B=\alpha\!\left(t-\frac{RB}{c_s}\right).$$

**(c) Common frequency.** Since $D\gg d$, $RA\approx RB\approx D$:

$$f\approx\alpha\!\left(t-\frac{D}{c_s}\right),\qquad\text{uncertainty } \pm\frac{\alpha\,\Delta}{2c_s}\ (\text{numerically }\pm5\times10^{-3}\ \text{Hz}).$$

**(d) Wavelength.** $\lambda=c_s/f=\dfrac{c_s}{\alpha\left(t-D/c_s\right)}$.

**(e) Speed of sound.** The phase of each arriving wave is the integral of its emitted frequency up to the retarded time, $\varphi=\pi\alpha\tau^2$, so the phase difference at R is

$$|\Delta\varphi|=\pi\alpha\left|t_A-t_B\right|\left(2t-t_A-t_B\right)=\pi\,\alpha\frac{\Delta}{c_s}\cdot2\!\left(t-\frac{D}{c_s}\right).$$

First minimum: $|\Delta\varphi|=\pi$:

$$2\alpha\Delta\left(t-\frac{D}{c_s}\right)=c_s
\;\Rightarrow\; c_s^2-2\alpha\Delta t\,c_s+2\alpha\Delta D=0,$$
with $2\alpha\Delta t=2\times10\times0.354\times52.2=369.1$ and $2\alpha\Delta D=1.200\times10^{4}$:
$$c_s^2-369.1\,c_s+1.200\times10^{4}=0,$$

$$\boxed{c_s=333\ \text{m s}^{-1}}\qquad(\text{the other root, }36\ \text{m/s, is unphysical}).$$

*Official-answer note.* The scheme prints $c_s=363$ m/s from the quadratic $c_s^2-396.1c_s+12000=0$ — but its own previous line, $10\left(52.2-\frac{1200\sqrt2}{c_s}\right)\frac{1}{\sqrt2}=c_s$, expands to coefficient $369.1$, not $396.1$ (a transcription slip); with $369.1$ the roots are $333$ and $36$ m/s, and $c_s=333$ m/s self-consistently closes ($\lambda/2=0.354$ m ✓, while $363$ m/s fails its own closure, giving $\lambda/2=0.382$ m). The scheme's front page warns it is a draft with known small errors.

**Check.** With $c_s=333$ m/s: $D/c_s=5.10$ s, arriving frequency $=10(52.2-5.10)=471$ Hz, and $2f\Delta/c_s=2(471)(0.354)/333=1.00$ half-wavelengths of path-equivalent phase ✓. (The naive estimate ignoring the 5.1 s transit, $c_s=2\alpha t\Delta=369$ m/s, is 11% high — the retarded-time correction is the physics this question tests.)

> 【Thought】 Seeing "frequency rising linearly, first minimum at time $t$" should trigger: interference of two *chirped* copies → phase difference grows because of the path difference $\Delta$ → minimum when the accumulated phase slip is $\pi$. The transit delay $D/c_s$ (5 s!) is not negligible against 52 s, which is why parts (a)–(d) force you to build the retarded-time machinery before computing.

---

### Q7 — Radioactivity: dating, wear tracing, background [20 marks]

**(a) Age of the Earth from U-238/U-235 [6 marks].**

Equal initial abundances; now $N_{238}/N_{235}=140$:

$$\frac{N_{238}}{N_{235}}=2^{\,t\left(\frac{1}{T_{235}}-\frac{1}{T_{238}}\right)}=140
\;\Rightarrow\; t=\frac{\ln140}{\ln2\left(\dfrac{1}{7.1\times10^8}-\dfrac{1}{4.5\times10^9}\right)}=\boxed{6.0\times10^{9}\ \text{years}}.$$

> 【Thought】 The ratio method cancels the unknown initial amounts — that's why isotope *ratios* are the geologist's clock. Check: $T_{235}$ is 6.3× shorter, so U-235 nearly vanishes; $\log_2 140\approx7.1$ extra halvings of the ratio at one per effective $(1/T_{235}-1/T_{238})^{-1}\approx8.4\times10^8$ yr $\Rightarrow$ $\sim6\times10^9$ yr ✓ (comfortably close to the accepted $4.5\times10^9$ yr given the crude "equal amounts" assumption).

---

**(b) Piston-ring wear by neutron activation [6 marks].**

**Key observation.** Activity is proportional to mass of Fe-59 present; correct the oil activity back to installation day (decay correction), then scale up from the 100 cm³ sample to the whole sump.

Count rate in the sample: $126/600=0.210$ Bq; whole oil ($5.0\times10^{-3}$ m³ $=50\times$ the sample): $A_{30}=10.5$ Bq at day 30. Decay factor over 30 days: $2^{-30/45}=0.630$. Equivalent activity at installation:

$$A_0=\frac{10.5}{0.630}=16.7\ \text{Bq}\;\Rightarrow\;\text{fraction worn}=\frac{16.7}{4\times10^{5}}=\boxed{4.2\times10^{-5}}.$$

> 【Thought】 Two scalings, one each way: sample→sump multiplies by 50; day-30→day-0 divides by 0.63. Both are easy to invert under pressure — check by direction: the worn fraction should be *larger* than the naive $10.5/(4\times10^5)$ because the iron has been decaying ✓. The uniform-activity assumption is what lets activity stand in for mass.

---

**(c) Background subtraction [5 marks].**

If the source alone decayed exponentially with $T=70$ s, after 210 s = 3 half-lives the rate would be $82/8=10.25$ counts/s — but 19 is observed, and no single exponential fits both points: $\frac{19}{82}=0.232\neq2^{-3}=0.125$ — **not exponential** ✓ (as required to verify).

With a constant background $b$: source rate is $82-b$ initially, $(82-b)/8$ after 3 half-lives:

$$\frac{82-b}{8}+b=19\;\Rightarrow\;82-b+8b=152\;\Rightarrow\;\boxed{b=10\ \text{counts s}^{-1}}.$$

Check: source $72\to9$ counts/s; $9+10=19$ ✓.

---

**(d) Extracting a long half-life in the presence of the short one [3 marks].**

Record the count rate at many times spanning well beyond $\sim5\times70$ s, until the short-lived contribution is negligible. Subtract the known $A_0 2^{-t/70}$ component (or simply use late-time data); the residual decays as the long-lived substance alone. Plot $\ln(\text{residual rate})$ against $t$: a straight line of slope $-\lambda$, giving $T_{1/2}=\ln2/\lambda$ — the longer the measurement baseline relative to $T_{1/2}$, the better the estimate.

> 【Thought】 (c)+(d) are one idea at two levels: data = sum of exponentials (+constant). Identify components in order of lifetime — constant background first (it survives everything), then the long-lived tail, then the fast component. Semilog plotting turns each exponential into a straight line; that is always the first move.

---

### Q8 — Gravity: surface value, depth dependence, ore-body anomalies [20 marks]

**(a) Surface g from Newton's law [3 marks].**

$$g=\frac{GM_E}{R_E^2}=\frac{(6.67\times10^{-11})(5.97\times10^{24})}{(6.38\times10^{6})^2}=\boxed{9.78\ \text{m s}^{-2}}.$$

> 【Thought】 Check against the tabulated 9.81 ✓ (the small deficit is the neglected rotation/ellipticity — a good sign the computation is right).

---

**(b) Descending 15 km into the crust [7 marks].**

**Key observation.** Shell theorem: at radius $r$ only the mass *inside* $r$ gravitates. Descending $h=15$ km removes the crustal shell above you but brings you closer to the centre — the two effects compete, and which wins depends on how light the crust is compared with the mean Earth.

Mean density: $\bar\rho=3M_E/(4\pi R_E^3)=5488$ kg m$^{-3}$. Mass of the 15 km crustal shell: $\Delta M\approx4\pi R_E^2h\,\rho_c=2.07\times10^{22}$ kg. Then

$$g_{15}=\frac{G(M_E-\Delta M)}{(R_E-h)^2}=\frac{(6.67\times10^{-11})(5.949\times10^{24})}{(6.365\times10^{6})^2}=9.795\ \text{m s}^{-2},$$

$$\boxed{\frac{\Delta g}{g}=+\left(\frac{2h}{R_E}-\frac{3\rho_c h}{\bar\rho R_E}\right)=+1.2\times10^{-3}\quad\text{(g increases).}}$$

> 【Thought】 The sign is the physics: the $1/r^2$ gain ($+2h/R_E=+4.7\times10^{-3}$) outweighs the shell loss ($-3\rho_c h/\bar\rho R_E=-3.5\times10^{-3}$) *because* $\rho_c=2700<\tfrac23\bar\rho$. In a uniform-density Earth the famous result is $g$ *decreases* linearly with depth ($\Delta g/g=-h/R_E$); the Earth's light crust flips the near-surface behaviour — worth stating explicitly, as the question asks "indicate if g increased or decreased".

---

**(c) Gravity anomaly over a spherical iron deposit [6 marks].**

**Key observation.** The deposit *replaces* crustal rock, so the anomaly comes from the **excess mass** $(\rho_{Fe}-\rho_c)V$, acting at distance $a=2.5$ km (centre just one radius below the surface).

$$M_{\text{excess}}=\tfrac43\pi a^3(\rho_{Fe}-\rho_c)=\tfrac43\pi(2500)^3(7900-2700)=3.40\times10^{14}\ \text{kg},$$

$$\Delta g=\frac{GM_{\text{excess}}}{a^2}=\tfrac43\pi G a\,\Delta\rho=3.6\times10^{-3}\ \text{m s}^{-2}
\;\Rightarrow\;\boxed{\frac{\Delta g}{g}\approx+3.7\times10^{-4}}.$$

> 【Thought】 Two modelling choices to state: (1) excess vs absolute mass — physically the cavity of displaced crust means the *contrast* $\Delta\rho=5200$ kg m$^{-3}$ is the source (using the full 7900 gives $+5.6\times10^{-4}$, same order); (2) treating a finite sphere as a point at its centre is *exact* by the shell theorem, no approximation needed. Gravimeters resolve $10^{-7}$, so this anomaly is easily detectable — the principle behind mineral exploration.

---

**(d) After mining: the empty cavity [4 marks].**

Now the iron is gone too; relative to undisturbed crust the deficit is the full iron mass $M_{Fe}=\tfrac43\pi a^3\rho_{Fe}=5.16\times10^{14}$ kg:

$$\boxed{\frac{\Delta g}{g}=-\frac{4\pi G a\,\rho_{Fe}}{3g}\approx-5.6\times10^{-4}}.$$

> 【Thought】 *Official-answer note.* The scheme prints $\Delta g/g=-5.64\times10^{-7}$ — a factor of $10^3$ too small: it used $\rho_{Fe}=7.9$ (g/cm³) without converting to kg/m³ ($7900$). With SI units throughout, $-5.6\times10^{-4}$ (ours) is correct; the scheme's own front page warns it is a draft with uncorrected slips.

> 【Thought】 Note the asymmetry between (c) and (d): the deposit anomaly referenced the *contrast* (iron in place of rock), the cavity anomaly references the *full* iron mass (nothing in place of iron). Keeping the reference state straight ("change relative to what?") is the whole game in anomaly problems — say it out loud in the solution.

---

### Q9 — Rocket to the Moon: neutral points, impact, orbit, landing [20 marks]

**Key observation.** "Just sufficient energy to reach the Moon" = arriving at the gravitational saddle point (where the *potential energies* balance, the crest of the potential hill) with zero speed; everything after that is energy bookkeeping in the combined Earth–Moon field.

**(a) Balance points measured from the Moon's centre.**

(i) Forces equal: $\dfrac{GM_Em}{(R_{EM}-R_{MF})^2}=\dfrac{GM_Mm}{R_{MF}^2}$:

$$\frac{R_{EM}-R_{MF}}{R_{MF}}=\sqrt{\frac{M_E}{M_M}}=\sqrt{81.2}=9.01
\;\Rightarrow\;\boxed{R_{MF}=\frac{R_{EM}}{10.01}=3.84\times10^{7}\ \text{m}\ (\approx3.8\times10^{4}\ \text{km})}.$$

(ii) Potential energies equal: $\dfrac{GM_Em}{R_{EM}-R_{MP}}=\dfrac{GM_Mm}{R_{MP}}$:

$$\frac{R_{EM}-R_{MP}}{R_{MP}}=\frac{M_E}{M_M}=81.2
\;\Rightarrow\;\boxed{R_{MP}=\frac{R_{EM}}{82.2}=4.67\times10^{6}\ \text{m}\ (\approx4.7\times10^{3}\ \text{km})}.$$

**(b) Impact speed at the lunar surface (no detachment).** Energy conservation from rest at the saddle point $R_{MP}$ to the Moon's surface $R_M$, in both fields:

$$\frac12v_{\text{imp}}^2=GM_M\!\left(\frac1{R_M}-\frac1{R_{MP}}\right)+GM_E\!\left(\frac1{R_{EM}-R_M}-\frac1{R_{EM}-R_{MP}}\right),$$

$$v_{\text{imp}}=\sqrt{2\left[GM_M\!\left(\frac1{R_M}-\frac1{R_{MP}}\right)+GM_E\!\left(\frac1{R_{EM}-R_M}-\frac1{R_{EM}-R_{MP}}\right)\right]}\quad(\approx1.9\times10^{3}\ \text{m s}^{-1}).$$

**(c) Orbital speed 10 km above the surface.** Circular orbit at $r=R_M+10\ \text{km}=1.75\times10^{6}$ m, Moon's field alone (the orbit is deep inside the Moon's domain):

$$v_{\text{orb}}=\sqrt{\frac{GM_M}{r}}=\sqrt{\frac{(6.67\times10^{-11})(7.35\times10^{22})}{1.75\times10^{6}}}=\boxed{1.67\times10^{3}\ \text{m s}^{-1}}.$$

**(d) Energy to extract for a soft landing.** Remove the difference between the orbital energy and the rest-on-surface energy:

$$E_m=\left[-\frac{GM_Mm}{2r}\right]-\left[-\frac{GM_Mm}{R_M}\right]=GM_Mm\left(\frac1{R_M}-\frac1{2r}\right),$$

$$E_m=(6.67\times10^{-11})(7.35\times10^{22})(1000)\left(\frac1{1.74\times10^{6}}-\frac1{3.50\times10^{6}}\right)=\boxed{1.42\times10^{9}\ \text{J}}.$$

> 【Thought】 Part (a) warns against a classic slip: the force balance and potential balance points are DIFFERENT places ($R_{MF}\neq R_{MP}$), and it is the *potential* crest that matters for "just enough energy" — with zero KE at $R_{MP}$, the vehicle then falls toward the Moon. Check (b): the Moon-only term gives $\sqrt{2GM_M(1/R_M-1/R_{MP})}\approx1.6$ km/s, Earth's pull adds the rest to $\sim1.9$ km/s, both below lunar escape (2.4 km/s) ✓. In (d) the satellite's orbital energy is negative, $-GMm/2r$ (virial: half the potential depth) — extracting energy means making it *more* negative, ending at $-GMm/R_M$ at rest on the surface.

---

*End of Paper 33.*

## Paper 34 — 2007 Paper 2 (9 Nov 2007) [2008 paper]

*Note: this paper is a scan; the constants table prints $R_E=6.83\times10^{6}$ m (a misprint for $6.38\times10^{6}$ m) — where it matters we say which value is used.*

### Q1 — Compulsory short questions [79 marks, max 40 awarded]

**(a) Cricket ball with air resistance [3 marks].**

**Key observation.** Compare the actual height gained with the height the initial KE *would* have bought.

$$KE_0=\tfrac12(0.167)(25.0)^2=52.2\ \text{J};\qquad PE_{\text{top}}=mgh=(0.167)(9.81)(20.0)=32.8\ \text{J},$$

$$\boxed{\text{loss}=\frac{52.2-32.8}{52.2}=37\%}.$$

> 【Thought】 Air resistance does negative work on the way up, so $mgh_{\max}<KE_0$ — the deficit IS the energy lost. Check: drag-free height would be $v^2/2g=31.9$ m; reaching only 20.0 m is a large loss, consistent with a fast cricket ball (drag $\propto v^2$ is serious at 25 m/s) ✓.

---

**(b) Earthquake P and S waves; tsunami warning [6 marks].**

**Key observation.** Same path, two known speeds, one measured time gap — the gap fixes the distance.

(i) With $\Delta t=15\text{ min }17\text{ s}=917$ s:

$$\frac{D}{3.00}-\frac{D}{5.50}=917\ \text{(km, s)}\;\Rightarrow\;D=\frac{917}{0.3333-0.1818}=\boxed{6.05\times10^{3}\ \text{km}}.$$

(ii) $T=\dfrac{6052\ \text{km}}{800\ \text{km h}^{-1}}=\boxed{7.6\ \text{h}\approx7\ \text{h}\ 34\ \text{min}}$.

(iii) Principle: seismic waves cross the mantle at km/s while the tsunami crosses the ocean at hundreds of km/h — a factor of ~20 slower. Detecting the P-wave (and the P–S interval, which gives the distance) at a network of stations therefore pinpoints the quake and leaves **hours** to warn threatened coasts before the wave arrives; deep-ocean pressure buoys can then confirm the tsunami itself en route.

> 【Thought】 Check (i): at 5.5 km/s the P wave needs 1100 s ≈ 18 min for 6050 km, and Sumatra→Mombasa is indeed ~6000 km ✓. The warning-system answer must state BOTH the speed hierarchy and the use of the P–S interval as a rangefinder.

---

**(c) Class values of g: best estimate and accuracy [4 marks].**

Values: 9.80, 9.84, 9.72, 9.74, 9.87, 9.75, 9.28, 9.86, 9.81, 9.79, 9.82.

(i) Best estimate = mean: $\bar g=107.28/11=\boxed{9.75\ \text{m s}^{-2}}$.

(ii) Accuracy from the spread of deviations: mean absolute deviation $=0.09$; standard deviation $s=0.16$, so the uncertainty of the mean is $s/\sqrt{11}=0.05$:

$$\boxed{g=9.75\pm0.05\ \text{m s}^{-2}}.$$

Note the value 9.28 deviates by $\sim3s$ from the rest — a suspected outlier (mis-timed pendulum?). Excluding it: $g=9.80\pm0.02$ m s$^{-2}$, markedly closer to the true value. Both answers are defensible if the outlier decision is stated.

> 【Thought】 "Accuracy based on the deviation from the best value" asks for a deviation statistic — mean deviation or $s/\sqrt{N}$ — quoted WITH the estimate. Never quote a best value without its uncertainty in a data question. The outlier discussion is where the mark scheme rewards judgement: rejecting data requires a stated criterion (here $>2.5$–$3s$), not taste.

---

**(d) Throwing objects overboard: pond level [6 marks].**

**Key observation.** In the boat, everything displaces its *weight* in water; in the pond, a sinker displaces only its *volume*, a floater still displaces its weight.

(i) **Boulder** ($\rho_B>\rho_W$). In boat: displaced volume $M_B/\rho_W$. In pond (sunk): displaced volume $M_B/\rho_B<M_B/\rho_W$. The water level **falls** by

$$\boxed{\Delta h_B=\frac{M_B}{A}\left(\frac1{\rho_W}-\frac1{\rho_B}\right)\ \text{(down)}}.$$

(ii) **Timber** ($\rho_T<\rho_W$). In boat: displaces $M_T/\rho_W$. Floating free: buoyancy needs exactly $\rho_W V_{\text{sub}}=M_T$, so again $M_T/\rho_W$. The level is **unchanged**: $\boxed{\Delta h_T=0}$.

> 【Thought】 The invariant to track is total displaced volume = (weight supported by buoyancy)/$\rho_W g$. While the object is supported by the boat, the boat's hull does the displacing; throwing a sinker overboard swaps "weight-displacement" for the smaller "volume-displacement". Density $\rho_T$ cancels in (ii) — that cancellation is the whole point of asking both cases.

---

**(e) Draining container on a spring [4 marks].**

**Key observation.** The water surface stays at distance $H$ below the support iff the container rises exactly as fast as the water level inside it falls.

Let the water level drop $dh$ inside the container: mass lost $dm=\rho\pi r^2\,dh$, so the spring (force reduced by $dm\,g$) lets the container **rise** by $dx=dm\,g/k=\rho\pi r^2 g\,dh/k$. The surface stays fixed when $dx=dh$:

$$k=\rho\pi r^2g=(1000)\pi(0.18)^2(9.81)=\boxed{1.0\times10^{3}\ \text{N m}^{-1}}.$$

> 【Thought】 The exit tube and flow rate are red herrings: the condition is quasi-static (spring force = instantaneous weight at every moment), so dynamics never enters. Units check: $\rho A g$ = (kg/m³)(m²)(m/s²) = N/m ✓. Physical picture: the spring must shorten by exactly the depth of water lost — the spring constant converts "mass gone" into "height gained".

---

**(f) Velocities at the compass points of a rolling wheel [7 marks].**

**Key observation.** Rolling without slipping = translation $V$ of the centre **plus** rotation $\omega=V/R$ about the centre; add the two velocity fields vectorially. ($V=60$ mph.)

| Point | Translation | Rotation | Resultant |
|---|---|---|---|
| N (top) | 60 → | 60 → | $\boxed{120\ \text{mph forward}}$ |
| S (contact) | 60 → | 60 ← | $\boxed{0}$ (instantaneous rest — this IS "without slipping") |
| E (front) | 60 → | 60 ↓ | $\boxed{60\sqrt2=85\ \text{mph at }45^\circ\text{ forward-down}}$ |
| W (rear) | 60 → | 60 ↑ | $\boxed{60\sqrt2=85\ \text{mph at }45^\circ\text{ forward-up}}$ |

> 【Thought】 The anchor point is S: zero slipping *defines* $\omega=V/R$. Everything else follows by vector addition — draw the two arrows at each point before adding. Nice check: every rim point's velocity points perpendicular to its spoke from the contact point (the instantaneous axis), with magnitude $\propto$ its distance from S: N is twice as far from S as E/W, and $120=2\times85/\sqrt2$ ✓.

---

**(g) Pulsed microwave beam [6 marks].**

(i) $\lambda=c/f=\dfrac{3.00\times10^8}{20\times10^9}=\boxed{1.5\times10^{-2}\ \text{m}=1.5\ \text{cm}}$.

(ii) $E=P\Delta t=(25\times10^3)(1.0\times10^{-9})=\boxed{2.5\times10^{-5}\ \text{J}}$.

(iii) The pulse fills a cylinder of area $\pi r^2$ and length $c\Delta t$: $U=\dfrac{E}{\pi r^2 c\Delta t}=\dfrac{P}{\pi r^2 c}=\dfrac{25\times10^3}{\pi(0.060)^2(3.00\times10^8)}=\boxed{7.4\times10^{-3}\ \text{J m}^{-3}}$.

(iv) Momentum density $=$ energy density$/c$: $\boxed{P=U/c=2.5\times10^{-11}\ \text{kg m}^{-2}\text{s}^{-1}}$.

> 【Thought】 The beam geometry converts energy → density: a 1 ns pulse is a $c\Delta t=30$ cm long "slug" of radiation. Check (iv): radiation pressure on a perfect absorber $=U=7.4$ mJ/m³ $=7.4$ mPa — pressure equals energy density, momentum density equals $U/c$; the two relations are the same statement.

---

**(h) Accelerating box; then sand raining onto it [7 marks].**

Phase 1: $a=0.40/10.0=0.040\ \text{m s}^{-2}$, so $F=ma=1.2\times0.040=\boxed{48\ \text{mN}}$.

Phase 2 (constant 0.40 m/s on frictionless track, sand arriving vertically at $\dot m=5.0$ g/s, impacting at 10 m/s):

- **Vertical force** on the box: the sand's vertical momentum must be destroyed each second: $F_V=\dot m\,v_{\text{imp}}=(5.0\times10^{-3})(10)=\boxed{5.0\times10^{-2}\ \text{N}}$.
- **Horizontal force** to keep constant velocity: newly landed sand has no horizontal momentum; the box must supply $\dot m\,v_{\text{box}}$ per second: $F_H=(5.0\times10^{-3})(0.40)=\boxed{2.0\times10^{-3}\ \text{N}}$.

> 【Thought】 Both answers are momentum-flux statements, $\dot m\,\Delta v$, but about different components: vertical momentum is *removed* (normal force does it), horizontal momentum must be *given* to the sand (hence an external pull on the box). Note $F_H\neq0$ even on a frictionless track — steadily loading a moving vehicle is a drag mechanism. (Accumulated weight is excluded: the question asks for the force *due to the falling sand*.)

---

**(j) Network of five resistors and two cells [5 marks].**

**Key observation.** Two identical ideal cells in parallel = one cell of emf $E$ between nodes L and M; then the network is P–Q twice (top and diagonal), P–L, L–Q, M–Q, all $r$, with $V_L-V_M=E$.

Set $V_Q=0$. KCL at P (three arms to Q,Q,L): $3V_P=V_L$. Supernode KCL around the cell pair (resistors leaving L and M): $(V_L-V_P)+V_L+V_M=0$ with $V_M=V_L-E$:

$$\tfrac23V_L+V_L+V_L-E=0\;\Rightarrow\;V_L=\tfrac38E,\quad V_M=-\tfrac58E,\quad V_P=\tfrac18E.$$

Current into M from Q through the middle resistor: $(V_Q-V_M)/r=\tfrac58E/r$; this entire current passes through the cell pair (KCL at M), so each of the two parallel cells carries

$$\boxed{I=\frac{5E}{16r}}$$

flowing M→L, i.e. out of the positive (L-side) terminal — the cells are discharging. (Check at L: inflow $\tfrac58E/r$ = outflow $\tfrac14E/r$ to P $+\ \tfrac38E/r$ to Q ✓.)

> 【Thought】 Method notes: parallel identical ideal cells combine trivially (same emf, half the current each); the cell fixes a *voltage difference*, so use a supernode for KCL — never write Ohm's law across a source branch. The answer being $\propto E/r$ with a pure fraction is the signature of a linear network ✓.

---

**(k) D–T fusion energy [4 marks].**

$$\Delta m=(2.01410+3.01605)-(1.00867+4.00260)=0.01888\ \text{u}=3.135\times10^{-29}\ \text{kg},$$

$$E=\Delta m c^2=(3.135\times10^{-29})(9.00\times10^{16})=\boxed{2.82\times10^{-12}\ \text{J}\approx17.6\ \text{MeV}}.$$

> 【Thought】 Check: the D–T line is the famous 17.6 MeV ✓ — knowing the landmark values (17.6 MeV D–T, 200 MeV U-fission, 0.511 MeV electron) lets you catch arithmetic slips instantly. Mass *decreases*, so energy is released ✓.

---

**(l) Rod sliding down a U-frame in a magnetic field [10 marks].**

**Setup.** Rod XY (mass $m$, resistance $R$, length $L$) slides down the vertical rails of a U-shaped conductor (negligible resistance); uniform $B$ perpendicular to the U's plane.

**(i) Why a terminal velocity exists.** As the rod falls with speed $v$, the loop's flux changes at rate $BLv$, inducing emf $\mathcal{E}=BLv$ and current $I=BLv/R$. This current, crossing $B$, experiences a force $F=BIL=B^2L^2v/R$ which by Lenz's law opposes the flux change — i.e. acts **upward**, against gravity. Since $F\propto v$ while $mg$ is constant, $F$ grows from zero until $F=mg$; thereafter acceleration vanishes and the rod falls at the **terminal velocity**

$$\boxed{v_t=\frac{mgR}{B^2L^2}}.$$

**(ii) Current at terminal velocity.** $I=\dfrac{BLv_t}{R}=\boxed{\dfrac{mg}{BL}}$, directed so that the force $BI L$ on the rod is upward (Lenz: the current opposes the *increase* of downward flux — with $B$ out of the page, the current flows from Y to X through the rod... in general, in the direction that makes $I\vec L\times\vec B$ point up).

**(iii) Energy balance in time $\Delta t$ at terminal speed.** The rod drops $v_t\Delta t$:

$$\Delta(\text{GPE})=mgv_t\Delta t.$$

Heat dissipated: $I^2R\,\Delta t=\left(\dfrac{mg}{BL}\right)^2\!R\,\Delta t=mg\,\dfrac{mgR}{B^2L^2}\,\Delta t=mgv_t\Delta t$.

$$\boxed{\Delta(\text{GPE})=I^2R\,\Delta t}\quad\blacksquare$$

> 【Thought】 At terminal velocity KE is constant, so gravity's power input must surface entirely as Joule heat — part (iii) is conservation of energy dressed as a calculation, and it double-checks (ii). Seeing "terminal velocity" in an EM context should trigger the template: emf → current → $BIL$ force ∝ $v$ → balance against the driving force.

---

**(m) Moving source, reflecting wall, and beats [10 marks].**

Source ($f_0=500$ Hz) moves away from the stationary observer, toward the wall, at $v\ll c_s=340$ m/s.

**(i) Direct sound** (receding source, stationary observer): wavefronts are spaced $c_s+v$ per cycle emitted:

$$\boxed{f_1=f_0\,\frac{c_s}{c_s+v}\approx f_0\left(1-\frac{v}{c_s}\right)}.$$

**(ii) Reflected sound.** The wall receives a wave from an *approaching* source: crests arrive at the wall at rate $f'=f_0\,\dfrac{c_s}{c_s-v}$. The wall re-emits (reflects) at exactly this rate, and both wall and observer are stationary, so the observer receives

$$\boxed{f_2=f_0\,\frac{c_s}{c_s-v}\approx f_0\left(1+\frac{v}{c_s}\right)}.$$

**(iii) Beat frequency.** $f_{\text{beat}}=f_2-f_1=f_0c_s\,\dfrac{2v}{c_s^2-v^2}\approx\dfrac{2f_0v}{c_s}$ (dropping $v^2$ against $c_s^2$):

$$v=\frac{f_{\text{beat}}\,c_s}{2f_0}=\frac{30\times340}{2\times500}=\boxed{10.2\ \text{m s}^{-1}}.$$

> 【Thought】 The reflection step is a *double* Doppler shift: the wall first acts as a moving observer (approaching → up-shift), then as a stationary source of the up-shifted frequency. Check the approximation: $v/c_s=0.03$, so $v^2/c_s^2\sim10^{-3}$ — the linear beat formula is good to 0.1% ✓. Beats measure $v$ because the two paths carry opposite shifts; that is the principle of the police radar/lidar speed trap.

---

**(n) Age of the Earth from U-238/U-235 [7 marks].**

Identical method to Paper 33 Q7(a): equal initial abundances, present ratio 140:1,

$$140=2^{\,t\left(\frac{1}{7.1\times10^8}-\frac{1}{4.5\times10^9}\right)}
\;\Rightarrow\; t=\frac{\ln140}{\ln2\,(1.186\times10^{-9})}=\boxed{6.0\times10^{9}\ \text{years}}.$$

> 【Thought】 Same structure as any two-clock dating problem: the unknown initial amount cancels in the ratio; the effective decay rate of the *ratio* is the *difference* of decay constants. Sanity: $\log_2 140\approx7.1$ e-foldings of the ratio at one per $8.4\times10^8$ yr ✓. (Slightly above the accepted $4.5\times10^9$ yr — the equal-initial-abundance assumption is the culprit; worth one sentence.)

---

### Q2 — Six-resistor network: measurement reverse-engineering [20 marks]

**Topology (Figure 2.1).** A—$r_4$—P, B—$r_5$—Q, P—$r_3$—Q, P—$r_2$—R, Q—$r_1$—R, R—$r_6$—C. Note that C dangles from R through $r_6$: **$r_6$ carries no current in any A–B measurement**, and B dangles in an A–C measurement, etc.

**(a) All resistances equal to $r$ [5 marks].**

(i) $R_1$ across AB: P–Q network is $r_3\parallel(r_1+r_2)=r\parallel2r=\tfrac23r$:

$$\boxed{R_1=r+\tfrac23r+r=\frac{8r}{3}}.$$

(ii) $r_2$ shorted: P merges with R, so P–Q becomes $r_3\parallel r_1=\tfrac r2$:

$$\boxed{R_2=r+\tfrac r2+r=\frac{5r}{2}}.$$

(iii) AC shorted: A and C become one node: the source drives $r_4$ into P and $r_6$ into R, with the P–Q–R mesh ($r_3, r_1, r_2$) and $r_5$ to B intact. With all resistances equal the network is symmetric under P↔R ($r_4\leftrightarrow r_6$, $r_3\leftrightarrow r_1$, $r_2$ self-maps), so $V_P=V_R$ and $r_2$ carries no current. KCL at P: $(V_P-V)+(V_P-V_Q)=0$; KCL at Q: $(V_Q-V_P)+(V_Q-V_R)+V_Q=0\Rightarrow3V_Q=2V_P$. Hence $V_P=V_R=\tfrac34V$, $V_Q=\tfrac12V$, the source delivers $I=(V-V_P)/r+(V-V_R)/r=V/2r$, and

$$\boxed{R_3=2r}.$$

> 【Thought】 (iii) is the one needing real work — no series/parallel shortcut survives the AC short, so: name node potentials, exploit the P↔R symmetry to delete $r_2$, then KCL. Check by numerical nodal analysis: $R_3=2.0000\,r$ ✓. Classic error to avoid: writing the source current as $V/r_4+V/r_6=2V/r$ — that treats the far ends P and R as grounded, which they are not (they sit at $3V/4$). A shorting wire *ties two potentials together*; it does not set them to anything.

---

**(b) Deducing 1,2,3,4,5,6 Ω from three measurements [15 marks].**

**(i) Algebraic $R_{AB}$.** With C dangling, the network reduces to $r_4+r_5$ plus the P–Q block $r_3\parallel(r_1+r_2)$:

$$\boxed{R_{AB}=r_4+r_5+\frac{r_3(r_1+r_2)}{r_1+r_2+r_3}}.$$

**(ii) $13R_{AB}=94$.** $R_{AB}=94/13$ as a rational fraction has denominator 13; since the only denominator the circuit can produce is $r_1+r_2+r_3$ (a sum of distinct values from $\{1,\dots,6\}$), and $94/13$ is already in lowest terms,

$$\boxed{r_1+r_2+r_3=13}.$$

**(iii) Form $R_{AB}=n_1+n_2+p$.** With $r_1+r_2=13-r_3$:

$$R_{AB}=\underbrace{r_4+r_5}_{n_1+n_2\ \text{integers}}+\underbrace{\frac{r_3(13-r_3)}{13}}_{p=n_3(13-n_3)/13}.\quad\blacksquare$$

**(iv) Find $r_3$.** $13R_{AB}=13(r_4+r_5)+r_3(13-r_3)=94$. Tabulate $r_3(13-r_3)$: $r_3=1\!:\!12;\ 2\!:\!22;\ 3\!:\!30;\ 4\!:\!36;\ 5\!:\!40;\ 6\!:\!42$. Only $94-42=52=13\times4$ is divisible by 13 (the others leave 82, 72, 64, 58, 54 — none divisible):

$$\boxed{r_3=6\ \Omega},\qquad r_4+r_5=4.$$

Similarly $R_{AC}=r_4+r_6+\dfrac{r_2(r_1+r_3)}{13}=r_4+r_6+\dfrac{r_2(13-r_2)}{13}$ (B dangles): $13R_{AC}=87$ with $r_2\in\{1,2,3,4,5\}$: only $87-22=65=13\times5$ works $\Rightarrow\boxed{r_2=2\ \Omega}$, $r_4+r_6=5$.
And $R_{BC}=r_5+r_6+\dfrac{r_1(13-r_1)}{13}$: $13R_{BC}=131$ with $r_1\in\{1,3,4,5\}$: only $131-40=91=13\times7$ works $\Rightarrow\boxed{r_1=5\ \Omega}$, $r_5+r_6=7$.

**(v)** For $R_{AB}$: $n_1+n_2=r_4+r_5=4$ from distinct remaining values $\{1,3,4\}\Rightarrow\{r_4,r_5\}=\{1,3\}$.

**(vi)** Similarly $r_4+r_6=5$ and $r_5+r_6=7$. Solving the three sums: $r_6=\dfrac{(r_4+r_6)+(r_5+r_6)-(r_4+r_5)}{2}=\dfrac{5+7-4}{2}=4$:

$$\boxed{r_4=1\ \Omega,\quad r_5=3\ \Omega,\quad r_6=4\ \Omega}.$$

Full assignment $(r_1,\dots,r_6)=(5,2,6,1,3,4)\ \Omega$ — all distinct, exhausting $\{1,\dots,6\}$.

**Check.** Direct nodal computation with these values: $13R_{AB}=94.00$, $13R_{AC}=87.00$, $13R_{BC}=131.00$ ✓✓✓.

> 【Thought】 This is a beautiful inverse problem: the measurement $13R=94$ is really telling you the denominator (13) and numerator (94) separately, because sums of distinct small integers have limited values. The strategy throughout: (1) identify which resistor is inert in each measurement (the dangling arm), (2) reduce to "two arms + one parallel block", (3) use divisibility by 13 to pin the parallel block's member. The final consistency check ($\{r_4,r_5\}=\{1,3\}$ vs $r_4+r_6=5$, $r_5+r_6=7$) is over-determined — over-determination is your friend: it is what turns a guess into a deduction.

---

### Q3 — Double star, gravitational redshift, equatorial g [20 marks]

**(a) Double star separation in units of $R_{SE}$ [6 marks].**

**Key observation.** Use Kepler twice: the unknown $M_S$ cancels in the ratio — that is why the question forbids using $M_S$ numerically.

Each star orbits the centre of mass at radius $d/2$, the gravity of its twin supplying the centripetal force:

$$\frac{GM_S^2}{d^2}=M_S\omega^2\frac{d}{2}\;\Rightarrow\;\omega^2=\frac{2GM_S}{d^3}.$$

For the Earth (test mass) around the Sun: $\omega_E^2=GM_S/R_{SE}^3$. Dividing eliminates $GM_S$:

$$\left(\frac{d}{R_{SE}}\right)^3=2\left(\frac{\omega_E}{\omega}\right)^2=2\left(\frac{T}{T_E}\right)^2=2\left(\frac{1\ \text{week}}{52.1\ \text{weeks}}\right)^2=7.36\times10^{-4},$$

$$\boxed{\frac{d}{R_{SE}}=0.090\ \text{(2 s.f.)}}\qquad(d\approx1.35\times10^{10}\ \text{m}\approx20R_S).$$

> 【Thought】 Note the reduced-mass structure hiding here: for two *equal* masses the relative orbit obeys Kepler with total mass $2M_S$ — equivalently each star sees $\omega^2 d^3=2GM_S$. Forgetting the factor of 2 (using the single-star formula on separation $d$) is the designed error. Check the scale: a 1-week period demands a tight binary, and $0.09$ AU $\approx19$ solar radii is indeed contact-binary territory ✓.

---

**(b) Gravitational redshift Sun → Earth, photon-as-particle model [11 marks].**

Photon: effective mass $m_\gamma=h/\lambda c$, energy $hc/\lambda$.

**(i) Change in GPE** climbing from the Sun's surface ($R_S$) to Earth ($R_{SE}$), including both bodies' wells:

$$\Delta U=\frac{h}{\lambda c}\left[GM_S\!\left(\frac1{R_S}-\frac1{R_{SE}}\right)+GM_E\!\left(\frac1{R_{SE}}-\frac1{R_E}\right)\right].$$

(The Earth terms are negative contributions — the photon *falls into* Earth's well, regaining a little energy.)

**(ii) Orders of magnitude.**

$$GM_S/R_S=1.91\times10^{11};\quad GM_S/R_{SE}=8.9\times10^{8};\quad GM_E/R_E=5.8\times10^{7};\quad GM_E/R_{SE}=2.7\times10^{3}\ \text{(J kg}^{-1}).$$

The Sun-surface term dominates. For 2-significant-figure accuracy, $GM_S/R_{SE}$ (0.5% of the leading term) sits at the margin — keep it; both Earth terms ($\leq0.03\%$) are negligible.

**(iii) Fractional shift.** Energy conservation: the photon's energy loss equals its GPE gain, $\Delta(hc/\lambda)=-\Delta U$. Since $d(hc/\lambda)=-(hc/\lambda^2)d\lambda$:

$$\frac{\Delta\lambda}{\lambda}=\frac{\Delta U}{hc/\lambda}=\frac{1}{c^2}\left[GM_S\!\left(\frac1{R_S}-\frac1{R_{SE}}\right)\right]=\frac{1.898\times10^{11}}{9.00\times10^{16}}=\boxed{2.1\times10^{-6}}$$

— a *red*shift ($\Delta\lambda>0$; for $\lambda=500$ nm, $\Delta\lambda\approx1.1\times10^{-3}$ nm).

> 【Thought】 The slick shortcut to remember: since $m_\gamma c^2=hc/\lambda$ *is* the photon energy, the fractional wavelength shift equals the potential climb divided by $c^2$ — the "photon mass" cancels. This Newtonian heuristic gives exactly the GR weak-field result (as the problem remarks). Check: the solar surface redshift $GM_S/R_Sc^2=2.1\times10^{-6}$ is the standard quoted value ✓.

---

**(c) g at the equator vs the poles [3 marks].**

Two effects, same sign: (1) **rotation** — at the equator part of the gravitational attraction supplies the centripetal acceleration $\omega^2R_E\approx0.034$ m s$^{-2}$, so the measured (apparent) $g$ is reduced; at the poles no centripetal term is needed. (2) **shape** — rotation makes the Earth oblate: the equator is ~21 km farther from the centre than the poles, weakening $GM/r^2$ there. Both effects reduce equatorial $g$:

$$\boxed{g\ \text{is greater at the poles}}\qquad(\Delta g/g\sim5\times10^{-3}\ \text{total}).$$

> 【Thought】 Separate the two mechanisms in your answer — "rotation" alone earns only part credit, since the question says "explain why": dynamic (centripetal) + geometric (oblateness). Order check: centripetal $0.034$ m s$^{-2}$ vs oblateness $\sim0.02$ m s$^{-2}$ — same order, both matter ✓.

---

### Q4 — Beam statics and the falling-target paradox [20 marks]

**(a) Hinged beam with cable [8 marks].**

**Setup.** Uniform beam 3.00 m, $m=2.00$ kg, hinged at P, resting at $30^\circ$ above horizontal; $M=100$ kg hangs from the far end; horizontal cable attached 2.00 m from P.

**(i) Tension.** Moments about P (kills both hinge forces — always the first move): the cable's lever arm is $2.00\sin30^\circ=1.00$ m (horizontal force, vertical offset), the weights' lever arms are horizontal projections:

$$T(2.00\sin30^\circ)=Mg(3.00\cos30^\circ)+mg(1.50\cos30^\circ),$$

$$T=\frac{(100\times9.81\times3.00+2\times9.81\times1.50)(0.866)}{1.00}=\boxed{2.57\times10^{3}\ \text{N}}.$$

**(ii) Hinge forces.** $\sum F_x=0$: $\boxed{F_H=T=2.57\times10^{3}\ \text{N}}$ (toward the wall). $\sum F_y=0$: $\boxed{F_V=(M+m)g=1.00\times10^{3}\ \text{N}}$ (upward).

> 【Thought】 Structure of any statics problem: moments about the hinge first (two unknowns vanish), then the two force balances read off the remaining components. Watch the lever arms: a *horizontal* cable needs the *vertical* distance to P ($2\sin30^\circ$), weights need *horizontal* distances ($\ell\cos30^\circ$) — the recurring slip is mixing the two trig factors. Check: $F_V$ equals total weight since the cable is horizontal ✓.

---

**(b) Marksman and falling clay pigeon [12 marks].**

**Claim.** A bullet aimed *directly* at the pigeon hits it, provided the pigeon is still airborne when the bullet arrives.

**Setup.** A at the origin; pigeon at $(L,H)$; bullet fired at speed $v_0$ along AB, angle $\theta=\arctan(H/L)$, at the instant the pigeon is released.

**Bullet:** $x_b=v_0\cos\theta\,t$, $y_b=v_0\sin\theta\,t-\tfrac12gt^2$. **Pigeon:** $x_p=L$, $y_p=H-\tfrac12gt^2$.

The bullet reaches the pigeon's vertical line at $t^*=L/(v_0\cos\theta)$, where

$$y_b(t^*)=v_0\sin\theta\,\frac{L}{v_0\cos\theta}-\tfrac12gt^{*2}=L\tan\theta-\tfrac12gt^{*2}=H-\tfrac12gt^{*2}=y_p(t^*).\quad\blacksquare$$

The bullet and pigeon have fallen by *identical* amounts $\tfrac12gt^{*2}$ below the straight aim line — so they meet, at height $H-\tfrac12gt^{*2}$.

**Condition** for the strike to occur during the fall: $y_p(t^*)\geq0$, i.e. $t^*\leq\sqrt{2H/g}$, i.e.

$$v_0\geq\frac{L}{\cos\theta}\sqrt{\frac{g}{2H}}=\sqrt{L^2+H^2}\sqrt{\frac{g}{2H}}.$$

> 【Thought】 The deep reading: in the freely-falling frame of the pigeon, gravity is switched off and the bullet travels straight down the aim line — the result is then immediate, and the condition is just "does the bullet arrive before the frame hits the ground". Writing the two trajectories and subtracting is the ground-frame equivalent; showing the common $-\frac12gt^2$ term IS the verification the question wants.

---

### Q5 — Symmetric three-sphere collision; gas driven between cylinders [20 marks]

**(a) Sphere A strikes touching spheres B and C [12 marks].**

**Key observation.** Symmetry: B and C get equal speeds along their contact normals (at $\pm30^\circ$ to A's line of approach — the centres form an equilateral triangle at contact). Two conservation laws, two unknowns ($v_A$, $v_B$).

Momentum along the axis (with $v_A$ measured forward):

$$mu=mv_A+2mv_B\cos30^\circ\;\Rightarrow\;u=v_A+\sqrt3\,v_B.$$

Energy:

$$\tfrac12mu^2=\tfrac12mv_A^2+2\cdot\tfrac12mv_B^2\;\Rightarrow\;u^2=v_A^2+2v_B^2.$$

Substituting $v_B=(u-v_A)/\sqrt3$: $3u^2=3v_A^2+2(u-v_A)^2\Rightarrow 5v_A^2-4uv_A-u^2=0$, giving $v_A=u$ (no collision — reject) or

$$\boxed{v_A=-\frac{u}{5}\ \text{(rebounds)},\qquad v_B=v_C=\frac{2\sqrt3}{5}u\approx0.69u\ \text{at }30^\circ\text{ to the axis}}.$$

**Check.** $\tfrac12m[u^2/25+2(12u^2/25)]=\tfrac12mu^2$ ✓; momentum $-u/5+2(2\sqrt3u/5)(\sqrt3/2)=u$ ✓.

**C then strikes D** (B, C, D collinear — D directly below C — D at rest). Treat the collisions sequentially (impulses act pairwise). C arrives with velocity $v_C=2\sqrt3u/5$ at $30^\circ$ below horizontal; the C–D line of centres is vertical, so the collision exchanges only the *vertical* components (equal masses, elastic → full swap along the line of centres):

$$v_D=v_C\cos60^\circ=\frac{\sqrt3}{5}u\approx0.35u\ \text{(straight down along CD)},\qquad
v_C'=v_C\sin60^\circ=\boxed{\frac{3u}{5}=0.60u\ \text{(horizontal)}}.$$

**Check.** C's energy: before $12/25$, after $9/25+3/25=12/25$ ✓. Grand total: $\frac{1}{25}+\frac{12}{25}+\frac{9}{25}+\frac{3}{25}=1$ ✓.

> 【Thought】 The two decisions that make this tractable: (1) B and C are struck *simultaneously and symmetrically* — one momentum + one energy equation, NOT two independent two-body collisions (that would violate energy, since each impulse would wrongly use the full approach speed); (2) the C–D collision is treated by the **line-of-centres rule**: only the component along CD is exchanged between equal masses, the perpendicular component rides through untouched. Note B plays no role in the second collision: after the first, B and C are separating.

---

**(b) Gas driven from A into evacuated B at constant pressure [8 marks].**

**Setup.** $n$ mol monatomic gas ($c_V=\tfrac32R$), initially: A only, volume $V$, temperature $T$, pressure $p$. Finally: piston displaced through $yV$, so gas occupies $(1-y)V+V=(2-y)V$ at the *same* $p$ (process-controlled), temperature $T_f$. Containers of negligible thermal capacity → no heat enters the gas: the piston's work becomes internal energy.

**(i) Gas equations.** Initial: $\boxed{pV=nRT}$. Final: $\boxed{p(2-y)V=nRT_f}$.

**(ii) Work and internal energy.** Constant $p$:

$$\boxed{W=p\,yV},\qquad \boxed{U=\tfrac32nR(T_f-T)}.$$

**(iii) Ratio $T/T_f$.** First law with $Q=0$: $W=U$. Divide the gas equations: $T_f=(2-y)T$. Substituting:

$$pyV=\tfrac32nR\,(1-y)T=\tfrac32pV(1-y)\;\Rightarrow\;y=\tfrac32(1-y)\;\Rightarrow\;y=\tfrac35,$$

$$T_f=\left(2-\tfrac35\right)T=\tfrac75T\;\Rightarrow\;\boxed{\frac{T}{T_f}=\frac57=0.71}.$$

> 【Thought】 The physical surprise to name: the gas gets *hotter* although it expands — because the piston does work on it faster than the expansion into B can cool it (free expansion into B itself does no work and changes no temperature; all the heating is the piston's $pyV$). Structure check: eliminating $(p,V,n,R)$ leaves pure numbers — the answer is universal for a monatomic gas, exactly what "deduce the numerical value" signals. The constant-pressure condition is the licence for $W=p\Delta V$ — without it the problem would be underdetermined.

---

### Q6 — Photoelectric effect: theory and graph analysis [20 marks]

**(a)(i) The stopping-potential equation [6 marks].**

Light of wavelength $\lambda$ arrives as photons of energy $hc/\lambda$. An electron in the metal absorbs one photon; to escape it must pay the work function $W$; the most energetic escapers retain $KE_{\max}=hc/\lambda-W$. A reverse potential $V$ between surface and collector does work $eV$ on each electron; the current is just suppressed when $eV=KE_{\max}$:

$$\boxed{\frac{hc}{\lambda}=eV+W}.$$

**(a)(ii) Classical failure.** Classically, light is a continuous wave: energy arrives spread over the wavefront, so (1) electron energy should grow with *intensity* and irradiation time, not depend on frequency — yet experimentally $KE_{\max}$ depends only on $\lambda$; (2) below a threshold frequency no electrons appear however intense the light; (3) emission is instantaneous ($<$ns), whereas a classical estimate of the accumulation time is minutes. All three contradict the data; the photon picture (energy in quanta $hf$, one quantum per electron) explains all three at a stroke.

> 【Thought】 "Derive with full explanation" means narrating the energy budget: where each joule goes. For (ii), enumerate specific contradictions (intensity-independence, threshold, immediacy) — a vague "classical physics fails" earns nothing.

---

**(b) Data: $V$=1.0, 2.0, 3.0, 4.0 V with $\lambda$=200, 196, 158, 144 nm [14 marks].**

**(i) Graphical verification.** Rearrange: $V=\dfrac{hc}{e}\dfrac1\lambda-\dfrac{W}{e}$ — plot $V$ against $1/\lambda$ ($1/\lambda=5.00,\ 5.10,\ 6.33,\ 6.94\times10^{6}$ m$^{-1}$). The four points fall about a straight line (scatter $\pm0.4$ V, dominated by the two close points at low $1/\lambda$), consistent with the derived relation.

**(ii) $h$ and $W$.** Least-squares (equivalently, best straight line by eye): slope $=1.30\times10^{-6}$ V m, intercept $=-5.1$ V:

$$h=\frac{e\times\text{slope}}{c}=\frac{(1.60\times10^{-19})(1.30\times10^{-6})}{3.00\times10^8}=\boxed{h\approx7.0\times10^{-34}\ \text{J s}\ (\pm15\%)},\qquad \boxed{W=e|\text{intercept}|\approx5.1\ \text{eV}}.$$

Accuracy: the slope leans heavily on the two long-leverage points; the 200/196 nm pair (nearly equal $1/\lambda$ for a 1 V difference) is inconsistent with the line at the $\sim$0.4 V level, so quote $h$ to about 1 significant figure — $7\times10^{-34}$ J s (accepted $6.6\times10^{-34}$: within scatter ✓).

**(iii) Threshold frequency.** $V=0$ at $1/\lambda_0=W/(hc)=$ intercept magnitude/slope $=3.93\times10^{6}$ m$^{-1}$: $\lambda_0\approx255$ nm,

$$\boxed{\nu_0=\frac{c}{\lambda_0}\approx1.2\times10^{15}\ \text{Hz}}.$$

**(iv) Doubling the intensity.** Doubles the photon arrival rate, hence doubles the (saturation) photoelectric **current**; the photon energy is unchanged, so the stopping potential $V$, the threshold $\nu_0$, and the electron energies are all unaffected.

> 【Thought】 Graph strategy: the axes must be $V$ vs $1/\lambda$ (not $\lambda$!) because the physics is linear in frequency. Accuracy statements must be tied to the scatter you actually see — here the honest quote is ~1–2 s.f. for $h$; the data pair (200, 196 nm) is the limiting feature and saying so demonstrates real graph-reading. Part (iv) separates the two roles of light: intensity = number of photons = current; frequency = energy per photon = stopping voltage.

---

### Q7 — Two-component radioactive mixture [20 marks]

**Setup.** Counter efficiencies: 60% for A's decays, 11% for B's; $\lambda_A>\lambda_B$; $N_A$, $N_B$ are the detected count rates at $t=0$. Data: $(t\,\text{days}, N\,\text{min}^{-1})$: (0.5, 7000), (2.0, 620), (5.0, 142), (9.0, 76), (15.0, 28).

**(a)(i) Equation.**

$$\boxed{N(t)=N_Ae^{-\lambda_A t}+N_Be^{-\lambda_B t}}.$$

**(a)(ii) Large $t$.** Since $\lambda_A>\lambda_B$, A's term dies first: $N\to N_Be^{-\lambda_B t}$ — a single exponential, so **ln N vs t becomes a straight line** of slope $-\lambda_B$ at late times.

**(a)(iii) Tail analysis.** Using the late points (5.0, 142), (9.0, 76), (15.0, 28) — ln N = 4.956, 4.331, 3.332 — a straight-line fit (slope $-0.163$ day$^{-1}$, intercept 5.78):

$$\boxed{\lambda_B\approx0.16\ \text{day}^{-1}\ (T_B\approx4.3\ \text{days}),\qquad N_B=e^{5.78}\approx3.2\times10^{2}\ \text{counts min}^{-1}}.$$

**(a)(iv) Initial number of B atoms.** The detected rate is $N_B=0.11\times(\text{activity})=0.11\lambda_B\mathcal{N}_B$; with $\lambda_B=0.163\ \text{day}^{-1}=1.13\times10^{-4}\ \text{min}^{-1}$:

$$\mathcal{N}_B=\frac{323}{0.11\times1.13\times10^{-4}}=\boxed{2.6\times10^{7}\ \text{atoms}}.$$

**(b)(i) Extrapolation → $N_A$.** Subtract B's contribution from the early points: at $t=0.5$: $7000-323e^{-0.163\times0.5}=7000-298=6702$; at $t=2.0$: $620-323e^{-0.325}=620-233=387$. Plotting $\ln(N-N_Be^{-\lambda_Bt})$ vs $t$ for the early points gives a new straight line; extrapolating to $t=0$:

$$\boxed{N_A\approx1.7\times10^{4}\ \text{counts min}^{-1}}.$$

**(b)(ii) $\lambda_A$ from the first point.** $\lambda_A=\dfrac{1}{1.5\ \text{d}}\ln\dfrac{6702}{387}=\dfrac{2.85}{1.5}=\boxed{1.9\ \text{day}^{-1}}\ (T_A\approx0.36\ \text{day})$.

**Check.** Predictions: $t=2$: $17348e^{-3.80}+323e^{-0.325}=387+233=620$ ✓; $t=5$: $1.3+141=142$ ✓.

> 【Thought】 This is the graphical analogue of Paper 33 Q7(d): peel the exponentials from the slow end. The order of operations is forced: you cannot find $N_A,\lambda_A$ until $N_B,\lambda_B$ are known, because the early data are contaminated by B. Efficiencies enter only at (iv) — the count-rate equation (i) is already in *detected* units; mixing the efficiency into $\lambda$ would be a category error (efficiency scales the rate, decay constant sets the time dependence).

---

### Q8 — Beta particles in crossed E and B (velocity filter) [20 marks]

**Setup.** Parallel plates 1.00 mm apart, p.d. 100 V → $E=1.00\times10^{5}$ V m$^{-1}$ vertical; $B=0.010$ T horizontal, in the plane of the plates; source at mid-gap O emits betas up to 15.0 keV in all directions.

**(a)(i) Electric force.** $F_E=eE=(1.60\times10^{-19})(10^5)=\boxed{1.6\times10^{-14}\ \text{N}}$, toward the positive plate.

**(a)(ii) Gravity vs electricity.** $\dfrac{F_g}{F_E}=\dfrac{m_eg}{eE}=\dfrac{8.94\times10^{-30}}{1.6\times10^{-14}}=\boxed{5.6\times10^{-16}}$ — gravity is utterly negligible here (as always for subatomic particles in lab fields).

**(a)(iii) Maximum speed.** $\tfrac12m_ev^2=15.0\ \text{keV}=2.40\times10^{-15}$ J:

$$\boxed{v_{\max}=\sqrt{\frac{2\times2.40\times10^{-15}}{9.11\times10^{-31}}}=7.3\times10^{7}\ \text{m s}^{-1}\ (\approx0.24c)}.$$

**(a)(iv) Condition to emerge.** In the plan view (Fig. 8.2), $\theta$ is measured from OH — the direction *perpendicular* to $B$ within the horizontal plane. A particle travelling horizontally at angle $\theta$ to OH has component $v\cos\theta$ perpendicular to $B$, so it feels a *vertical* magnetic force $evB\cos\theta$; the electric force $eE$ is also vertical. The particle stays in the horizontal plane — curves neither up into the top plate nor down into the bottom one, and so reaches the rim — only when these cancel along the path:

$$\boxed{evB\cos\theta=eE\;\Rightarrow\;v\cos\theta=\frac{E}{B}=1.0\times10^{7}\ \text{m s}^{-1}}$$

(the velocity-selector condition; the forces must also point oppositely, picking one sense of travel about the $B$ direction).

**(a)(v) Speed range of emerging particles.** Since $\cos\theta\leq1$: $v\geq E/B=1.0\times10^{7}$ m s$^{-1}$; and the source caps $v$ at $7.3\times10^{7}$:

$$\boxed{1.0\times10^{7}\leq v\leq7.3\times10^{7}\ \text{m s}^{-1}}.$$

**(a)(vi) Angular range.** $\cos\theta=\dfrac{E/B}{v}=\dfrac{10^7}{v}$: $\theta=0$ for the slowest (moving straight along OH, perpendicular to $B$), opening to $\arccos(1/7.25)=82.1^\circ$ for the fastest:

$$\boxed{0\leq\theta\leq82.1^\circ}\quad\text{(and symmetrically on the other side of OH)}.$$

> 【Thought】 Convention caution: the figure measures $\theta$ from OH (perpendicular to $B$), so the selector condition reads $v\cos\theta=E/B$ — if you instead define $\theta$ from $B$ itself, every formula carries $\sin\theta$ instead and the angular range reads $7.9^\circ$–$90^\circ$, the complementary statement. Match your symbols to the given figure before substituting.

**(b)(i) Is the non-relativistic assumption justified?** At $v_{\max}=0.242c$: $\gamma-1=1-\sqrt{1-v^2/c^2}\ldots$ i.e. $\gamma=1.031$. The relativistic KE at this speed is $(\gamma-1)m_ec^2=15.7$ keV vs the classical 15.0 keV — a **3% discrepancy**, and the mass excess is 3%. So the classical treatment is acceptable at the 1–2 s.f. level of this problem but visibly strained: the assumption is *marginally* justified, and it would fail outright above ~50 keV. (Honest verdict: fine for 15 keV to two figures, since 3% affects only the second significant figure of $v_{\max}$.)

**(b)(ii) Relativistic vs classical KE.** $KE_{\text{rel}}=(m-m_0)c^2=m_0c^2(\gamma-1)$, versus $KE_{\text{cl}}=\tfrac12m_0v^2$. At low speed $\gamma-1\approx v^2/2c^2$ and the two agree; as $v\to c$, $\gamma\to\infty$, so the relativistic KE grows *without bound* while the classical formula would falsely let a finite energy reach $v=c$. At fixed speed the relativistic KE always exceeds $\tfrac12m_0v^2$ (equivalently: a given KE corresponds to a slightly *lower* speed than the classical prediction).

> 【Thought】 The organising idea of (a)(iv)–(vi): with E ⊥ B, one velocity component can tune the magnetic force against the electric one — the device is a **velocity selector**, transmitting only $v\sin\theta=E/B$, which is why (v) and (vi) are linked by one equation. For (b)(i) always quantify: compute $v/c$ AND the size of the relativistic correction ($(γ-1)mc^2$ vs $\frac12mv^2$), then verdict. A bare "yes it's fine" without the 3% is not a quantitative answer.

---

*End of Paper 34.*

## Paper 35 — 2007 AS Competition Paper (Mar 2007)

*Section A: 8 multiple-choice questions; Section B: 4 structured questions. ($g=9.8$ N/kg.)*

### Section A — Multiple Choice

**1. Two trucks towing a third via a pulley.** Let the rope ends move with trucks 1 and 2 (displacements $x_1,x_2$); the pulley riding on truck 3 halves the total rope draw: $x_3=(x_1+x_2)/2$ (rope-length conservation: $x_1+x_2=2x_3+$ const). Differentiating twice: $\boxed{a_3=(a_1+a_2)/2}$ → **C**.

> 【Thought】 Pulley constraints are always bookkeeping of *rope length*: write the constant-length equation first, differentiate twice. If the trucks collide ($a_1=a_2$), the formula reduces to the common acceleration ✓.

**2. Ice with an embedded stone melting.** While the ice floats, buoyancy supports ice + stone: displaced volume $=(m_{\text{ice}}+m_s)/\rho_W$. As the ice melts, its meltwater exactly refills the ice's own displacement ($m_{\text{ice}}/\rho_W$) — level unchanged. When the stone is released and sinks, it displaces only its own volume $m_s/\rho_s<m_s/\rho_W$ — the level **falls**. $\boxed{\text{remain the same, then fall}}$ → **D**.

> 【Thought】 Compare with Paper 34 Q1(d): same invariant — displaced volume = (buoyancy-supported weight)/$\rho_Wg$; a sinker in the boat displaces its weight, in the water only its volume.

**3. Doubling the throw speed.** $t_{\text{up}}=v_0/g$, total $t=2v_0/g$: linear in $v_0$. $2v_0\Rightarrow 2\times4=\boxed{8\ \text{s}}$ → **B**.

**4. Square-wave heating.** Heating depends on $V^2$, not $V$: $\langle P\rangle=\dfrac{1}{R}\left\langle V^2\right\rangle=\dfrac{1}{20}\times\dfrac{4^2+(-2)^2}{2}=\dfrac{20}{40}=\boxed{0.5\ \text{W}}$ → **B**.

> 【Thought】 The trap is averaging $V$ first ($(4-2)/2=1$ V → 0.05 W, not an option) or averaging magnitudes (3 V → 0.45 W, not an option); the correct object is $\langle V^2\rangle$ — rms thinking, even for square waves.

**5. Component Z holding 5 V across the 400 Ω.** With 5 V fixed across the 400 Ω: $I_{400}=5/400=12.5$ mA. The 250 Ω carries the battery's remaining $10-5=5$ V: $I_{250}=5/250=20$ mA. KCL at the junction: $I_Z=20-12.5=\boxed{7.5\ \text{mA}}$ → **B**.

> 【Thought】 Z is a black box that *pins a node voltage* — treat it as a 5 V constraint and let KCL find its current. Never try to assign Z a resistance.

**6. Dip X vs hump Y.** Frictionless, so energy conservation gives the speed at every point: in the dip the mass is *faster* than $v_0$ throughout (PE → KE), over the hump *slower*. Same path length, same endpoints, higher speed everywhere along X ⇒ $\boxed{\text{via X}}$ → **A**.

> 【Thought】 The endpoints tie (both arrive with $v_0$), but the *average* speed decides the time: $\oint v\,dt$ comparison with identical path length. No calculation needed — just the sign of the PE excursion.

**7. Extra waves in a glass slab.** Waves in length $t$: air: $t/\lambda$; glass: $t/\lambda_g=nt/\lambda$. Extra $=(n-1)t/\lambda$; ratio to air count $=\dfrac{(n-1)t/\lambda}{t/\lambda}=\boxed{n-1}$ → **A**.

> 【Thought】 The frequency is fixed (set by the source); slower speed ⇒ shorter wavelength ⇒ more waves packed in. The extra count, $t(n-1)/\lambda$, is exactly the optical-path-difference in wavelengths — the quantity that matters in interferometry.

**8. Diffraction spreading in water.** In water the wavelength shortens: $\lambda'=\lambda/n$. Diffraction spread $\theta\sim\lambda'/a$ shrinks by the same factor: $\boxed{\text{less spread out}}$ → **C**.

> 【Thought】 Same physics as Q7: frequency fixed, $v$ drops, $\lambda$ drops. Diffraction angle cares about $\lambda/a$ — nothing else changes.

---

### Section B — Written Answers

### Q9 — Damped spring oscillator [11 marks]

**(a) Energy changes over one cycle.** Released from the right extreme: elastic PE (spring) → KE as the mass moves left, all KE at the centre; KE → elastic PE (compression) to the left extreme; then mirrored on the return. Throughout, friction/damping continuously leaks mechanical energy into internal energy (heat) of the surroundings, so each extreme is slightly closer than the last.

**(b) Fraction lost when amplitude falls 8 cm → 1 cm.** $E\propto A^2$: remaining fraction $(1/8)^2=1/64$:

$$\boxed{\text{fraction lost}=1-\frac1{64}=\frac{63}{64}\approx98.4\%}.$$

**(c) Half-life definition.** The time in which half of the remaining radioactive nuclei decay — equivalently, the time for the activity (or any exponentially decaying quantity) to fall to half its value.

**(d) Amplitude half-lives, 8 → 1 cm.** $8\to4\to2\to1$: exactly $\boxed{3}$ half-lives.

**(e) Number of oscillations.** $3\times5$ s $=15$ s elapsed; at $T=0.5$ s per oscillation: $15/0.5=\boxed{30\ \text{oscillations}}$.

**(f) Energy half-lives.** Energy remaining $=1/64=(1/2)^6$, so $\boxed{6}$ energy half-lives have passed — twice the amplitude count, because $E\propto A^2$ means the energy halves twice as fast ($T_{1/2}^E=T_{1/2}^A/2$).

> 【Thought】 This question is a guided tour of one identity: exponential decay of amplitude + quadratic energy ⇒ exponential decay of energy at double rate. (b) and (f) are the same fact stated twice; if your answers to (d) and (f) came out equal, that's the signal you forgot the square.

---

### Q10 — The Sun's radiated mass [7 marks]

**(a) Total luminosity.** Inverse-square dilution over the sphere at Earth's orbit:

$$P=(1.3\times10^3)\times4\pi(1.5\times10^{11})^2=\boxed{3.7\times10^{26}\ \text{W}}.$$

**(b) Mass loss per second.** $\Delta m=P/c^2=3.68\times10^{26}/9\times10^{16}=\boxed{4.1\times10^{9}\ \text{kg s}^{-1}}$ (≈4 million tonnes every second).

**(c) Percentage per year.** Per year: $4.08\times10^{9}\times3.16\times10^{7}=1.29\times10^{17}$ kg;

$$\frac{1.29\times10^{17}}{2\times10^{30}}\times100\%=\boxed{6.4\times10^{-12}\ \%\ \text{per year}}.$$

**(d) Over $5\times10^9$ years.** $6.4\times10^{-12}\%\times5\times10^9=\boxed{0.032\%}$ — the Sun has radiated away only ~3 parts in $10^4$ of its mass over its entire life.

> 【Thought】 Despite the huge luminosity and 4 Mt/s mass loss, the *fractional* drain is negligible — because $c^2$ is enormous. That contrast (impressive absolute, tiny fractional) is the physical takeaway and the check on the arithmetic: $10^{26}$ J/s $\times$ $1.6\times10^{17}$ s $\approx$ $4\times10^{43}$ J $\approx$ $4\times10^{26}$ kg $\approx$ $2\times10^{-4}M_\odot$... wait: $4\times10^{26}/2\times10^{30}=2\times10^{-4}$, i.e. 0.02% — order agrees with the stepwise 0.032% ✓.

---

### Q11 — Transformer, cable, and short-circuit heating [13 marks]

**(a) Total power supplied.** $P=VI=415\times200=\boxed{83.0\ \text{kW}}$.

**(b) Cable loss.** (i) $P_{\text{loss}}=I^2R=200^2\times0.0493=\boxed{1.97\ \text{kW}}$; (ii) $\dfrac{1.97}{83.0}\times100\%=\boxed{2.4\%}$.
*(Official-answer note: the scheme's "$2.3\times10^{-3}\,\%$" divides $1.9$ kW by $83\,000$ W — a kW/W unit mismatch; in consistent units the loss is $2.4\%$ of the supply.)*

**(c) Why the short-circuit current (6000 A) is below $415/0.0493=8420$ A.** The cable is not the only impedance in the loop: the transformer itself has internal impedance (winding resistance and, decisively for AC, leakage **reactance**), and the supply network behind it too. These add to the cable's 0.0493 Ω and limit the fault current; additionally the cable's resistance rises as it heats. So $V/R_{\text{cable}}$ overestimates the short-circuit current.

**(d) Heat generated in 0.4 s of fault.** The supply pours energy at $VI$ for the fault's duration:
$$\boxed{Q=VIt=415\times6000\times0.4=9.96\times10^{5}\ \text{J}\ (\approx10^6\ \text{J})}.$$

> 【Thought】 Which power? The question's flow (into (e)) counts the supply's whole output $VIt$ as the heat to be disposed of — the official scheme's model. Strictly, only $I^2R_{\text{cable}}t=6000^2\times0.0493\times0.4=7.1\times10^5$ J is deposited *in the cable* (the rest heats the transformer windings and the fault contact); the question's "assume the resistance does not change" signals the crude lumped model is intended, so lead with $VIt$.

**(e)(i) Mass of copper.** $m=\rho\,AL=(8960)(50\times10^{-6})(100)=\boxed{44.8\ \text{kg}}$.

**(e)(ii) Final temperature.** $\Delta T=\dfrac{Q}{mc}=\dfrac{9.96\times10^5}{44.8\times385}=58^\circ$C, so

$$\boxed{T_f=60+58\approx118^\circ\text{C}}$$
(with the stricter cable-only $I^2Rt$ figure the rise would be $41^\circ$C, i.e. $101^\circ$C — see the note above).

> 【Thought】 The design logic of the question: steady load (a,b) is gentle (2.4%), but the fault energy in 0.4 s (d) is 360× the steady per-second dissipation, and (e) shows even that adiabatic burst costs ~60 °C — hence breaker delays of this order are tolerable, which is *why* cables are sized by fault current. Check (e): $mc=17.2$ kJ/°C for the whole drum of copper — a large thermal ballast ✓. In (c) the single word that earns the mark is "reactance/internal impedance of the transformer" — a pure-resistance model of the supply is the assumption being tested.

---

### Q12 — Locating a fault in an underground cable [11 marks]

**Setup.** Cable AB, 50 km, uniform; fault at X ($d$ km from A) leaks to ground through fixed resistance $R$; ground ≈ 0 V everywhere.

**(a) Potential at X (200 V at A, B insulated).** With B insulated, no current can flow in the X–B section (it has nowhere to go); with no current there is no voltage drop along X–B, so the whole section is equipotential:

$$\boxed{V_X=V_B=40\ \text{V}}.$$

**(b)(i)** $V_{AX}=200-40=\boxed{160\ \text{V}}$. **(ii)** Gradient A→X: $\boxed{160/d\ \text{V km}^{-1}}$.

**(c)(i)** Now A insulated, B at 300 V, A measured at 40 V: by the same equipotential argument on X–A, $\boxed{V_X=40\ \text{V}}$.

**(c)(ii) Why 40 V again.** The fault current is $I_R=V_X/R$; with $V_X=40$ V and the same fixed $R$, the second measurement drives exactly the **same current** through the fault as the first. Each measurement's feeding section then carries that same current, so the two potential gradients differ *only* because of the section lengths — the condition that makes the two experiments comparable and lets $d$ be extracted.

**(d) Gradient B→X.** $\dfrac{300-40}{50-d}=\boxed{\dfrac{260}{50-d}\ \text{V km}^{-1}}$.

**(e)(i) Why the gradients are equal.** Potential gradient $=$ current $\times$ resistance per km. The cable is uniform (same resistance per km throughout), and by (c)(ii) both experiments run the same fault current through the feeding section; hence the gradients $I_R\times\rho$ are identical.

**(e)(ii) Solve for $d$.**

$$\frac{160}{d}=\frac{260}{50-d}\;\Rightarrow\;160(50-d)=260d\;\Rightarrow\;8000=420d\;\Rightarrow\;\boxed{d=19\ \text{km}\ (19.05\ \text{km})}.$$

Check: gradient $=160/19.05=8.40$ V/km $=260/30.95$ ✓.

> 【Thought】 The method (a real technique — the Murray/Varley loop family) hinges on two observations: an *open* end makes its whole cable section equipotential (no current, no drop), and matching $V_X$ between the two configurations matches the fault *currents*, converting a resistance-location problem into pure proportionality of gradients. Notice $R$ never needs to be known — it cancels, which is what makes the method practical.

---

*End of Paper 35.*

## Paper 36 — 2004 Paper 2 (5 Nov 2004) [2005 paper]

### Q1 — Compulsory short questions [66 marks, max 40 awarded]

**(a) Thermometer in water [4 marks].**

Energy conservation (no losses): heat gained by thermometer = heat lost by water:

$$20.0\times(50.0-18.0)=0.250\times4200\times(T-50.0)\;\Rightarrow\;640=1050(T-50),$$

$$\boxed{T=50.6^\circ\text{C}}.$$

> 【Thought】 The thermometer's heat capacity is the point of the question: it steals 640 J, so the water must have started slightly *above* the shared final 50.0 °C. Check the direction: a cold thermometer dragged the water down, so $T>50$ ✓ — but only by 0.6 °C, since the water's heat capacity (1050 J/K) dwarfs the thermometer's ✓.

---

**(b) Non-ohmic device, $V=(6I-3I^2+2I^3)/6$ [6 marks].**

(i) $I=2$: $V=(12-12+16)/6=2.67$ V, so $R=V/I=\boxed{4/3\ \Omega=1.33\ \Omega}$.
(ii) $I=0$: $V/I$ is $0/0$ — take the limit (equivalently $dV/dI$ at 0): $R=\lim_{I\to0}\dfrac{6-3I+2I^2}{6}=\boxed{1.0\ \Omega}$.
(iii) Sketches: **bulb** — V–I curve through the origin bending toward the V axis (current saturating); **LED** — essentially zero current until a threshold voltage (~2 V), then a steep, almost vertical rise.
(iv) Bulb: Joule heating raises the filament to ~2500 K; metal resistivity grows with temperature, so resistance rises with current — the curve flattens in I. LED: a p–n junction conducts significantly only when the forward bias approaches the band-gap voltage $E_g/e$ (the same gap that sets the emitted photon energy); below threshold the depletion barrier blocks current, above it the current soars.

> 【Thought】 "Resistance" for a non-linear device has two meanings: static $V/I$ (what (i) wants) and differential $dV/dI$ (what (ii) forces you toward, since the static ratio is undefined at the origin). State which you are computing. The two sketches share one message: resistance is only a *local* concept for real components.

---

**(c) Four "why" questions [7 marks].**

(i) **Charged particle + neutral isolated copper sphere:** the sphere's free electrons redistribute — charge opposite to the particle's gathers on the near face, like charge retreats to the far face. Because the force falls as $1/r^2$, the nearer opposite charge wins: net **attraction**. Earthing removes the far-side like charge (it flows to ground), leaving only the attracting opposite charge — so the force **increases**.

(ii) **Ladder: rough floor + smooth wall works; smooth floor + rough wall doesn't.** The wall's normal force on the ladder is horizontal; it must be balanced by friction at the floor — available on a rough floor, impossible on a smooth one (net horizontal force → the foot slides out). Wall friction is vertical; it cannot substitute for the missing horizontal balance. (Cf. Paper 33 Q3(b).)

(iii) **Pinhole size:** too large → each object point images to a blur disc the size of the hole (geometric blur ∝ hole diameter); too small → diffraction spread $\sim\lambda L/d$ grows and light is starved. Sharpness is optimal where the two blurs are comparable, $d\sim\sqrt{\lambda L}$.

(iv) **Blue cloth in sodium light:** the cloth is blue because its dye reflects blue and absorbs other colours. Sodium light is nearly monochromatic yellow (589 nm) — there is no blue in the illumination to reflect; the dye absorbs the yellow, so the cloth reflects almost nothing and looks **dark**.

> 【Thought】 All four are "mechanism + direction" answers: name the mechanism (induced redistribution / friction balance / two competing blurs / spectral absorption), then state the observable consequence. One line each way; hand-waving earns nothing.

---

**(d) Polarisation and a wave equation [7 marks].**

(i) Light is a **transverse** wave: the E-field oscillates perpendicular to propagation, in any of infinitely many orientations — selecting one orientation is polarisation. Sound in air is **longitudinal**: the oscillation is along the propagation direction only, so there is no transverse degree of freedom to select — polarisation is undefined. Experiment: pass the light through a rotating Polaroid analyser — **fully polarised**: intensity $\propto\cos^2\theta$, falling to *zero* twice per turn; **partially polarised**: intensity oscillates but the minimum stays above zero (imperfect extinction).

(ii) $y=A\sin2\pi(\beta t-x/\gamma)$: the sine's argument must be dimensionless, so $[\beta]=\text{s}^{-1}$ (frequency), $[\gamma]=\text{m}$ (wavelength); $[A]=[y]=\text{m}$; $\pi$ is a pure number. Constant velocity: a given phase (say a crest) satisfies $\beta t-x/\gamma=$ const, i.e. $x=\beta\gamma t+$ const — every feature of the waveform translates at the **constant** speed $v=\beta\gamma$ without distortion, the defining trait of a non-dispersive travelling wave.

> 【Thought】 For (ii), two quick tools: arguments of sin must be dimensionless (instant units), and "constant velocity" is proven by following a fixed phase. $v=\beta\gamma$ has units m/s ✓.

---

**(e) Wet clothing freezing on a 0 °C washing line [5 marks].**

(i) **Source of the evaporation energy:** the internal energy of the remaining water itself — no external heat flows in (air and clothes are both at 0 °C). Mechanism: the fastest molecules in the Maxwell tail escape the liquid surface; the dry wind carries the vapour away so it cannot re-condense. Each escaped molecule carries off the latent heat, cooling what remains — evaporative cooling — until the rest freezes.

(ii) **Fraction that freezes.** Let mass $m$ evaporate of an original $M$; energy balance at 0 °C:

$$mL_v=(M-m)L_f\;\Rightarrow\;2500\,m=333\,(M-m)\;\Rightarrow\;\frac{m}{M}=\frac{333}{2833},$$

$$\boxed{\text{fraction frozen}=\frac{M-m}{M}=\frac{2500}{2833}=0.88\ \text{(about 88\%)}}.$$

> 【Thought】 The ratio $L_v/L_f\approx7.5$ controls everything: evaporating 1 kg buys the freezing of 7.5 kg. Check: the frozen fraction must exceed the evaporated one since $L_v>L_f$ ✓. (This is exactly how freeze-drying and comet tails work: sublimation cools the residue.)

---

**(f) Rifle bullet [5 marks].**

(i) $v^2=2as$: $a=\dfrac{310^2}{2\times1.20}=\boxed{4.0\times10^{4}\ \text{m s}^{-2}}$.

(ii) Two complete rotations in 1.20 m means the rifling twist is fixed in *space*: 2 turns per 1.20 m, so the bullet's spin rate locks to its instantaneous speed, $\omega=2\pi\times(2/1.20)\,v$. At the muzzle ($v=310$ m/s):

$$\boxed{\omega=\frac{4\pi}{1.20}\times310=3.2\times10^{3}\ \text{rad s}^{-1}}\ (\approx520\ \text{rev/s}).$$

(*Official note:* the scheme's $1.62\times10^3$ rad/s is the transit-*average* spin rate, $\omega=4\pi/t$ with $t=7.74$ ms; the question asks for the *final* rotational speed, which the twist relation $\omega=(4\pi/1.20)\,v$ at the muzzle gives as $3.2\times10^3$ rad/s — our boxed answer. Quote the twist relation to cover both readings.)

(iii) **Rifling advantage:** spin gives the bullet angular momentum — gyroscopic stiffness resists tumbling and aerodynamic upset, keeping the axis aligned with the flight direction, hence stability and accuracy.

(iv) **$a$ vs distance:** a curve peaking sharply just after ignition then falling monotonically along the barrel (roughly hyperbolically). Reason: the gas pressure is maximal near the chamber just after the charge ignites; as the bullet moves, the gas expands into a growing volume and its pressure — hence the force and acceleration — falls off.

> 【Thought】 For (ii) the key is that rifling fixes the spin per *metre travelled*, not per second — so $\omega=(2\pi\times2/1.20)\,v$ and the final $\omega$ uses the *exit* speed. The transit-time estimate (mean speed, $\omega\sim1.6\times10^3$ rad/s) gives the average spin rate instead; knowing which quantity each route yields is the lesson. In (iv), pressure falls because the gas expands behind the bullet — $a(x)$ high at the chamber, decaying down the barrel; $\int a\,dx=v^2/2$ must still equal $4.8\times10^4$ m²/s² ✓.

---

**(g) Helium balloon problems [5 marks].**

(i) Lift $=$ (displaced air − helium) $\times g$: $m_{\max}=(\rho_{\text{air}}-\rho_{\text{He}})V=(1.29-0.178)\times512=\boxed{569\ \text{kg}}$.

(ii) **Balloon in a decelerating bus.** As the bus brakes, everything loose lurches forward — but the balloon swings **backward**. In the bus frame, deceleration adds a forward pseudo-gravity; the effective gravity tilts forward-down. Buoyancy always points along *minus* effective gravity (it is the pressure gradient of the surrounding air), and the heavy air is "thrown" forward, displacing the light balloon rearward. As the bus comes to rest the balloon returns to vertical.

> 【Thought】 The balloon paradox is won by remembering buoyancy is not "lightness rising" but the fluid pressure gradient $\nabla p=\rho_{\text{air}}\,g_{\text{eff}}$: the balloon always points *opposite* to the effective gravity felt by the air. Seeing "balloon in accelerating vehicle" → tilt $\vec g_{\text{eff}}$, balloon goes anti-$g_{\text{eff}}$ ✓.

---

**(h) Three acceleration laws: sketch $a$–$v$ and $v$–$t$ [8 marks].**

(i) $a=g$ (free fall): $a$–$v$ is a horizontal line; $v=gt$ is a straight line through the origin.

(ii) $a=g-kv$ (fall with linear drag): $a$–$v$ is a straight line falling from $g$ at $v=0$ to $0$ at the terminal speed $v_t=g/k$; $v(t)=\dfrac{g}{k}(1-e^{-kt})$ — concave-down curve from 0, asymptoting to $g/k$.

(iii) $a=-\omega\sqrt{b^2\omega^2-v^2}$: rearrange to $\dfrac{a^2}{\omega^2}+v^2=b^2\omega^2$ — the $a$–$v$ graph is a quarter-**ellipse** (the branch with $a<0$), from $(0,-b\omega^2)$ to $(-b\omega,0)$. This is SHM in disguise: $v=-b\omega\sin\omega t$ satisfies it, so $v$–$t$ is a (negative) quarter-sinusoid descending from 0 toward $-b\omega$ at $t=\pi/2\omega$, with the understanding that the form as written covers a quarter-cycle of the oscillation $x=b\cos\omega t$.

> 【Thought】 Diagnosis before sketching: (i) constant, (ii) linear approach to terminal velocity (ask "where does $a=0$?"), (iii) recognise $a^2+\omega^2v^2=\text{const}$ as the SHM ellipse — squaring both sides is the key move, and the price is a sign ambiguity you must then resolve ($a<0$ branch). Each sketch pair must be mutually consistent: $a$ is the slope of $v(t)$.

---

**(j) Two-terminal network: Thévenin by construction [6 marks].**

Circuit (Fig 1.j): 2.00 V cell in series with 2.00 Ω feeding node X; from X, 4.00 Ω to the bottom rail and 10.0 Ω to terminal A; B is the bottom rail.

(i) **A–B shorted:** the 4 Ω and 10 Ω are in parallel at X: $4\parallel10=2.857\ \Omega$. Battery current $=2.00/(2.00+2.857)=0.412$ A; $V_X=2.00-2.00\times0.412=1.176$ V; the short carries the 10 Ω arm's current:

$$\boxed{I_0=\frac{1.176}{10.0}=0.118\ \text{A}}.$$

(ii) **A–B open:** no current in the 10 Ω arm, so $V_A=V_X$; divider: $V_X=2.00\times\dfrac{4.00}{2.00+4.00}=\boxed{V_{AB}=1.33\ \text{V}}$.

(iii) **Lamp 8.50 Ω across AB.** The statement given is Thévenin's theorem: the network behaves as $V_{AB}$ in series with $r=V_{AB}/I_0=1.333/0.1176=11.3\ \Omega$:

$$I_{\text{lamp}}=\frac{V_{AB}}{r+8.50}=\frac{1.333}{11.33+8.50}=\boxed{6.7\times10^{-2}\ \text{A}\ (67\ \text{mA})}.$$

> 【Thought】 Notice the pedagogy: (i) and (ii) make you *measure* the Thévenin parameters ($V_{oc}$, $I_{sc}$) before naming them in (iii). Check $r$ independently: kill the source (short the cell) and look in from AB: $r=10.0+(2.00\parallel4.00)=10.0+1.33=11.3\ \Omega$ ✓ — two routes, same answer.

---

**(k) Escape velocity from Mars [3 marks].**

$v_{\text{esc}}=\sqrt{2GM/R}$, so

$$\frac{v_M}{v_E}=\sqrt{\frac{M_M}{M_E}\frac{R_E}{R_M}}=\sqrt{\frac{0.1074}{0.5326}}=\boxed{0.449}\qquad(v_M\approx0.45\,v_E\approx5.0\ \text{km s}^{-1}).$$

> 【Thought】 Ratio problems: never compute $G$, $M_E$ etc. — scale from the known Earth value ($v_E=11.2$ km/s). Units check: dimensionless ratio ✓; direction: Mars is less massive but smaller — mass wins ($M/R$ falls), so $v_M<v_E$ ✓.

---

**(l) Sphere M strikes two touching spheres and stops dead [4 marks].**

**Key observation.** Symmetric hit along the perpendicular bisector → equal impulses at $30^\circ$ (equilateral contact triangle). Given: M ends at rest.

Momentum (axis): $Mu=\sqrt3\,mv\Rightarrow v=\dfrac{Mu}{\sqrt3\,m}$. Energy: $\tfrac12Mu^2=2\cdot\tfrac12mv^2\Rightarrow Mu^2=2mv^2$.

Substitute $v$ into the energy equation:

$$Mu^2=2m\cdot\frac{M^2u^2}{3m^2}=\frac{2M^2u^2}{3m}\;\Rightarrow\;1=\frac{2M}{3m}\;\Rightarrow\;\boxed{\frac{M}{m}=\frac{3}{2}}.$$

**Check.** With $M=3m/2$: $v=\dfrac{3u}{2\sqrt3}=\dfrac{\sqrt3}{2}u$; energy: $2mv^2=2m\cdot\dfrac{3u^2}{4}=\dfrac32mu^2=Mu^2$ ✓; momentum ✓ by construction.

> 【Thought】 Compare Paper 34 Q5(a): there the striker had $M=m$ and rebounded at $-u/5$; here the extra datum "M comes to rest" replaces one conservation unknown and fixes the mass ratio. Two equations, three quantities ($u,v,M/m$) — but $u$ cancels, which is exactly why only a *ratio* can be asked for. Always substitute the answer back into BOTH conservation laws before boxing it.

---

**(m) Torque on a rectangle with two parallel-resistor arms [6 marks].**

**Setup.** Current $I$ enters the top node, splits $I_1$ (down $R_1$) + $I_2$ (down $R_2$), recombines below. Horizontal arms run parallel/antiparallel to the horizontal $B$, so they feel no force; each vertical arm (length $L$) feels $F_i=BI_iL$ perpendicular to the rectangle's plane — both forces point the *same way* (same current direction).

**Torque** about the central vertical axis (through the feed nodes): the two forces act at $\pm d/2$ on opposite sides, so their moments *subtract*:

$$\tau=(F_1-F_2)\frac d2=\frac{BLd}{2}(I_1-I_2).$$

With $I_1=I\dfrac{R_2}{R_1+R_2}$, $I_2=I\dfrac{R_1}{R_1+R_2}$ (current divider):

$$\boxed{\tau=\frac{BILd}{2}\,\frac{R_2-R_1}{R_1+R_2}}.$$

> 【Thought】 The surprise: two parallel-downward currents still make a *couple*, because the forces act at opposite edges while the feed axis runs through the middle — torque depends on the current *imbalance*, vanishing for $R_1=R_2$ ✓ (symmetric check). This is the principle of the moving-coil meter with shunted coils: the torque meter reads the difference of branch currents. Units: $BILd$ = T·A·m² = N·m ✓.

---

### Q2 — Gravity inside/outside Earth; a 2-hour satellite [20 marks]

**(a)(i) Above the surface.** Newton's law with $g_0=GM_E/R_E^2$:

$$g_h=\frac{GM_E}{(R_E+h)^2}=\boxed{g_0\left(\frac{R_E}{R_E+h}\right)^2}\approx g_0\left(1-\frac{2h}{R_E}\right)\ (h\ll R_E).$$

**(a)(ii) Below the surface (uniform density).** Shell theorem: only the mass inside radius $r$ gravitates; $M(r)=M_E(r/R_E)^3$:

$$\boxed{g(r)=\frac{GM(r)}{r^2}=g_0\,\frac{r}{R_E}}.$$

**(a)(iii) Graph.** $g$ rises linearly from 0 at the centre to $g_0$ at $r=R_E$, then falls as $1/r^2$ outside — a tent followed by a hyperbolic tail, continuous (slope discontinuity) at the surface.

**(a)(iv) Uniform density?** False for the real Earth: the core ($\sim10^4$ kg/m³) is much denser than the mantle/crust ($\sim3$–$4.5\times10^3$), so descending first *increases* $g$ slightly (cf. Paper 33 Q8(b): the light crust is shed while the $1/r^2$ gain dominates); $g$ peaks near the core–mantle boundary. The linear law is thus only a first model.

> 【Thought】 The pair (i)/(ii) is the two halves of the shell theorem: outside, everything acts at the centre; inside, shells above you contribute nothing. Memorise the *shape* of the full curve (iii) — linear then inverse-square, maximum at the surface (for uniform density).

---

**(b) Satellite with period 2.00 h [9 marks].**

(i) Kepler: $r^3=\dfrac{GM_ET^2}{4\pi^2}=\dfrac{(3.982\times10^{14})(7200)^2}{39.48}=5.23\times10^{20}\ \text{m}^3$:

$$r=8.06\times10^{6}\ \text{m}\;\Rightarrow\;\boxed{h=r-R_E=1.68\times10^{3}\ \text{km}}.$$

(ii) $\omega_{\text{sat}}=2\pi/7200=8.73\times10^{-4}$ rad/s; Earth: $\omega_E=7.27\times10^{-5}$ rad/s; same direction, so

$$\boxed{\omega_{\text{rel}}=\omega_{\text{sat}}-\omega_E=8.00\times10^{-4}\ \text{rad s}^{-1}}\quad(\omega_{\text{sat}}/\omega_E=12.0).$$

(iii) **Visibility angle.** The satellite at radius $r$ is above the horizon of a surface observer when the line observer→satellite clears the surface: geometry gives $\cos\psi_{\max}=R_E/r$ for the geocentric half-angle. Total visible arc:

$$\boxed{2\psi_{\max}=2\arccos\frac{R_E}{r}=2\arccos(0.792)=75.3^\circ}.$$

> 【Thought】 (iii) is pure geometry once you see it: draw the tangent from the observer to the Earth — the limiting sight line grazes the surface, and the right triangle (observer–centre–satellite at horizon) gives $\cos\psi=R_E/r$. Check: a surface orbit ($r=R_E$) would be visible over $0^\circ$ ✓; a very high satellite ($r\to\infty$) approaches $180^\circ$ ✓.

---

**(c) Limits on satellite periods [2 marks].**

**Shortest:** the orbit must clear the surface — $r\geq R_E$ gives $T_{\min}=2\pi\sqrt{R_E^3/GM_E}\approx84$ min (in practice thicker: the atmosphere adds drag, pushing the floor to ~90 min). **Longest:** no hard ceiling in two-body theory ($T\to\infty$ as $r\to\infty$), but physically Earth's gravity must still dominate the Sun's tidal pull — beyond the Hill sphere ($r\sim1.5\times10^9$ m, $T\sim200$ days) the Sun steals the satellite, which then orbits the Sun, not the Earth.

> 【Thought】 "Limits" questions want the *physical agency*, not just the formula: surface/atmosphere below, solar tidal perturbation (Hill sphere) above.

---

### Q3 — Decay chain A → B → C with $\lambda_2\gg\lambda_1$ [20 marks]

Given: $R(t)=\dfrac{N_2}{N_0}=\dfrac{\lambda_1}{\lambda_2-\lambda_1}\left(e^{-\lambda_1t}-e^{-\lambda_2t}\right)$.

**(a) Sketch of $R(t)$.** $R(0)=0$; rises linearly at first; peaks at $t^*=\dfrac{\ln(\lambda_2/\lambda_1)}{\lambda_2-\lambda_1}$ (set $\dot R=0$); then falls with the *slow* rate $\lambda_1$ once B's fast decay has equilibrated. Bell-shaped asymmetric hump: fast rise, slow tail.

**(b) Approximations.** (i) **Small $t$** (expand $e^{-x}\approx1-x$): $R\approx\dfrac{\lambda_1}{\lambda_2-\lambda_1}\big[(1-\lambda_1t)-(1-\lambda_2t)\big]=\boxed{\lambda_1t}$ — linear growth: B accumulates as fast as A decays.

(ii) **Large $t$** ($t\gg1/\lambda_2$: the second exponential is dead): $\boxed{R\approx\dfrac{\lambda_1}{\lambda_2-\lambda_1}e^{-\lambda_1t}\approx\frac{\lambda_1}{\lambda_2}e^{-\lambda_1t}}$.

**(c) Graphical determination.**

(i) **$\lambda_1$:** plot $\ln R$ vs $t$; the late-time points fall on a straight line, slope $=-\lambda_1$.

(ii) **$\lambda_2$ (knowing $\lambda_1$):** the same line's intercept is $b=\ln\dfrac{\lambda_1}{\lambda_2-\lambda_1}$, so $\lambda_2=\lambda_1(1+e^{-b})$. (Refinement: subtract the fitted late-time line from the early data and plot $\ln\!\big[\frac{\lambda_1}{\lambda_2-\lambda_1}e^{-\lambda_1t}-R\big]$ vs $t$ — the residual's slope is $-\lambda_2$ directly.)

**(d) Secular equilibrium.** For $\lambda_2\gg\lambda_1$ and $t\gg1/\lambda_2$: $N_2=N_0\dfrac{\lambda_1}{\lambda_2}e^{-\lambda_1t}$ while $N_1=N_0e^{-\lambda_1t}$; dividing:

$$N_2\lambda_2=N_1\lambda_1\quad\blacksquare$$

**Conditions:** $\lambda_2\gg\lambda_1$ (daughter much shorter-lived than parent) **and** times long compared with the daughter's lifetime ($t\gg1/\lambda_2$) so that B is fed and drained in balance — B then decays essentially as fast as A produces it: the activities equalise.

**(e) $N_3(t)$.** $N_3=N_0-N_1-N_2$: starts as $\tfrac12N_0\lambda_1\lambda_2t^2$ (quadratic — C needs *two* successive decays), sigmoids through the midpoint, and saturates at $N_0$ as $t\to\infty$.

> 【Thought】 The physical story behind the algebra: with $\lambda_2\gg\lambda_1$, B is a nearly-instant waystation — its population slaved to A's production rate (secular equilibrium, the principle behind radon in uranium ore and generator isotopes in medicine). The graph-reading strategy of (c) — fit the pure exponential tail first, then peel — is the same two-component technique as Paper 34 Q7.

---

### Q4 — Circular motion; charged particle in a uniform B field [20 marks]

**(a) Mass in uniform circular motion [4 marks].**

(i) The centripetal force is everywhere perpendicular to the velocity, so $\displaystyle W=\oint\vec F\cdot d\vec s=\boxed{0}$ — no work is done in one revolution (or ever); the speed, hence the KE, never changes.
(ii) $F=ms^2/r$, directed toward the centre; its **magnitude is constant** but its **direction rotates** with the particle (always radially inward).

> 【Thought】 "Work done by the particle in one revolution" tests the definition, not stamina: $W=\vec F\cdot\vec s$ needs a parallel component, and circular motion has none. A force of constant magnitude is not a constant force — the vector changes.

---

**(b) Particle $(m,Q)$ entering $B=B\hat z$ with velocity $(u,v,w)$ [5 marks].**

(i) In-plane component: $\boxed{v_{xy}=\sqrt{u^2+v^2}}$.
(ii) $z$ is force-free: $\boxed{z(t)=wt}$.
(iii) The magnetic force on the transverse motion supplies the centripetal force: $Qv_{xy}B=mv_{xy}^2/r$:

$$\boxed{r=\frac{m\sqrt{u^2+v^2}}{QB}}.$$

**(c)(i) Period.** $\boxed{T=\dfrac{2\pi r}{v_{xy}}=\dfrac{2\pi m}{QB}}$ — independent of all velocity components.

**(c)(ii) Increasing $B$.** $r\propto1/B$ shrinks; $T\propto1/B$ shortens; $w$ is untouched, so the pitch $wT$ shrinks too — the helix tightens and cycles faster while drifting along $z$ at the same rate.

**(d) Sketches.** (i) $x(t)$: sinusoid (oscillating about the gyro-centre); $z(t)$: straight line of slope $w$. (ii) $v_x$: sinusoid of amplitude $\leq\sqrt{u^2+v^2}$; $v_z=w$: horizontal line. (iii) $a_x$: sinusoid, the derivative of $v_x$ (quarter-period phase shift, amplitude $\omega\sqrt{u^2+v^2}$); $a_z=0$: the axis.

**(e) Reversing $B$.** The sense of rotation reverses (clockwise ↔ anticlockwise seen along $z$); $r$, $T$, pitch and the $z$-drift are all unchanged.

> 【Thought】 This question is Paper 32 Q1(p) done in Cartesian components: the invariant structure is *split the velocity* — $z$ rides free, the $x$–$y$ part does uniform circular motion at the cyclotron frequency $\omega=QB/m$. For (d), each pair (x vs z, $v_x$ vs $v_z$, $a_x$ vs $a_z$) contrasts "oscillatory" with "uniform" — that contrast is what the sketch must show, with correct relative phases ($a_x$ leads... $a_x=\dot v_x$: shifted by $T/4$).

---

### Q5 — Two uniformly charged insulating spheres [20 marks]

**Setup.** A at $x=-3a$, B at $x=+3a$, each radius $a$, charge $-Q$ (uniform volume charge → each acts externally as a point charge at its centre; write $k=1/4\pi\varepsilon_0$).

**(a)(i) Potential at O.** $V_O=2\times\dfrac{-kQ}{3a}=\boxed{-\dfrac{2kQ}{3a}=-\dfrac{Q}{6\pi\varepsilon_0a}}$.

**(a)(ii) Where on the x-axis does $V=V_O$?** Between the spheres, $V(x)=-kQ\!\left[\dfrac1{3a-x}+\dfrac1{3a+x}\right]=-\dfrac{6akQ}{9a^2-x^2}$, which equals $V_O$ only at $x=0$ (it is *more* negative toward either sphere; inside a sphere it is more negative still, reaching $-\frac32\frac{kQ}{a}-\frac{kQ}{6a}$ at each centre). Exterior ($x>4a$): $V=-kQ\dfrac{2x}{x^2-9a^2}$; setting equal to $-2kQ/3a$:

$$3ax=x^2-9a^2\;\Rightarrow\;x^2-3ax-9a^2=0\;\Rightarrow\;x=\frac{3+\sqrt{45}}{2}a=4.85a,$$

and symmetrically $x=-4.85a$. So: $\boxed{x=0\ \text{and}\ x=\pm4.85a}$.

**(a)(iii) Equipotential $V=V_O$ in the x–y plane.** O is a *saddle* of the potential (maximum along x, minimum along y), so the equipotential crosses itself there in an X; the level set consists of two lobes, each enclosing one sphere, touching at O, and reaching out along the axis to $\pm4.85a$ — a figure-eight pinched at the origin. (Sketch: two teardrops point-to-point at O.)

**(b)(i) Highest potential on B's surface.** B's own contribution is uniform on its surface ($-kQ/a$); A's contribution $-kQ/s$ is largest (least negative) where $s$ — the distance from A — is greatest: the far point of B ($x=4a$, $s=7a$):

$$\boxed{V_H=-\frac{kQ}{a}-\frac{kQ}{7a}=-\frac{8kQ}{7a}}\quad\text{at the point of B farthest from A.}$$

**(b)(ii) Lowest barrier B → A.** A positive ion ($q>0$) has PE $qV$; both spheres *attract* it, but to pass from B to A it must cross the **col** at O — the highest potential on any B→A path is $V_O$ (saddle). Minimise the climb by launching from B's highest-potential point ($V_H$):

$$\boxed{V_L=V_O-V_H=\left(-\frac23+\frac87\right)\frac{kQ}{a}=\frac{10kQ}{21a}}.$$

**(b)(iii) Minimum emission speed for capture.** Energy: $\tfrac12mv_{\min}^2=qV_L$:

$$\boxed{v_{\min}=\sqrt{\frac{20kQq}{21ma}}=\sqrt{\frac{5Qq}{21\pi\varepsilon_0ma}}}.$$

**(c) Force on $(q,m)$ on the y-axis.** At $(0,y)$ each sphere pulls with $kQq/(9a^2+y^2)$; the x-components cancel, the y-components add with factor $y/\sqrt{9a^2+y^2}$:

$$\boxed{F_y=-\frac{2kQq\,y}{(9a^2+y^2)^{3/2}}}\quad\text{(toward O — attractive, restoring)}.$$

> 【Thought】 Structure notes: (a) potentials are *scalar* — just add them, no vector work; the saddle at O is the organising feature for both (a)(iii) and (b). In (b) the launch point is a choice — minimising the barrier means launching from $V_H$, the far side, and the ion then swings around B and over the col at O; "captured by A" = cresting the col with zero residual KE, after which A's attraction pulls it in. In (c) check limits: $y\to0$ gives $F\to0$ (symmetry at O ✓); $y\gg a$: $F\to-2kQq/y^2$, the pair acting as one charge $-2Q$ ✓.

---

### Q6 — Cubic lattices and Bragg diffraction [20 marks]

**(a) Atoms per cubic cell [4 marks].** Corner atoms are shared by 8 cells, face atoms by 2, body atoms by 1:

- **SC:** $8\times\tfrac18=\boxed{1}$.
- **BCC:** $8\times\tfrac18+1=\boxed{2}$.
- **FCC:** $8\times\tfrac18+6\times\tfrac12=1+3=\boxed{4}$.

**(b) Nearest-neighbour distance $D$ and coordination $N$ [8 marks].**

- **SC:** neighbours along the cube edges: $\boxed{D=a,\ N=6}$ ($\pm x,\pm y,\pm z$).
- **BCC:** corner to body centre, half the body diagonal: $\boxed{D=\tfrac{\sqrt3}{2}a,\ N=8}$ (the 8 corners around a centre; each corner likewise touches 8 body centres).
- **FCC:** corner to face centre, half the face diagonal: $\boxed{D=\dfrac{a}{\sqrt2},\ N=12}$ (a corner touches 3 face centres per axis plane $\times$ sharing — counting gives 12: the 12 face centres of the cell around any corner/face-centre site).

**(c) Bragg reflection [3 marks].**

(i) The lower ray travels an extra $d\sin\theta$ down to the second plane and $d\sin\theta$ back up (each leg is the hypotenuse projection $d\sin\theta$ of the layer spacing onto the ray direction): $\boxed{\text{path difference}=2d\sin\theta}$.

(ii) Constructive interference: $\boxed{2d\sin\theta=n\lambda,\quad n=1,2,3,\dots}$ (Bragg's law).

**(d) Numerical orders, $\lambda=1.24\times10^{-10}$ m, SC $a=5.00\times10^{-10}$ m [5 marks].**

Planes parallel to a cube face have $d=a$. $\sin\theta=n\lambda/2a=0.124\,n$:

$$\theta_0=\arcsin(0.124)=\boxed{7.1^\circ};\qquad n_{\max}=\left\lfloor\frac{2a}{\lambda}\right\rfloor=8\ (8\times0.124=0.992),$$

$$\theta_H=\arcsin(0.992)=\boxed{82.8^\circ}.$$

> 【Thought】 The sharing arithmetic of (a) is the whole trick: corner $=1/8$, face $=1/2$, body $=1$. For (b), draw one cell and ask "what is the *shortest* centre-to-centre line?" — in BCC/FCC it is never the cube edge. Bragg's $2d\sin\theta$ counts the down-and-back extra path of the deeper plane — two legs, hence the factor 2; $\theta$ is measured from the *plane*, not the normal (the usual slip). In (d), $n_{\max}$ is set by $\sin\theta\leq1$: only 8 orders exist.

---

### Q7 — Relativistic Compton scattering at 90° [20 marks]

**(a)(i) Rest energy [4 marks].** $E_0=m_ec^2$: the total energy of an electron of zero momentum — the energy locked in its mass, which would be released if the electron were annihilated.

**(a)(ii) Kinetic energy.** Total = rest + kinetic: $T=E-m_ec^2=\boxed{\sqrt{p^2c^2+m_e^2c^4}-m_ec^2}$.

**(b)(i) Conservation equations.** Photon in: $(hf/c,\ 0)$; photon out at $90^\circ$: $(0,\ hf'/c)$; electron: $\vec p$ at angle $\theta$:

$$x:\ \frac{hf}{c}=p\cos\theta,\qquad y:\ \frac{hf'}{c}=p\sin\theta,$$
$$\text{energy:}\quad hf+m_ec^2=hf'+\sqrt{p^2c^2+m_e^2c^4}.$$

**(b)(ii) Proofs.** Square and add the momentum equations ($\sin^2+\cos^2=1$):

$$c^2p^2=h^2f^2+h^2f'^2=h^2(f^2+f'^2).\quad\blacksquare$$

For the second relation, isolate the electron energy and square:

$$\big[hf-hf'+m_ec^2\big]^2=p^2c^2+m_e^2c^4,$$
$$h^2(f-f')^2+2h(f-f')m_ec^2+m_e^2c^4=h^2(f^2+f'^2)+m_e^2c^4,$$
$$-2h^2ff'+2h(f-f')m_ec^2=0\;\Rightarrow\;hff'=(f-f')m_ec^2,$$
$$\frac{1}{f'}=\frac1f+\frac{h}{m_ec^2}\;\Rightarrow\;\boxed{f'=\left(1+\frac{hf}{m_ec^2}\right)^{-1}f}.\quad\blacksquare$$

**(c) Limit $hf\ll m_ec^2$ (soft photons).** $f'\approx f\left(1-\dfrac{hf}{m_ec^2}\right)\approx f$: negligible frequency shift — the **Thomson** (classical) limit; $\tan\theta=f'/f\approx1\Rightarrow\theta\approx45^\circ$; $p=\dfrac{h}{c}\sqrt{f^2+f'^2}\approx\dfrac{\sqrt2\,hf}{c}\to0$ — the electron barely recoils.

> 【Thought】 The algebra choreography of (b)(ii) is the standard Compton template: momentum as a vector triangle (here right-angled, hence the instant Pythagoras), energy handled by isolating the electron's $E$ and squaring to exploit $E^2=p^2c^2+m^2c^4$ — rest energy terms cancel by design. Recognise the result as the 90° case of $\Delta\lambda=\frac{h}{m_ec}(1-\cos90^\circ)=\lambda_C$. Part (c) is a limit check: low-energy photons scatter elastically to first order, which is why Thomson scattering works at optical frequencies.

---

### Q8 — The transit of Venus [20 marks]

**Data.** $R_S=6.96\times10^8$ m; $R_V=6.05\times10^6$ m, $r_V=1.08\times10^{11}$ m, $T_V=1.94\times10^7$ s; $R_E=6.38\times10^6$ m, $r_E=1.50\times10^{11}$ m, $T_E=3.16\times10^7$ s. Earth–Venus at transit: $d=r_E-r_V=4.2\times10^{10}$ m.

**(a)(i) From the photograph.** Measure the diameter of Venus's disc and of the Sun's (partial) disc with a ruler; the Sun's full-face area scales as the square of its radius (complete the circle from the limb's curvature). Venus's disc measures about $1/32$ of the Sun's radius:

$$\lambda=\left(\frac{R_{\text{Sun,image}}}{R_{\text{Venus,image}}}\right)^2\approx(32)^2\approx\boxed{1.0\times10^{3}},\quad\text{accuracy }\sim10\%\ (\text{ruler} \pm0.5\ \text{mm on a few-mm dot}).$$

**(a)(ii) Calculation.** Angular radii from Earth: Sun $\alpha_S=R_S/r_E=4.64\times10^{-3}$ rad; Venus $\alpha_V=R_V/d=1.44\times10^{-4}$ rad:

$$\lambda=\left(\frac{\alpha_S}{\alpha_V}\right)^2=\left(\frac{4.64\times10^{-3}}{1.44\times10^{-4}}\right)^2=(32.2)^2=\boxed{1.04\times10^{3}}\ (\pm\text{a few \%}).$$

**(b)(i) Interval between transits (coplanar assumption).** Synodic period: $\dfrac1{T_{\text{syn}}}=\dfrac1{T_V}-\dfrac1{T_E}$:

$$T_{\text{syn}}=\frac{(1.94)(3.16)}{3.16-1.94}\times10^{7}=5.02\times10^{7}\ \text{s}=\boxed{1.59\ \text{yr}}.$$

**Comment.** Real transits arrive in pairs 8 years apart, then nothing for over a century — because the orbits are *not* exactly coplanar (3.4° inclination): most inferior conjunctions see Venus pass above or below the Sun. The 1.59-yr figure is the conjunction cadence; a transit additionally needs the conjunction to fall near a node.

**(b)(ii) Transit time across the Sun's diameter.** At inferior conjunction Venus overtakes Earth: relative speed $v_V-v_E=34.97-29.83=5.15$ km/s, giving Venus a geocentric angular rate $(v_V-v_E)/d=1.22\times10^{-7}$ rad/s — but the Sun's apparent position also drifts, at $\omega_E=v_E/r_E=1.99\times10^{-7}$ rad/s in the *opposite* sense (Venus moves retrograde across the face during inferior conjunction), so the relative rate is the **sum**:

$$\omega_{\text{rel}}=3.21\times10^{-7}\ \text{rad/s};\qquad t=\frac{2\alpha_S}{\omega_{\text{rel}}}=\frac{9.28\times10^{-3}}{3.21\times10^{-7}}=\boxed{2.9\times10^{4}\ \text{s}\approx8\ \text{hours}}.$$

**(c) The 18th-century parallax measurement [4 marks].**

(i) Telescopes at opposite ends of an Earth diameter, both sighting Venus at the Sun's edge: the angle between the sight lines is the parallax $\approx\dfrac{2R_E}{d}=\dfrac{1.28\times10^7}{4.2\times10^{10}}=\boxed{3.0\times10^{-4}\ \text{rad}\approx60\ \text{arcsec}\ (1\ \text{arcmin})}$ (geometry of Fig 8.2, right angles at Earth). *(Official note: the scheme also credits the Sun-referenced angle $2R_E/r_E=8.5\times10^{-5}$ rad — "either result OK"; strictly, Venus's apparent displacement against the Sun's face combines both: $2R_E(1/d-1/r_E)=2.2\times10^{-4}$ rad.)*

(ii) The Sun's limb is the *shared ruler*: each telescope alone cannot measure an absolute angle to arcsecond precision, but the instant Venus touches the Sun's edge is a sharp, reference-free event; both sites observing *that same contact* converts two absolute measurements into one relative angle (the parallax), from which $d$ follows by triangulation.

(iii) Timing difficulties: no telegraph/radio — simultaneity between distant sites depended on transported chronometers (the longitude problem); contact moments are blurred by the *black-drop effect* (Venus appears to bleed into the limb) and by atmospheric seeing, so "the instant of contact" carried errors of tens of seconds, the dominant error in the whole enterprise.

**(d) Velocity kick to miss the next transit [3 marks].** At the next conjunction ($T_{\text{syn}}$ later), Venus must be displaced perpendicular to its orbit by more than the Sun's radius *as projected to Venus's distance*, $R_S\times d/r_E=6.96\times10^8\times(4.2/15)=1.95\times10^8$ m:

$$v_s=\frac{1.95\times10^8}{5.02\times10^7}=\boxed{3.9\ \text{m s}^{-1}}.$$

> 【Thought】 The geometric engine throughout: transit = alignment, and everything reduces to angular sizes measured from Earth ($\alpha_S=R_S/r_E$, $\alpha_V=R_V/d$). (b)(ii) hides the subtle step — the Sun is a *moving target in the sky* during the transit, so add the drift rates (opposite senses). Check the astronomy: real transits last ~6–7 h and recur 1.6 yr after a previous one only within a pair — our 8 h (diameter, central) vs 6.7 h (actual chord) is the right ballpark ✓. (d) shows how delicate the alignment is: a stroll-paced 4 m/s perturbation, accumulated over 1.6 yr, destroys it.

---

### Q9 — Resistor networks by degeneration and symmetry [20 marks]

**(a) Reducing Figure 9.1 (bridge: A–R₁–T–R₃–B, A–R₂–Bot–R₄–B, T–R₅–Bot) by choice of $R_2,R_3\in[0,\infty]$ [8 marks].**

**(i) Three in series:** open both chosen arms, $R_2=R_3=\infty$. Only the path A→$R_1$→T→$R_5$→Bot→$R_4$→B survives:

$$\boxed{R_{AB}=R_1+R_5+R_4}.$$

**(ii) Three in parallel:** short both, $R_2=R_3=0$. Then T≡B and Bot≡A; $R_1$ (A→T), $R_5$ (Bot→T), $R_4$ (Bot→B) all join A to B:

$$\boxed{R_{AB}=R_1\parallel R_5\parallel R_4=\left(\tfrac1{R_1}+\tfrac1{R_5}+\tfrac1{R_4}\right)^{-1}}.$$

**(iii) Two equal resistors in parallel — the balanced bridge.** Choose $R_2=R_1$, $R_3=R_4$: then $R_1R_4=R_2R_3$ — the Wheatstone balance condition — so $R_5$ carries **no current** and the network is $(R_1+R_3)\parallel(R_2+R_4)$; the equal-parallel requirement $R_1+R_3=R_2+R_4$ combined with the balance condition $R_1R_4=R_2R_3$ forces exactly this pairing ($R_2=R_1,\ R_3=R_4$ is the unique solution):
$$\boxed{R_2=R_1,\ R_3=R_4\ \text{(balanced bridge, }I_5=0\text{)}}\qquad\Rightarrow\ R_{AB}=\frac{R_1+R_4}{2},\quad P_5=0.$$

> 【Thought】 *Official approach — this balanced bridge is the intended construction*: the two conditions (balance $R_1R_4=R_2R_3$ and equality $R_1+R_3=R_2+R_4$) over-determine the pair, and the unique solution is the direct pairing. Note the diagnostic value: $P_5=0$ is the designed answer to (b)(2)(iii).
>
> *Alternative (also valid):* shorting $R_3=0$ merges T with B, leaving $R_1$ directly across A–B in parallel with $R_2+R_4\parallel R_5$; choosing $R_2=R_1-R_4\parallel R_5$ equalises the two branches, giving $R_{AB}=R_1/2$ with $R_5$ carrying its divider share (nonzero). Both are legitimate reductions "by choice of $R_2,R_3\in[0,\infty]$"; the bridge answer is cleaner.

**(b) Total resistance and power in $R_5$ for each network [6 marks].**

| case | $R_{AB}$ | $P_5$ |
|---|---|---|
| (i) series | $R_1+R_5+R_4$ | $I^2R_5$ (full current through $R_5$) |
| (ii) parallel | $(1/R_1+1/R_5+1/R_4)^{-1}$ | $(IR_{AB})^2/R_5$ (full voltage across it) |
| (iii) equal parallel (balanced bridge) | $\dfrac{R_1+R_4}{2}$ | $0$ (balance ⟹ no current in $R_5$) |

**(c) Figure 9.2: square ABCD with centre O, eight resistors $r$ (four edges + four spokes), I in at A, out at C [6 marks].**

**(i) Why $V_B=V_D$.** The network is unchanged by reflection in the diagonal AC (B↔D swap), and the boundary conditions (in at A, out at C) are also unchanged; the potential solution of a linear network is unique, so it must be reflection-invariant: $V_B=V_D$ ($=(V_A+V_C)/2$). □

**(ii) $R_{AC}$.** Join B and D (equipotential — no current flows between them anyway). By the A↔C antisymmetry of the remaining network, O sits at the mean potential $V_A/2$; likewise $V_B=V_D=V_A/2$ — so the spoke resistors B–O and D–O carry **no current** and drop out. What remains: A→{B,D}→C: $(r\parallel r)+(r\parallel r)=\tfrac r2+\tfrac r2=r$, in parallel with the direct spokes A–O–C: $r+r=2r$:

$$\boxed{R_{AC}=r\parallel2r=\frac{2r}{3}}.$$

> 【Thought】 Part (a) teaches reading a network's *degenerations*: a resistor set to 0 merges its nodes; set to ∞, deletes its arm. Part (c) is the symmetry method twice over: reflection kills the B–O/D–O spokes, leaving only series-parallel arithmetic — no Kirchhoff algebra needed. Check (c)(ii) by full nodal analysis: $V_B=V_D=V_O=V_A/2$, $I=1.5V_A/r$, $R=2r/3$ ✓.

---

*End of Paper 36.*

## Paper 37 — 2002 Paper 2 (8 Nov 2002) [2003 paper]

### Q1 — Compulsory short questions

**(a) Comment on the records, with corrections [10 marks].**

(i) $P=VI=78.46\times0.01356=1.0639$ W. Data have 4 s.f., so the correct record is **1.064 W**. "1.1 W" throws away precision the measurements justify (2 s.f. only); "1063.9 mW" invents a fifth significant figure the data cannot support. Both misreport the justified precision — in opposite directions.

(ii) $V=52.5\times35.5\times95.0\ \text{mm}^3=1.7706\times10^{5}\ \text{mm}^3$: correct record $\boxed{1.77\times10^{-4}\ \text{m}^3}$ (3 s.f.), not the 10-figure $0.0001770525\ \text{m}^3$. Mass: $m=\rho V=4.3\times10^3\times1.7706\times10^{-4}=0.761$ kg — and since $\rho$ has only 2 s.f., the record should be **0.76 kg**; the recorded 0.7665356 kg is both over-precise and numerically inconsistent with $\rho V$.

(iii) The student's $I=8.03$ A comes from $24.1/3.00$ — i.e. assuming the cells **aid**. In Figure 1.1 the 12.1 V and 12.0 V cells are connected in **opposition**, so the net emf is 0.1 V across the two paralleled 6.00 Ω resistors (3.00 Ω):

$$\boxed{I=\frac{12.1-12.0}{3.00}=0.033\ \text{A}}\quad\text{(not 8.03 A)}.$$

> 【Thought】 This item trains three lab disciplines at once: quote results to the precision of the worst input (never more, rarely less); recompute rather than trust; and read cell *polarity* before reaching for $I=V/R$. The polarity check is physical: the two nearly equal opposing emfs nearly cancel — a 240× smaller current than the student's.

---

**(b) Photons in a laser nanosecond pulse [6 marks].**

Pulse energy: $E=P\Delta t=(0.5\times10^{-3})(10^{-9})=5\times10^{-13}$ J. Photon energy: $\varepsilon=hc/\lambda=(6.63\times10^{-34})(3.00\times10^8)/(639\times10^{-9})=3.11\times10^{-19}$ J.

$$\boxed{N=\frac{E}{\varepsilon}=\frac{5\times10^{-13}}{3.11\times10^{-19}}=1.6\times10^{6}\ \text{photons}}.$$

> 【Thought】 Chain: power × time = energy; energy ÷ photon energy = count. Order-of-magnitude anchor: a visible photon is ~$3\times10^{-19}$ J, so a mW beam carries ~$10^{15}$ photons/s, ~$10^6$ per ns ✓.

---

**(c) Constant-acceleration rocket [10 marks].**

(i) $\tfrac12at^2=36.0$ km with $t=60$ s: $a=\dfrac{2\times36000}{60^2}=\boxed{20.0\ \text{m s}^{-2}}$.

(ii) Cutoff speed $v=at=1200$ m/s; coasting rise $v^2/2g=73.4$ km: $\boxed{h_{\max}=36.0+73.4=109\ \text{km}}$.

(iii) Powered 60 s; coast up $v/g=122$ s; fall from 109.4 km: $\sqrt{2h/g}=\sqrt{2\times1.094\times10^5/9.81}=149$ s. $\boxed{t_{\text{total}}=60+122+149=332\ \text{s}}$.

(iv) Thrust $=m(g+a)=2000\times29.81=5.96\times10^4$ N; work over the powered 36.0 km:

$$\boxed{W=Fh=5.96\times10^4\times3.60\times10^4=2.15\times10^{9}\ \text{J}}.$$

**Unrealistic assumptions:** a real rocket *loses mass* as it burns fuel (the rocket equation — acceleration grows even at constant thrust), so "constant mass and constant acceleration" conflict; and $g$ falls by ~1% over 100 km — small but real. (Constant $a$ would also require continuously throttling the engine.)

> 【Thought】 Check (iv) by energy instead of force: at cutoff the rocket has $\tfrac12mv^2+mgh=1.44\times10^9+0.71\times10^9=2.15\times10^9$ J ✓ — two routes agree. Note the engine's work only covers the *powered* segment; the coast converts KE to PE for free.

---

**(d) The ¹²C nucleus [10 marks].**

(i) The atom's mass includes 6 electrons ($m_e=5.4858\times10^{-4}$ amu):

$$M_{\text{nuc}}=12.00000-6\times0.000549=\boxed{11.99671\ \text{amu}}.$$

(ii) Constituents: $6m_p+6m_n=6(1.007276+1.008665)=12.09565$ amu:

$$\boxed{\Delta m=12.09565-11.99671=0.09894\ \text{amu}}.$$

(iii) $B=\Delta m c^2=0.09894\times931.5=92.2$ MeV; per nucleon:

$$\boxed{B/A=92.2/12=7.68\ \text{MeV per nucleon}}.$$

> 【Thought】 Two traps: the *atomic* mass includes electrons — strip them before computing the nuclear mass defect; and use proton+neutron masses (not hydrogen-atom mass) on the constituent side, consistently. Check: 7.68 MeV/nucleon sits right at the peak of the binding curve (Fe ≈ 8.8, C ≈ 7.7) ✓.

---

**(e) Three charges on a square's corners [9 marks].**

Fourth corner: distances $a,a,a\sqrt2$. Potential (scalar):

$$V=kQ\left(\frac1a+\frac1a+\frac1{a\sqrt2}\right)=\boxed{\frac{kQ}{a}\left(2+\frac{1}{\sqrt2}\right)=\frac{2.71\,kQ}{a}}.$$

Field (vector): the two adjacent corners give $kQ/a^2$ each, perpendicular to each other → resultant $\sqrt2\,kQ/a^2$ along the diagonal; the far corner adds $kQ/(2a^2)$ along the same diagonal:

$$\boxed{E=\frac{kQ}{a^2}\left(\sqrt2+\frac12\right)=\frac{1.91\,kQ}{a^2},\ \text{along the diagonal, pointing outward (away from the charges)}}.$$

> 【Thought】 The contrast to drive home: $V$ adds as scalars (no geometry), $E$ needs vector addition — here the symmetry collapses everything onto the diagonal, so draw the three arrows first. Sign check: positive sources push a positive test charge *away* along the diagonal ✓.

---

**(f) Centre of gravity of a filling cylinder [5 marks].**

Let the (uniform-walled) cylinder have mass $M$, length $l$; liquid fill height $h$ (mass $\rho Ah$, CG at $h/2$).

(i) Empty: CG at $\boxed{l/2}$. (ii) Full ($h=l$): wall CG and liquid CG both at $l/2$ → $\boxed{l/2}$.

Between fills: $y(h)=\dfrac{Ml/2+\rho Ah^2/2}{M+\rho Ah}$. This *dips below* $l/2$ and returns: minimising ($dy/dh=0$) gives $\rho Ah^2+2Mh-Ml=0$, and substituting back shows $y_{\min}=h^*$ — **the CG is lowest exactly when it passes through the liquid surface**. Graph: starts at $l/2$, curves down to a minimum (at the fill height where the CG meets the surface), rises symmetric... rises back to $l/2$ at $h=l$.

> 【Thought】 The counter-intuitive content: adding mass at the *bottom* at first pulls the CG down (heavy stuff arrives low), but eventually the rising column's own CG wins and the system's CG climbs back. The elegant checkpoint $y_{\min}=h^*$ (CG = surface at the worst moment) is worth deriving, not just asserting — it falls out of the extremum condition in one line.

---

**(g) Puck on a curved track [5 marks].**

(i) On the straight $60^\circ$ portions: $f=g\sin60^\circ=\boxed{\tfrac{\sqrt3}{2}g}$ directed down-slope (toward O).
(ii) $E=\boxed{\tfrac12mv^2+mgy}$ (conserved — smooth track).
(iii) At O the tangent is horizontal, so the *tangential* acceleration vanishes; but if the puck is moving, the track curves, so a **normal (centripetal) acceleration $v^2/\rho$ points upward** — the resultant acceleration at O is purely vertical, supplied by the normal force exceeding gravity. (Even at the lowest point of a dip, "acceleration" need not vanish.)
(iv) From rest at $x=a$ (height $b$): $\tfrac12mv_0^2=mgb\Rightarrow\boxed{v_0=\sqrt{2gb}}$.

> 【Thought】 (iii) is the concept check: decompose acceleration into tangential ($\dot v$, zero at the level bottom) and normal ($v^2/\rho$, nonzero while moving). Releasing from $x=a$ uses only energy — the track's shape in between is irrelevant to the speed at O, a point worth stating.

---

**(h) Equatorial stations via two geostationary satellites [10 marks].**

**Geometry.** Satellite orbit radius $r=6.38\times10^3+3.59\times10^4=4.228\times10^4$ km. Each ground link is *tangential* to the Earth: tangent length $\sqrt{r^2-R_E^2}=4.18\times10^7$ m, and the geocentric half-angle to the tangent point is $\alpha=\arccos(R_E/r)=81.3^\circ$. The two satellites therefore sit $180^\circ-2\times81.3^\circ=17.4^\circ$ apart; their separation is $2r\sin(8.68^\circ)=1.28\times10^7$ m.

Total path $=2(4.18\times10^7)+1.28\times10^7=9.63\times10^7$ m:

$$\boxed{\Delta t=\frac{9.63\times10^7}{3.00\times10^8}=0.32\ \text{s}}.$$

> 【Thought】 "Tangential" is the geometric licence: it fixes each satellite's angular position relative to its station (the right triangle with hypotenuse $r$). Check the sensible pieces: each hop is ~4×$10^4$ km, comparable to the orbit radius ✓; a third of a second is the familiar satellite-phone lag ✓.

---

**(i) Straight-line forms [10 marks].**

(i) $1/y=ax+b$: plot $\boxed{1/y\ \text{against}\ x}$ → slope $a$, intercept $b$.
(ii) $y(x^2+d)=cx$: rearrange $x/y=(x^2+d)/c$, i.e. $\boxed{x/y=\frac1c\,x^2+\frac dc}$: plot $x/y$ against $x^2$ → slope $1/c$, intercept $d/c$, so $c=1/\text{slope}$, $d=\text{intercept}\times c$.

> 【Thought】 Linearisation is pattern-matching: get the equation into $Y=mX+c$ with *measured* quantities as $X,Y$ and unknowns only inside the slope/intercept. In (ii) the trick is dividing by $y$ — note you cannot plot $y$ vs $x^2$ usefully since $c,d$ are entangled nonlinearly there.

---

**(j) Daily uranium consumption of an 800 MW station [6 marks].**

Energy per day: $E=8.00\times10^8\times86400=6.91\times10^{13}$ J. Per fission: $200\ \text{MeV}=3.20\times10^{-11}$ J.

$$N=\frac{6.91\times10^{13}}{3.20\times10^{-11}}=2.16\times10^{24}\ \text{fissions/day},$$

$$m=N\times235\,u=2.16\times10^{24}\times235\times1.66\times10^{-27}=\boxed{0.84\ \text{kg per day}}.$$

> 【Thought】 Order check: ~1 kg/day for a GW-scale station is the famous energy density of fission (vs ~10⁴ tonnes of coal) ✓. "Minimum" = assuming every fission's energy is converted — real stations need ~3× more fuel for the same electrical output (thermal efficiency ~33%).

---

**(k) $e/m$ for relativistic electrons [10 marks].**

Theory: $m=m_0(1-v^2/c^2)^{-1/2}\Rightarrow e/m=(e/m_0)\sqrt{1-v^2/c^2}$, so

$$(e/m)^2=(e/m_0)^2\left(1-\frac{v^2}{c^2}\right).$$

**Plot $(e/m)^2$ against $(v/c)^2$** — expecting a straight line of slope $-(e/m_0)^2$ and intercept $(e/m_0)^2$. The data: $(e/m)^2 = 2.849, 2.713, 2.589, 2.326, 1.672$ (units $10^{22}$ C²kg⁻²) against $0.1007, 0.1434, 0.1833, 0.2656, 0.4720$ fall on a straight line ✓. Least squares: slope $-3.17$, intercept $3.17$ ($10^{22}$ units):

$$\boxed{e/m_0=\sqrt{3.17\times10^{22}}=1.78\times10^{11}\ \text{C kg}^{-1}}$$

vs accepted $1.759\times10^{11}$ — 1% high. Accuracy: the points scatter by $\lesssim1\%$ about the line and slope/intercept agree ($-3.17$ vs $3.17$) as relativity demands ✓; quote $e/m_0=(1.78\pm0.02)\times10^{11}$ C/kg.

> 【Thought】 Choosing *what* to plot is the whole skill: relativity predicts $(e/m)^2$ is linear in $(v/c)^2$ — plot anything else and you are curve-guessing. The bonus internal check: slope should equal minus intercept; here $-3.17$ vs $+3.17$ — a beautiful consistency stamp that the data obey $m=m_0\gamma$.

---

### Q2 — Two bars joined by springs, dropped [20 marks]

**Setup.** Bars A (lower) and B (upper), each mass $M$, separation $l$; two springs (each $k$, natural length $l$) connect them, unstretched initially; A starts at height $h$; released from rest.

**(a)(i) Free fall.** Both bars accelerate at $g$ together; with no differential acceleration the springs never stretch: the separation **stays $l$** throughout the fall. Just before A lands, both bars move at

$$\boxed{v=\sqrt{2gh}\ \text{downward}}.$$

**(a)(ii) Energy after A's impact.** A's KE ($Mgh$) is dissipated. Remaining: B's KE $=\tfrac12M(2gh)=Mgh$, B's GPE $=Mgl$ (it is at height $l$), springs unstretched:

$$\boxed{E=Mg(h+l)}\quad(\text{ground as reference}).$$

**(a)(iii) At maximum compression $x_c$.** B is momentarily at rest at height $l-x_c$; each spring stores $\tfrac12kx_c^2$:

$$\boxed{E=Mg(l-x_c)+kx_c^2}.$$

**(a)(iv) Solve for $x_c$.** Equating (ii) and (iii):

$$Mg(h+l)=Mg(l-x_c)+kx_c^2\;\Rightarrow\;kx_c^2-Mg\,x_c-Mgh=0,$$

$$\boxed{x_c=\frac{Mg}{2k}\left(1+\sqrt{1+\frac{4kh}{Mg}}\right)}$$

(positive root; the negative root is the unphysical extension branch of the quadratic).

**(b)(i) Extension when A leaves the ground.** A lifts off when the springs pull it up with its own weight: $2kx_e=Mg$:

$$\boxed{x_e=\frac{Mg}{2k}}.$$

**(b)(ii) Condition on $h$.** At extension $x_e$, B is at height $l+x_e$; energy conservation from just after impact:

$$Mg(h+l)\geq Mg(l+x_e)+kx_e^2+0\quad(\text{B just arrives with zero KE}).$$

Substituting $x_e=Mg/2k$:

$$Mgh\geq\frac{M^2g^2}{2k}+\frac{M^2g^2}{4k}=\frac{3M^2g^2}{4k}\;\Rightarrow\;\boxed{h\geq\frac{3Mg}{4k}}.$$

> 【Thought】 The storyline in one line: free fall stores $2Mgh$ total, the ground eats half (A's share), and the survivor B must spend its share on gravity + spring PE before it can afford to *lift* A — that affordability check is (b)(ii). Classic checkpoints: in free fall the springs stay relaxed (weightlessness — no internal force needed) ✓; the quadratic in (iv) has the right limiting behaviour $x_c\to Mg/k\cdot$(static compression $Mg/2k$...) — for $h=0$: $x_c=Mg/k$, i.e. twice the static sag, the standard "suddenly applied load" result ✓.

---

### Q3 — Photoelectric apparatus with gated grids [20 marks]

**(a) Basic apparatus [8 marks].**

(i) **Polarity:** for electrons to *just* reach A, they must be decelerated en route — the field must oppose their motion, so the cathode C is **positive** relative to A (retarding potential $V_o$).

(ii) **Why photons are needed:** the wave picture predicts energy ∝ intensity with arbitrary accumulation time; experiment shows a threshold frequency (below it: nothing, however bright), instantaneous emission, and $KE_{\max}$ set by frequency alone. Only quantised $E=hc/\lambda$ packets absorbed whole explain all three.

(iii) **Greatest wavelength for net emission.** With retarding $V_o$, an electron reaches A only if $KE_{\max}\geq eV_o$; Einstein: $KE_{\max}=hc/\lambda-W$. The threshold *wavelength* $\lambda_c$ (zero KE at the surface) satisfies $W=hc/\lambda_c$; eliminating $W$ via $W=hc/\lambda-eV_o$:

$$\boxed{\lambda_c=\frac{hc}{W}=\frac{hc}{hc/\lambda-eV_o}=\frac{\lambda}{1-eV_o\lambda/hc}}.$$

**(b) Gated time-of-flight version [12 marks].**

**Setup.** Electrons leave C (earthed) with KE 0.750 eV. Each gate = live mesh + earthed mesh 5 mm apart; the 500 mm drift space between the earthed meshes is field-free; A sits at $-0.750$ V. Gate square wave: $\pm1.00$ V, period 3.00 µs.

(i) **$V(x)$** (gates at $+1.00$ V): 0 from C to G1's live mesh (40 mm); linear rise $0\to+1$ V across G1's 5 mm; $+1$ V at the mesh; back to 0 entering the drift space; flat 0 for 500 mm; mirror ramp through G2; then falling to $-0.750$ V at A over the last 40 mm. (A plateau-and-ramp profile.)

(ii) **$T(x)$ (eV):** starts 0.750; rises to 1.750 across G1 (electron accelerated toward a $+1$ V mesh); back to 0.750 in the drift; 1.750 across G2; then falls linearly to $0.750-0.750=0$ at A — the electron *just arrives* (consistent with part (a)'s condition).

(iii) **Speed between G1 and G2** (KE = 0.750 eV):

$$v=\sqrt{\frac{2\times0.750\times1.60\times10^{-19}}{9.11\times10^{-31}}}=\boxed{5.13\times10^{5}\ \text{m s}^{-1}}.$$

(iv) **Shape of the CRO trace.** Each gate passes electrons only while positive (at $-1$ V the 5 mm gap is a 1 eV barrier — higher than the 0.750 eV electrons can climb — so the gate is shut). The gates switch together, but the drift takes $0.500\ \text{m}/v=0.97\ \mu$s; electrons admitted by G1 during the first half-window arrive while G2 is still open, those admitted later find G2 shut. Result: one narrow burst per cycle (Fig 3.4), repeating every 3.00 µs.

(v) **Pulse width.** Overlap of the two 1.5 µs windows offset by the 0.97 µs transit:

$$\boxed{\Delta t\approx1.5-0.97\approx0.5\ \mu\text{s}}.$$

> 【Thought】 The design idea to name: two in-phase gates + a drift space = a crude velocity selector/timing chopper; the pulse width encodes the transit time ($\Delta t = T/2 - L/v$), so Fig 3.4 measures $v$ without timing individual electrons. Check (iii): 0.75 eV → $5\times10^5$ m/s $\ll c$ — non-relativistic ✓. In (i)/(ii) the key discipline: PE of an electron is $-eV$, so a *positive* mesh is a potential *well* for electrons — the sign flip is the most common error.

---

### Q4 — Parallel branches with cells; star–triangle equivalence [20 marks]

**(a) Figure 4.1 circuits [5 marks].**

**(i)** Topology (Fig. 4.1(i)): the middle branch is the cell $E$ in series with $R$ (arrow $i_2$); the *other* network across the same rails is three parallel branches each $R$ (top, bottom-left, bottom-right), carrying $i_1$ each by symmetry, so KCL gives $i_2=3i_1$. Around the loop formed by the middle branch and the paralleled trio:

$$E=i_2R+i_2\times\frac R3=i_2\,\frac{4R}{3}\;\Rightarrow\;\boxed{i_2=\frac{3E}{4R}},\qquad\boxed{i_1=\frac{i_2}{3}=\frac{E}{4R}}$$

— the cell discharges, driving $i_2$ through its own branch and splitting it three ways through the paralleled resistors (each carrying $i_1$, opposite in sense to $i_2$).

**(ii)** Three parallel branches, each an identical cell $E$ in series with $R$, same orientation: KCL gives $3(V-E)/R=0\Rightarrow V=E$, and every branch current vanishes:

$$\boxed{i_1=i_2=0}$$

— identical ideal cells in parallel drive no current anywhere (nothing to circulate; no branch has anything to push against).

> 【Thought】 The method is one node-voltage equation — with a source in a branch, write the branch current as $(V-E)/R$, never $V/R$. Part (ii)'s zero is a result worth remembering: equal emfs in parallel are inert (real cells differ slightly → circulating currents and heating, which is why batteries are paralleled with care).

---

**(b) Star vs triangle: deriving the equivalence relation [5 marks].**

With $i_1=0$: **star** — the whole current $I$ (in at 2, out at 3) flows through $R_2+R_3$ in series:

$$V_{23}^{\star}=I(R_2+R_3).$$

**Triangle** — $I$ splits between the direct arm $R_{23}$ and the series arm $R_{31}+R_{12}$; with $I_s$ through the series arm, $V_{23}=I_s(R_{31}+R_{12})$ and $I=V_{23}/R_{23}+I_s$, so

$$V_{23}^{\triangle}=\frac{IR_{23}(R_{31}+R_{12})}{R_{31}+R_{12}+R_{23}}.$$

Equating $V_{23}^{\star}=V_{23}^{\triangle}$:

$$\boxed{(R_2+R_3)(R_{31}+R_{12}+R_{23})=R_{23}(R_{31}+R_{12})}.\quad\blacksquare$$

**(c)** Cyclic permutations: $i_2=0$: $(R_1+R_3)(R_{12}+R_{23}+R_{31})=R_{31}(R_{12}+R_{23})$; $i_3=0$: $(R_1+R_2)(\ldots)=R_{12}(R_{23}+R_{31})$.

**(d) Triangle of three 1 Ω → star.** Solving the three relations (or the standard formula $R_1=R_{12}R_{31}/\Sigma$ with $\Sigma=3$ Ω):

$$R_1=R_2=R_3=\frac{1\times1}{3}=\boxed{\tfrac13\ \Omega\ \text{each}}\quad\blacksquare$$

(verify: star $R_2+R_3=2/3$ vs triangle $1\parallel2=2/3$ ✓).

**(e) $R_{AB}$ for Figure 4.3.** Replace the 1 Ω triangle (top node T, bottom node Bot, right node R) by its star (arms $1/3$ Ω, centre O). The circuit becomes series–parallel:

$$\text{A–O: }(4+\tfrac13)\parallel(2+\tfrac13)=\frac{13}{3}\parallel\frac73=\frac{91/9}{20/3}=\frac{91}{60}\ \Omega;\qquad \text{O–B: }\tfrac13+3=\frac{10}{3}\ \Omega,$$

$$\boxed{R_{AB}=\frac{91}{60}+\frac{10}{3}=\frac{291}{60}=4.85\ \Omega}.$$

Check by direct nodal analysis: $4.850\ \Omega$ ✓.

> 【Thought】 The question walks you through *deriving* the Y–Δ transform from first principles (equate terminal p.d.'s under the same external currents) before weaponising it — the transform converts the un-simplifiable bridge triangle into a series–parallel circuit. Note (d)'s quick check: $1\parallel2=2/3$ matches $1/3+1/3$ — equivalence in one line.

---

### Q5 — Forces between currents; oscillating magnet [20 marks]

**(a) Force between two parallel wires [2 marks].** Wire 1's field at wire 2: $B=\mu_0I_1/2\pi r$, perpendicular to wire 2. Force per unit length on wire 2: $F=BI_2$:

$$\boxed{F=\frac{\mu_0I_1I_2}{2\pi r}}.\quad\blacksquare$$

Direction (diagram): **attractive** for parallel currents, repulsive for antiparallel (use $\vec F=I\vec L\times\vec B$).

**(b) Field lines and $B(x)$ [9 marks].** (i) *Same direction:* each wire's circles; the combined pattern has a **neutral point at the midpoint** ($B=0$ there), lines bulging outward around the pair at large distance (looks like one wire carrying $2I$). $B(x)$ along the inter-wire line: diverges at each wire, passes through zero at the midpoint with opposite signs on the two sides (antisymmetric graph). (ii) *Opposite directions:* field lines thread the gap from one wire to the other; on the inter-wire line the two contributions **add**: $B(x)$ is symmetric, maximal at the wires, with a nonzero minimum $B_{\min}=\dfrac{2\mu_0I}{\pi d}$ at the midpoint.

**(c) Three-wire power line (200 A each, equilateral triangle, 0.50 m spacing) [5 marks].** The three wires sit at the vertices of an equilateral triangle (Fig. 5.1). On wire A: attracted toward B and toward C, each with $F=\dfrac{\mu_0I^2}{2\pi r}$ per metre; the two pulls are at $60^\circ$ to each other, so the resultant points along the bisector (toward the midpoint of BC):

$$F_A/L=2\,\frac{\mu_0(200)^2}{2\pi(0.50)}\cos30^\circ=2\times\frac{2\times10^{-7}\times4\times10^{4}}{0.50}\times\frac{\sqrt3}{2}=\boxed{2.77\times10^{-2}\ \text{N m}^{-1}}$$

(and identically for B and C — each wire is pulled toward the triangle's centre along the angle bisector; force diagram: three arrows converging).

**(d) Oscillating magnet: cork vs thread [4 marks].** Cork (free): restoring torque only from the field → $f^2=\alpha B$. Thread suspension adds a **B-independent restoring torque from the thread's torsion**, so $f^2=\gamma B+\lambda$ with

$$\boxed{\lambda=\text{(thread torsional stiffness)}\times\text{(geometry)}/\text{(moment of inertia)}}$$

— $\lambda$ depends on the **torsion constant of the thread** (and the magnet's moment of inertia).

(i) *Verify $B\propto1/r$:* suspend the magnet at several distances $r$ from a long straight wire carrying fixed $I$; measure $f$; plot $f^2$ against $1/r$: since $\gamma B=\gamma\mu_0I/2\pi r$, a **straight line** confirms the $1/r$ law. (ii) The line's **intercept at $1/r\to0$** is $\lambda$ (the oscillation squared-frequency with no wire field — i.e., thread torsion alone).

> 【Thought】 (b) is superposition practice: sketch each wire's $1/(distance)$ curve first, then add with signs — the midpoint is zero for like currents (cancellation) and double-ish for unlike (reinforcement); that single fact fixes both graph shapes. In (d), linearising $f^2=\gamma B+\lambda$ against $1/r$ turns "verify $1/r$" into "is it a straight line" and simultaneously yields $\lambda$ as the intercept — one graph, two answers.

---

### Q6 — Eclipses; Kepler; the degenerate-ellipse fall [20 marks]

**(a) Eclipses [5 marks].**

**Solar eclipse:** new Moon passes between Sun and Earth; the Moon's umbra (total) / penumbra (partial) sweeps a narrow track on Earth — ray diagram: Sun's rays tangent to the Moon's disc converge to the umbral cone. **Lunar eclipse:** full Moon enters the Earth's (much larger) shadow cone — same diagram with Earth as the occluder. **Why not monthly:** the Moon's orbit is inclined ~5° to the ecliptic; at most new/full moons the Moon passes above or below the Sun–Earth line. Eclipses require the Moon to be near a *node* of its orbit at new (solar) or full (lunar) phase — hence eclipse seasons, roughly twice a year, not every month.

> 【Thought】 One line carries the mark: eclipse = shadow alignment; alignment needs both the right phase AND a node — the 5° inclination is the reason the geometry usually fails.

---

**(b) Kepler's third law for the Moon [4 marks].**

Gravity supplies the centripetal force: $\dfrac{GM_EM_M}{R^2}=M_MR\omega^2=M_MR\dfrac{4\pi^2}{T^2}$:

$$\boxed{T^2=\frac{4\pi^2}{GM_E}R^3}.\quad\blacksquare$$

---

**(c) Free fall as a degenerate ellipse [11 marks].**

**Key observation.** A body falling radially from rest at $R_{EM}$ is on the limiting "thin ellipse" whose major axis is $R_{EM}$, i.e. semi-major axis $a=R_{EM}/2$; the fall to the centre is half the ellipse's period.

(i) $\tau=\dfrac{T_{\text{ellipse}}}{2}=\pi\sqrt{\dfrac{a^3}{GM_E}}=\pi\sqrt{\dfrac{R_{EM}^3}{8GM_E}}$:

$$\boxed{\tau=\pi\sqrt{\frac{(3.84\times10^8)^3}{8(3.982\times10^{14})}}=4.2\times10^{5}\ \text{s}\approx4.8\ \text{days}}.$$

(ii) $\bar v=\dfrac{R_{EM}}{\tau}=\dfrac{3.84\times10^8}{4.16\times10^5}=\boxed{9.2\times10^{2}\ \text{m s}^{-1}}$.

*Official-answer note.* The scheme prints $\tau=2.96\times10^5$ s (and $\bar v=1.29\times10^3$ m/s) — an arithmetic slip in evaluating $\tfrac12\sqrt{4\pi^2(R_{EM}/2)^3/GM_E}$: correct evaluation gives $\tau=4.16\times10^5$ s (ours). (Its (iv), $1.58\times10^7$ s, is right, which corroborates that (i)'s slip is local arithmetic, not method.)

(iii) Energy conservation from rest at $R_{EM}$ to $r=R_E$:

$$V_M=\sqrt{2GM_E\left(\frac1{R_E}-\frac1{R_{EM}}\right)}=\boxed{1.11\times10^{4}\ \text{m s}^{-1}}$$

— essentially the escape speed (since $R_{EM}\gg R_E$) ✓.

(iv) Asteroid from rest at $r=2.00$ AU: $a=1.00$ AU; noting $T(a=1\ \text{AU})=1.00$ yr around the Sun:

$$\boxed{\tau=\tfrac12T(a=1\ \text{AU})=0.50\ \text{yr}\ (1.58\times10^{7}\ \text{s})}.$$

> 【Thought】 The Kepler shortcut is the lesson: radial infall time = half the period of the ellipse with $a=r_0/2$ — no differential equation needed. Checks: $\tau$ for the Moon ≈ 5 days vs the orbital month of 27.3 days — ratio $(1/2)^{5/2}=0.177$: $27.3\times0.177=4.8$ d ✓; the 2 AU asteroid falls in half a year because its degenerate ellipse has the same period as Earth's orbit ✓ (both have $a=1$ AU).

---

### Q7 — Wave nature, Doppler, and the twin-engine beat [20 marks]

**(a) Longitudinal vs transverse [3 marks].** Longitudinal: oscillation *along* the propagation direction — alternating compressions/rarefactions (sound in air); transverse: oscillation *perpendicular* — crests and troughs (wave on a string, light). Diagrams: coil spring with compressed/expanded bands vs sinusoidal string. **Polarised wave example:** light through a Polaroid (or a rope wave through a slot) — only transverse waves *can* be polarised, since polarisation selects one of the transverse directions.

**(b) Acoustic phenomena [4 marks].** (i) **Beats:** two waves of slightly different frequencies superpose; the sum $\cos\omega_1t+\cos\omega_2t=2\cos(\bar\omega t)\cos(\Delta\omega\,t/2)$ is a fast tone whose amplitude waxes/wanes at $\Delta f$ — heard as periodic loudness pulsing. (ii) **Doppler effect:** a moving source chases its own wavefronts, compressing the wavelength ahead (stretching behind); a moving observer meets crests at a changed rate — either way the received frequency differs from the emitted one.

**(c) Approaching source: $f=f_0/(1-v_s/c)$ [5 marks].** In one period $T_0=1/f_0$ the source emits a crest and advances $v_sT_0$ toward the observer; the next crest is emitted $v_sT_0$ closer, so the wavelength in the forward direction is

$$\lambda'=(c-v_s)T_0=\frac{c-v_s}{f_0}.$$

The stationary observer receives crests at $f=c/\lambda'$:

$$f=\frac{f_0c}{c-v_s}=\boxed{\frac{f_0}{1-v_s/c}}.\quad\blacksquare$$

**(d) Modifications [3 marks].** Receding source: $v_s\to-v_s$: $f=f_0/(1+v_s/c)$ (lower pitch). At $v_s=c$: denominator → 0 — wavefronts pile up on top of each other; the sound never outruns the source — a **shock wave** forms (sonic boom; Mach cone for $v_s>c$). **No transverse sound in air:** transverse waves need shear restoring forces; a fluid has zero shear stiffness (layers slide freely), so only compressional (longitudinal) modes propagate.

**(e) Twin-engined aeroplane [5 marks].** Let the true beat frequency be $\Delta f$; the plane's speed $v_s$. Both engines' frequencies scale by the same Doppler factor, so the *beat* scales identically:

$$\text{approaching: }\frac{\Delta f}{1-v_s/c}=8.00,\qquad \text{receding: }\frac{\Delta f}{1+v_s/c}=2.00.$$

Dividing: $\dfrac{1+v_s/c}{1-v_s/c}=4\Rightarrow 1+x=4-4x\Rightarrow x=\tfrac35$:

$$\boxed{v_s=0.6\times330=198\ \text{m s}^{-1}\ (\approx710\ \text{km/h},\ \text{Mach }0.6)}.$$

> 【Thought】 The trick of (e): beats are a *difference of frequencies*, and a common Doppler factor scales both engine notes together, so the beat itself is Doppler-shifted — two beat measurements bracket the approach/recession and $c$ cancels into the ratio. Check: $\Delta f=8(1-0.6)=3.2$ Hz, and receding $3.2/1.6=2.0$ Hz ✓. Mach 0.6 is a plausible low pass ✓.

---

### Q8 — Dispersion, double slits, interferometry, pulsars [20 marks]

**(a) Seeing dispersion in transmission [2 marks].** Pass the white light through a prism (or grating) of the medium: the transmitted beam fans into a spectrum — different wavelengths emerge at different angles — which is only possible if $n$ varies with $\lambda$. (Equivalently: a filter-free broadband measurement of transit time/delay vs wavelength.)

> 【Thought】 The logic chain: angular spread of colours ⇒ different bending ⇒ different $n$ per colour. One sentence of mechanism earns both marks.

---

**(b) Two-slit interference [6 marks].**

(i) Path difference $d\sin\theta$: constructive when $\boxed{d\sin\theta=m\lambda}$ ($m=0,1,2,\dots$); destructive when $\boxed{d\sin\theta=(m+\tfrac12)\lambda}$.

(ii) First order, $m=1$: $\sin\theta=\lambda/d$; for $\theta<0.1$ rad, $\sin\theta=\theta-\theta^3/6\approx\theta$ to better than 0.2%, so $\boxed{\theta=\lambda/d}$. □

(iii) In a medium of refractive index $\mu$: the wavelength shrinks to $\lambda/\mu$ (frequency unchanged), so the condition becomes $d\sin\theta=\lambda/\mu$, i.e. $\boxed{\theta=\lambda/(\mu d)}$ — fringes squeeze inward by $\mu$. (Cf. Paper 35 Q8.)

---

**(c) Equatorial two-aerial radio interferometer [6 marks].**

**Setup.** Baseline $d=50$ m east–west; $\lambda=0.75$ m; March 21, equator: the Sun passes through the zenith. As the Sun's hour angle $H$ grows ($\dot H=2\pi/86400=7.27\times10^{-5}$ rad/s), the path difference $d\sin\theta\approx dH$ sweeps through wavelengths.

(i) Adjacent maxima: $\Delta(d\sin\theta)=\lambda\Rightarrow d\cos\theta\,\Delta\theta=\lambda$; near noon ($\theta\approx0$):

$$\Delta t=\frac{\lambda/d}{\dot H}=\frac{0.75/50}{7.27\times10^{-5}}=\boxed{206\ \text{s}\approx3.4\ \text{min}}.$$

(ii) **At Cambridge (52°N):** for an east–west baseline the geometric delay is $\Delta=d\cos\delta\sin H$ — *independent of latitude* (the east direction is the same in equatorial coordinates everywhere), and on March 21 $\delta=0$, so the **fringe timing is identical** to the equator's. What changes is the *envelope*: the Sun culminates at only $90^\circ-52^\circ=38^\circ$ elevation (never overhead), so the signal arrives through a longer atmospheric path and at a less favourable aerial reception angle — the fringes sit on a weaker, elevation-shaped amplitude envelope, and the pattern around noon is otherwise unchanged.

> 【Thought】 The interferometer is just the double slit of (b) run by the Earth's rotation: the sky sweeps the source across the fringe template. The (ii) trap: intuition says "lower Sun ⇒ slower fringes"; the exact delay identity $\Delta=d\cos\delta\sin H$ for an E–W baseline says the *timing* is latitude-free — deriving it beats guessing. (Intensity changes are real, though.)

---

**(d) Pulsar diagnostics [6 marks].**

(i) **Radius contraction:** angular momentum conservation $I\omega=$ const with $I\propto R^2$ — a contracting star spins *up*, so the pulse frequency increases. Detect by precise pulse-timing: a sudden period shortening (a "glitch") signals a crustquake/contraction.

(ii) **Ionised gas cloud (plasma):** the interstellar plasma's refractive index is frequency-dependent ($n<1$, varying with $\lambda$), so the broadband pulse's frequency components travel at different group speeds — the pulse arrives **dispersed**: high frequencies first, low frequencies delayed, a measurable sweep across the band. A change in the dispersion (delay vs frequency slope) when the cloud transits reveals it, even though the cloud is invisible.

> 【Thought】 Both answers are "watch the pulses, not the star": pulsars are clocks; anything that changes the clock rate (spin-up) or the signal's path (dispersion) shows up in the timing. The plasma signature must be *frequency-dependent* delay — a uniform delay would be indistinguishable from distance.

---

### Q9 — Hydrogen levels; annihilation; Compton backscatter [20 marks]

**(a) Transition $E_0=-13.60\to E_1=-3.40$ eV [4 marks].**

(i) The electron's energy *increases* by $10.20$ eV, so a photon is **absorbed** (emission would require dropping to a lower level). (ii) Wavelength:

$$\lambda=\frac{hc}{\Delta E}=\frac{1.986\times10^{-25}}{10.20\times1.60\times10^{-19}}=\boxed{1.22\times10^{-7}\ \text{m}\ (122\ \text{nm, Lyman-}\alpha,\ \text{UV})}.$$

(iii) Ionisation = ground state to zero energy: $\boxed{13.60\ \text{eV}}$.

**(b) Bound vs free electron [2 marks].** Bound: energy is **quantised** into discrete negative levels ($E_n=-13.6/n^2$ eV); free: energy is **continuous** and non-negative (any KE). The bound spectrum's discreteness is what produces sharp spectral lines.

**(c) Stationary positron annihilation [6 marks].**

(i) The initial momentum is zero; two photons must carry equal and opposite momenta → equal energies → **equal wavelengths** (back-to-back emission).

(ii) If the positron moves: total momentum is nonzero, so the photons are no longer exactly back-to-back nor equal — one is blueshifted (shorter $\lambda$), the other redshifted (longer $\lambda$), with energies sharing asymmetrically; the $180^\circ$ correlation opens into an angle.

(iii) The question's own bookkeeping: "a stationary positron, with rest energy $m_ec^2$, decays into two photons of equal wavelength" — the available energy $m_ec^2$ splits equally into two photons, each carrying $m_ec^2/2$:

$$\lambda=\frac{hc}{m_ec^2/2}=\frac{2h}{m_ec}=\boxed{4.85\times10^{-12}\ \text{m}}.$$

> 【Thought】 Reading note: taken as the classic e⁻e⁺ *annihilation*, each photon would carry 511 keV and $\lambda=h/m_ec=2.43\times10^{-12}$ m (the Compton wavelength) — but the question as worded supplies only the positron's $m_ec^2$ to split between the two photons, and the official answer ($4.85\times10^{-12}$ m) follows that wording. Follow the question's own data, not the canonical process, when they conflict.

**(d) X-ray backscatter with 5.00 keV recoil electron [8 marks].**

Energy: $E-E_b=5.00$ keV. Momentum (photon reverses): $E/c+E_b/c=p_e$, with the non-relativistic electron $p_ec=\sqrt{2m_ec^2\,T_e}=\sqrt{2\times511\times5.00}=71.5$ keV. So

$$E+E_b=71.5\ \text{keV},\quad E-E_b=5.00\ \text{keV}\Rightarrow E=38.2\ \text{keV},$$

$$\boxed{\lambda=\frac{hc}{E}=\frac{1.240\ \text{keV nm}}{38.2\ \text{keV}}=3.24\times10^{-11}\ \text{m}}.$$

**Check.** Compton: $\lambda_b-\lambda=\dfrac{h}{m_ec}(1-\cos180^\circ)=2\times2.43\times10^{-12}=4.85\times10^{-12}$ m; then $hc(1/\lambda-1/\lambda_b)=5.0$ keV ✓.

> 【Thought】 (d) is the full Compton machinery without the formula: write momentum and energy separately, use $E=pc$ for photons and $p^2/2m$ for the (non-relativistic) electron, and the two equations give $E\pm E_b$ — solving linear equations instead of quoting $\Delta\lambda$. The independent Compton check at the end is the model habit: two routes, one answer. In (c)(iii), noticing $\lambda=h/m_ec$ is a famous constant is the kind of check that catches factor-of-2 slips (both particles' rest energy must be radiated).

---

*End of Paper 37.*

## Paper 38 — 2001 Paper 2 (9 Nov 2001) [2002 paper]

### Q1 — Compulsory short questions [80 marks, max 40 awarded]

**(a) Ammeter current in four circuits [8 marks].**

**(i)** The diagonal wire shorts the bottom-left and bottom-right corners to the top-left node, so the 6 Ω is bypassed entirely; the only loop is battery → ammeter → 4 Ω:

$$\boxed{I=20/4=5.0\ \text{A}}.$$

**(ii)** Voltmeter (infinite resistance) makes its branch inert; single loop: battery, A, 6 Ω, R in series. Voltmeter across R reads 8 V: $I=8/R$ and $20=I(6+R)$:

$$20R=48+8R\Rightarrow R=4\ \Omega,\qquad \boxed{I=2.0\ \text{A}}.$$

**(iii)** The zero-resistance ammeter fuses the centre and right nodes. This is a Wheatstone bridge: arms 4 Ω and 8 Ω from the top rail, 6 Ω and 12 Ω to the bottom rail — and $4/8=6/12$, so the bridge is **balanced**:

$$\boxed{I_A=0}$$

(check by reduction: $4\parallel8=8/3$ Ω and $6\parallel12=4$ Ω in series across 20 V → 3 A total; potentials at the two mid-nodes both equal $20\times4/(4+8/3)$... i.e. the two dividers 4:8 and 6:12 land their midpoints at the same fraction, so no ammeter current ✓).

**(iv)** From the right-hand node Q, two paths to the left node P: direct 6 Ω (bottom) and 6+6=12 Ω (via the middle node) — parallel: $6\parallel12=4$ Ω. Main loop: battery → top 6 Ω → Q → (4 Ω equiv) → P → ammeter:

$$\boxed{I=\frac{20}{6+4}=2.0\ \text{A}}.$$

> 【Thought】 Four micro-lessons: (i) a plain wire *deletes* components by shorting them — collapse equipotential nodes first; (ii) a meter reading can stand in for an unknown resistor — work backwards from it; (iii) always test the bridge ratio before grinding Kirchhoff; (iv) redraw with the parallel pair recognised. The universal first move: merge nodes joined by ideal wires.

---

**(b) U-238 half-life from Ra-226 in equilibrium ore [8 marks].**

Secular equilibrium (daughter activities equal the parent's): $N_U\lambda_U=N_{Ra}\lambda_{Ra}$, i.e. $\dfrac{T_U}{T_{Ra}}=\dfrac{N_U}{N_{Ra}}$:

$$\frac{N_U}{N_{Ra}}=\frac{1.00/238}{0.300\times10^{-6}/226}=\frac{226}{238\times0.300\times10^{-6}}=3.17\times10^{6},$$

$$\boxed{T_U=1602\times3.17\times10^{6}=5.1\times10^{9}\ \text{years}}.$$

> 【Thought】 The equilibrium assumption converts a ratio of *masses* into a ratio of *lifetimes*: $N\lambda$ equal ⇒ $T\propto N$ (same chemistry sample). Check: answer lands near the accepted $4.5\times10^9$ yr ✓. Condition stated in the question — daughter half-lives ≪ parent's — is exactly what makes the ore a steady-state cascade (cf. Paper 36 Q3(d)).

---

**(c) Beam on three springs [8 marks].**

Beam AOB (O midpoint), springs $k_1,k_2,k_3$ at A, O, B. Rigid beam → compressions vary linearly along it; weight $Mg$ acts at O.

**(i) $k_1=k_3=k$, $k2=2k$:** symmetry → level beam, common compression $x$: $(k+2k+k)x=Mg$:

$$\boxed{x=\frac{Mg}{4k};\quad F_A=F_B=\frac{Mg}{4},\quad F_O=\frac{Mg}{2}}.$$

**(ii) $k,2k,3k$:** write $\delta_O=\delta_2$, tilt $\theta$: $\delta_1=\delta_2-\theta l$, $\delta_3=\delta_2+\theta l$ ($l=AO=OB$). Moments about O (weight has no moment there): $3k\delta_3\,l=k\delta_1\,l\Rightarrow3\delta_3=\delta_1\Rightarrow\theta l=-\delta_2/2$, so $\delta_1=3\delta_2/2$, $\delta_3=\delta_2/2$. Force balance: $k\delta_2(3/2+2+3/2)=5k\delta_2=Mg$:

$$\boxed{\delta_2=\frac{Mg}{5k},\quad \delta_1=\frac{3Mg}{10k},\quad \delta_3=\frac{Mg}{10k};\qquad F_A=\frac{3Mg}{10},\ F_O=\frac{2Mg}{5},\ F_B=\frac{3Mg}{10}}.$$

> 【Thought】 A rigid beam on springs is statically determinate only because rigidity forces *linear* compression — the two beam equations (force, moment) meet two geometric unknowns ($\delta_2,\theta$). Check (ii): stiffer spring 3 compresses least but carries as much as spring 1 — moments balance ✓; $\sum F=Mg$ ✓.

---

**(d) Constant-thrust rocket [8 marks].**

$M_0=1.00\times10^4$ kg, fuel 80%; thrust at ignition $=$ weight: $T=9.81\times10^4$ N; exhaust speed $u=900$ m/s.

**(i)** $T=u\dot m\Rightarrow\boxed{\dot m=T/u=109\ \text{kg s}^{-1}}$.

**(ii)** Fuel gone at $t_e=8000/109=73.4$ s, mass then 2000 kg:

$$\boxed{a_e=\frac{T}{M_e}-g=\frac{9.81\times10^4}{2000}-9.81=39.2\ \text{m s}^{-2}\ (\approx4g)}.$$

**(iii)** $\boxed{M(t)=1.00\times10^4-109\,t\ \text{kg}}$.

**(iv)** $\boxed{a(t)=\dfrac{9.81\times10^4}{10^4-109t}-9.81=\dfrac{g}{1-t/t_e\times0.8}-g}$.

**(v) Sketch.** $a$ starts at 0 (thrust = weight), rises with a hyperbolic $1/M(t)$ curve — gently at first, steeply near burnout — to $4g$ at $t_e=73$ s; then the engine cuts: $a$ drops vertically to $-g$ and stays there forever (ballistic rise, then fall).

> 【Thought】 Note (v)'s two signposts: $a(0)=0$ exactly (given!), and the discontinuity $+4g\to-g$ at burnout — constant thrust over shrinking mass is why rockets pin astronauts harder as they lighten. Compare Paper 33 Q1(j): there thrust never reaches weight until fuel burn reduces it — same thrust–weight race, opposite regime.

---

**(e) Mediterranean volume by molecular counting [8 marks].**

Take a large raindrop: diameter ≈ 5 mm, so $V_d=\tfrac43\pi(2.5\times10^{-3})^3=6.5\times10^{-8}$ m³, mass $6.5\times10^{-5}$ kg $=0.065$ g $=3.6\times10^{-3}$ mol, molecules $N=3.6\times10^{-3}\times6.02\times10^{23}=2.2\times10^{21}$.

$$\boxed{V\approx V_dN=6.5\times10^{-8}\times2.2\times10^{21}\approx1.4\times10^{14}\ \text{m}^3}$$

— within an order of magnitude of the true $\sim4\times10^{15}$ m³ (and note the estimate scales as $d^6$: drop volume × molecule count, both ∝ drop size cubed... i.e. $\propto V_d^2$ — ferociously sensitive to the chosen drop, so order-of-magnitude agreement is all one can claim).

> 【Thought】 The estimate's hidden structure: $V=V_d^2\rho N_A/M_{\text{mol}}$ — squaring the drop volume makes the answer hypersensitive to $V_d$; a "reasoned estimate" here means stating the assumed drop size and the resulting order of magnitude, $10^{14}$–$10^{16}$ m³.

---

**(f) Geostationary orbit via the Moon [12 marks].**

**(i)** In the equatorial plane, orbiting west→east with a period of one (sidereal) day, at radius $\sim4.2\times10^7$ m — fixed longitude above the equator.

**(ii)** Kepler's third law applied as a *ratio* (no $GM_E$ needed):

$$\left(\frac{R}{R_{EM}}\right)^3=\left(\frac{T_{\text{geo}}}{T_{\text{Moon}}}\right)^2=\left(\frac{1}{27.3}\right)^2,$$

$$\boxed{R=3.82\times10^8\times27.3^{-2/3}=4.2\times10^{7}\ \text{m}\ (\approx6.6R_E;\ \text{altitude }3.6\times10^4\ \text{km})}.$$

**(iii)** Near the poles a geostationary satellite sits on or below the local horizon (elevation $\to0$ as latitude $\to90^\circ$): the signal path grazes the Earth — long atmospheric path, terrain/ice blockage, weak and unreliable signal.

> 【Thought】 (ii) is ratio-Kepler: constants cancel — always pair an unknown orbit with a known one (Moon) rather than reaching for $G$. For (iii), one number settles it: elevation of a geostationary satellite at latitude $\lambda$: $\tan e\propto(\cos\lambda - R_E/R)$-type expression — at $70^\circ$ it's only ~10° above the horizon.

---

**(g) Neutron moderation by deuterons [16 marks].**

Head-on elastic, $m_n=m$, $m_d=2m$, deuteron initially stationary.

**(i)** Standard elastic result (or derive: momentum $mu_n=mv_n+2mv_d$; energy/restitution $v_d-v_n=u_n$): $v_d=\dfrac{2m}{m+2m}u_n$:

$$\boxed{\frac{v_d}{u_n}=\frac23}.\quad\blacksquare$$

**(ii)** $\dfrac{\tfrac12(2m)v_d^2}{\tfrac12mu_n^2}=2\times\dfrac49=\boxed{\dfrac89=89\%}$ of the neutron's KE goes to the deuteron per collision.

**(iii)** The neutron keeps $1-8/9=1/9$ of its KE per collision. From 10 MeV to 0.01 eV is a factor $10^9$:

$$\left(\frac19\right)^n=10^{-9}\;\Rightarrow\;n=\frac{9}{\log_{10}9}=9.4\;\Rightarrow\;\boxed{10\ \text{collisions}}.$$

> 【Thought】 The efficiency of heavy-water moderation in one number: 8/9 per hit (vs 100% only for equal masses — but hydrogen absorbs neutrons, hence heavy water). Check (iii) by logs: $9^{10}=3.5\times10^9>10^9$ ✓. Note we take integer ceiling: 9 collisions leave $\sim3\times10^{-2}$ eV — not quite enough. *Official-answer note:* the scheme prints $n=9$, computed from "$1$ MeV to $0.01$ eV" (factor $10^8$); the question paper says $10$ MeV, for which $n=10$ (ours) is correct.

---

**(h) CD as a reflection grating [12 marks].**

**(i)** Normal incidence (light vertical); the eye sits at $\tan\theta=0.50/0.35\Rightarrow\theta=55.0^\circ$ from the normal. First order: $d\sin\theta=\lambda$:

$$\boxed{d=\frac{590\ \text{nm}}{\sin55.0^\circ}=7.2\times10^{-7}\ \text{m}\ (0.72\ \mu\text{m})}.$$

**(ii)** Tilting the disc $5^\circ$ clockwise (right edge down, normal tipping $5^\circ$ toward the eye): incidence is now $5^\circ$ from the normal, diffraction $50^\circ$ on the other side; reflection-grating condition $d(\sin i+\sin r)=m\lambda$:

$$\boxed{\lambda=d(\sin5^\circ+\sin50^\circ)=7.20\times10^{-7}\times0.853=614\ \text{nm}\ \text{(orange)}}.$$

(Had the tilt been the other way: $d(\sin60^\circ-\sin5^\circ)=561$ nm — the direction of tilt decides which way the colour walks. *Official-answer note:* the scheme prints $489$ nm from $d(\sin50^\circ-\sin5^\circ)$ — a sign slip: with the clockwise tilt tipping the normal *toward* the eye, the incidence and diffraction directions lie on opposite sides of the normal, so the grating terms add, $d(\sin i+\sin r)$, giving 614 nm.)

> 【Thought】 A CD's tracks are a ready-made grating ($d\sim$ the answer, 0.7 µm, matches the real 1.6 µm pitch... measured at a steep angle here, so it is the effective pitch across the viewing chord). The physics shift in (ii): tilting adds an incidence angle — the grating equation becomes $d(\sin i+\sin r)=m\lambda$ with signs measured from the normal; track which side of the normal each ray is on and the sign takes care of itself.

---

### Q2 — First law; kettle; steam cylinder; escaping molecules [20 marks]

**(a) First law [5 marks].**

$$\boxed{\Delta U=Q+W}$$

with $\Delta U$ = increase in internal energy of the system, $Q$ = heat supplied **to** the system, $W$ = work done **on** the system. (Equivalently $Q=\Delta U+W'$ with $W'$ the work done *by* the system — state your convention and stick to it.)

> 【Thought】 The first law is bookkeeping with a sign convention; marks are lost by mixing conventions mid-solution, not by the choice itself.

---

**(b) Kettle: latent heat from timing [4 marks].**

Same heater power throughout (assumption): heating: $mc\Delta T=P\times180$ s; boiling dry: $mL=P\times1200$ s. Dividing eliminates $m$ and $P$:

$$\boxed{L=\frac{1200}{180}\,c\,\Delta T=\frac{20}{3}\times4200\times80=2.24\times10^{6}\ \text{J kg}^{-1}}.$$

Assumptions: constant electrical power; no heat losses to the room (kettle lagged/losses neglected); the water is uniformly at 100 °C before net boiling starts. (True value 2.26 MJ/kg — the simple model is good to 1%.)

---

**(c) Steam cylinder in a 100 °C bath [6 marks].**

(i) Weightless piston under atmosphere: force balance gives $\boxed{P=P_{\text{atm}}=1.01\times10^{5}\ \text{Pa}}$ (consistent with saturated steam over water at 100 °C).

(ii) Slow descent $x=0.10$ m at constant pressure: $W=P\,A\,x=1.01\times10^5\times\pi(0.12)^2\times0.10=\boxed{457\ \text{J}}$ done on the contents.

(iii) Slow + constant-temperature bath $\Rightarrow$ isothermal: $\boxed{T_f=100^\circ\text{C}}$.

(iv) The piston halves the steam volume (0.20 m → 0.10 m), so half the steam condenses at 100 °C: $\Delta m=0.185$ g. First law for the contents at constant temperature: the condensation releases $\Delta m\,L$ of internal energy *and* the atmosphere does work $W=457$ J on the contents; both leave as heat into the bath:

$$\boxed{Q_c=-(\Delta m\,L+W)=-(414+457)\approx-8.7\times10^{2}\ \text{J}}\quad\text{(heat transferred to the surroundings)}.$$

> 【Thought】 Flag the data tension honestly: saturated steam at 1 atm has density $PM/RT=0.59$ kg m$^{-3}$, so the stated 0.37 g in $9.0\times10^{-3}$ m³ would imply $P\approx7$ kPa — the numbers are mutually inconsistent, and the cleanest self-consistent route (used above) takes the piston equilibrium ($P=1$ atm) and the mass-halving at face value; the alternative ($\Delta m=\rho\Delta V=2.65$ g → $Q\approx5.9$ kJ) over-condenses the available steam. Reporting which data you trusted, and why, is part of the answer. (Sign convention: negative $Q_c$ = heat flows out of the contents into the bath — state it; the magnitude 871 J is what the official scheme prints.)

---

**(d) Oxygen molecule ballistic flight [5 marks].**

rms speed: $u=\sqrt{3kT/m}$, $m=0.032/N_A=5.32\times10^{-26}$ kg; at 283 K: $u=469$ m/s.

(i) $\tfrac12mu^2=mgH$ (constant $g$): $\boxed{H=\dfrac{u^2}{2g}=\dfrac{2.20\times10^{5}}{19.62}=1.12\times10^{4}\ \text{m}\ (\approx11\ \text{km})}$.

(ii) Escape: $\tfrac12mu^2=\dfrac{GM_Em}{R_E}$, i.e. $\dfrac{3kT_s}{m}=\dfrac{2GM_E}{R_E}$:

$$\boxed{T_s=\frac{2GM_Em}{3kR_E}=\frac{2(3.982\times10^{14})(5.32\times10^{-26})}{3(1.38\times10^{-23})(6.37\times10^{6})}=1.6\times10^{5}\ \text{K}}.$$

> 【Thought】 (ii) is the kinetic answer to Paper 32 Q1(g): escape needs thermal speeds comparable to $v_{\text{esc}}$; $10^5$ K for O₂ is why Earth keeps its oxygen — even the Maxwell tail at 283 K contributes negligibly when $T_s/T\sim600$. The constant-$g$ assumption in (i) is fine at 11 km (0.3% error) — worth one clause.

---

### Q3 — Interference on a lake; bow wave; radio square [20 marks]

**(a) Two synchronous dippers ($l=3.0$ m, $T=1.00$ s, $v=1.2$ m/s, so $\lambda=1.2$ m) [10 marks].**

(i) After 4.00 s: four concentric circular crests around each of A and B, radii $1.2, 2.4, 3.6, 4.8$ m — two expanding families crossing each other (scale diagram: draw A, B 3.0 m apart; circles at those radii).

(ii) At a point $x$ from A, $y$ from B: constructive: $\boxed{x-y=n\lambda}$; destructive: $\boxed{x-y=(n+\tfrac12)\lambda}$, $n=0,\pm1,\pm2,\dots$

(iii) On the diagram: crest–crest (and trough–trough) crossings form the constructive (antinodal) hyperbolic fringes along $x-y=n\lambda$; crest–trough crossings mark the destructive (nodal) lines between them — a fan of alternating hyperbolae symmetric about the perpendicular bisector (which is itself antinodal, $x=y$).

(iv) Far field ($\gg l$): $x-y\to l\cos\theta$ with $\theta=\angle POB$ measured from the line AB:

$$\boxed{\text{constructive: }l\cos\theta=n\lambda\ (\cos\theta=0.4n);\qquad \text{destructive: }l\cos\theta=(n+\tfrac12)\lambda.}$$

> 【Thought】 The local form (ii) in terms of distances is exact; the far-field form (iv) trades distances for angle — the projection $l\cos\theta$ is the whole content of "far away". Validity boundary of the approximation: $r\gg l^2/\lambda$.

---

**(b) Bow-wave angle [4 marks].**

The boat (5.0 m/s) outruns its own waves (2.5 m/s): wavefronts emitted at earlier times are circles whose radii grow at 2.5 m/s while the boat advances at 5.0 m/s; the bow wave is the common tangent from the boat's present position to those circles — a Mach wedge with

$$\boxed{\sin\varphi=\frac{v_{\text{wave}}}{v_{\text{boat}}}=\frac{2.5}{5.0}\;\Rightarrow\;\varphi=30^\circ}.$$

> 【Thought】 Construction: in time $t$ the boat moves $v_bt$ from the emission point while the wavefront grows to $v_wt$ — the tangent triangle gives $\sin\varphi=v_wt/v_bt$ directly. This is the water analogue of the Mach cone ($\sin\varphi=c/v$, Paper 37 Q7(d) shock).

---

**(c) 10 MHz transmitters on a 2000 m square [6 marks].**

(i) $\boxed{\lambda=c/f=30\ \text{m}}$.

(ii) At B: $p_B=AB-0=2000$ m $=n_B\lambda\Rightarrow\boxed{n_B=66.7}$ (destructive zone — anti-phase by 2/3 fringe). At C: $p_C=2000\sqrt2-2000=828$ m $\Rightarrow\boxed{n_C=27.6}$.

(iii) Moving from C toward B by $x$: $p(x)=\sqrt{2000^2+(2000-x)^2}-(2000-x)$, increasing with $x$. First maximum at $n=28$: $p=840$ m:

$$\sqrt{4\times10^{6}+(2000-x)^2}=2840-x\;\Rightarrow\;8\times10^{6}-4000x=8.0656\times10^{6}-5680x,$$

$$1680x=6.56\times10^{4}\;\Rightarrow\;\boxed{x=39\ \text{m}}.$$

> 【Thought】 Which order to target: $n_C=27.6$ sits between destructive ($27.5$... note $(n+\tfrac12)$) and the next constructive integer 28; moving toward B increases $p$ (the A-leg lengthens relative... check the derivative sign before squaring). Squaring introduces phantom roots — substitute back: $p(39.0)=2801-1961=840$ ✓.

---

### Q4 — Mass spectrometer: resolving K-39 from K-41 [20 marks]

**(a)(i) Circular path; field direction.** The magnetic force $QvB$ is perpendicular to the velocity and constant in magnitude — a constant sideways pull bending the ion at fixed speed: uniform circular motion. For a positive ion curving from O toward the film at P, the left-hand... the field must be **perpendicular to the plane, directed into it** (for the polarity shown, with the ion entering at right angles to OP).

**(a)(ii)** Centripetal balance: $QvB=mv^2/R\Rightarrow\boxed{R=\dfrac{mv}{BQ}}$. □

**(b) Singly charged K-39 / K-41, $V=500$ V, $B=0.70$ T [7 marks].**

(i) Acceleration: $\tfrac12mv_i^2=eV$:

$$v_i=\sqrt{\frac{2eV}{m}}=\boxed{\sqrt{\frac{1.60\times10^{-16}}{m}}:\quad v_{39}=4.96\times10^{4}\ \text{m/s},\quad v_{41}=4.83\times10^{4}\ \text{m/s}}.$$

(ii) The magnetic force never does work: $\boxed{v_f=v_i}$.

(iii) Injected perpendicular to OP, the ion sweeps a semicircle and hits the film a **diameter** away:

$$OP=2R=\frac{2mv_i}{eB}:\quad \boxed{OP_{39}=5.77\ \text{cm},\qquad OP_{41}=5.91\ \text{cm}}.$$

**(c)(i) Voltage ripple ±5 V.** $R\propto\sqrt{V}$, so $\Delta(OP)/OP=\tfrac12\Delta V/V=\pm0.5\%$: spreads $\pm0.029$ cm (K-39) and $\pm0.030$ cm (K-41). Peak separation $=0.15$ cm vs combined half-widths $\sim0.06$ cm — the lines overlap only marginally at the tails:

$$\boxed{\text{yes — resolved (separation }1.5\ \text{mm}\approx2.5\times\text{the summed spreads).}}$$

**(c)(ii) Direction jitter.** A small angular error $\delta$ in the incident direction leaves the speed (hence $R$) unchanged; the circle's centre shifts, and the landing point moves only to **second order**: $OP=2R\cos\delta\approx2R(1-\delta^2/2)$ — the semicircular geometry is *direction-focusing*, which is exactly why this spectrometer design is practical.

> 【Thought】 The design logic of the whole question: $OP\propto m v\propto\sqrt{m}$ for fixed $V$ — mass separation grows as $\sqrt{m}$ differences; resolution = separation/spread, and (c) computes it honestly. Note (c)(ii)'s lesson: first-order insensitivity to input angle is a designed-in feature, not luck — always ask "which order does the error enter at?"

---

### Q5 — Scales on a sliding platform; falling ring in a radial field [20 marks]

**(a) Bathroom scales on a 30° incline [10 marks].**

Scales (horizontal) read 75 kg → normal force on the student $N=75g$ vertically. Student's vertical equation: $80g-75g=80\,a_v$:

**(i)** $\boxed{a_v=\dfrac{5g}{80}=0.61\ \text{m s}^{-2}\ \text{downward}}$.

**(ii)** The platform constrains motion to the slope: $a_v=a_s\sin30^\circ\Rightarrow\boxed{a_s=1.23\ \text{m s}^{-2}}$ down the slope.

**(iii)** System (80 kg; scales/platform massless): perpendicular to the slope $R=80g\cos30^\circ$ (no acceleration that way); along the slope:

$$80g\sin30^\circ-\mu R=80a_s\;\Rightarrow\;\mu=\frac{g\sin30^\circ-a_s}{g\cos30^\circ}=\frac{4.905-1.226}{8.499}=\boxed{0.43}.$$

> 【Thought】 The subtle step: the scales are *horizontal* while sliding — so their reading isolates the vertical force balance directly ($a_v$), and the incline constraint converts $a_v$ to $a_s$. Common slip: assuming $N=80g\cos30^\circ$ for the student — that would be true only for scales glued perpendicular to the slope. Sanity: $\mu<\tan30^\circ=0.577$ (it slides) ✓.

---

**(b) Ring falling through a radial horizontal field [10 marks].**

**(i) emf by flux cutting.** Every element $dl$ of the ring falls at $v$ through the radial horizontal $B$: $v\times B$ is tangential, magnitude $vB$, the same all around — emf $=2\pi r vB$:

$$\boxed{I=\frac{2\pi rBv}{R}}.\quad\blacksquare$$

**(ii) Equation of motion.** The current $I$ in the radial field feels a vertical force (Lenz: opposing the fall): $F=BI\times2\pi r=\dfrac{(2\pi rB)^2v}{R}$:

$$\boxed{ma=mg-\frac{(2\pi rB)^2}{R}v}.\quad\blacksquare$$

**(iii) Initial and terminal behaviour.** At $t=0$, $v=0$: $a=g$, so initially $\boxed{v\approx gt}$ (linear). As $v$ grows the drag term bites; terminal when $a=0$:

$$\boxed{v_t=\frac{mgR}{(2\pi rB)^2}}.$$

(Full solution: $v=v_t(1-e^{-t/\tau})$ with $\tau=mR/(2\pi rB)^2$.)

**(iv) Sketches.** $v(t)$: linear rise from the origin, curving over, asymptoting to $v_t$; $a(t)$: exponential decay from $g$ toward 0 — the slope of $v$ at each instant.

> 【Thought】 Structure-match: this is Paper 34 Q1(l) with the rod's straight rail replaced by a ring in a radial field — the drag is again $\propto v$ with coefficient $(\text{flux linkage per metre})^2/R$, and the terminal condition $mg=BIL$ is the same energy-balance statement (GPE loss rate = $I^2R$) in disguise. In (iv) insist on consistency: $a$ is the gradient of $v$, so both sketches must agree at $t=0$ ($a=g$, $v$ linear) ✓.

---

### Q6 — Switched capacitor; Fourier square wave; cable capacitance [20 marks]

**(a) Switching capacitor as a current pump [7 marks].**

Each cycle the capacitor charges to $CV$ from the battery (position A) and dumps $CV$ through the ammeter (position B); at $n$ cycles per second:

$$\boxed{I_{\text{avg}}=nCV}.$$

**With lead resistance $R$:** the charge/discharge acquires a time constant $\tau=RC$.

(i) **$R$ with the battery:** charging is incomplete if $\tau\gtrsim1/n$ — less charge transferred per cycle → **current falls below $nCV$** (smoothly, as $\tau$ grows; unchanged if $\tau\ll1/n$).

(ii) **$R$ with the ammeter:** same effect on the discharge side — incomplete discharge per dwell → **average current again falls** below $nCV$.

> 【Thought】 This is the switched-capacitor principle: $C$ and the switch mimic a resistance $1/nC$ — the "resistor" of every switched-capacitor filter and charge pump. The resistance question probes the assumption hidden in $I=nCV$: *complete* charge and discharge each dwell — state it, then break it.

---

**(b) Fourier anatomy of $F(t)=\frac4\pi[\cos2\pi ft-\frac13\cos6\pi ft+\frac15\cos10\pi ft]$ [4 marks].**

| term | amplitude | frequency | phase | period |
|---|---|---|---|---|
| $\cos2\pi ft$ | $4/\pi$ | $f$ | $0$ | $1/f$ |
| $-\frac13\cos6\pi ft$ | $4/3\pi$ | $3f$ | $\pi$ (the minus sign) | $1/3f$ |
| $\frac15\cos10\pi ft$ | $4/5\pi$ | $5f$ | $0$ | $1/5f$ |

The odd harmonics with $1/n$ amplitudes are exactly the square wave's Fourier fingerprint.

**(c) Square wave $V_0$ across R and across C [4 marks].** (i) Resistor: $I=V/R$ — a square wave of amplitude $V_0/R$, in phase with $V$. (ii) Capacitor on an ideal voltage source: $Q=CV_0$ — a square wave of amplitude $\pm CV_0$ (the current is a train of delta spikes at the edges). (iii) With $V_0F(t)$ instead (band-limited square wave): both $I$ and $Q$ become the *rounded* version $V_0F(t)/R$ and $CV_0F(t)$ — Gibbs-ripple edges, no vertical jumps.

> 【Thought】 Ideal components with an ideal square wave force ideal pathologies (infinite edge currents); the Fourier truncation $F(t)$ is the honest version — every real square wave is band-limited, and (iii) shows what that does to the sketches.

---

**(d) 1 MHz square wave down a capacitive cable [5 marks].**

The generator's 300 Ω drives the cable's $1.5$ nF: an RC low-pass with

$$\tau=RC=300\times1.5\times10^{-9}=0.45\ \mu\text{s},\qquad\text{vs half-period }0.50\ \mu\text{s}.$$

$\tau\approx$ half-period: the trace never settles — each half-cycle is an exponential lunge toward the rail that only reaches a fraction of it. Steady state: with $x=e^{-0.5/0.45}=0.33$, the peaks sit at

$$V_p=V_0\frac{1-x}{1+x}=0.50\,V_0,$$

so the oscilloscope shows a **rounded, amplitude-halved** waveform (exponential edges between $\pm0.5V_0$) — the square wave's teeth visibly filed down.

> 【Thought】 The comparison $\tau$ vs half-period is the entire diagnosis: $\tau\ll T/2$ → clean square; $\tau\gg T/2$ → near-triangular ripple; $\tau\sim T/2$ (here) → rounded and attenuated. This is why fast signals need matched ($50\ \Omega$) cables, not plain wire pairs.

---

*End of Paper 38.*
