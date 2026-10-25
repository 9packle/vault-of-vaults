# UKChO Round 1 — Heuristic Solutions Collection

**Conventions.** Every sub-part is written in two layers:
- **L1 · Answer** — the explicit, mark-anchor chain you could copy into an answer booklet;
- **L2 · Thought** — why that route was chosen, which alternatives were rejected, and the transferable move with its failure condition.

Structures are given as condensed formulas plus SMILES for unambiguity; wedge/dash stereochemistry is described in words. Derived quantities are checked dimensionally and, where possible, against an independent physical anchor.

---

# Paper 1 — 2025 UKChO Round 1 (57th IChO selection)

*6 questions, 83 marks, 2 h → budget ≈ 1.4 min per mark. Marks: Q1 = 8, Q2 = 9, Q3 = 20, Q4 = 12, Q5 = 19, Q6 = 15.*

## Q1 — Clay pigeon shooting: nitrocellulose chemistry (8 marks)

### (a)(i) Equation for cellulose → cellulose trinitrate
**L1 · Answer**
$$C_6H_7(OH)_3O_2 + 3\,HNO_3 \longrightarrow C_6H_7(ONO_2)_3O_2 + 3\,H_2O$$
Atom audit: C 6 = 6; N 3 = 3; H: left 7 (cellulose backbone C–H) + 3 (the three –OH hydrogens) + 3 (from 3 HNO₃) = 13, right 7 + 6 (3 H₂O) = 13 ✓; O: left 5 + 9 = 14, right 11 + 3 = 14 ✓.

**L2 · Thought** Seeing "empirical formula of reactant and product given" → triggers the **conservation audit**: count what changed. Each –OH became –ONO₂, i.e. H was replaced by NO₂ three times, so exactly 3 HNO₃ enter and 3 H₂O leave. The trap is writing "H₂O" without the coefficient 3, or adding O₂ because the context is combustion — **wording audit**: this is esterification (condensation), not burning. If the stem had said "in air", O₂ would still not belong here.

### (a)(ii) Dot-and-cross diagram of NO₂⁺
**L1 · Answer** Linear O=N=O⁺. Electron budget: 5 (N) + 2×6 (O) − 1 (charge) = 16 e⁻. Draw two N=O double bonds (each = 2 N electrons [dots] + 2 O electrons [crosses]) and **two lone pairs on each O**; N carries no lone pair. Formal charges: FC(N) = 5 − 0 − ½(8) = **+1**; FC(O) = 6 − 4 − ½(4) = 0 → overall +1, placed on N: [O=N=O]⁺.

**L2 · Thought** Trigger: "dot-and-cross" → **octet/formal-charge audit**. The common failure is giving N a lone pair (then N would be −1 and both O neutral — total charge wrong) or drawing single bonds (O would carry +1 each and fail the electronegativity check: positive charge prefers the less electronegative N, and double bonds satisfy every octet with no charge separation beyond the required +1).

### (b) Formation of the intermediate H₂NO₃⁺
**L1 · Answer**
$$HNO_3 + H_2SO_4 \rightleftharpoons H_2NO_3^+ + HSO_4^-$$
(proton transfer from the stronger acid H₂SO₄ onto a nitrate O of HNO₃.)

**L2 · Thought** The stem hands you the roles: "nitric acid acts as a Lewis base and **accepts a proton**" → this is pure proton transfer, no redox. Command word is *write the equation* → balanced + charges; reversible arrows acceptable, charges mandatory. Trap: writing HNO₃ + H⁺ → H₂NO₃⁺ (free H⁺ does not exist in this medium; the proton source must be shown).

### (c) Decomposition of H₂NO₃⁺
**L1 · Answer**
$$H_2NO_3^+ \longrightarrow NO_2^+ + H_2O$$
Atom/charge audit: N 1=1, O 3 = 2+1 ✓, H 2=2 ✓, charge +1 = +1 ✓.

**L2 · Thought** Seeing "decomposes to form the nitronium ion" → the only heavy fragment available after removing NO₂⁺ from H₂NO₃⁺ is H₂O. This is exactly the acid-catalysed leaving-group logic of aromatic nitration: protonation converts a poor leaving group (OH⁻) into an excellent one (H₂O). Transferable signal: *protonate first, then lose water*.

### (d) Complete combustion of C₆H₇N₃O₁₁
**L1 · Answer** Complete combustion → CO₂, H₂O and the gaseous element N₂, **with O₂ as a reactant**:
$$4\,C_6H_7N_3O_{11} + 9\,O_2 \longrightarrow 24\,CO_2 + 14\,H_2O + 6\,N_2$$
(Atom audit: C 24=24; H 28=28; N 12=12; O 44+18 = 62 = 48+14 ✓.)

**L2 · Thought** Two traps. (1) Forgetting O₂: nitrocellulose is oxygen-rich but not oxygen-balanced — balancing C₆H₇N₃O₁₁ → 6 CO₂ + 3.5 H₂O + 1.5 N₂ leaves product O = 15.5 > 11, so 4.5 O atoms (2.25 O₂) per formula unit must come from outside. (2) Writing CO: "complete" combustion means fully oxidised carbon (CO₂). **The ΔfH(CO) datum is a deliberate distractor** — see (e).

### (e) Standard enthalpy of combustion
**L1 · Answer** Hess cycle on the equation from (d), per mole of cellulose trinitrate:
$$\Delta_c H^\circ = [6\,\Delta_fH^\circ(CO_2) + 3.5\,\Delta_fH^\circ(H_2O)] - \Delta_fH^\circ(\text{trinitrate})$$
$$= [6(-393.5) + 3.5(-285.8)] - (-653.1) = -3361.3 + 653.1 = \mathbf{-2708.2\ kJ\ mol^{-1}}$$
(elements O₂ and N₂ have ΔfH° = 0; ΔfH°(CO) is not needed for *complete* combustion.)

**L2 · Thought** Trigger: enthalpy data table → **Hess cycle, products minus reactants**. Step marking rewards the explicit cycle, so the bracket structure above is written before any numbers. **Data audit**: four enthalpies were given; only three are used — ΔfH(CO) is bait for students who chose CO in (d). If your (d) had CO, this datum rescues consequential marks — that is why it is printed.

### (f) Decomposition in the cartridge (no O₂, all products gaseous)
**L1 · Answer**
$$2\,C_6H_7N_3O_{11} \longrightarrow 3\,CO_2 + 9\,CO + 7\,H_2O + 3\,N_2$$
(Audit: C 12 = 3+9 ✓; H 14 = 14 ✓; N 6=6 ✓; O 22 = 6+9+7 ✓.)

**L2 · Thought** Wording audit first: "no oxygen is formed" and no air available → all oxidising power comes from the molecule itself. Assign the most oxidised carbon product CO₂ and the balance as CO (the ΔfH(CO) datum now becomes relevant context). Solve the atom balances: N fixes 3 N₂ per 2 formula units; H fixes 7 H₂O; then C: a+b = 12 and O: 2a+b+7 = 22 → a = 3, b = 9. Self-check: fractional version C₆H₇N₃O₁₁ → 1.5 CO₂ + 4.5 CO + 3.5 H₂O + 1.5 N₂ is acceptable, integers preferred.

### (g) Volume of gas from 5.00 g at 200 °C
**L1 · Answer**
M(C₆H₇N₃O₁₁) = 6(12.01) + 7(1.008) + 3(14.01) + 11(16.00) = 297.15 g mol⁻¹
n(trinitrate) = 5.00 / 297.15 = 1.683 × 10⁻² mol
Gas per equation (f): 11 mol gas per mol trinitrate (4.5 CO + 3.5 H₂O + 1.5 N₂ + 1.5 CO₂) → n(gas) = 1.683 × 10⁻² × 11 = **0.1851 mol**
$$V = \frac{nRT}{p} = \frac{0.1851 \times 8.314 \times 473}{101325} = \mathbf{7.18\times10^{-3}\ m^3}$$
(7.21 × 10⁻³ m³ at 1.01 × 10⁵ Pa — same to 2 s.f. Mark scheme: 7.18 × 10⁻³ m³; the question demands m³ explicitly.)

**L2 · Thought** Three silent decisions, each worth stating: (1) **water is gaseous at 200 °C** — the stem's "assume all products are gaseous" licenses counting 7 H₂O in n(gas); at 25 °C this move would fail. (2) Convert °C → K (473 K) *before* substitution. (3) "Atmospheric pressure" from the data sheet. Dimensional check: mol × J K⁻¹ mol⁻¹ × K / Pa = J/Pa = m³ ✓. Sanity: 0.185 mol of gas ≈ 4.4 dm³ at r.t.p., scaled by 473/298 → ≈ 7 dm³ ✓. The gas multiplier from the integer equation is 22 mol per 2 mol = 11 mol per mole of trinitrate — keying in ×5.5 by accident would halve the volume; the sanity line above is what exposes such a slip.

---

## Q2 — BrAt: astatine chemistry (9 marks)

### (a) Natural abundance of At atoms
**L1 · Answer**
$$N = \frac{m}{M}\,N_A = \frac{30\ \text{g}}{219\ \text{g mol}^{-1}} \times 6.022\times10^{23}\ \text{mol}^{-1} = \mathbf{8.2\times10^{22}\ atoms}$$

**L2 · Thought** Trigger: "estimate … assume all astatine is ²¹⁹At" → the isotope mass number *is* the molar mass in g mol⁻¹ (219, not the periodic-table entry, which barely exists for At). Two sig figs in, two out.

### (b) Empirical formula of alloy A
**L1 · Answer** Per 100 g: Ca 7.91 g, Mg 9.60 g, Bi 82.49 g (no lead).
n(Ca) = 7.91/40.08 = 0.1974; n(Mg) = 9.60/24.31 = 0.3950; n(Bi) = 82.49/208.98 = 0.3947
Ratio Ca : Mg : Bi = 0.1974 : 0.3950 : 0.3947 = 1 : 2.00 : 2.00 → **CaMg₂Bi₂**

**L2 · Thought** Standard mass-% → moles → divide-by-smallest drill. The near-perfect 1:2:2 within rounding confirms no arithmetic slip (if a ratio landed at 1:1.5:2.7, re-check before forcing integers). Note the result is the real Zintl phase CaMg₂Bi₂ — a good physical plausibility anchor.

### (c) Chlorination products B and C
**L1 · Answer** **B = MgCl₂, C = CaCl₂** — the stem's "B and C **in a 2:1 ratio**" reads n(B) : n(C) = 2 : 1, so B is the salt formed in two parts (MgCl₂, from the two Mg per formula unit) and C the one-part salt (CaCl₂). The mark scheme awards no credit the wrong way around — the order is decided by that ratio clause. Consistent equation:
$$CaMg_2Bi_2 + 3\,Cl_2 \longrightarrow 2\,Bi + 2\,MgCl_2 + CaCl_2$$
(audit: Cl 6 = 4 + 2 ✓, Ca 1, Mg 2, Bi 2 ✓).

**L2 · Thought** Seeing "alloy + Cl₂ → Bi + two ionic compounds" → chlorine oxidises the electropositive metals to their only stable chlorides (Ca²⁺, Mg²⁺; no higher chlorides exist), liberating the less reactive Bi(0). The "2:1 ratio" clause does double duty: it is a checksum against (b)'s Mg : Ca = 2 : 1, *and* it fixes the B/C reading order (B first = the 2-part compound). This is **consequential-marking design**: (c) is answerable from (b)'s formula even if (b)'s arithmetic slipped.

### (d) The astatine isotope
**L1 · Answer** Mass: 209 + 4 − 2 = **211**; atomic number: 83 + 2 − 0 = **85** → **²¹¹₈₅At**.

**L2 · Thought** Nuclear conservation audit: mass number and atomic number conserved separately; the 2 neutrons carry mass 2, charge 0. (²¹¹At is indeed the isotope used in real α-therapy research — plausibility anchor.)

### (e) Bi + concentrated HNO₃
**L1 · Answer** The colourless gas of M = 30.01 g mol⁻¹ is NO (14.01 + 16.00 = 30.01 ✓; NO₂ would be 46.01):
$$Bi + 4\,HNO_3 \longrightarrow Bi(NO_3)_3 + NO\uparrow + 2\,H_2O$$
Audit: N 4 = 3+1 ✓; H 4=4 ✓; O 12 = 9+1+2 ✓; electrons: Bi → Bi³⁺ + 3e⁻; N(+5) + 3e⁻ → N(+2) ✓.

**L2 · Thought** Two-step logic: first **identify the gas from its molar mass** (a mini *deduce* inside the *write-the-equation* task) — colourless + M = 30.01 nails NO, not brown NO₂. Then balance by oxidation-state audit: Bi climbs 0 → +3 (loses 3e⁻), so exactly one N(+5) → N(+2) per Bi; nitrate for Bi³⁺ needs 3 more HNO₃ — total 4. Trap: concentrated HNO₃ on most metals gives NO₂; Bi's product here is specified by the molar mass, so the data override the habit.

### (f) D and E
**L1 · Answer** **E = IBr** (iodine monobromide); **D = I₂**.
Route: Br₂ + I₂ → 2 IBr ("compound E only"); then 2 IBr + At₂ → 2 BrAt + I₂ (D regenerated ✓).
Mass-spec check: I⁷⁹Br⁺ = 126.90 + 78.92 = **205.82** ✓; I⁸¹Br⁺ = 126.90 + 80.92 = **207.82** ✓ — a 1:1 doublet, Δ = 2.00 u, the signature of **exactly one Br** (⁷⁹Br:⁸¹Br ≈ 1:1). Br₂ would give a 1:2:1 triplet at 158/160/162 — ruled out.

**L2 · Thought** This is the **isotope-signature move** in full: equal-intensity doublet → one Br; the residual mass 205.82 − 78.92 = 126.90 identifies iodine (the only common element at ~127). Then the cycle logic: E + At₂ → BrAt + D means D is displaced *out* of E by the more reactive... — careful: At is the *least* reactive halogen, yet the scheme asserts it happens, so accept the displacement as given and use it only to identify D = I₂ (what comes out must have gone in). Seeing "reacts with D to make E **only**" → D + Br₂ gives a single product → D = I₂ (IBr is the single interhalogen), not e.g. Cl₂ (ICl/IBr mixtures). Boundary: this move fails if the molecular-ion cluster overlaps other fragments — always check Δ and intensity ratio first.

### (g) Length of BrAt Bear Summer
**L1 · Answer** 3.60 g remaining 3.65 mg:
$$n = \log_2\!\frac{m_0}{m} = \log_2\!\frac{3.60}{3.65\times10^{-3}} = \log_2(986.3) = 9.95\ \text{half-lives}$$
$$t = 9.95 \times 433\ \text{min} = 4.31\times10^{3}\ \text{min} = 71.8\ \text{h} \approx \mathbf{72\ hours}$$

**L2 · Thought** Unit discipline first: g and mg must share a unit before the log. log₂(x) = ln x / ln 2 — no special calculator needed. "Nearest hour" → 72 h; quoting 71.78 h ignores the instruction (command-word compliance is a marking point here).

---

## Q3 — Epoxides and epoxy resin (20 marks)

### (a) General formula of an n-carbon epoxide
**L1 · Answer** **CₙH₂ₙO**. A saturated acyclic ether is CₙH₂ₙ₊₂O; closing one ring removes H₂ → CₙH₂ₙO (equivalently: DBE = 1, the ring).

**L2 · Thought** Trigger: "general formula … n carbons" → **DBE budget**. Fastest route is the homologous anchor: ethylene oxide C₂H₄O fits CₙH₂ₙO, then verify against a second case (methyloxirane C₃H₆O ✓). Failure condition: the formula assumes the epoxide ring is the *only* unsaturation — an unsaturated epoxide (e.g. vinyl oxirane) would need DBE 2.

### (b) C–C–O bond angles (tick table)
**L1 · Answer**
- C₂H₅OC₂H₅: tick **109.5°** — the O is tetrahedral (2 bonds + 2 lone pairs); C–C–O ≈ tetrahedral angle.
- Ethylene oxide (oxirane): tick **60°** — the ring is (almost) an equilateral triangle of two C and one O, so the internal C–C–O angle is forced to ≈ 60°.

**L2 · Thought** Deciding criterion: *what geometry does the connectivity force?* Acyclic ether → free tetrahedral; three-membered ring → the triangle's internal angle. The 45° gap between the two answers *is* the ring strain the question stem keeps mentioning — this table is quietly teaching why epoxides are reactive. Boundary: do not tick 104.5° for the ether (that is water's H–O–H, compressed by two lone pairs repelling two *bonds to H*; in ethers the C–O–C angle is ~111°, but the question asks C–C–O, tetrahedral at carbon).

### (c) Compound A (peroxyacid epoxidation by-product)
**L1 · Answer** **A = R–COOH**, the carboxylic acid corresponding to the peroxyacid (generic acyl group R–C(=O)–OH).
Atom audit on the scheme: peroxyacid RCO₃H + alkene → epoxide + A; the epoxide took one O, so A = RCO₂H.

**L2 · Thought** The bracketed transition state is the Prilezhaev "butterfly": the alkene π bond attacks the terminal O of the O–O–H unit while the acidic H transfers onto the carbonyl O — all in one concerted step. Reading the arrows: O–O breaks, C=O stays, O–H breaks, and the proton lands on the carbonyl oxygen → the leaving fragment is the carboxylic acid. Because the step is **concerted**, the two new C–O bonds form on the same face — that is why (d) and (e) can talk about *syn* addition and stereoisomer counts.

### (d) Both stereoisomers from propene
**L1 · Answer** Propene oxide (2-methyloxirane) has one stereocentre (C2, bearing H/CH₃/O/CH₂). Epoxidation from the top face and the bottom face gives the two enantiomers:
- **(R)-2-methyloxirane** — ring O drawn as the triangle at top, CH₃ on a solid wedge (toward viewer): SMILES `C[C@H]1CO1`
- **(S)-2-methyloxirane** — CH₃ on a hashed wedge (behind): SMILES `C[C@@H]1CO1`

**L2 · Thought** Trigger: "stereoisomers … approach from above or below" → count stereocentres created *in the product*. The CH₂ ring carbon keeps two H's → not stereogenic; only C2 is. Concerted syn addition on a *planar, unsymmetrical* alkene → two enantiomeric products in equal amounts (racemate). Trap to avoid: do not invent E/Z labels for the alkene here — propene has none.

### (e) Number of epoxide stereoisomers from each C₄H₈ isomer (tick table)
**L1 · Answer**

| C₄H₈ isomer | Epoxide product(s) | Tick |
|---|---|---|
| but-1-ene, CH₂=CHCH₂CH₃ | 1,2-epoxybutane has **one stereocentre** (C2: H/Et/O/CH₂) → (R) + (S) enantiomers | **2** |
| cis-but-2-ene | syn addition preserves cis: cis-2,3-dimethyloxirane = (2R,3S), an internal mirror plane → **meso**, one compound | **1** |
| trans-but-2-ene | trans-2,3-dimethyloxirane = (2R,3R) + (2S,3S), an enantiomeric pair | **2** |
| 2-methylpropene | 2,2-dimethyloxirane: no stereocentre (one ring C has two CH₃, the other two H) | **1** |

**L2 · Thought** Deciding criterion: inventory the stereocentres *in each product*, then apply the 2ⁿ budget **with the meso correction**. cis-Alkene → both CH₃ on the same face → the product's mirror plane survives → meso (1). trans-Alkene → methyls on opposite faces → no plane → enantiomeric pair (2). Terminal/unsymmetrical alkenes → one stereocentre → 2. Quaternary-substituted → 0 → 1. Boundary condition for the whole move: it works *because* epoxidation is concerted and syn; a stepwise radical epoxidation would scramble these counts.

### (f) Ring-openings of ethylene oxide: B, C, D
**L1 · Answer** Epoxide opening by H–Nu gives HO–CH₂–CH₂–Nu:
- **B** = CH₃S–CH₂CH₂–OH (2-(methylthio)ethan-1-ol; SMILES `CSCCO`)
- **C** = H₂N–CH₂CH₂–OH (2-aminoethan-1-ol; SMILES `NCCO`)
- **D** = N(CH₂CH₂OH)₃ (triethanolamine; SMILES `OCCN(CCO)CCO`)

**L2 · Thought** Seeing "1 equiv." vs "⅓ equiv." → the *equivalents are the message*. NH₃ has three N–H bonds; with ⅓ equiv. NH₃ (3 equiv. epoxide per N) all three N–H's alkylate sequentially (2-aminoethanol → diethanolamine → triethanolamine). With 1 equiv. the mono-adduct is drawn. Regiochemistry is not an issue for symmetrical ethylene oxide — but note the general rule for (g): nucleophile attacks the **less hindered** ring carbon under basic/neutral conditions.

### (g) Epichlorohydrin + sodium phenoxide: E⁻ and F
**L1 · Answer**
- **E⁻** = PhO–CH₂–CH(O⁻)–CH₂Cl (sodium 3-chloro-2-phenoxypropan-2-olate; SMILES `[O-]C(CCl)COc1ccccc1`). Phenoxide O attacks the **terminal CH₂ of the epoxide ring** (less hindered), opening it to the alkoxide.
- **F** = phenyl glycidyl ether: PhO–CH₂–CH––CH₂ closed into a new epoxide (2-(phenoxymethyl)oxirane; SMILES `c1ccccc1OCC1CO1`). The alkoxide does an intramolecular SN2 on the –CH₂–Cl carbon, ejecting Cl⁻.
Formula audit: E⁻ = [C₉H₁₀O₂Cl]⁻ ✓ matches the scheme (PhO⁻ C₆H₅O⁻ + epichlorohydrin C₃H₅OCl); cyclisation ejects Cl⁻ and the alkoxide O⁻ is neutralised by forming the ring C–O bond: net E⁻ → F + Cl⁻, so F = C₉H₁₀O₂ ✓.

**L2 · Thought** Two site-selection calls, each with a reason kept in L1 brackets: (1) attack at the epoxide CH₂, *not* the CH₂Cl carbon (had the phenoxide done intermolecular SN2 on CH₂Cl first, the Cl would already be gone — but the scheme's bracketed intermediate [C₉H₁₀O₂Cl]⁻ retains Cl, so the epoxide must have opened first; the alkoxide-then-SN2 route is the only one that *loses* Cl in the second step, matching F = C₉H₁₀O₂); (2) ring-size check: the alkoxide closing onto –CH₂–Cl forms a **3-membered** ring — allowed because intramolecular epoxide formation is fast; no alternative ring size is geometrically available from this connectivity. The **formula audit is what makes this deduction rigorous** rather than a guess.

### (h) Benzene → BADGE: G, H, I
**L1 · Answer**
- **G = nitrobenzene**, C₆H₅NO₂ (SMILES `O=[N+]([O-])c1ccccc1`) — conc. HNO₃/conc. H₂SO₄ = electrophilic nitration (the NO₂⁺ chemistry of Q1!).
- **H = benzenediazonium chloride**, [C₆H₅N₂]⁺ Cl⁻ (SMILES `c1ccccc1[N+]#N.[Cl-]`) — aniline + NaNO₂/HCl = diazotisation; matches the printed formula [C₆H₅N₂]Cl ✓. Charge placement matters (mark scheme explicit): the positive charge sits on the nitrogen **directly attached to the ring**, Ph–N⁺≡N (4-bond N, FC = +1; terminal N neutral with one lone pair).
- **I = bisphenol A** = 2,2-bis(4-hydroxyphenyl)propane, (4-HO–C₆H₄)₂C(CH₃)₂ (SMILES `CC(C)(c1ccc(O)cc1)c1ccc(O)cc1`) — phenol + propanone under H⁺: twice Friedel–Crafts-type hydroxyalkylation at the *para* position, with water lost. Formula audit: C₁₅H₁₆O₂ ✓ matches the scheme.
(The final step, base then epichlorohydrin, is exactly (g)'s chemistry run twice: phenoxide opens epichlorohydrin's epoxide, alkoxide closes on CH₂Cl → BADGE.)

**L2 · Thought** This sub-scheme is a guided tour of classic benzene functionalisation: NO₂ → NH₂ → N₂⁺ → OH is the standard "upgrade benzene to phenol" ladder (reduction, diazotisation, hydrolysis). Recognising the ladder early makes G and H one-line answers. For I: seeing "phenol + acetone, H⁺" and the target name **bisphenol A diglycidyl ether** → the name itself discloses the carbon skeleton (bisphenol A = two phenols joined by C(CH₃)₂); the protonated acetone carbonyl is the electrophile, phenol's para position the nucleophile, twice. Keep the chain visible for consequential marking: even if G were wrong, H and I are answerable from the reagents alone.

### (i) Hardeners J and K (reverse-read the repeat units)
**L1 · Answer** Reading each repeat unit backwards — every –NH–CH₂–CH(OH)– junction was born from an N–H opening an epoxide ring:
- **J = H₂N–CH₂CH₂–N(CH₃)–CH₂CH₂–N(CH₃)–CH₂CH₂–NH₂** (N2,N3-dimethyltriethylenetetramine; SMILES `NCCN(C)CCN(C)CCN`). Its repeat unit is linear: –CH₂CH₂–N(CH₃)–CH₂CH₂–NH–CH₂–CH(OH)–[BADGE]–CH(OH)–CH₂–NH–CH₂CH₂–N(CH₃)–. Only the two terminal –NH₂ groups can open epoxides; the two internal nitrogens are **tertiary (N–CH₃) and carry no N–H**, so they stay inert → **linear** polymer.
- **K = (H₂NCH₂CH₂)₂N–CH₂CH₂–N(CH₂CH₂NH₂)₂** (N,N,N′,N′-tetrakis(2-aminoethyl)ethane-1,2-diamine; SMILES `NCCN(CCN)CCN(CCN)CCN`). The two internal tertiary nitrogens each bear **two –CH₂CH₂NH₂ arms**; all four primary amines open epoxides → every hardener molecule stitches into four BADGE units → the **crosslinked network** drawn (two tertiary N joined by –CH₂CH₂–, each radiating –CH₂CH₂–NH–CH₂–CH(OH)–[BADGE] arms).

**L2 · Thought** This is the **repeat-unit back-reading** move. Steps: ① locate the bonds that did not exist in the monomers — here the C–N bonds between –CH₂–CH(OH)– (opened epoxide) and nitrogen; ② break them mentally and restore an H on each such N; ③ whatever remains bonded to N (CH₃ in J, CH₂CH₂NH₂ in K) was already there in the monomer. The decisive observation: J's internal N's show a **methyl cap** (plain line end, no H) → dead ends → linear; K's internal N's show **three carbon arms** with amine ends → branch points → network. The design contrast is the lesson: methyl-capping the backbone nitrogens converts a crosslinker into a chain-extender. Boundary: if the repeat unit showed ester links instead, you'd restore –OH/–COOH and add back the lost H₂O — same move, different bookkeeping.

---

## Q4 — Carbon nanotubes and Raman spectroscopy (12 marks)

### (a) Nanotube side reaction from ethyne combustion
**L1 · Answer**
$$n\,C_2H_2 + \tfrac{n}{2}\,O_2 \longrightarrow 2\,C_n + n\,H_2O$$
(equivalently ½n C₂H₂ + ¼n O₂ → Cₙ + ½n H₂O; audit: C 2n = 2n ✓; H 2n = 2n ✓; O n = n ✓.)

**L2 · Thought** Wording audit: the side reaction "occurs **during the combustion** of ethyne" — so O₂ is available and the H-sink is water, not H₂ (any H₂ formed would simply burn). The O₂-inclusive form above is the intended equation; the oxygen-free pyrolysis form n C₂H₂ → 2 Cₙ + n H₂ balances too, but it describes a different (oxygen-free) environment — with the stem's combustion setting, include O₂.

### (b) Percentage of carbon ending in nanotubes
**L1 · Answer** n(C₂H₂) = pV/RT = (1.01 × 10⁵ Pa × 40.00 × 10⁻³ m³)/(8.314 J K⁻¹ mol⁻¹ × 298 K) = 1.63 mol (1.636 mol at 101 325 Pa)
m(C total) = 1.63 × 2 × 12.01 = 39.2 g (all ethyne carbon — nanotubes are a side product of *this* carbon pool)
% = 0.242 / 39.2 × 100 % = **0.62 %** (mark scheme: 0.616 %; also accepts 0.603 % via the 24 dm³ molar volume)

**L2 · Thought** The conceptual key: the denominator is **all carbon in the ethyne burned**, not the mass of ethyne and not the mass of products — the question says "percentage by mass of **carbon**". Ideal-gas at 298 K/atmospheric pressure; state the ideal-gas assumption before substituting (skeleton 7.5). 1.63 mol × 24.02 g of C per mol C₂H₂ keeps the "carbon only" logic visible for consequential marking.

### (c) Compound A (ethyne trimer)
**L1 · Answer** **Benzene**, C₆H₆ (SMILES `c1ccccc1`): 3 C₂H₂ → C₆H₆.

**L2 · Thought** "Three molecules of ethyne trimerise" → the classic cyclotrimerisation. The follow-on clues confirm it: Raman's 1928 sample was liquid benzene, and part (f)'s IR peaks just above 3000 cm⁻¹ (aromatic C–H) and ~1600 cm⁻¹ (ring C=C) fit benzene exactly — a mid-question consistency anchor.

### (d) Repeat unit of polymer B
**L1 · Answer** Poly(ethyne) (polyacetylene): **[–CH=CH–]ₙ**, repeat unit –CH=CH–.

**L2 · Thought** Addition polymerisation across the triple bond leaves one π bond per monomer: n HC≡CH → (–CH=CH–)ₙ. The conjugated backbone is also why polyacetylene conducts — links to the stem's "variable electrical conductivity" remark (context sentences in UKChO are rarely decorative).

### (e) Raman line arithmetic
**L1 · Answer**
(i) ν₁ = c/λ₁ = 2.998 × 10⁸ / (5028.8 × 10⁻¹⁰) = 5.962 × 10¹⁴ Hz; ν_X = 2.998 × 10⁸ / (4358.3 × 10⁻¹⁰) = 6.879 × 10¹⁴ Hz
Δν = ν_X − ν₁ = **9.17 × 10¹³ Hz**
(ii) ν̃₂ = 1/λ₂ = 1/(4683.9 × 10⁻⁸ cm) = 2.1350 × 10⁴ cm⁻¹; ν̃_X = 1/(4358.3 × 10⁻⁸ cm) = 2.2945 × 10⁴ cm⁻¹
Δν̃ = ν̃_X − ν̃₂ = **1595 cm⁻¹** (mark scheme: 1600 cm⁻¹ via Δf₂ = 4.78 × 10¹³ Hz ÷ c — same quantity, rounding only)

**L2 · Thought** Two habits make this trivial: (1) work the **Stokes** direction — scattered light has *less* energy, so subtract line-from-incident, never the reverse (the magnitude is marked, but the sign tells you the physics); (2) unit ladder: Å → m for frequency (1 Å = 10⁻¹⁰ m), Å → cm for wavenumber (1 Å = 10⁻⁸ cm). Hidden gem for later: Δν̃ for line 1 = 22945 − 1/(5028.8 × 10⁻⁸) = 22945 − 19885 = **3059 cm⁻¹**, and for line 2 = 1595 cm⁻¹ — these *are* the answers to (f) before you even read it.

### (f) Which vibration for each Raman line (tick table)
**L1 · Answer**
- **Line 1** (λ 5028.8 Å; Raman shift 3059 cm⁻¹) → **C–H stretch** (aromatic C–H sits just above 3000 cm⁻¹ ✓ matches the IR clue).
- **Line 2** (λ 4683.9 Å; Raman shift 1595 cm⁻¹) → **conjugated C=C stretch** (benzene ring mode ~1600 cm⁻¹ ✓).

**L2 · Thought** Deciding criterion: convert each line's wavelength into a **Raman shift** (ν̃_X − ν̃_line) and match against the IR anchor peaks given (just above 3000; around 1600). The distractors eliminate themselves: C≡C ~2200 cm⁻¹ (not present), isolated C–C ~800–1200 cm⁻¹ (too low), O–H ~3400 cm⁻¹ broad (no O in benzene!). This is why (e) asked for one line in Hz and the other in cm⁻¹ — it forces you to be fluent in both units before the table.

### (g) The nanotube calibration
**L1 · Answer** The mode's wavenumber is the **Raman shift**: ν̃_mode = ν̃_laser − ν̃_scattered = A/d, with d = 2r. So a plot of ν̃_scattered against 1/(2r) is linear with slope −A/2 and intercept ν̃_laser.

Data as (1/2r in nm⁻¹, ν̃_scat in cm⁻¹): (0.4310, 9302.2), (0.3817, 9313.3), (0.3521, 9319.9), (0.3205, 9327.1)
Least-squares fit (or a careful two-edge-point gradient):
slope = (9327.1 − 9302.2)/(0.3205 − 0.4310) = 24.9/(−0.1105) = −225 cm⁻¹ nm → **A = 225 cm⁻¹ nm** (accept 224–226)

(i) **A ≈ 225 cm⁻¹·nm** (one compound unit, cm⁻¹·nm, since ν̃ = A/d must carry cm⁻¹ — not two separate units; mark scheme: 223, accepted range 201–245 — note halving by forgetting d = 2r gives ~112, which the scheme also pens at reduced credit).
(ii) intercept ν̃_laser = 9302.2 + 225 × 0.4310 = 9399 cm⁻¹ → λ_laser = 10⁷/9399 = **1064 nm** (mark scheme: intercept 9398.5 cm⁻¹ → 1064 nm ✓).
(iii) The stem gives the **diameter** directly: d = 2.4 nm → shift = 225/2.4 = 93.8 cm⁻¹; ν̃_scat = 22945 − 93.8 = 22851 cm⁻¹ → λ = 10⁸/22851 = **4376 Å**. (Note: the printed mark scheme here divides by 1.20 nm — obtaining 186 cm⁻¹ and 4394 Å — i.e. it treats the 2.4 nm as a *radius*; the stem says "a **2.4 nm diameter**", and ν̃ = A/d is defined on the diameter, so d = 2.4 nm is the stem-faithful substitution and is the one shown. Both use the identical method — only the value of d differs; if a scheme/answer uses 1.20 nm, it has taken the diameter for a radius.)

**L2 · Thought** This is the **hidden-calibration move**: nobody recorded the laser frequency, so the four calibration points must determine *both* A and ν̃_laser. Linearising the model (ν̃_scat = ν̃_laser − A/2r) turns two unknowns into slope + intercept. Two physical anchors then validate the fit independently: A ≈ 225 cm⁻¹ nm matches the known radial-breathing-mode relation for single-walled nanotubes (≈227/d), and λ_laser = 1064 nm is the Nd:YAG line — a real Raman laser. If your intercept landed at, say, 500 nm, refit before trusting A. Traps: forgetting d = 2r (halves A to ~112 — the diameter is what the physics uses); plotting raw 1/r without a model statement; quoting A without units (the mark scheme style point: "appropriate units" is written into the question).

---

## Q5 — Agarwood: the agarospirol synthesis (19 marks)

*Structural roadmap (all spiro compounds share one quaternary carbon joining a cyclohexane-derived left ring and a second ring):*

**Agarospirol (target)** = spiro[4.5]decane skeleton, C₁₅H₂₆O: a 6-membered ring spiro-fused to a 5-membered ring; the 6-ring has a C=C next to the spiro atom with a CH₃ on the spiro-adjacent sp² carbon, plus a second CH₃ on the carbon adjacent to the spiro atom on the other side; the 5-ring bears a –C(OH)(CH₃)₂ group two atoms from the spiro atom. SMILES: `CC1=CCCC(C)C12CC(C(O)(C)C)CC2` (formula-audited: C₁₅H₂₆O, rings 5+6 ✓).

### (a) Stereocentres in agarospirol (circle task)
**L1 · Answer** Three stereocentres:
1. **the spiro carbon** — the two paths around the 6-ring differ (one meets the C=C(CH₃), the other the CH–CH₃) *and* the two paths around the 5-ring differ (one reaches CH–C(OH)Me₂ in one step, the other in two) → four different substituents;
2. **the CH–CH₃ carbon of the 6-ring** (H, CH₃, and two non-equivalent ring paths);
3. **the CH carbon of the 5-ring bearing –C(OH)(CH₃)₂** (H, the carbinol substituent, and two non-equivalent ring paths).

Not stereocentres: the two sp² alkene carbons; the carbinol carbon C(OH)(CH₃)₂ (two identical methyls); all CH₂'s.

**L2 · Thought** Move: stereocentre inventory = "four different substituents" test applied atom by atom, with the **spiro rule**: a spiro atom qualifies iff *both* rings are unsymmetrically substituted — check each ring separately (if the 5-ring were unsubstituted cyclopentane, the two 5-ring paths would be identical and the spiro C would fail the test). The C(OH)(CH₃)₂ carbon is the classic trap: it *looks* chiral but carries two methyls. Natural agarospirol being "a single isomer" is the stem hinting the circles matter.

### (b) First part: A, B, C and intermediate D
**L1 · Answer**
- **A** = the bis-carboxylic acid from hydrolysing both nitriles: 2,2-bis(2-carboxyethyl)-3-methylcyclohexan-1-one — quaternary α-C bearing –CH₂CH₂COOH ×2, methyl on the carbon adjacent to it (SMILES `CC1CCCC(=O)C1(CCC(=O)O)CCC(=O)O`). Formula audit: C₁₃H₂₀O₅ ✓ (ketone O + 2 × CO₂H = 5 O; 6+1+3+3 = 13 C). (The substitution pattern — quaternary C2 with the two arms, methyl at C3 — is read from the scheme's drawing; a reader working from the text alone could misplace the methyl, so note its source.)
- **B** = the corresponding **dimethyl ester** (Fischer esterification, CH₃OH/acid): `CC1CCCC(=O)C1(CCC(=O)OC)CCC(=O)OC` (C₁₅H₂₄O₅).
- **C** = the **Dieckmann cyclisation** product — a spiro β-keto ester: the enolate of one ester's α-CH₂ attacks the other ester's carbonyl carbon, closing a **second six-membered ring** through the shared quaternary carbon; C = the spiro[5.5] β-keto ester (new ring: spiroC–CH₂–CH₂–C(=O)–CH(CO₂Me)–CH₂–; SMILES `O=C1CCCC(C)C12CCC(=O)C(C(=O)OC)C2`; audited: C₁₄H₂₀O₄, rings 6+6 ✓). (The two bracketed species shown in the paper are the enolate and the tetrahedral alkoxide intermediate before MeO⁻ leaves.)
- **D** = the **β-keto acid** from LiI demethylation of the methyl ester (I⁻ does SN2 on the O–CH₃: −CH₃I): `O=C1CCCC(C)C12CCC(=O)C(C(=O)O)C2` (C₁₃H₁₈O₄) — which then decarboxylates (−CO₂) through its six-membered cyclic transition state to the spiro dione `O=C1CCCC(C)C12CCC(=O)CC2` (C₁₂H₁₈O₂ ✓).

**L2 · Thought** Chain of triggers: ① "NaOH, heat" on a dinitrile + A's formula O₅ → both C≡N hydrolysed to COOH (audit: C≡N + 2 H₂O → COOH + NH₃, net +2O +2H per nitrile; SM C₁₃H₁₈N₂O → A C₁₃H₂₀O₅: +4O +4H −2N ✓ exactly matches double hydrolysis). ② "CH₃OH, acid" → Fischer. ③ "base … anion … cyclises" + the bracketed arrows → Dieckmann (intramolecular Claisen); the **only** enolate geometry that closes a strain-free ring is α-CH₂ of one arm onto the other arm's ester C=O → 6-membered ring sharing the quaternary C → spiro. ④ LiI/−CH₃I is the signature of **ester demethylation** (Krapcho logic, with decarboxylation held back to the next step); ⑤ −CO₂ from a β-keto acid → ketone. Each reagent pair is a named-reaction baton pass; the formula of A is the anchor that makes step ① a *deduction*, not a guess. Failure boundary: if A's formula had kept an N or shown fewer oxygens, partial hydrolysis would be indicated instead — always audit before drawing.

### (c) Second part: E, F⁻, G
**L1 · Answer** The Wittig/ketal sequence first: the dione + Ph₃P=CH₂ (1 equiv.) methylenates the **less hindered right-ring ketone** → exocyclic =CH₂ (`O=C1CCCC(C)C12CCC(=C)CC2`, C₁₃H₂₀O); then ethylene glycol/TsOH/reflux protects the **left-ring ketone** as a dioxolane ketal *and* acid-isomerises the exocyclic methylene into the ring (trisubstituted alkene, CH₃ on the ring sp² carbon). Call this ketal-alkene **P** (SMILES `CC1=CCC2(CC1)C(C)CCCC21OCCO1`, C₁₅H₂₄O₂ — ketal contributes 2 O).
- **E** (C₁₅H₂₄O₄) = ozonolysis (O₃/Me₂S, reductive work-up) of P: the right ring's C=C is cleaved, opening the 6-ring into **two carbonyl arms on the spiro atom**: –CH₂–CHO (from the =CH– side, 2 carbons) and –CH₂CH₂–C(=O)–CH₃ (from the =C(CH₃)– side, 4 carbons); the left-ring ketal is untouched (SMILES `CC(=O)CCC1(CC=O)C(C)CCCC12OCCO2`; audited: C₁₅H₂₄O₄ ✓, O = ketal(2) + CHO(1) + ketone(1) ✓).
- **F⁻** = the enolate formed by deprotonating the **CH₂ α to the ketone on the 3-oxobutyl arm** (the CH₂ between the spiro-side CH₂ and the C=O): `CC(=O)[CH-]CC1(CC=O)C(C)CCCC12OCCO2`.
- **G** (C₁₅H₂₂O₃) = intramolecular **aldol condensation**: F⁻ attacks the aldehyde carbon → 5-membered-ring β-hydroxy ketone → dehydration (−H₂O) to the conjugated enone: ring = spiroC–CH₂–C(COCH₃)=CH–CH₂– (i.e. a cyclopent-1-ene with the acetyl group on the alkene α-carbon), SMILES `CC(=O)C1=CCC2(C1)C(C)CCCC21OCCO1`. Audit: E − H₂O = C₁₅H₂₂O₃ ✓.
(H₂ (1 equiv.)/Pd then reduces only the enone C=C → the shown cyclopentane with the –COCH₃ substituent, `CC(=O)C1CCC2(C1)C(C)CCCC21OCCO1`, C₁₅H₂₄O₃; the ketal survives.)

**L2 · Thought** The decisive step is choosing *which* enolate cyclises onto *which* carbonyl. Enumerate honestly, then filter:
- ① enolate of the acetyl **CH₃** attacking the aldehyde → ring path runs through 7 atoms → **7-membered ring ✗** (ring-size filter);
- ② enolate of the aldehyde-arm α-CH₂ (between spiro C and CHO) attacking the **ketone** → a *5-membered* ring — passes the size filter — but the product would carry a **–CHO substituent** and a ring C(OH)(CH₃); after dehydration and H₂ that gives a cyclopentane bearing CHO + CH₃, which contradicts the **shown hydrogenation product** (single –COCH₃ substituent, no aldehyde) ✗;
- ③ enolate of the ketone-arm α-CH₂ (between the spiro-side CH₂ and C=O) attacking the **aldehyde** → **5-membered ring** with –COCH₃ as a substituent and –OH on the ex-aldehyde carbon ✓ — consistent with E's formula, G = E − H₂O, *and* the drawn downstream product.
So ring size alone narrows to two candidates (② vs ③); the **downstream structure** breaks the tie — that is why the L1 keeps the pruning reason in brackets. Dehydration then goes toward conjugation with the surviving ketone (enone), which is also why 1 equiv. H₂/Pd cleanly reduces only the C=C, leaving ketal and ketone untouched.

### (d) Final part: H, I, J, K, L⁺, M
**L1 · Answer** (starting from the hydrogenated spiro ketal ketone, `CC(=O)C1CCC2(C1)C(C)CCCC21OCCO1`)
- **H** (C₁₄H₂₂O₄) = **haloform-reaction carboxylic acid**: NaOH/Br₂ converts the methyl ketone –COCH₃ → –COOH (CHBr₃ leaves), ketal intact (base-stable): `O=C(O)C1CCC2(C1)C(C)CCCC21OCCO1`. Audit: 14 C (−1 C leaves in CHBr₃); O count = ketal(2) + COOH(2) = 4 ✓.
- **I** = **methyl ester** from diazomethane (CH₂N₂ methylates COOH → COOCH₃, −N₂): `COC(=O)C1CCC2(C1)C(C)CCCC21OCCO1`, C₁₅H₂₄O₄ ✓.
- **J** = **ketal hydrolysis** (HCl(aq)) restoring the left-ring **cyclohexanone**, ester untouched: `COC(=O)C1CCC2(C1)C(C)CCCC2=O`, C₁₃H₂₀O₃ ✓.
- **K** (C₁₄H₂₂O₂) = **Wittig methylenation** of that ketone: left-ring C=O → C=CH₂ (exocyclic methylene; the right-ring ester is inert to the ylide): `C=C1CCCC(C)C12CC(C(=O)OC)CC2`.
- **L⁺** = the **tertiary carbocation** from Markovnikov protonation of K's exocyclic methylene: H⁺ adds to the CH₂, placing the + on the ring carbon that bears the new CH₃ and sits adjacent to the spiro atom: `COC(=O)C1CCC2(C1)C(C)CCC[C+]2C`.
- **M** (C₁₄H₂₂O₂) = **deprotonation of L⁺ toward the ring**: loss of the β-H on the non-spiro side gives the trisubstituted endocyclic alkene — C=C(CH₃) between the former cation carbon and its non-spiro neighbour: `COC(=O)C1CCC2(C1)C(C)CCC=C2C`. K and M are isomers (C₁₄H₂₂O₂) ✓.
- Finally M + 2 CH₃Li then H₂O: the ester carbonyl takes two methyls → **–C(OH)(CH₃)₂** → **agarospirol**, `CC1=CCCC(C)C12CC(C(O)(C)C)CC2` (C₁₅H₂₆O — sesquiterpene alcohol audit ✓).

**L2 · Thought** Reading order matters: work **backwards from agarospirol** and **forwards from the reagents** until they meet. ① NaOH/Br₂ = haloform signature → acid; H's O₄ confirms the ketal survived (had it hydrolysed, O₃). ② CH₂N₂ = the mildest COOH → COOMe methylator (nothing else acidic enough is present: ketal silent). ③ HCl(aq) selectively hydrolyses the ketal (acetals are acid-labile; methyl esters need harsher forcing). ④ Wittig puts =CH₂ exactly where the ketone was — and note the whole point of the protection choreography (ketal on, haloform, esterify, ketal off) was to methylenate *this* ketone while the other carbonyl had been converted to the ester handle. ⑤ K → M under TsOH/reflux is a **cationic alkene walk**: protonate the less substituted end of =CH₂ (Markovnikov → tertiary cation L⁺ — the only cation consistent with both K and M), then deprotonate toward the ring interior to give the more substituted (trisubstituted) alkene; the alternative deprotonation back to the exocyclic methylene just returns K. ⑥ The target's C=C position (methyl on the sp² carbon next to the spiro atom) is the evidence that selects L⁺'s regiochemistry — this is the bracket-worthy "candidate pruning" kept inside L1. ⑦ 2 CH₃Li on an ester → tertiary alcohol (first equivalent gives a ketone after collapse, second adds; water work-up protonates) — the –C(OH)(CH₃)₂ of agarospirol drops out, closing the loop with the target.

---

## Q6 — Iodination of ketones: three kinetic regimes (15 marks)

*Mechanism: ketone A ⇌ enol B (steps 1/2, k₁/k₂), enol + I₂ → product C + HI (step 3, k₃). A = 3-methylbutan-2-one CH₃COCH(CH₃)₂; B = the less substituted enol CH₂=C(OH)CH(CH₃)₂; C = ICH₂COCH(CH₃)₂; D = the more substituted enol CH₃C(OH)=C(CH₃)₂; E = CH₃COC(CH₃)₂I. Given: k₂ = 8.3 s⁻¹, k₃ = 5.2 × 10⁵ mol⁻¹ dm³ s⁻¹; later k₄ = 2.9 × 10⁻⁶ s⁻¹, k₅ = 2.1 × 10⁻² s⁻¹, k₆ = 5.2 × 10⁵ mol⁻¹ dm³ s⁻¹.*

### (a) Species in the rate equation at high [I₂] (tick all)
**L1 · Answer** Tick **A only**. With step 1 rate-determining, only species *in or before* the RDS can appear; B, I₂, C, HI all act after it.

**L2 · Thought** Deciding criterion is printed in the stem: "any species involved in **or before** the rate-determining step." Once B forms it is consumed instantly, so [I₂] cannot influence the rate — this is the whole point of zero-order-in-I₂ kinetics that (b) then exploits.

### (b) Rate law and k₁ at high [I₂]
**L1 · Answer**
(i) RDS = step 1 → **rate = k₁[A]** (zero order in [I₂]).
(ii) The graph (rate vs [A]) is linear through the origin with slope = k₁:
gradient = (600 μmol dm⁻³ s⁻¹)/(14 mol dm⁻³) = 42.9 × 10⁻⁶ s⁻¹ ⇒ **k₁ = 4.3 × 10⁻⁵ s⁻¹** (mark scheme: 4.29 × 10⁻⁵ s⁻¹, accepted 4.08–4.50 × 10⁻⁵; the μmol → mol conversion, ×10⁻⁶, is the mark).

**L2 · Thought** Two checkpoints: the graph's linearity-through-origin *is itself evidence* for first order in A and zero in I₂ (curve would have meant otherwise — always let the shape argue the order before extracting constants); and the unit conversion μmol → mol is the classic silent slip (getting 42 s⁻¹ means you forgot it). Reading the extreme gridline (14, 600) minimises interpolation error; the scheme's tolerance band (4.08–4.50 × 10⁻⁵ s⁻¹) absorbs honest graph-reading spread.

### (c) [B] at equilibrium
**L1 · Answer** At equilibrium k₁[A] = k₂[B]:
$$[B] = \frac{k_1}{k_2}[A]$$

**L2 · Thought** One line — but note the stem *defines* K_eq = k₁/k₂, so this is a *deduce*, anchored to "rate forward = rate backward at equilibrium."

### (d) Rate law at low [I₂]
**L1 · Answer**
$$\text{rate} = k_3[B][I_2] = \frac{k_1 k_3}{k_2}[A][I_2]$$

**L2 · Thought** Pre-equilibrium skeleton: fast reversible step 1/2 holds B at its equilibrium population; slow step 3 drains it without disturbing the ratio. The rate must contain [I₂] here (step 3 is the bottleneck) — if your expression lost [I₂], you recycled (b)'s regime by mistake.

### (e) Rate law at intermediate [I₂]
**L1 · Answer** Using the given steady-state form for [B]:
$$\text{rate} = k_3[B][I_2] = \frac{k_1 k_3 [A][I_2]}{k_2 + k_3[I_2]}$$
Limiting-case check: k₃[I₂] ≫ k₂ → collapses to k₁[A] ✓ (regime b); k₃[I₂] ≪ k₂ → collapses to (k₁k₃/k₂)[A][I₂] ✓ (regime d).

**L2 · Thought** The given [B] = k₁[A]/(k₂ + k₃[I₂]) *is* the steady-state approximation (d[B]/dt = k₁[A] − k₂[B] − k₃[B][I₂] = 0) — worth deriving once in thought even though the stem gifts it, because the **limiting-case check** is your insurance: a derived law that fails to collapse to both known regimes is wrong, full stop. This three-regime arc (RDS switch as a reagent concentration moves the denominator's balance) is the transferable lesson of the whole question.

### (f) C vs E statement table (tick per row)
**L1 · Answer**

| Statement | Answer | Criterion |
|---|---|---|
| Larger rate constant for the first step | **C** | k₁ = 4.2 × 10⁻⁵ s⁻¹ > k₄ = 2.9 × 10⁻⁶ s⁻¹ |
| Major product at high [I₂] | **C** | rate_C = k₁[A] > rate_E = k₄[A]; the pathway whose enol *forms faster* wins (kinetic control) |
| Larger K_eq | **E** | K_C = k₁/k₂ = 5.1 × 10⁻⁶ ≪ K_E = k₄/k₅ = 1.4 × 10⁻⁴ — the more substituted enol D is thermodynamically preferred |
| Major product at low [I₂] | **E** | rate ∝ (k_enolisation/k_reverse)[A][I₂], i.e. ∝ K_eq; K_E > K_C → E (thermodynamic control) |

**L2 · Thought** This table *is* the kinetic-vs-thermodynamic product-control lesson. High [I₂]: every enol molecule is trapped instantly, so product ratio = ratio of enol *formation* rates → the kinetic enol (B, less substituted, forms faster: k₁ > k₄) gives C. Low [I₂]: enolisation equilibrates before iodination, so product ratio tracks enol *stability* (K_eq) → the more substituted enol D gives E. Note the beautiful internal consistency: k₁/k₂ ≪ k₄/k₅ mainly because k₂ ≫ k₅ (the less stable enol reverts faster) — exactly what alkene-stability chemistry predicts. Boundary: this analysis needs k₃ = k₆ (given: both 5.2 × 10⁵); if the trapping rates differed, low-[I₂] selectivity would blend formation and trapping terms.

### (g) [I₂] for equal rates of C and E formation
**L1 · Answer** Set the two intermediate-regime rates equal (the general form from (e) applies to both pathways):
$$\frac{k_1 k_3 [A][I_2]}{k_2 + k_3[I_2]} = \frac{k_4 k_6 [A][I_2]}{k_5 + k_6[I_2]}$$
Cancel [A][I₂] (≠ 0) and use k₃ = k₆ = 5.2 × 10⁵:
$$k_1(k_5 + k_6[I_2]) = k_4(k_2 + k_3[I_2])$$
$$[I_2] = \frac{k_4 k_2 - k_1 k_5}{k_1 k_6 - k_4 k_3} = \frac{(2.9\times10^{-6})(8.3) - (4.3\times10^{-5})(2.1\times10^{-2})}{(4.3\times10^{-5})(5.2\times10^{5}) - (2.9\times10^{-6})(5.2\times10^{5})}$$
(using (b)'s k₁ = 4.3 × 10⁻⁵ s⁻¹; with 4.2 × 10⁻⁵ the answer is identical to 2 s.f. — both lie inside the scheme's graph-reading tolerance)
$$= \frac{2.41\times10^{-5} - 8.8\times10^{-7}}{21.8 - 1.51} = \frac{2.32\times10^{-5}}{20.3} = \mathbf{1.1\times10^{-6}\ mol\ dm^{-3}}$$
Dimensional audit: numerator s⁻¹·s⁻¹, denominator s⁻¹·(mol⁻¹ dm³ s⁻¹) → mol dm⁻³ ✓.

**L2 · Thought** Which regime? The stem's hint says use the intermediate form — and self-consistently the answer (10⁻⁶ mol dm⁻³) sits where k₃[I₂] ≈ 0.6 s⁻¹ is comparable with k₂ = 8.3 s⁻¹ and k₅ = 0.021 s⁻¹: genuinely intermediate for the E pathway, comfortably high-ish for the C pathway — no contradiction, the equality equation only needed both general laws. Two algebraic hygiene points: cancelling [A][I₂] first (it can never be zero in the question's sense) avoids dragging symbols; and k₃ = k₆ lets the k₆[I₂] and k₃[I₂] terms combine cleanly — always scan the data table for equal constants before grinding. Sanity: the crossing exists because C wins at high [I₂] (k₁ > k₄) and E wins at low [I₂] (K_E > K_C), so a crossing at *some* intermediate [I₂] is guaranteed — if your algebra returned a negative concentration, a sign slipped.

---

*End of Paper 1 (2025). Papers 2–23 (2024–2003) follow, one section per paper.*

---

# Paper 2 — 2024 UKChO Round 1 (56th IChO selection)

*5 questions, 82 marks, 2 h → ≈ 1.45 min per mark. Marks: Q1 = 8, Q2 = 15, Q3 = 20, Q4 = 24, Q5 = 15.*

## Q1 — Bronze: configurations, density and the fcc cell (8 marks)

### (a) Electronic configuration of a silver atom (tick)
**L1 · Answer** Tick **[Kr]4d¹⁰5s¹**.
**L2 · Thought** Ag sits below Cu in group 11; like Cu (3d¹⁰4s¹) it takes the filled-d¹⁰ anomaly, not d⁹s². The [Ar] options fail because Ag is period 5 (core = Kr).

### (b) Electronic configuration of Cu²⁺ (tick)
**L1 · Answer** Tick **1s²2s²2p⁶3s²3p⁶3d⁹** ([Ar]3d⁹).
**L2 · Thought** Transition-metal cations empty the **4s before the 3d** (once charged, 3d drops below 4s in energy): Cu [Ar]3d¹⁰4s¹ → Cu²⁺ [Ar]3d⁹. The classic trap is 3d¹⁰4s¹ → remove the wrong electron, or "4s²3d⁹" reordering without removal.

### (c) Volume of the trophy
**L1 · Answer** V = m/ρ = 4600 g / 10.5 g cm⁻³ = **438 cm³** (3 s.f.).
**L2 · Thought** One-line density drill; the "coated with gold" is a distractor — the stem says *assume solid silver*.

### (d) Percentage of tin in bronze of density 7.85 g cm⁻³
**L1 · Answer** Rearrange the given model: ρ·V·Nₐ/4 = M(Cu) + y(M(Sn) − M(Cu))
$$\frac{7.85 \times 5.93\times10^{-23} \times 6.022\times10^{23}}{4} = 70.08\ \text{g mol}^{-1}$$
$$y = \frac{70.08 - 63.55}{118.71 - 63.55} = 0.118 \;\Rightarrow\; \mathbf{11.8\ mol\%\ (atomic\ \%)\ Sn}$$
i.e. y is a **mole/atomic fraction** by the model's construction (the mark scheme insists on the percentage form: "do not accept 0.118"); if a *mass* percentage were wanted instead, it would be 0.118 × 118.71/70.08 = 20.1 mass%.
**L2 · Thought** The model treats the 4-atom unit cell's *average* molar mass as a linear interpolation — so y is an **atomic fraction**, and "percentage of tin" here means 11.8 at%. Reading which percentage is wanted is part of the wording audit. Guard digits: carry 70.08, round only at the end.

### (e) Side of the copper unit cell
**L1 · Answer** fcc: face diagonal = 4r = a√2 → a = 4r/√2 = 2√2 r = 2√2 × 128 pm = 362 pm = **3.62 × 10⁻⁸ cm**.
**L2 · Thought** Geometry first, units second: the contact direction in fcc is the *face* diagonal (not body diagonal — that is bcc). Convert pm → cm (1 pm = 10⁻¹⁰ cm) *before* cubing.

### (f) Volume of the unit cell
**L1 · Answer** V = a³ = (3.62 × 10⁻⁸)³ = **4.75 × 10⁻²³ cm³**.
**L2 · Thought** Carry the unrounded a (362.04 pm) through: (3.6204)³ = 47.45 → 4.745 × 10⁻²³; rounding a to 3 s.f. first would still give 4.74 ✓. Sanity anchor from skeleton 7.4: cell edge ~10⁻¹⁰ m ✓, volume ~10⁻²⁹ m³ = 10⁻²³ cm³ ✓.

### (g) Density of copper
**L1 · Answer** fcc has 4 atoms per cell (8 × ⅛ + 6 × ½):
$$\rho = \frac{4 \times 63.55}{6.022\times10^{23} \times 4.745\times10^{-23}} = \mathbf{8.89\ g\ cm^{-3}}$$
**L2 · Thought** Count shares *before* computing (skeleton 7.4 step ③). Plausibility anchor: real ρ(Cu) = 8.96 g cm⁻³ — 1 % off, consistent with the idealised hard-sphere cell. If you got ~4.4 or ~17.8, you used 2 or 8 atoms per cell — the share-count is where fcc answers die.

---

## Q2 — Iodate salts and the salesite mineral (15 marks)

### (a) Oxidation state of I in IO₃⁻
**L1 · Answer** x + 3(−2) = −1 → **+5**.
**L2 · Thought** One line; the trap is forgetting the ion's charge and solving x − 6 = 0.

### (b) Dot-and-cross of the iodate ion
**L1 · Answer** Electron budget: 7 + 3×6 + 1 = 26 e⁻. Draw three I–O single bonds (one dot–cross pair each), **three lone pairs on every O**, and **one lone pair on I**; square brackets with the −1 charge. (Formal charges: each O −1, I +2; resonance forms with I=O double bonds are acceptable alternatives, but the pyramidal single-bond form is what (c) refers to.)
**L2 · Thought** I is period 5 — hypervalence is *allowed* but not *required*; the 26-electron count closes with single bonds + an I lone pair, which is also the form that makes (c)'s VSEPR question coherent (you cannot ask for the O–I–O angle's deviation from 109.5° without a stereochemically active lone pair).

### (c) O–I–O bond angle (tick)
**L1 · Answer** Tick **< 109.5°**.
**L2 · Thought** Four domains around I (3 bonds + 1 lone pair), lone pair repels more → angles squeezed below tetrahedral, exactly the NH₃ precedent (~107°). Do not over-think period-5 size: VSEPR ordering is domain-count logic, not atom-size logic.

### (d) Mass of KIO₃ with the same iodine as 130 mg KI
**L1 · Answer** Equal moles of I (one I per formula unit in both):
$$m(KIO_3) = 130\ \text{mg} \times \frac{M(KIO_3)}{M(KI)} = 130 \times \frac{214.0}{166.0} = \mathbf{168\ mg}$$
**L2 · Thought** The conservation anchor is *moles of iodine atoms*, not mass of salt — a one-line sanity check: KIO₃ is heavier per I, so the answer must exceed 130 mg ✓. 167.6 mg rounds to 168 mg (3 s.f.).

### (e)(i) Iodate + iodide in acid
**L1 · Answer**
$$IO_3^- + 5\,I^- + 6\,H^+ \longrightarrow 3\,I_2 + 3\,H_2O$$
Audit: I 6 = 6; O 3 = 3; H 6 = 6; charge −1−5+6 = 0 = 0 ✓.
**L2 · Thought** Balance by oxidation-state audit: I(+5) gains 5 e⁻ → I(0); I(−1) loses 1 e⁻ → I(0); so 5 I⁻ per IO₃⁻ — then close O and H with water and acid. This is the **comproportionation** (the reverse of disproportionation) that anchors the whole salesite analysis below.

### (e)(ii) Reaction type (tick)
**L1 · Answer** Tick **redox** only.
**L2 · Thought** Trap: "disproportionation" is listed — but here two oxidation states of the *same* element converge to one (+5 and −1 → 0), which is comproportionation, the opposite direction. No C=C (elimination/polymerisation), no aromatic ring (electrophilic substitution).

### (f) Thiosulfate + iodine
**L1 · Answer**
$$2\,S_2O_3^{2-} + I_2 \longrightarrow S_4O_6^{2-} + 2\,I^-$$
Audit: S 4 = 4; O 6 = 6; charge −4 = −2−2 ✓.
**L2 · Thought** The analytical workhorse equation — memorise the tetrathionate product (S₄O₆²⁻), not sulfate. Stoichiometry 2 : 1 thiosulfate : iodine drives every titration calculation below.

### (g) Thiosulfate volume for the salesite aliquot
**L1 · Answer** (M(mineral) = 255.46 g mol⁻¹ is used here; its provenance: the mineral is salesite and the cation/anion mass budget of part (k) — 255.46 = 63.55 + 17.01 + 174.90 for Cu²⁺ + OH⁻ + IO₃⁻ — is what fixes it; strictly, (g) borrows (k)'s conclusion, so write the linkage when presenting)
n(mineral) = 1.000/255.46 = 3.914 × 10⁻³ mol in 100.0 cm³ stock → aliquot (10.00 cm³): n(IO₃⁻) = 3.914 × 10⁻⁴ mol (1 IO₃⁻ per formula unit)
n(I₂) = 3 × 3.914 × 10⁻⁴ = 1.174 × 10⁻³ mol (equation (e)(i))
n(S₂O₃²⁻) = 2 × 1.174 × 10⁻³ = 2.349 × 10⁻³ mol
$$V = \frac{2.349\times10^{-3}}{0.1000} = \mathbf{23.49\ cm^3}$$
**L2 · Thought** Chain-map before numbers: mineral → IO₃⁻ (×1) → I₂ (×3) → S₂O₃²⁻ (×2), with the **10-fold dilution** as the silent step (the single most common slip — the printed fallback "use 15.67 cm³" is the consequential-marking parachute for students who break the chain here). Keep 4 s.f. until the final rounding.

### (h) Iodine from the metal ion
**L1 · Answer** Actual I₂ = ½ × 0.1000 × 27.40 × 10⁻³ = 1.370 × 10⁻³ mol.
Extra I₂ from Mⁿ⁺ = 1.370 × 10⁻³ − 1.174 × 10⁻³ = 1.956 × 10⁻⁴ mol.
Per mole of Mⁿ⁺ (= moles of mineral in the aliquot, 3.914 × 10⁻⁴):
$$\frac{1.956\times10^{-4}}{3.914\times10^{-4}} = \mathbf{0.50\ mol\ I_2\ per\ mol\ M^{n+}}$$
**L2 · Thought** The "actual − expected" difference isolates the metal's contribution — always subtract in moles of I₂, not in titrant volume (though with the same titrant it is equivalent). 0.50 mol I₂ per mol M means each M accepts exactly **1 electron** (2 I⁻ → I₂ + 2 e⁻; 0.5 I₂ = 1 e⁻): Mⁿ⁺ + I⁻ → M⁽ⁿ⁻¹⁾⁺ + ½ I₂. This electron count is the key that (i) and (k) turn.

### (i) Oxidation state after reaction with iodide (tick)
**L1 · Answer** Tick **+(n−1)**.
**L2 · Thought** Directly from (h)'s 1 e⁻ per ion — iodide is oxidised, so the metal must be *reduced* by one unit. If your (h) had been 1.0 mol I₂, the tick would be +(n−2): consequential marking rewards keeping the symbolic link visible.

### (j) Anions excluded by "no effervescence"
**L1 · Answer** Any **two** of the gas-evolving anions: **CO₃²⁻ / HCO₃⁻** (→ CO₂↑), **SO₃²⁻ / HSO₃⁻** (→ SO₂↑), **NO₂⁻** (→ NO/NO₂↑ from unstable HNO₂). E.g. **CO₃²⁻ and SO₃²⁻**: CO₃²⁻ + 2 H⁺ → CO₂↑ + H₂O; SO₃²⁻ + 2 H⁺ → SO₂↑ + H₂O.
**L2 · Thought** The observation is *silence* — so the excluded anions are exactly those that *would* effervesce with dilute acid (gas-forming protonations). This is an open "give two" item, not a list pick — name the common carbonate/sulfite pair. (Mark scheme: two of HCO₃⁻/CO₃²⁻/HSO₃⁻/SO₃²⁻/NO₂⁻ expected; H⁻ is formally creditable — H⁻ + H⁺ → H₂↑ — but the scheme itself notes hydrides react with water and occur in no natural mineral, so in a *mineral* context prefer the oxyanions.)

### (k) Identify Mⁿ⁺ and Zᵐ⁻
**L1 · Answer** Mass budget: M(M) + M(Z) = 255.46 − M(IO₃) = 255.46 − 174.90 = 80.56 g mol⁻¹.
Candidates from the list: only **Cu²⁺ (63.55) + OH⁻ (17.01) = 80.56** fits → **Mⁿ⁺ = Cu²⁺, Zᵐ⁻ = OH⁻**, mineral = Cu(IO₃)(OH) (this is indeed the real mineral salesite).
Consistency checks assembled: Cu²⁺ + 2 I⁻ → CuI(s) + ½ I₂ gives 0.5 mol I₂ per mol Cu ✓ (h, i); OH⁻ dissolves silently in HNO₃ ✓ (j); charges balance 1 : 1 : 1 with IO₃⁻ ✓.
**L2 · Thought** This is multi-constraint pruning, solved by starting from the **hardest constraint** (the mass budget 80.56 — only one list pair fits) and then *verifying* the soft ones (redox stoichiometry, silence with acid). Reversing the order (guessing Cu²⁺ from the iodide reaction first) also works but leaves the mass check as the required confirmation — either way, write the cross-checks explicitly: they are the marking anchors, and they catch contradictions that a single-route guess would miss.

---

## Q3 — Fuel-producing bacteria: ring strain and enolate chemistry (20 marks)

### (a) Molecular formula of cyclopropane
**L1 · Answer** **C₃H₆**.
**L2 · Thought** DBE budget: one ring, no π bonds → CₙH₂ₙ. Count the skeletal drawing: 3 vertices, each CH₂.

### (b)(i) Combustion of cyclopropane
**L1 · Answer**
$$2\,C_3H_6 + 9\,O_2 \longrightarrow 6\,CO_2 + 6\,H_2O$$
**L2 · Thought** "Combustion" → O₂ included, products CO₂ + H₂O (wording audit, as in 2025 Q1). Integer coefficients preferred for the final equation; the per-mole form C₃H₆ + 4.5 O₂ → … is what (ii) actually uses.

### (b)(ii) Enthalpy of formation of cyclopropane
**L1 · Answer** Hess cycle on C₃H₆ + 4.5 O₂ → 3 CO₂ + 3 H₂O, ΔcH = −2091 kJ mol⁻¹:
$$\Delta_fH(C_3H_6) = [3(-393.5) + 3(-285.8)] - (-2091) = -2037.9 + 2091 = \mathbf{+53.1\ kJ\ mol^{-1}}$$
(elements in standard states have ΔfH° = 0; ΔfH°(CO) is a distractor again.)
**L2 · Thought** Sign check is built into the physics: cyclopropane is *strained*, so its formation enthalpy should be **endothermic (positive)** — a negative result here flags an inverted Hess cycle. Same data-audit discipline as Paper 1 Q1(e): the CO enthalpy is bait for an incomplete-combustion equation.

### (b)(iii) Combustion enthalpy per mole of carbon — cyclopropane
**L1 · Answer** ΔcH per C = −2091/3 = **−697.0 kJ mol⁻¹ (per mole of C)**. (An enthalpy *of combustion* is negative — the mark scheme refuses a bare positive value; "releases 697.0 kJ" is the magnitude statement.)

### (b)(iv) Per mole of carbon — cyclohexane
**L1 · Answer** ΔcH per C = −3951/6 = **−658.5 kJ mol⁻¹ (per mole of C)**.
**L2 · Thought** (iii)+(iv) are the point of the question: per carbon, cyclopropane releases 697.0 − 658.5 = 38.5 kJ mol⁻¹ *more* than strain-free cyclohexane → ring strain ≈ 3 × 38.5 = **115.5 kJ mol⁻¹ per cyclopropane ring** — matching the textbook value (~115 kJ mol⁻¹). Two disciplines here: keep the **negative sign** on the ΔcH values (enthalpy of combustion is a signed quantity; the mark scheme penalises a positive quote), and normalise "per mole of carbon" before comparing — the only fair comparison between C₃ and C₆ fuels, transferable to any per-bond / per-gram energy question.

### (c) Resonance form of the enolate
**L1 · Answer** The **carbanion** form: ⁻CH₂–C(=O)–CH₃ (charge on the α-carbon), partner of the given oxanion form CH₂=C(O⁻)–CH₃. The two are joined by the resonance double-headed arrow ↔.
**L2 · Thought** Arrow semantics: one curly arrow from C=O π bond onto O (gives the carbanion), the reverse for the oxanion. The carbanion form explains why α-carbon is the nucleophilic atom in (d) — even though the oxanion form is the major contributor, reactions at carbon dominate (C-alkylation) with alkyl halides.

### (d) Enolate + iodomethane (tick statement)
**L1 · Answer** Tick: **the enolate acts as a nucleophile; the iodomethane acts as an electrophile.**
**L2 · Thought** Polarity analysis: the enolate's α-C is electron-rich (δ−), iodomethane's C is δ+ (I pulls). It is an SN2 alkylation — no electron *transfer*, so no redox roles; no proton transfer, so no acid/base roles. The tick list is designed to catch students who reach for "reducing/oxidising agent" for any anion.

### (e) Compound A (enolate + carbonyl)
**L1 · Answer** The **aldol (β-hydroxy ketone)**: 4-hydroxy-4-methylpentan-2-one, (CH₃)₂C(OH)–CH₂–CO–CH₃, SMILES `CC(=O)CC(C)(C)O` — C₆H₁₂O₂ ✓ (acetone enolate adds to acetone's carbonyl; the alkoxide is protonated on work-up). The drawn final product (mesityl oxide, (CH₃)₂C=CH–CO–CH₃) is A minus H₂O.
**L2 · Thought** Formula audit: 2 × acetone (C₃H₆O) = C₆H₁₂O₂ ✓ addition, nothing lost — so A must be the *addition* intermediate (aldol), not the condensation product (which would be C₆H₁₀O). Naming the mechanism (aldol addition → dehydration) also tells you the final enone's geometry.

### (f)(i) Syntin scheme: B–E
**L1 · Answer**
- **B** = 5-chloropentan-2-one, CH₃–CO–CH₂CH₂CH₂–Cl, `CC(=O)CCCCl` (C₅H₉ClO ✓; HCl substitutes the –OH of 5-hydroxypentan-2-one).
- **C** = **cyclopropyl methyl ketone** (acetylcyclopropane), CH₃–CO–C₃H₅, `CC(=O)C1CC1` (C₅H₈O ✓): K₂CO₃ forms the enolate at the chain-side α-CH₂, which does an intramolecular SN2 on the terminal CH₂–Cl — a 3-exo-tet closure to the cyclopropane.
- **D** = the **aldol self-condensation dimer**: 1,3-dicyclopropyl-3-methylprop-2-en-1-one, cPr–C(=O)–CH=C(CH₃)–cPr, `O=C(C=C(C)C1CC1)C1CC1` (2 × C₅H₈O − H₂O = C₁₀H₁₄O ✓): the methyl-side enolate of one molecule attacks the carbonyl of another, then dehydrates to the α,β-unsaturated ketone. Al(OC(CH₃)₃)₃ is the Lewis-acidic aldol catalyst.
- **E** = the **hydrazone of D**, cPr–C(=N–NH₂)–CH=C(CH₃)–cPr, `NN=C(C=C(C)C1CC1)C1CC1` (D + H₂NNH₂ − H₂O: C₁₀H₁₄O + N₂H₄ − H₂O = C₁₀H₁₆N₂ ✓).
- Step 5 reagent: **strong base, heat** (Kishner cyclopropanation): the α,β-unsaturated hydrazone cyclises to a pyrazoline which extrudes N₂, closing the third cyclopropane across the former C=C → syntin = 1-methyl-1,2-dicyclopropylcyclopropane (C₁₀H₁₆ ✓ = E − N₂), `CC1(C2CC2)C(C2CC2)C1`.
**L2 · Thought** The formula audit drives every step: C₅H₈O (B → C) demands −HCl, i.e. C–C bond formation by deprotonation–alkylation; C₁₀H₁₄O (C → D) = exactly 2 C − H₂O, the aldol signature; C₁₀H₁₆N₂ (D → E) = +N₂H₂, the hydrazone signature; and "E + reagent → syntin + N₂" is the Wolff/Kishner-family signature — here the Kishner *cyclopropanation* variant (enone hydrazone → pyrazoline → cyclopropane + N₂), which is why the scheme feeds an α,β-unsaturated hydrazone rather than a saturated one. Note the carbon-skeleton bookkeeping: the two cyclopropyls and the methyl of syntin all trace back to two molecules of cyclopropyl methyl ketone (2 × cPr–CO–CH₃ provides 2 cPr + 2 CH₃; one CH₃ becomes the central ring's CH₂ after Kishner, the other stays as the ring methyl).

### (f)(ii) Steps involving enolate chemistry (tick)
**L1 · Answer** **Steps 2 and 3.**
**L2 · Thought** Step 2 = enolate α-alkylation; step 3 = enolate aldol. Step 1 (OH → Cl substitution), step 4 (hydrazone condensation at the carbonyl O–N level), step 5 (pyrazoline thermolysis) do not pass through an α-carbanion/enolate. Definition-first ticking: "enolate chemistry" = chemistry of the α-deprotonated carbonyl, not "has a carbonyl somewhere".

### (g) Reaction type of enzyme 2 (tick)
**L1 · Answer** **Reduction** (β-keto thioester → β-hydroxy thioester: C=O → CH–OH).
**L2 · Thought** Bond audit: a C=O becomes CH–OH — gain of H (hydride from NADPH in vivo). Not isomerisation (O position changes), not hydrolysis (thioester intact ✓ — check the S∼ survives, which it does in the drawing).

### (h) Products X and Y of enzyme 3
**L1 · Answer** Malonyl-S-enzyme (HOOC–CH₂–CO–S∼) + acetyl-S-enzyme (CH₃–CO–S∼) → acetoacetyl-S-enzyme (CH₃–CO–CH₂–CO–S∼) + **X = CO₂** + **Y = HS-enzyme (HS∼, the free enzyme thiol)**.
**L2 · Thought** This is the Claisen/decarboxylative-condensation logic of fatty-acid/polyketide biosynthesis: the malonyl unit's carboxyl is the leaving handle (decarboxylation drives the condensation), and the acetyl's thioester is hydrolysed off as the free thiol. Atom audit: left C₅H?O… — simpler: the product C₄ skeleton (CH₃COCH₂CO–S) = acetyl (C₂) + malonyl (C₃) − CO₂ ✓; the second enzyme's sulfur must leave as HS∼ ✓ (it reappears as the free enzyme for the next cycle).

### (i) Enzyme order for fuelomycin A's first sequence
**L1 · Answer** malonyl-S + acetyl-S →(3)→(2)→(4)→(1)→ 2-methylcyclopropanecarbonyl-S:
1. **enzyme 3**: condensation + decarboxylation → acetoacetyl-S (CH₃COCH₂CO–S∼);
2. **enzyme 2**: reduction of the β-ketone → 3-hydroxybutyryl-S (CH₃CH(OH)CH₂CO–S∼);
3. **enzyme 4**: elimination (dehydration) → but-2-enoyl-S (CH₃CH=CHCO–S∼);
4. **enzyme 1**: cyclopropanation across the C=C → 2-methylcyclopropanecarbonyl-S∼ (the drawn product).
**L2 · Thought** Each enzyme is used exactly once, so this is an ordering puzzle solved by *substrate matching*: only enzyme 3 accepts the given pair (it needs the malonyl + acetyl thioesters); only then does a β-keto exist for enzyme 2 to reduce; the OH is needed before enzyme 4 can eliminate it; the C=C is needed before enzyme 1 can cyclopropanate it. Working backwards from the product (cyclopropane ⇒ enzyme 1 last) and forwards from the substrates (enzyme 3 first) meets in the middle — same bidirectional strategy as synthesis schemes (cf. 2025 Q5(d)).

---

## Q4 — Gadopiclenol: ligand synthesis and relaxation analysis (24 marks)

### (a) Compounds A–D
**L1 · Answer**
- **A** = 2-bromopentanedioyl dichloride, ClOC–CH₂CH₂–CHBr–COCl, `O=C(Cl)CCC(Br)C(=O)Cl` (C₅H₅BrCl₂O₂ ✓; SOCl₂ converts both COOH → COCl).
- **B** = diethyl 2-bromopentanedioate, EtO₂C–CH₂CH₂–CHBr–CO₂Et, `CCOC(=O)CCC(Br)C(=O)OCC` (acid chlorides + ethanol → diester).
- **C** = [pyridine-2,6-diyl]dimethanol (2,6-bis(hydroxymethyl)pyridine), `OCc1cccc(CO)n1` (C₇H₉NO₂ ✓; NaBH₄ reduces both ring-flanked COOH → CH₂OH).
- **D** = 2,6-bis(bromomethyl)pyridine, `BrCc1cccc(CBr)n1` (C₇H₇Br₂N ✓; PBr₃ converts both CH₂OH → CH₂Br).
**L2 · Thought** Formula audit chain: A's printed formula confirms *both* acids became acid chlorides (2 Cl, Br retained); C₇H₉NO₂ vs the diacid C₇H₅NO₄ means +4 H − 2 O = two COOH → CH₂OH (each CH₂OH carries only one O — the classic miscount is to expect NO₃); D's C₇H₇Br₂N then forces the dibromide. (Note for context: NaBH₄ reducing a carboxylic acid is unusual — LiAlH₄ is the textbook choice — but the printed formula forces the diol; answer the formula, not the habit.) D's two CH₂Br groups are the two electrophilic hooks used in the macrocyclisation below.

### (b) Stereocentres on H (circle task)
**L1 · Answer** Circle the **three arm carbons N–CH(COOH)–CH₂CH₂–COOH** (one on each of the three macrocycle nitrogens). Each is bonded to four different groups (N, H, COOH, CH₂CH₂COOH).
Not stereocentres: all CH₂'s, the pyridine carbons, the carboxyl carbons.
**L2 · Thought** Same inventory rule as 2025 Q5(a): apply the "four different substituents" test atom by atom; CH₂ and sp² atoms are eliminated before the interesting ones are discussed. Three chiral arms is also chemically sensible — gadopiclenol is used as a single stereoisomer set derived from a chiral pool… here from the bromodiester's stereocentre (the CHBr of B is where each arm's CH comes from: the stereocentre is *installed* at B and *transferred* through the alkylation).

### (c) Compounds E–G
**L1 · Answer**
- **E** = N,N′,N′′-tris(tosyl)diethylenetriamine, TsNH–CH₂CH₂–N(Ts)–CH₂CH₂–NHTs (C₂₅H₃₁N₃O₆S₃ ✓ = DETA + 3 TsCl − 3 HCl; SMILES `Cc1ccc(S(=O)(=O)NCCN(S(=O)(=O)c2ccc(C)cc2)CCNS(=O)(=O)c2ccc(C)cc2)cc1`).
- **F** = the **tris-tosyl macrocycle**: E's two terminal sulfonamide N's each alkylate one CH₂Br of D (double SN2, K₂CO₃ as base), closing the 12-membered pyridine-containing macrocycle (pyclen core) with all three N's still tosyl-protected.
- **G** = the **hexa-ethyl-ester ligand**: after conc. H₂SO₄/NaOH detosylation (the drawn free pyclen macrocycle, `C1CNCCNCc2cccc(n2)CN1`), the three macrocyclic NH's are alkylated by B at its CHBr carbon → each N bears a –CH(CO₂Et)–CH₂CH₂–CO₂Et arm (3 arms, 6 esters).
(Hydrolysis of G's six esters (NaOH then HCl) gives **H**, the hexacarboxylic acid drawn.)
**L2 · Thought** The tosyl group is doing silent work: it acidifies the sulfonamide N–H so K₂CO₃ (a *mild* base) can deprotonate it for the double alkylation, and it caps the central N against over-alkylation — recognising "Ts = protecting/activating group for amines" is the transferable signal. The macrocycle forms by a 1 : 1 E : D double SN2 (two hooks, two nucleophiles — high dilution logic, no polymer). In G→B's role: B's CHBr is the single electrophilic carbon (α-bromo esters are SN2-reactive), so all three arms install at the same position, which is what guarantees the three identical stereocentres of (b).

### (d) Mass of gadolinium per dose
**L1 · Answer** M(gadopiclenol, C₃₅H₅₄GdN₇O₁₅) = 35(12.011) + 54(1.008) + 157.25 + 7(14.007) + 15(15.999) = 970.10 g mol⁻¹.
m(gadopiclenol) = 6.00 × 10⁻³ dm³ × 485.05 g dm⁻³ = 2.910 g
$$m(Gd) = 2.910 \times \frac{157.25}{970.10} = 0.4717\ \text{g} = \mathbf{472\ mg}$$
**L2 · Thought** Two-step mass-fraction drill: solution volume × concentration → agent mass; agent mass × (M(Gd)/M(agent)) → element mass. The volume unit trap: cm³ = 10⁻³ dm³ must be converted before multiplying by g dm⁻³.

### (e) Type of electromagnetic radiation (tick)
**L1 · Answer** **Radiowave.**
**L2 · Thought** NMR/MRI flips nuclear spins in a tesla-scale field: ΔE = hν with ν in the 10–1000 MHz region → radiofrequency. Every higher-energy option (microwave upward) is orders of magnitude too energetic for nuclear Zeeman splitting.

### (f) Net magnetisation at t = 3τ
**L1 · Answer** M = M₀(1 − e^(−3τ/τ)) = M₀(1 − e⁻³) = M₀(1 − 0.0498) = **95.0 % of M₀** (three sig. figs., as the calculation justifies).
**L2 · Thought** Direct substitution with the exponent computed *before* subtraction (premature rounding of e⁻³ = 0.0498 to "≈0.05" still gives 95.0 % ✓, but carry 4 digits anyway). Physical reading: after 3 time constants the system is ~95 % recovered — the classic "3τ ≈ fully relaxed" rule of thumb this question is quietly justifying.

### (g) Molar fraction χ
**L1 · Answer** Per dm³ of tissue: n(gadopiclenol) = 0.0500 mol; n(H₂O) = 1000 g / 18.015 g mol⁻¹ = 55.51 mol.
$$\chi = \frac{0.0500}{55.51} = \mathbf{9.01\times10^{-4}}$$
**L2 · Thought** The hidden step is converting water *density* (kg dm⁻³) into *molar concentration* (mol dm⁻³) — the two n's in χ must both be per the same volume. (The provided fallback χ = 0.00100 confirms the intended magnitude.)

### (h) Field-independent relaxation time
**L1 · Answer** With τ = τc + k/B² (k = the proportionality constant of τe):
$$k = \frac{\tau_1 - \tau_2}{B_1^{-2} - B_2^{-2}} \;\Rightarrow\; \tau_c = \tau_1 - \frac{k}{B_1^2} = \frac{\tau_2 B_2^2 - \tau_1 B_1^2}{B_2^2 - B_1^2}$$
**L2 · Thought** Two-unknowns-two-equations elimination: write both field conditions, subtract to kill τc, solve k, back-substitute. Symbol discipline (no numbers given) is exactly what skeleton 7.5 trains: keep symbols to the end, check limits — if B₂ → ∞, τc → τ₂ ✓ (infinite field kills τe, leaving τc).

### (i) Linearised Arrhenius form
**L1 · Answer** τc = 1/(qχ rc) and rc = A T e^(−ΔH/RT) ⇒ τc = e^(ΔH/RT)/(qχ A T).
Multiply by T and take logs:
$$\ln(\tau_c\,T) = \frac{\Delta H}{R}\cdot\frac{1}{T} - \ln(Aq\chi)$$
So **y = ln(τc T), a = ΔH/R, b = −ln(Aqχ)**.
**L2 · Thought** The 1/T factor inside rc is what forces the "multiply by T first" move — a naive ln(τc) vs 1/T plot is not linear here. Declaring the rearrangement target (y = a/T + b) before manipulating is the skeleton-7.5 discipline: it tells you exactly what to isolate.

### (j) Value of Aqχ
**L1 · Answer** Two points: y₁ = ln(4.775 × 10⁻⁴ × 275) = −2.0302; y₂ = ln(3.326 × 10⁻⁴ × 280) = −2.3738.
$$a = \frac{y_2 - y_1}{1/280 - 1/275} = \frac{-0.3436}{-6.494\times10^{-5}} = 5292\ \text{K} \;(= \Delta H/R)$$
$$b = y_1 - a/275 = -2.0302 - 19.24 = -21.27 \;\Rightarrow\; Aq\chi = e^{-b} = e^{21.27} = \mathbf{1.73\times10^{9}\ K^{-1}\ s^{-1}}$$
**L2 · Thought** Two-point straight line: compute slope first (ΔH/R — notice its magnitude ~5 × 10³ K corresponds to ΔH ≈ 44 kJ mol⁻¹, a sensible activation enthalpy for water exchange — physical anchor), then intercept, then exponentiate *with the sign watched*: b = −ln(Aqχ) → Aqχ = e^(−b), not e^b. The fallback value (2.00 × 10⁹) confirms the order of magnitude.

### (k) Number of coordinated waters q
**L1 · Answer** Form the two combinations: A² = (Aqχ)(A/qχ) = 1.731 × 10⁹ × 6.618 × 10¹⁴ = 1.146 × 10²⁴ → A = 1.070 × 10¹².
$$q = \frac{A}{(A/q\chi)\cdot\chi} = \frac{1.070\times10^{12}}{6.618\times10^{14} \times 9.007\times10^{-4}} = \mathbf{1.80}$$
≈ 2 coordinated water molecules on average.
**L2 · Thought** The algebra is a conjugate-pair trick: given Aqχ and A/qχ, their product isolates A and their ratio isolates q — but q still needs χ from (g) (consequential chain: (g) → (j) → (k)). Sanity anchor: q ≈ 1.8 sits between 1 and 2, exactly the "average number of coordinated waters" the stem describes exchanging with solvent; an answer of 600 or 0.002 (the two classic mis-combinations) should trigger a re-check of which quantity you isolated. (With the fallback numbers: A = √(2.00 × 10⁹ × 6.618 × 10¹⁴) = 1.15 × 10¹², q = 1.15 × 10¹²/(6.618 × 10¹⁴ × 0.00100) = 1.74 — same ballpark ✓.)

---

## Q5 — Sulfur chemistry in the atmosphere (15 marks)

*Scheme identities: A = (CH₃)₂S⁺–CH₂CH₂–COO⁻ (DMSP); B = (CH₃)₂S(=O)–CH₂CH₂–COO⁻; C = CH₃–S–CH₃ (DMS); J• = (CH₃)₂S(•)(OH); N• = CH₃–S–CH₂•; D = CH₃–S(=O)–CH₃ (DMSO); E = CH₃–S(=O)–OH (methanesulfinic acid); F = CH₃–S(=O)₂–OH (methanesulfonic acid); G = SO₃; L• = •OH.*

### (a) Oxidation states of S in B, C and E
**L1 · Answer** (Method: assign each bond's electrons to the more electronegative partner — note **S 2.58 > C 2.55**, so S *wins* the C–S electrons — then OS = 6 − allocated.)
- **B** (sulfoxide S: 1 lone pair, 2 × S–C, 1 × S=O): allocated = 2 + 2×2 = 6 → **S = 0**.
- **C** (DMS: 2 lone pairs, 2 × S–C): allocated = 4 + 4 = 8 → **S = −2**.
- **E** (CH₃–S(=O)–OH: 1 lone pair, 1 × S–C, 1 × S=O, 1 × S–OH): allocated = 2 + 2 = 4 → **S = +2**.
**L2 · Thought** The given worked example (CH₃–S–OH → S = 0) calibrates the one unusual rule: because S edges C on electronegativity, every C–S bond *adds* electrons to sulfur — so thioether S comes out at −2, not "0" as many students instinctively write. Sulfoxide S = 0 is the same effect: the S=O costs it everything the two C–S bonds donated.

### (b)(i) Equation for C + O₂ → D
**L1 · Answer**
$$2\,CH_3SCH_3 + O_2 \longrightarrow 2\,CH_3S(=O)CH_3$$
**L2 · Thought** D is the direct +1-oxygen product on the path C → D → E → F → G (each rung adds one O to sulfur). Balancing: 2 S on each side, 1 O₂ ✓.

### (b)(ii) Structure of D
**L1 · Answer** Dimethyl sulfoxide: CH₃–S(=O)–CH₃, trigonal-pyramidal S with one lone pair (drawn S→O or S=O; SMILES `CS(=O)C`).
**L2 · Thought** DMSO is the natural first oxidation rung of DMS and the required precursor of methanesulfinic acid E below it in the scheme. Check the pyramidality claim against (b) of Q2 — one lone pair on S, same VSEPR logic.

### (c) Formula of G
**L1 · Answer** **SO₃** (SO₃ + H₂O → H₂SO₄, the diprotic acid).
**L2 · Thought** "Highly soluble, dissolves to give a diprotic acid" is the fingerprint of SO₃ (→ H₂SO₄). SO₂ is out: it gives H₂SO₃, which *is* also diprotic — but G sits *above* F (methanesulfonic) in the oxidation ladder and atmospheric oxidation terminates at the +6 trioxide; the word "highly soluble" plus the ladder position jointly select SO₃.

### (d) pH of the solution
**L1 · Answer** n(SO₃) = pV/RT = (1.00 × 10⁵ × 13.4 × 10⁻⁶)/(8.314 × 323) = 4.99 × 10⁻⁴ mol → [H₂SO₄] = 4.99 × 10⁻⁴ mol dm⁻³ in 1.000 dm³.
Full dissociation of **both** protons: [H⁺] = 9.98 × 10⁻⁴ mol dm⁻³ → **pH = 3**.
**L2 · Thought** Two declared approximations (skeleton 7.5): ideal gas at 323 K, and full dissociation of the *diprotic* acid (factor of 2 — forgetting it gives pH 3.3, which still rounds to 3, but the factor belongs in the working). "To the nearest whole number" is a command word — quote pH = 3, not 3.00.

### (e) What happens to C forming J• and N• (tick table)
**L1 · Answer** (the scheme deducts a mark per *incorrect* tick, so tick exactly these and no more: for J• only "radical addition" and "oxidation of sulfur"; for N• only "loss of a H•")
- Forming **J•** ((CH₃)₂S + •OH → (CH₃)₂S(•)OH): tick **radical addition** and **oxidation of sulfur** (S: allocated 2 + 1 + 4 = 7 → OS = −1, up from −2 in DMS).
- Forming **N•** ((CH₃)₂S + •OH → CH₃–S–CH₂• + H₂O): tick **loss of a H• only**. Sulfur keeps 2 lone pairs + 2 S–C bonds → OS stays −2, so *no* redox-of-S tick; nothing is atomised.
**L2 · Thought** The two pathways of •OH toward a sulfide are the two generic radical attack modes: add to a lone-pair-rich centre (addition) or abstract a hydrogen atom. The discriminating computation is the oxidation-state audit on each product — addition *does* oxidise S (a lone pair is consumed into an S–O bond whose electrons then live on O), abstraction leaves S at −2. Classification discipline: the scheme classifies H-atom abstraction here as "loss of a H•" alone — although the step is formally an SH2 *radical substitution*, that box is **not** ticked in the scheme, and the −1-per-wrong-tick rule punishes hedging. Tick-table lesson (§7.7): when categories overlap, choose the single most specific intended classification rather than every defensible one.

### (f) Formula of L•
**L1 · Answer** **•OH** (the hydroxyl radical).
**L2 · Thought** The only common atmospheric radical that both adds to sulfides and abstracts α-hydrogens, and whose addition product (CH₃)₂S(•)OH and abstraction product CH₃SCH₂• match the drawn J•/N• exactly — structural back-check rather than a guess.

### (g) Orders a and b
**L1 · Answer** **a = 1, b = 1.**
Order in L•: within experiment 1, [L•] falls 1.00 → 0.50 → 0.25 µmol dm⁻³, halving every 10 s — constant fractional decay = first-order disappearance of L•, so rate ∝ [L•]¹ → b = 1. (Check with J• growth: rate falls 0.050 → 0.025 µmol dm⁻³ s⁻¹ as [L•] halves ✓.)
Order in C: pseudo-first-order constant k_obs = ln 2 / 10 s = 6.93 × 10⁻² s⁻¹ at [C] = 1000; in experiment 2, [L•] falls by the factor 2.00 → 1.42 → 1.00, i.e. k_obs = ln(1/0.707)/10 s = 3.47 × 10⁻² s⁻¹ at [C] = 500. k_obs ∝ [C]ᵃ: 6.93/3.47 = 2.00 = (1000/500)ᵃ → a = 1.
**L2 · Thought** Method choice: the clean observable is the **decay of [L•]** (large dynamic range), not the noisy increments of [J•]. Within one experiment, [C] is ~constant (1000 vs ~1 µmol dm⁻³ — huge excess, zero-order in C *locally*), so each experiment isolates b; comparing the two pseudo-first-order constants across experiments isolates a. This "vary one factor at a time" logic is the gas-phase cousin of the bench kinetics skeleton 7.8.

### (h) Termolecular rate constant k₃
**L1 · Answer** The apparent law rate = k₂[N•][O₂] hides [X]: k₂ = k₃[X], with [X] = total gas concentration = 40.4 mmol dm⁻³ (given).
Convert: [X] = 0.0404 mol dm⁻³ × (1 dm³/10³ cm³) × 6.022 × 10²³ = 2.43 × 10¹⁹ molecules cm⁻³.
$$k_3 = \frac{k_2}{[X]} = \frac{5.7\times10^{-12}\ \text{cm}^3\text{ molecule}^{-1}\text{ s}^{-1}}{2.43\times10^{19}\ \text{molecules cm}^{-3}} = \mathbf{2.3\times10^{-31}\ cm^6\ molecule^{-2}\ s^{-1}}$$
**L2 · Thought** Dimensional audit first: k₂ (second-order, cm³ molecule⁻¹ s⁻¹) divided by a concentration (molecules cm⁻³) gives third-order units cm⁶ molecule⁻² s⁻¹ ✓. The hint "[X] is only determined by the total pressure" is the instruction to use the *given* total concentration (any gas molecule can be X — inert gas included). Plausibility anchor: ~10⁻³¹ cm⁶ molecule⁻² s⁻¹ is the canonical magnitude of a termolecular association rate constant — a wrong unit conversion (e.g. forgetting dm³ → cm³, giving 10⁻²⁸) is instantly visible against it.

---

*End of Paper 2 (2024). Next: 2023 Round 1.*

---

# Paper 3 — 2023 UKChO Round 1 (55th IChO selection)

*5 questions, 86 marks, 2 h → ≈ 1.4 min per mark. Marks: Q1 = 7, Q2 = 20, Q3 = 18, Q4 = 21, Q5 = 20.*

## Q1 — Rocket fuels (7 marks)

### (a) Hydrogen + oxygen
**L1 · Answer** 2 H₂(g) + O₂(g) → 2 H₂O(g) (as written per mole of H₂ in (b): H₂(g) + ½ O₂(g) → H₂O(g)).
**L2 · Thought** "Fuel components are first vaporised" → water is **gaseous**; the state symbol is not decoration, it sets the enthalpy used in (b) (−241 kJ mol⁻¹, not −286).

### (b) O=O bond enthalpy
**L1 · Answer** For H₂ + ½ O₂ → H₂O(g), ΔH = −241 kJ mol⁻¹:
broken: 432 + ½ x; formed: 2 × 460 = 920
−241 = (432 + x/2) − 920 → **x = 494 kJ mol⁻¹**
**L2 · Thought** ΔH = bonds broken − bonds formed; the only unknown is O=O. Plausibility anchor: tabulated O=O ≈ 498 kJ mol⁻¹ ✓. If you doubled everything and still got ~247, you forgot the ½ on O₂.

### (c)(i) Moles of H₂ in 1 dm³ of liquid hydrogen
**L1 · Answer** m = 0.071 g cm⁻³ × 1000 cm³ = 71 g → n = 71/2.016 = **35.2 mol**.
### (c)(ii) Energy released on combustion
**L1 · Answer** 35.2 × 241 = **8.49 × 10³ kJ** (≈ 8.5 MJ released).
**L2 · Thought** The point of the pair: liquid hydrogen packs 35 mol into a dm³ — the volumetric energy density is the engineering reason rockets tolerate cryogenics. Note (c) reuses (b)'s per-mole enthalpy directly (consequential chain).

### (d)(i) Sabatier process
**L1 · Answer** CO₂ + 4 H₂ → CH₄ + 2 H₂O. (Audit: C 1=1; O 2=2; H 8=4+4 ✓.)
### (d)(ii) Oxidation numbers
**L1 · Answer** C: **+4** (CO₂) → **−4** (CH₄); H: **0** (H₂) → **+1** (CH₄ and H₂O).
**L2 · Thought** Methanation is an 8-electron reduction of carbon — oxidation-state audit is how you *find* the 4 H₂ coefficient if the equation is given unbalanced. If you balanced first, use this part as the cross-check.

### (e) Liquid CH₄ + liquid O₂ → gaseous products
**L1 · Answer** Vaporise both reactants first, then combust:
ΔH = ΔvapH(CH₄) + 2 ΔvapH(O₂) + ΔcH = 8.2 + 2(6.8) + (−890.8) = **−869.0 kJ**
**L2 · Thought** Hess path choice: liquid → gas (pay vaporisation) → react in gas phase. The 2 mol O₂ per mole CH₄ is the easy multiplier to miss. Energy returned is slightly *less* than the gas-phase combustion because vaporisation is paid up front.

---

## Q2 — Electronegativity, bonding and BN structures (20 marks)

### (a) Pauling Δχ(Cl–H)
**L1 · Answer**
$$\Delta\chi = 0.102\sqrt{427 - \tfrac{432+244}{2}} = 0.102\sqrt{89} = \mathbf{0.96}$$
**L2 · Thought** The "extra" A–B bond strength over the geometric-mean baseline is Pauling's ionic-resonance energy; the square root is inside the definition — do not square the 0.102 instead.

### (b) χ(Cl)
**L1 · Answer** χ(Cl) = χ(H) + Δχ = 2.20 + 0.96 = **3.16**.
**L2 · Thought** Consistency check against trend knowledge: Cl should sit just below N (3.04) and above Br (2.96) — 3.16 ✓. The sign choice (add, not subtract) is decided by "Cl is more electronegative than H" — state it.

### (c) Adjusted Mulliken χ(N)
**L1 · Answer** Convert Eᵢ to kJ mol⁻¹ first: Eᵢ = 14.5 × 96.49 = 1399 kJ mol⁻¹.
χ(N) = 0.00197 × (1399 + 6.80) + 0.19 = 0.00197 × 1406 + 0.19 = **2.96**.
**L2 · Thought** Unit trap: Eᵢ is in eV, Eₑₐ in kJ mol⁻¹ — the conversion must happen *before* the sum (mixing units gives χ ≈ 0.23, obviously wrong against the 2.20 reference scale). Anchor: N ≈ 3.0 on Pauling's scale ✓.

### (d) Positions on the van Arkel triangle
**L1 · Answer** (χ̄ = mean, Δχ = difference, then match to the lettered grid):

| substance | χ̄ | Δχ | letter |
|---|---|---|---|
| (i) AlP | (1.61+2.19)/2 = 1.90 | 0.58 | **I** (2.0, 0.6) |
| (ii) CsH | 1.50 | 1.41 | **E** (1.55, 1.35) |
| (iii) BrF | 3.47 | 1.02 | **L** (3.4, 1.05) |
| (iv) HgO | 2.72 | 1.44 | **G** (2.7, 1.4) |
| (v) SiC | 2.22 | 0.65 | **J** (2.25, 0.65) |

(The intended letters are I, E, L, G, J. Note on (ii): CsH's computed position (1.50, 1.41) falls on top of the close D/E pair — D (1.40, 1.42) and E (1.55, 1.30) bracket it almost equally; the intended letter is **E**. The transferable habit is unchanged: compute both coordinates, then pick the nearest letter — and when two letters are equidistant, say so rather than agonising.)

**L2 · Thought** Compute both coordinates for every substance *before* looking at the grid — matching one coordinate at a time is how near-miss confusions happen (AlP vs SiC differ mainly in χ̄: 1.90 vs 2.22; CsH's computed position falls between the close D/E pair — the intended letter is E, and D should be read as "close but not best" rather than wrong-by-method). Keep both coordinates to 2 d.p. — the grid spacing is ~0.2–0.3.

### (e) Greatest metallic character
**L1 · Answer** **AlP.**
**L2 · Thought** Metallic character lives at the **bottom-left** of the triangle (small Δχ, low-to-mid χ̄). Among the five, AlP has the smallest Δχ (0.58) with a low-ish χ̄ — CsH has lower χ̄ but a *large* Δχ, which pulls it up toward the ionic corner (CsH is a saline hydride). So "most metallic" ≠ "contains the most metallic metal" — the difference coordinate decides.

### (f) Second plot (Cs, CsBr, CO given as anchors)
**L1 · Answer**
- (i) **CsCl → B**: χ(Cl) ≈ 3.16 (from (b)), χ̄ ≈ 1.98, Δχ ≈ 2.37 — just above the CsBr anchor (Δχ 2.17) ✓.
- (ii) **NaK → N**: both metals, χ̄ ≈ 0.88, Δχ ≈ 0.1 — beside the Cs anchor but marginally higher χ̄ ✓.
- (iii) **GaN → E**: χ(Ga) ≈ 1.81 (just above Al, group trend), χ(N) ≈ 3.04: χ̄ ≈ 2.43, Δχ ≈ 1.23 ✓.
**L2 · Thought** The three anchors are calibration: Cs fixes the left edge (χ ≈ 0.8), CsBr fixes the ionic staircase, CO fixes the covalent right. For unlisted elements (Cl, Ga, N), interpolate on the periodic table (Cl > Br slightly; Ga ≈ Al slightly less; N just below O) — the question says so explicitly ("your knowledge of trends").

### (g)(i) Reaction (1): boric acid + ammonia
**L1 · Answer** H₃BO₃ + NH₃ → BN + 3 H₂O. (Audit: B 1=1; N 1=1; O 3=3; H 6=6 ✓.)
**L2 · Thought** Dehydration/condensation logic: the only atoms present are B,N,O,H; water is the only O/H sink. If you found yourself writing N₂ or H₂ products, the atom audit fails — check before writing.

### (g)(ii) Reaction (2): B₂O₃ + N₂ + CaB₆
**L1 · Answer** 3 CaB₆ + B₂O₃ + 10 N₂ → 20 BN + 3 CaO. (Audit: Ca 3=3; B 20=20; N 20=20; O 3=3 ✓.)
**L2 · Thought** Balance order that avoids fractions: Ca fixes 3 CaO per 3 CaB₆; O fixes the single B₂O₃; B then totals 20 → 20 BN; N follows: 10 N₂. Electron audit as a cross-check: N₂ is *reduced* (0 → −3, 60 e⁻ total), the boride borons are *oxidised* toward +3 — the driving force is why an exotic reagent like CaB₆ appears at all.

### (h) BN unit cells
**L1 · Answer**
(i) V(c-BN) = a³ = (3.63 × 10⁻⁸ cm)³ = **4.78 × 10⁻²³ cm³**.
(ii) Zinc-blende cell = 4 BN: ρ = (4 × 24.82/6.022 × 10²³)/4.783 × 10⁻²³ = **3.45 g cm⁻³**.
(iii) V(h-BN) = hexagon area × c = (3√3/2)(1.47 × 10⁻⁸)² × 6.66 × 10⁻⁸ = **3.74 × 10⁻²³ cm³**.
(iv) Atom count in the hexagonal prism: top face ring 6 × ⅙ = 1 atom; bottom face = 1; middle honeycomb ring (shared between 3 prisms in-plane, but on no vertical boundary) 6 × ⅓ = 2 → total 4 atoms = 2 BN. ρ = (2 × 24.82/6.022 × 10²³)/3.739 × 10⁻²³ = **2.20 g cm⁻³**.
(v) w-BN prism (share accounting): B: **1 fully interior** + 4 corners × 1/12 + 4 corners × 2/12 = **2 B**; N: **1 fully interior** + 2 edges × 1/6 + 2 edges × 2/6 = **2 N**. (Both atoms: interior = 1, then fractional shares at the prism's corners/edges; the totals 2 + 2 are the marked answer.)
**L2 · Thought** Three lessons. (1) The hexagon-area formula (3√3/2)b² is *not* the crystallographic rhombic-cell area (a² sin 60°) — here the prism base is the full honeycomb hexagon, and the side b = 1.47 Å is the B–N bond length, so use (3√3/2)b². (2) Shares differ by position: corner ⅛ (cubic) vs ⅙ (hexagonal-prism vertex on a boundary face) vs ⅓ (in-plane ring vertex with no boundary), edge ¼, interior 1 — the share-count comes *before* any arithmetic (skeleton 7.4). (3) Density anchors: c-BN 3.45 (real 3.49 ✓), h-BN 2.20 (real 2.27 ✓) — the layered form must be the *less* dense one (van der Waals gaps), which is the sanity check on the atom count in (iv): counting 3 BN instead would give ρ = 3.3 > c-BN, physically backwards.

---

## Q3 — Amino acid complexes (18 marks)

### (a) Isoleucine structures
**L1 · Answer**
(i) pH 2: fully protonated cation: ⁺NH₃–CH(CH(CH₃)CH₂CH₃)–COOH (SMILES `CCC(C)C([NH3+])C(=O)O`).
(ii) pH 11: fully deprotonated anion: H₂N–CH(R)–COO⁻ (`CCC(C)C(N)C(=O)[O-]`).
**L2 · Thought** Compare each pH to both pKa values (2.36 COOH; 9.60 NH₃⁺): pH 2 < both → everything protonated; pH 11 > both → everything deprotonated. The skeleton is unchanged — only protonation states move.

### (b) Isoelectric point
**L1 · Answer** (i) The **zwitterion**: ⁺NH₃–CH(R)–COO⁻ (net charge 0). (ii) pI = (pKa₁ + pKa₂)/2 = (2.36 + 9.60)/2 = **5.98**.
**L2 · Thought** For a neutral side chain (R = sec-butyl), pI is the plain average of the two pKa's — the side chain never ionises, so there are exactly two pKa's to average. (For acidic/basic side chains the averaging rule changes — pick the two pKa's flanking the neutral species.)

### (c) Titration curve identification
**L1 · Answer** **The bottom-middle curve** (starts ≈ pH 2, steep rise centred ≈ 13–15 cm³, then rises to ≈ pH 12 at 40 cm³).
**L2 · Thought** Compute before choosing — 1.25 mmol of the fully protonated cation H₂A⁺ vs 0.1 mol dm⁻³ NaOH: equivalence points at **12.5 cm³** (COOH) and **25.0 cm³** (NH₃⁺). A full charge-balance simulation (pKa₁ 2.36, pKa₂ 9.60) gives: pH 2.1 (0) → 3.1 (10) → 6.0 (12.5, ampholyte) → 9.0 (15) → 9.8 (20) → 10.9 (25) → 12.2 (40). Only the bottom-middle option starts acidic and ends at ~12 with the main steep region just after 12.5 cm³; the top-middle option's single jump sits at ~20 cm³ (merged-step trap); the downward curves die at the direction check (base is being *added*). The lesson: three computed landmarks (start pH ≈ ½(pKa₁−log c), ampholyte pH = pI, excess-base pH) are enough to kill five of six options without plotting anything.

### (d) Stereoisomers of square-pyramidal Cu(gly)₂(H₂O)
**L1 · Answer** The water stays axial; the two bidentate glycinates span the square base in two connectivities:
- **trans**: the two N donors opposite (180°), the two carboxylate O's opposite — has a mirror plane → achiral.
- **cis**: the two N donors adjacent (90°), O's adjacent — mirror plane through the axial H₂O bisecting the N–Cu–N and O–Cu–O angles → achiral.
(Both are flat-topped square pyramids; draw the N–Cu–N arc as curved brackets with the O ends matching.)
**L2 · Thought** With two identical unsymmetrical bidentates (N,O) the only degree of freedom is *which equatorial atoms sit opposite* — N-trans-N or N-cis-N; O follows automatically. This is the classic bis(glycinato)copper(II) cis/trans pair (the thermal cis→trans isomerisation the question cites). Square-pyramidal with one axial ligand adds no new isomerism because the axial site is unique.

### (e) Stereoisomers of octahedral MMt₃
**L1 · Answer** Three identical unsymmetrical bidentates give two geometrical isomers:
- **fac** (facial): the three N's occupy one triangular face, the three O's the opposite face — **chiral** (Δ/Λ pair; draw one enantiomer).
- **mer** (meridional): the three N's lie in a plane through the metal (two trans, one cis to both) — **chiral** (also Δ/Λ; draw one enantiomer).
**L2 · Thought** Systematic enumeration for M(AB)₃: fix ligand 1, then ask whether the remaining two N's can be mutually trans (mer) or must all be cis (fac) — no third connectivity exists. Chirality: with *symmetrical* bidentates a mer isomer could keep a mirror plane, but here each ligand is unsymmetrical (N≠O), so every candidate plane maps an N site onto an O site — not a symmetry operation — and both fac and mer come out chiral. Hence "draw one enantiomer" applies to both.

### (f) RhMt₃ and CuMt₂
**L1 · Answer**
- **RhMt₃**: Rh(III) = **d⁶**. Two arrangements: high spin t₂g⁴ eg² (↑↓ ↑ ↑ ↑ ↑) → n = 4 unpaired → μ = √(4×6) = **4.90 BM**; low spin t₂g⁶ eg⁰ (↑↓ ↑↓ ↑↓) → n = 0 → μ = **0 BM**.
- **CuMt₂**: Cu(II) = **d⁹**. Only one arrangement possible: t₂g⁶ eg³ (↑↓ ↑↓ ↑↓ ↑↓ ↑) → n = 1 → μ = √(1×3) = **1.73 BM**.
**L2 · Thought** Framework rule in action: the HS/LS question exists only for d⁴–d⁷ — d⁹ has a forced configuration, so do not invent a second diagram (that over-drawing costs the mark). d-count method: group number − oxidation state (Rh: 9 − 3 = 6; Cu: 11 − 2 = 9).

### (g) FeMt₃ spin state
**L1 · Answer** Fe(III) = d⁵: HS μ = √(5×7) = **5.92 BM**; LS (t₂g⁵) μ = 1.73 BM. Observed 5.63 BM ≈ 5.92 → **high spin**.
**L2 · Thought** Compare to *both* theoretical values, not just the nearer one by accident: 5.63 is far closer to 5.92 (5 % low, normal spin–orbit quenching) than to 1.73 (3× off). Deciding criterion: Δ₀ vs P — methionine is a weak-field ligand (N,O donors), consistent with the HS assignment.

---

## Q4 — Vaping: vitamin E acetate, ketene, and the synthesis (21 marks)

### (a)(i) Functional groups (tick)
**L1 · Answer** **Ester** (the acetate –O–COCH₃ on the phenol) and **ether** (the chroman ring O).
### (a)(ii) x in CₓH₅₂O₃
**L1 · Answer** **x = 31** (C₃₁H₅₂O₃).
**L2 · Thought** Count by fragments: chroman bicyclic core (6 aromatic + 3 heterocycle C) + 4 methyls + acetate (2 C) + C₁₆ side chain = 9 + 4 + 2 + 16 = 31 ✓. The tick-list in (i) is a trap for "ketone": the C=O belongs to the ester, not a ketone — carbonyl classification asks what *else* is bonded to the carbonyl carbon.

### (b) The toxic product (✓/✗ table)
**L1 · Answer** Toxic product = **ketene, CH₂=C=O** (M = 42; the pyrolysis product of the acetate, as in the cited PNAS study).

| structure | mass spec (loss 207.2 − 165.2 = 42) | ¹H NMR: 1 signal | ¹³C NMR: 2 signals |
|---|---|---|---|
| ethynol, HC≡C–OH (M 42) | ✓ | ✗ (≡CH and OH differ) | ✓ (2 C) |
| **ketene, CH₂=C=O (M 42)** | ✓ | ✓ (2 equivalent H) | ✓ (CH₂ vs C=O) |
| propanone, (CH₃)₂C=O (M 58) | ✗ | ✓ (6 equivalent H) | ✓ (CH₃ vs C=O) |
| oxirene, c-C₂H₂O (M 42) | ✓ | ✓ (2 equivalent H) | ✗ (2 equivalent C → 1 signal) |

Only ketene is consistent with all three.
**L2 · Thought** This is the evidence-table skeleton (7.3) in miniature: three independent filters, each row pruned on the first failure. Note the elegant trap design — all four candidates pass *at least two* tests, so stopping after two techniques leaves the answer ambiguous; run every filter on every candidate. (Also note the ¹³C spectrum being taken in D₂O is the hint that the product is small and polar/gaseous, not a steroid fragment.)

### (c) Wittig reaction table
**L1 · Answer** (Rule given: ylide carbon adjacent to C=O or C=C → E major; otherwise Z major.)
- **Row 1**: ethanal (CH₃CHO) + **cyclohexylidenetriphenylphosphorane**, Ph₃P=C1CCCCC1 (the ylidic carbon is the ring vertex) → **ethylidenecyclohexane**, CH₃CH=C1CCCCC1 (SMILES `CC=C1CCCCC1`). No E/Z exists here: the ring-side sp² carbon carries two identical ring paths — the mark scheme explicitly notes "no difference between E and Z" for this product, so the selectivity rule is not even needed.
- **Row 2**: 2-methylpropanal + the conjugated dienylide Ph₃P=CH–CH=CH–CH=CH–CH₂CH₃ (ylidic C adjacent to a C=C) → the **newly formed** C=C is **E**: (CH₃)₂CH–CH=CH–CH=CH–CH=CH–CH₂CH₃, the two pre-existing diene double bonds keeping their drawn (E) geometry.
- **Rows 3/4 ("OR")**: target = **(2E,4Z)-hepta-2,4-diene**, CH₃–CH=CH–CH=CH–CH₂–CH₃ with the left C=C trans (E) and the right C=C cis (Z) as drawn. Two complementary disconnections:
  - **Route A** (form the *left*, E bond): **ethanal** + crotyl-type ylide **Ph₃P=CH–CH=CH–CH₂CH₃** with its internal C=C drawn **Z** (it becomes the target's right bond). The ylide has an adjacent C=C → new bond **E** ✓.
  - **Route B** (form the *right*, Z bond): **(E)-but-2-enal (crotonaldehyde, CH₃–CH=CH–CHO, drawn E)** + unstabilised **propylide Ph₃P=CH–CH₂CH₃** → new bond **Z** ✓.
  (Marking note: the two answers containing C=C bonds — route A's ylide, route B's aldehyde — must carry the correct E/Z geometry for the marks.)
**L2 · Thought** The classification key is the *ylide's* substitution, never the carbonyl's: stabilised ylide (adjacent π) → E; unstabilised → Z. For the reverse problem (given the alkene), a Wittig C=C can be disconnected **on either side** — that is why the table offers "OR". The subtlety that makes this item: the target diene has one E and one Z bond, so the two disconnections are *not* interchangeable — route A must make the E bond (stabilised crotylide), route B must make the Z bond (unstabilised propylide), and the pre-existing C=C inside each partner must be drawn with the geometry it will have in the product. Check each route's selectivity *against the specific bond it forms* before claiming the geometry.

### (d) First synthesis part: A, B, C, D
**L1 · Answer**
- **A** = 4,6-dihydroxy-2,3,5-trimethylbenzaldehyde (formyl-trimethylhydroquinone): ring bearing CHO, 2 OH, 3 CH₃ (C₁₀H₁₂O₃ ✓; + 2 Ac₂O − 2 HOAc → the C₁₄H₁₆O₅ diacetate shown ✓).
- **B** = the **(E)-enone** Ar–CH=CH–COCH₃ (Ar = 4,6-diacetoxy-2,3,5-trimethylphenyl): Wittig of the aryl aldehyde with Ph₃P=CH–COCH₃ — the ylide carbon is adjacent to C=O → **E** major (the rule from (c), applied back).
- **C** = Ar–CH₂CH₂–COCH₃ (4-arylbutan-2-one; H₂ reduces the C=C of B, ketone untouched).
- **D** = the **diphenol** 4,6-dihydroxy-2,3,5-trimethylphenyl–CH₂CH₂–C(OH)(CH₃)–C≡CH (C₁₅H₂₀O₃ ✓): 5 equivalents of HC≡CMgBr do three jobs — 1 equiv. adds to the ketone (→ tertiary propargylic alcohol), and 2 × 2 equiv. cleave the two phenol acetates (each acetate consumes 2 equiv., releasing 2 molecules of the drawn by-product 3-methylpent-1,4-diyn-3-ol, (CH₃)C(OH)(C≡CH)₂).
**L2 · Thought** The "5 equivalents" and the "× 2" by-product are the bookkeeping clues that force the *full* deacetylation in D: 1 (ketone) + 2 × 2 (two acetates) = 5 ✓ — the reagent count is a hidden atom ledger (formula audit). C₁₅H₂₀O₃ confirms: 2 phenol O + 1 alcohol O = 3 O ✓, and the C count (ring 6 + 3 CH₃ + chain 4 + alkyne 2 = 15 ✓) leaves no room for any acetate. Had D retained one acetate it would be C₁₇H₂₂O₄ — the printed formula kills it.

### (e) The intermediate carbocation
**L1 · Answer** Ar–CH₂CH₂–**C⁺**(CH₃)–C≡CH — the **tertiary** (and propargylic) cation from protonation of D's tertiary alcohol and loss of water; the ortho phenolic OH then closes the six-membered chroman ring onto it (+H₂O out overall).
**L2 · Thought** Ring-size filter: the phenol oxygen attacking this cation closes a 6-membered O-heterocycle (chroman) — the alternative (attack at the alkyne) would give a strained/endo product and would not lose "a molecule of water" as stated. "Tertiary carbocation" in the stem is the license to draw a cation α to both methyl and alkyne — stable enough to form under aqueous HCl.

### (f) Second part: W, X, Y, Z
**L1 · Answer**
- **W** = 6-acetoxy-2,5,7,8-tetramethyl-**2-vinylchroman** (Lindlar's catalyst reduces the ethynyl C≡CH of the C₁₇ compound to a *cis* vinyl –CH=CH₂, stopping at the alkene).
- **X** = 6-acetoxy-2,5,7,8-tetramethylchroman-2-**carbaldehyde**, ringC(CH₃)–CHO (ozonolysis of the terminal vinyl: the internal alkene carbon becomes the aldehyde).
- **Y** = **formaldehyde**, HCHO (the terminal =CH₂ carbon).
- **Z** = the **unstabilised Wittig ylide** Ph₃P=CH–CH₂–CH(CH₃)–CH₂CH₂CH₂–CH(CH3)–CH₂CH₂CH₂–CH(CH₃)₂ (C₁₆H₃₃P⁺=C⁻ skeleton, i.e. the farnesyl-derived ylide): X's aldehyde + Z → the drawn Z-alkene side chain (no π adjacent to the ylide carbon → Z major, exactly as drawn); final H₂ then saturates the C=C to give vitamin E acetate's phytyl side chain.
**L2 · Thought** Decode order: work backwards from the drawn products. The ozonolysis scheme printed in the stem says C=C → C=O + O=C, so W must contain the only oxidisable π bond (vinyl), X the aldehyde, Y formaldehyde — Lindlar is the standard alkyne→cis-alkene reagent, which is why it is named. For Z: count the carbons in the drawn side chain (16: =CH– + 14-C chain + the aldehyde carbon), subtract X's aldehyde carbon and the =CH– from the ylide carbon → the ylide's organic group is C₁₄H₂₉ with the isoprenoid 4',8',12'-methyl pattern visible in the drawing. The final H₂ step (no catalyst selectivity needed, just saturation) confirms the side chain's C=C was the only reducible group left — and the Z geometry of that C=C is the last consistency check with part (c)'s rule.

---

## Q5 — Cheese: fermentation equilibria and bubble physics (20 marks)

### (a)(i) Conjugate base of lactic acid
**L1 · Answer** Lactate: CH₃–CH(OH)–COO⁻ (`CC(O)C(=O)[O-]`).
### (a)(ii) pKa
**L1 · Answer** pKa = −log(1.38 × 10⁻⁴) = **3.86**.
**L2 · Thought** One line; guard against the common −log(1.38) slip (pKa ≈ 3.9 is the sensible zone for a carboxylic acid — if you got 0.14, you lost the 10⁻⁴).

### (b) Internal hydrogen bond in the conjugate base
**L1 · Answer** Draw lactate with the α-hydroxyl O–H pointing across to a carboxylate oxygen, O–H···O⁻(C=O) as a dashed bond closing a **five-membered ring** (O–H···O–C–C–O chelate).
**L2 · Thought** Ring-size filter again: a 5-membered pseudo-ring is the strain-free option (the alternative H-bond to the carbonyl O gives the same 5-ring — either carboxylate O accepted). This intramolecular H-bond stabilises the anion → stronger acid than propanoic acid, as the stem asserts — the drawing *is* the explanation, so the chelate ring must be closed explicitly.

### (c)(i) Reaction classification (tick)
**L1 · Answer** **Hydrolysis** (a disaccharide + water → two monosaccharides).
### (c)(ii) The monosaccharides
**L1 · Answer** **Glucose and galactose** (the two epimers of lactose's composition).
**L2 · Thought** Hydrolysis of the β-1,4-galactosidic bond — naming "glucose + glucose" is the classic error (that is maltose, not lactose); C₁₂H₂₂O₁₁ disaccharide = hexose + hexose, and lactose specifically = galactose–glucose.

### (d) Lactose → lactic acid
**L1 · Answer** C₁₂H₂₂O₁₁ + H₂O → 4 C₃H₆O₃. (Audit: C 12=12; H 24=24; O 12=12 ✓.)
**L2 · Thought** Lactic acid = C₃H₆O₃ (half a hexose, CH₃–CHOH–COOH); four of them per lactose. Note the elegance: no redox overall (average carbon oxidation state 0 on both sides) — fermentation here is pure disproportionation-free rearrangement + hydrolysis.

### (e) Propionibacterium fermentation
**L1 · Answer** 3 C₃H₆O₃ → 2 C₃H₆O₂ (propanoic) + C₂H₄O₂ (ethanoic) + CO₂ + H₂O.
(Audit: C 9 = 6+2+1 ✓; H 18 = 12+4+2 ✓; O 9 = 4+2+2+1 ✓; ethanoic acid and CO₂ equal (1 : 1) as required ✓.)
**L2 · Thought** Solve the balance as a small linear system, using the constraints in order: equal ethanoic/CO₂ (c = d), then C, H, O → ratio 3 : 2 : 1 : 1 : 1. This is the real Propionibacterium stoichiometry (3 lactate → 2 propionate + 1 acetate + CO₂ + H₂O) — the "eyes" of Emmental are the CO₂ term.

### (f)(i) Bubble volume
**L1 · Answer** V = (4/3)π(0.75 × 10⁻² m)³ = **1.77 × 10⁻⁶ m³**.
### (f)(ii) Mass of lactic acid fermented
**L1 · Answer** n(CO₂) = pV/RT = (101 325 × 1.767 × 10⁻⁶)/(8.314 × 294) = 7.32 × 10⁻⁵ mol.
n(lactic acid) = 3 n(CO₂) = 2.20 × 10⁻⁴ mol → m = 2.20 × 10⁻⁴ × 90.08 = **1.98 × 10⁻² g ≈ 20 mg**.
**L2 · Thought** Three explicit links, each a mark: sphere volume in SI (radius, not diameter — the 1.5 cm is a *diameter*, the first trap); ideal gas at 21 °C = 294 K (not 298); the 3 : 1 fermentation stoichiometry from (e) (the consequential chain). Dimensional audit: Pa·m³ = J, J/(J K⁻¹ mol⁻¹·K) = mol ✓.

### (g) [CO₂(ch)] at pH 5.20
**L1 · Answer** [H⁺] = 10⁻⁵·²⁰ = 6.31 × 10⁻⁶; ratio [HCO₃⁻]/[CO₂] = K/[H⁺] = 4.47 × 10⁻⁷/6.31 × 10⁻⁶ = 0.0708.
[CO₂(ch)] = 3.70 × 10⁻²/(1 + 0.0708) = **3.46 × 10⁻² mol dm⁻³**.
**L2 · Thought** Two-equation system (equilibrium ratio + mass balance) — solve by expressing both species through [CO₂]. Sanity: at pH 5.2, well below pKa 6.35, dissolved CO₂ should dominate (94 %) ✓ — if your answer came out below 1.85 × 10⁻², you inverted the ratio.

### (h) Molar amounts of the three CO₂ pools (tick expressions)
**L1 · Answer**
- n(CO₂(g)) = **4πr³p_b / 3RT** (ideal gas in the bubble volume 4πr³/3) — tick option 2.
- n(CO₂(ch)) = **k_H V_ch p_b** (Henry's law × cheese volume) — tick option 1.
- n(HCO₃⁻(ch)) = **K · 10^(pH) · k_H V_ch p_b** — tick option 4: from [HCO₃⁻] = K[CO₂]/[H⁺] and 1/[H⁺] = 10^(pH).
**L2 · Thought** Each pool is (concentration × its volume): gas phase → ideal gas; dissolved CO₂ → Henry's law; bicarbonate → the equilibrium ratio chained onto Henry's law. The 10^(+pH) (not 10^(−pH)) is the sign trap — derive it from K's definition rather than guessing.

### (i) The (a + br³)(p_atm + γ/r) = η form
**L1 · Answer** Sum the three pools and factor p_b = p_atm + γ/r:
$$\eta = \underbrace{k_H V_{ch}\left(1 + K\cdot 10^{pH}\right)}_{a}\, p_b + \underbrace{\frac{4\pi}{3RT}}_{b}\, r^3 p_b = (a + b r^3)\left(p_{atm} + \frac{\gamma}{r}\right)$$
**a = k_H V_ch (1 + K·10^(pH));  b = 4π/3RT.**
**L2 · Thought** Pure algebraic packaging: every term is proportional to p_b, so p_b factors; the r-dependence splits into a constant part (dissolved pools) and an r³ part (gas pool). Check the units of a and b against the given numerical values (a in mol Pa⁻¹, b in mol Pa⁻¹ m⁻³ ✓) — unit-matching to printed data is a valid audit when algebra gets heavy.

### (j) Two roots and the physical choice
**L1 · Answer** Substituting the numbers into (a + br³)(p_atm + γ/r) = η, i.e.
b·p_atm·r⁴ + bγ r³ + (a·p_atm − η) r + aγ = 0
with a = 1.70 × 10⁻⁹ mol Pa⁻¹, b = 1.75 × 10⁻³ mol Pa⁻¹ m⁻³, η = 2.35 × 10⁻⁴ mol, γ = 9.28 Pa m:
177.3 r⁴ + 0.01624 r³ − 6.275 × 10⁻⁵ r + 1.578 × 10⁻⁸ = 0
Real positive roots: **r = 6.96 × 10⁻³ m ≈ 7.0 mm** and **r = 2.5 × 10⁻⁴ m ≈ 0.25 mm** (exact roots of the quartic; the mark scheme's approximate truncated route quotes the small root as 1.16 × 10⁻⁴ m — approximate small-root estimates vary with the truncation used, but the discrepancy lives in the rejected root only and changes nothing: both fail the validity test below).
Physical test (γ/r ≪ p_atm): for 6.96 mm, γ/r = 1.33 × 10³ Pa = 1.3 % of p_atm ✓ — consistent with the approximation; for the small root (2.5 × 10⁻⁴ m), γ/r = 3.7 × 10⁴ Pa = 36 % of p_atm ✗ — the approximation is invalid there (the scheme's 1.16 × 10⁻⁴ m fails the same test even harder: γ/r ≈ 8 × 10⁴ Pa ≈ 79 %). **Correct physical solution: r ≈ 7.0 mm.**
Leading-order cross-check: r₀ = [(η/p_atm − a)/b]^(1/3) = [(6.19 × 10⁻¹⁰)/(1.75 × 10⁻³)]^(1/3) = 7.07 mm, within 2 % of the full root ✓.
**L2 · Thought** Three habits on show. (1) When the exact equation is a quartic, the *given* approximation is not a courtesy — the paper expects you to solve it (iteratively or, as here, by direct substitution of the printed numbers and root-finding) and to produce **both** roots. (2) The validity condition γ/r ≪ p_atm is not decoration either — it is the *selection criterion* between the two roots; always test each candidate against the assumption that generated it (skeleton: limiting-case check / approximation audit). (3) The leading-order estimate r₀ ≈ 7.07 mm from dropping the γ/r term entirely agrees with the larger root to 2 % — that agreement is what makes rejecting the small root intellectually safe rather than arbitrary.

---

*End of Paper 3 (2023). Next: 2022 Round 1.*

---

# Paper 4 — 2022 UKChO Round 1 (54th IChO selection)

*6 questions, 86 marks, 2 h → ≈ 1.4 min per mark. Marks: Q1 = 9, Q2 = 9, Q3 = 24, Q4 = 13, Q5 = 19, Q6 = 12.*

## Q1 — E10 petrol (9 marks)

### (a) 2,2,4-Trimethylpentane
**L1 · Answer** (CH₃)₃C–CH₂–CH(CH₃)₂: a pentane backbone with two methyls on C2 and one on C4 (SMILES `CC(C)CC(C)(C)C`).
**L2 · Thought** Name → structure drill: longest chain 5, substituents at 2,2,4. "Iso-octane" is the anti-knock reference — context tells you the branching must be extreme.

### (b) Photosynthesis
**L1 · Answer** 6 CO₂ + 6 H₂O → C₆H₁₂O₆ + 6 O₂. (Audit: C 6=6; H 12=12; O 18 = 6+12 ✓.)
**L2 · Thought** Glucose is C₆H₁₂O₆; O comes out as O₂. The equation is the reason ethanol's CO₂ is later "offset" (g) — the carbon was atmospheric to begin with.

### (c) Anaerobic fermentation
**L1 · Answer** C₆H₁₂O₆ → 2 C₂H₅OH + 2 CO₂. (Audit: C 6 = 4+2 ✓; H 12 = 12 ✓; O 6 = 2+4 ✓.)
**L2 · Thought** No O₂ (anaerobic → wording audit). The ethanol:CO₂ 1:1 molar ratio is reused conceptually in (g).

### (d) Enthalpy of combustion of octane (bond enthalpies)
**L1 · Answer** C₈H₁₈ + 12.5 O₂ → 8 CO₂ + 9 H₂O.
Broken: 7 C–C + 18 C–H + 12.5 O=O = 7(347) + 18(413) + 12.5(498) = 16 088 kJ
Formed: 16 C=O + 18 O–H = 16(805) + 18(464) = 21 232 kJ
ΔcH = 16 088 − 21 232 = **−5144 kJ mol⁻¹**
**L2 · Thought** Count structure, not formula alone: any C₈H₁₈ isomer has exactly 7 C–C and 18 C–H — *that* is why the method cannot distinguish isomers (the stem's hint). Sign check: formed > broken → exothermic ✓. (The printed fallback −6666 rescues consequential marks in (e)–(f); this value is the bond-enthalpy estimate, not the calorimetric one.)

### (e) Energy from 1 L of E10 and E5
**L1 · Answer**
E10: n(ethanol) = 100 × 0.789/46.07 = 1.713 mol → 2186 kJ; n(octane) = 900 × 0.703/114.23 = 5.539 mol → 28 492 kJ. **Total ≈ 3.07 × 10⁴ kJ (30 678 kJ).**
E5: n(ethanol) = 50 × 0.789/46.07 = 0.856 mol → 1093 kJ; n(octane) = 950 × 0.703/114.23 = 5.847 mol → 30 075 kJ. **Total ≈ 3.12 × 10⁴ kJ (31 168 kJ).**
**L2 · Thought** Volume → mass → moles → energy, two lanes per fuel. Note ethanol carries only ~7 % of E10's energy — the energy is dominated by the hydrocarbon, which is why (f) comes out close to 100 %.

### (f) E10 energy as % of E5
**L1 · Answer** 30 678/31 168 × 100 % = **98.4 %**.
**L2 · Thought** E10 releases marginally *less* energy per litre (ethanol has lower energy density than octane and displaces 5 % of it). A >100 % answer here would mean you compared per mole instead of per litre.

### (g) E10 CO₂ as % of E5 (octane only)
**L1 · Answer** CO₂ ∝ moles of octane isomers: 5.539/5.847 × 100 % = **94.7 %**.
**L2 · Thought** Ethanol's CO₂ is excluded (offset by growth) — so the ratio is just the octane mole ratio; the factor 8 (C per octane) cancels. The pedagogical point: E10 burns ~5 % less fossil carbon per litre even though it delivers ~98 % of the energy.

---

## Q2 — Nitrous oxide (9 marks)

### (a) Dot-and-cross of HNO₂
**L1 · Answer** Electron budget: 1 + 5 + 12 = 18 e⁻. Skeleton H–O–N=O: single bond H–O, single bond O–N, double bond N=O; lone pairs: 2 on the O–H oxygen, 1 on N, 2 on the terminal O. Formal charges all zero. (cis/trans about the O–N bond exists; one structure suffices.)
**L2 · Thought** Alternative N-centred skeletons (H–N(=O)–O) give formal charges and put H on N — the OH-on-nitrogen form is preferred because nitrous acid is an O–H acid (it *donates* the hydroxyl proton). Count first, then minimise formal charge, then sanity-check against chemistry.

### (b) Formula of A
**L1 · Answer** Per 100 g: H 1.60 g → 1.587 mol; N 22.23 g → 1.587 mol; O 76.17 g → 4.761 mol. Ratio H : N : O = 1 : 1 : 3 → **A = HNO₃** (nitric acid).
**L2 · Thought** "Reacts with O₂ to form A" + the analysis → HNO₂ is simply oxidised to HNO₃ (2 HNO₂ + O₂ → 2 HNO₃). Then NH₃ + HNO₃ → ammonium nitrate — and NH₄NO₃ decomposing to N₂O + 2 H₂O is the famous industrial/lab preparation of laughing gas. The whole route is then obvious in hindsight: [B⁺][C⁻] = NH₄NO₃.

### (c) Ions B⁺ and C⁻ with shapes
**L1 · Answer** **B⁺ = NH₄⁺, tetrahedral** (4 N–H bonds, no lone pair); **C⁻ = NO₃⁻, trigonal planar** (three N–O bonds, no lone pair on N; draw one N=O and two N–O⁻ with resonance, or three equivalent bonds).
**L2 · Thought** VSEPR domain counting, stated with the shape word ("tetrahedral", "trigonal planar") — the command is *draw … clearly showing their shape*, so the 3-D arrangement must be legible (wedges for NH₄⁺, planar trigonal for NO₃⁻). Thermal decomposition NH₄NO₃ → N₂O + 2 H₂O is the atom-audit that closes the scheme: N₂H₄O₃ → N₂O + 2 H₂O ✓.

### (d) D, E, F, X
**L1 · Answer** 2 HNO₂ → D + E + H₂O: balance: N 2, so D and E carry one N each; H 2 → H₂O ✓; O 4 − 1 = 3 shared: **D = NO, E = NO₂** (the brownish-red gas) — check: 2 HNO₂ → NO + NO₂ + H₂O ✓.
**X = N₂O₄** (colourless, in equilibrium with brown NO₂: 2 NO₂ ⇌ N₂O₄).
**F = N₂O₃**: D + E → NO + NO₂ ⇌ N₂O₃ ✓, which decomposes as printed, "F thermally decomposes to nitrous oxide and oxygen": **N₂O₃ → N₂O + O₂** (atom audit: N 2 = 2 ✓, O 3 = 1 + 2 ✓ — note each mole of N₂O₃ releases a full mole of O₂; the doubled form would be 2 N₂O₃ → 2 N₂O + 2 O₂, and writing only one O₂ against two N₂O₃ fails the oxygen audit). So **F = N₂O₃**.
**L2 · Thought** Solve as a jigsaw with constraints, hardest first: the brownish-red gas is the fingerprint of NO₂ (and its colourless dimer N₂O₄ is the named equilibrium partner — that is X for free). Then 2 HNO₂ − H₂O leaves N₂O₃ to split as NO + NO₂ (D + E), and the only stable nitrogen oxide that re-forms from NO + NO₂ is N₂O₃ (F). The final decomposition 2 N₂O₃ → 2 N₂O + O₂ is the audit.

### (e) Structure of N₂O
**L1 · Answer** N≡N⁺–O⁻ ↔ ⁻N–N⁺≡O: linear, central N. Draw both major resonance forms (electron budget 16 e⁻: N≡N⁺–O⁻ with central N formal +1, terminal O −1).
**L2 · Thought** Same 16-electron count as NO₂⁺/CO₂ (isoelectronic with CO₂ — hence linear). The asymmetry (N at the middle, stated in the stem) is what makes the two resonance forms non-equivalent; both should be shown for full marks.

---

## Q3 — Cubane (24 marks)

### (a) Molecular formula of cubane
**L1 · Answer** **C₈H₈** (8 vertices, each CH).
**L2 · Thought** Count vertices of the cube: 8 corners × CH. DBE = (16 + 2 − 8)/2 = 5 — five rings packed into one frame; that impossible strain is the whole point of the molecule.

### (b) ¹³C NMR peak counts
**L1 · Answer** (orbit sets given for the ring carbons, cube vertices at (±1,±1,±1))
- (i) Cubane: **1** (full O_h symmetry: all 8 C one orbit).
- (ii) Cubane-carboxylic acid: **5** — ring orbits {C1} (ipso), {C2,C6}, {C3,C5}, {C4} (mirror planes through the C1–C4 axis), plus {COOH}.
- (iii) 1,2-dicarboxylic acid: **4** — substituted edge C1=(1,1,1), C2=(1,1,−1). Symmetries: σ_z (z→−z, swaps C1↔C2) AND the diagonal mirror σ_d (x↔y, fixes both). Ring orbits: {C1,C2}; the four side vertices {(±1,∓1,±1)} merged into ONE orbit by the two mirrors together; the far edge {(−1,−1,±1)} one orbit; plus {COOH} → 3 + 1 = **4**.
- (iv) 1,3-dicarboxylic acid: **5** — face-diagonal substitution C1=(1,1,1), C3=(−1,−1,1). Symmetries: σ_d (x↔y, fixes both) and σ_v (swaps C1↔C3). Ring orbits: {C1,C3}; the two top vertices adjacent to both substituents {(1,−1,1),(−1,1,1)}; the bottom-diagonal pair {(1,1,−1),(−1,−1,−1)}; the remaining bottom pair {(1,−1,−1),(−1,1,−1)}; plus {COOH} → 4 + 1 = **5**.
- (v) 1,4-dicarboxylic acid: **3** — body-diagonal (D₃d): {C1,C4}, {the other six vertices}, {COOH}.

**L2 · Thought** Method: for each isomer find ALL symmetry operations of the substituted cube, orbit the carbons under them, count orbits; the COOH carbons merge into one orbit whenever the substituents are symmetry-related. The designed trap is 1,2-: a *single* mirror (the one swapping the two substituted vertices) gives 5 ring-orbits, but a **second, diagonal mirror** (x↔y) also survives the substitution and merges the four side vertices into one orbit → 4, not 5. The §7.3 whole-molecule automorphism rule in its purest form: equivalence verdicts need *every* global symmetry operation, not the first one found — a missed operation over-splits orbits and over-counts signals (the 1,2- and 1,3- answers 4 and 5 rest on the second mirror).

### (c) A and B
**L1 · Answer**
- **A** = cyclopentanone ethylene ketal: 1,4-dioxaspiro[4.4]nonane (C₇H₁₂O₂ ✓ = cyclopentanone + HOCH₂CH₂OH − H₂O).
- **B** = 3,3,4-tribromo derivative (one β-CH₂ carries two Br, the other one Br; by the molecule's mirror symmetry C3 and C4 are equivalent, so a single connectivity): C₇H₉O₂Br₃ ✓. All three Br sit on the two β-carbons — each Br is three bonds from both oxygens (O–C(ketal)–Cα–Cβ–Br ✓).
**L2 · Thought** Bromination of a ketone ketal goes α to the carbonyl *position* — but the carbonyl is masked, so Br₂ brominates the carbons α to the ketal carbon... wait, the constraint given is "three bonds from both oxygens": O–C1–Cα–Cβ means the β-carbons — the ketal carbon's α positions are the two CH₂'s adjacent to it; the next carbons out are β. Three Br on two equivalent β-carbons: the only unique answer. Then excess NaOH does double dehydrohalogenation to install the diene of C — this is why the synthesis needs Br there at all (bromine as a placeholder for the double bonds).

### (d) W and X (Diels–Alder)
**L1 · Answer**
- **W** = 1,2,5-trimethylcyclohex-1-ene: 2,3-dimethylbutadiene (diene) + propene (dienophile); the new ring carries the two diene methyls on the alkene carbons and the propene methyl on a saturated ring carbon (one regioisomer only, by the diene's symmetry).
- **X** = 2,3-dibromobicyclo[2.2.1]hept-5-ene (norbornene framework): cyclopentadiene as diene + Br–CH=CH–Br as dienophile; the two Br sit on the two saturated bridge carbons (from the dienophile), **endo** (pointing toward the C7 bridge, per the endo rule).
**L2 · Thought** Diels–Alder decoding routine: the diene's two termini form the new σ-bonds; the diene's internal C=C survives as the product's only double bond; everything on the dienophile ends up on the two saturated ring carbons. Stereochemistry: endo (electron-withdrawing groups under the bridge) is the default major product — state it even when not explicitly asked.

### (e) Starting material Y
**L1 · Answer** **Y = cyclohexa-1,3-diene**. The drawn dimer is the DA dimer: one molecule acts as diene (its ring supplies the bicyclo[2.2.2]octene bridge: the –CH₂–CH₂– bridge), the other as dienophile (its unreacted C=C remains as the bottom cyclohexene ring fused across the new bond).
**L2 · Thought** Retro-DA: find the product's cyclohexene that contains the *diene-derived* double bond (top of the cage), break the two σ-bonds at its other end — the 4-carbon diene fragment still has a –CH₂–CH₂– tether closing a six-membered ring → cyclohexadiene. The bottom ring (with its own C=C) is the second Y molecule, whose surviving double bond confirms Y had two.

### (f) Intermediate C
**L1 · Answer** C = **the bromocyclopentadiene spiro ketal**: the cyclopenta-2,4-diene ring with the **sp³ ketal carbon** as ring C1 (the spiro dioxolane carbon, bonded to both oxygens — it can carry no Br) and the surviving Br on an **sp² diene carbon**, C₇H₇O₂Br ✓. (From B by two dehydrohalogenations: 2 × HBr out installs the two C=C of the cyclopentadiene; one Br remains on a double bond. Naming note: writing "5-bromo-...-5,5-ethylene ketal" would put Br and both oxygens on the same sp³ carbon — impossible; the Br sits on a diene carbon, with its exact position read from the scheme's drawing.)
**L2 · Thought** Formula audit: B (C₇H₉O₂Br₃) − 2 HBr = C₇H₇O₂Br ✓ exactly. DBE check: 2 C=C + 2 rings (cyclopentadiene + dioxolane) = 4 ✓. The diene is *masked cyclopentadienone* — that is the synthetic logic: cyclopentadienone itself is too reactive to isolate, so it is carried as the ketal. C then does what cyclopentadiene always does: dimerise by Diels–Alder (one molecule as diene, one as dienophile) → the drawn cage D.

### (g) Favorskii: electrophilic carbon(s)
**L1 · Answer** Circle **both the carbonyl carbon and the α-carbon bearing Br** (on the α-bromoketone in the general scheme).
**L2 · Thought** Favorskii mechanism: hydroxide attacks the carbonyl C (electrophile #1) forming a cyclopropanone-like intermediate, and the C–Br carbon is the one that gets displaced/rearranged (electrophile #2) — the two electrophilic centres are what the semibenzilic rearrangement stitches together. (Simply deprotonating the α′-CH is the base's role; the *carbons* being attacked/rearranged are the answer.)

### (h) E and F
**L1 · Answer**
- **E** = the **diketone cage**: D with both ethylene ketals hydrolysed off (H₃O⁺): the two ketal carbons become C=O; the cage keeps its two C=C and two Br (C₁₀H₆O₂Br₂ ✓ = D − 2 × C₂H₄O).
- **F** = the **[2+2] photocycloadduct**: under UV the two C=C in the same cage snap together intramolecularly, closing **two cyclobutane rings** (C₁₀H₆O₂Br₂ — same formula, intramolecular isomerisation ✓); IR 1795 cm⁻¹ = strained cyclobutanone C=O ✓.
**L2 · Thought** "Intramolecularly" + "two four-membered rings" is the entire instruction: the two alkenes in E's cage are held face-to-face (the classic [2+2] geometry of the dicyclopentadiene skeleton), so UV does a [2+2] cycloaddition. This is Eaton's cubane strategy: build the strain gradually — Diels–Alder for the 6-ring cage, [2+2] for the 4-rings, Favorskii for the final ring contraction.

### (i) G and H
**L1 · Answer**
- **G** = cubane-1,4-dicarbonyl dichloride (both COOH → COCl with SOCl₂).
- **H** = the **bis-perester**: cubane-1,4-dicarbonyl di-tert-butyl diperoxide, C₁₈H₂₄O₆ ✓ (cubane-(C(=O)–O–O–C(CH₃)₃)₂: C 8+2+8 = 18 ✓; H 6+18 = 24 ✓; O 6 ✓). Heating H ejects 2 CO₂ and pairs the two cubyl radicals with loss of the two tert-butoxy/alcohol units → cubane + tBuOH + CO₂ (the drawn products).
**L2 · Thought** Formula audit makes (i) mechanical: H = C₁₈H₂₄O₆ with 6 oxygens can only be the diacyl diperoxide (each –CO–O–O–tBu contributes 3 O ✓). The decarboxylation of diacyl peroxides on heating is the standard way to strip carboxyls off a strained cage where direct decarboxylation would fail — a named-reaction baton pass (diacyl peroxide thermolysis).

### (j) Q, R, S, T (barrelene route)
**L1 · Answer**
- **Q** = the Diels–Alder adduct of **cis-3,5-cyclohexadiene-1,2-diol** (the drawn starting diol — note the two OH on *adjacent sp³* carbons and the two ring C=C) with **dimethyl acetylenedicarboxylate (DMAD)**: bicyclo[2.2.2]octa-2,5-diene bearing the cis vicinal diol on the saturated two-carbon bridge and the C(CO₂Me)=C(CO₂Me) bridge (C₁₂H₁₄O₆ ✓ = C₆H₈O₂ + C₆H₆O₄).
- **R** = the **cyclic thiocarbonate**: Q's vicinal diol + the thiocarbonyl diimidazole reagent → the –O–C(=S)–O– bridge across the two former OH oxygens (C₁₃H₁₂SO₆ ✓ = Q + C=S − H₂).
- **S** = **CO₂** (the gaseous product of the Corey–Winter elimination).
- **T** = **dimethyl bicyclo[2.2.2]octa-2,5,7-triene-2,3-dicarboxylate** (dimethyl barrelene-1,2-dicarboxylate, C₁₂H₁₂O₄ ✓): the Corey–Winter reagent (the diazaphospholidine shown) strips the thiocarbonate as CO₂ + P(=S) by-product, forming the third C=C of the barrelene; NaOH then hydrolyses the two esters to the drawn barrelene-1,2-dicarboxylic acid.
**L2 · Thought** The formula audit chain is what makes this solvable: R → T loses exactly **CSO₂** (= CO₂ + S), and the phosphorus by-product carries exactly one S — that pins S = CO₂ (a gas, as stated) and identifies the R→T step as a Corey–Winter olefination (cyclic thiocarbonate + trivalent phosphorus → alkene + CO₂ + P=S). The thiocarbonyl transfer reagent (thiocarbonyl diimidazole) is what converts a vicinal diol into the thiocarbonate. The deep design point: the diol's two sp³ carbons (visible in the starting material — *not* catechol, whose OHs are on an aromatic ring) are the future third double bond of the barrelene — read the starting material's saturation carefully before assuming "benzene + diol = catechol".

---

## Q4 — Coronavirus lateral flow test (13 marks)

### (a) Purpose of Na₂HPO₄/KH₂PO₄ (tick)
**L1 · Answer** **Make a buffered solution** (a weak-acid/conjugate-base pair at pH 7.4 ≈ physiological).
**L2 · Thought** H₂PO₄⁻/HPO₄²⁻ is the textbook phosphate buffer (pKa₂ ≈ 7.2). The two salts alone can never make "very acidic" or "very alkaline" — they are the weak acid/base pair itself.

### (b) pH after adding 1.0 cm³ of 0.10 mol dm⁻³ HCl (tick)
**L1 · Answer** **Very acidic** — capacity audit: the added strong acid (1.0 × 10⁻⁴ mol) overwhelms the buffer's base (HPO₄²⁻ present = 7.3 × 10⁻³ mol dm⁻³ × 1.0 cm³ = 7.3 × 10⁻⁶ mol, ≪ 1.0 × 10⁻⁴); excess [H⁺] ≈ (1.0 × 10⁻⁴ − 7.3 × 10⁻⁶)/(2.0 × 10⁻³ dm³) ≈ 4.6 × 10⁻² mol dm⁻³ → pH ≈ 1.3.
**L2 · Thought** This is the capacity audit (§4): a buffer only resists acid *up to* its capacity — compare moles of strong acid to moles of buffer base **before** ticking "pH stays". The "buffers always win" instinct gives the wrong tick (pH 7.4) here; the two-line mole comparison gives the right one. (Had the acid been 10⁻⁴ mol dm⁻³ instead of 10⁻¹, the buffer would indeed have held ~pH 7.4 — the audit, not the label, decides.)

### (c) [SP] in the test sample
**L1 · Answer** 7.1 × 10⁶ virus particles cm⁻³ × 20 spike proteins = 1.42 × 10⁸ SP cm⁻³
[SP] = 1.42 × 10⁸/(6.022 × 10²³) × 10³ = **2.36 × 10⁻¹³ mol dm⁻³**.
**L2 · Thought** Two unit conversions, both shown: particles → moles (Nₐ) and cm⁻³ → dm⁻³ (×10³). The fallback value 1.0 × 10⁻¹¹ confirms the magnitude (ours is smaller — the fallback is for a broken chain).

### (d) [SPNP] at equilibrium
**L1 · Answer** [NP]₀ = 1.6 × 10¹² cm⁻³ × 10³/(6.022 × 10²³) = 2.66 × 10⁻⁹ mol dm⁻³ (≫ [SP]₀ → treated as constant). With x = [SPNP], the mass balance [SP] = [SP]₀ − x inside K = x/([NP]₀([SP]₀ − x)) gives
$$x = \frac{K[NP]_0}{1 + K[NP]_0}\,[SP]_0 = \frac{31.9}{32.9} \times 2.36\times10^{-13} = 0.97\,[SP]_0 = \mathbf{2.29\times10^{-13}\ mol\ dm^{-3}}$$
**L2 · Thought** The license "NP in excess" makes [NP] constant — but NOT [SP]: the binding constant is so strong (K[NP]₀ = 32 ≫ 1) that 97 % of the SP is consumed, so the mass balance on SP is compulsory. Writing [SPNP] = K[NP][SP]₀ gives 7.5 × 10⁻¹² mol dm⁻³ — which *exceeds the total SP available* (2.36 × 10⁻¹³) and convicts itself. That is the competitive-occupancy move's own failure boundary (§4: "inventory comparable to demand → explicit mass-balance"); this item is the canonical demonstration. (The intended value: 2.29 × 10⁻¹³ ✓.)

### (e)(i) Antibodies on the test strip
**L1 · Answer** Area = 3.0 × 1.0 = 3.0 mm²; AB = 3.0 × 1.2 × 10⁹ = **3.6 × 10⁹ antibodies**.
### (e)(ii) SP and SPNP in a strip-sized volume
**L1 · Answer** V = 3.0 × 1.0 × 0.10 mm³ = 0.30 mm³ = 3.0 × 10⁻⁷ dm³.
SPNP: 2.29 × 10⁻¹³ mol dm⁻³ × 3.0 × 10⁻⁷ dm³ = 6.9 × 10⁻²⁰ mol → **4.1 × 10⁴ particles** (4.13 × 10⁴).
Free SP: [SP] = (2.36 − 2.29) × 10⁻¹³ = 7 × 10⁻¹⁵ mol dm⁻³ → 2.1 × 10⁻²¹ mol → **1.3 × 10³ proteins**.
**L2 · Thought** Volume unit ladder: mm³ → cm³ (÷10³) → dm³ (÷10³ again) — most errors in this question live in these conversions; write the ladder explicitly once and reuse it. Note the free-SP number comes from a *difference of close quantities* — keep full precision upstream (the scheme flags this: "7 × 10⁻¹⁵ if full accuracy not maintained").

### (f) Nanoparticles immobilised on the test strip
**L1 · Answer** Surface mass-balance with depletion: if y SPNP bind, [SPNP] falls as [SPNP]₀ − y/V; the capture equilibrium σ_ABSPNP/σ_AB = K[SPNP] then gives y(1 + K·σ_AB·A/V)-type bookkeeping — and since K·σ_AB·A/V ≫ 1 (the antibody sites are in vast excess: 3.6 × 10⁹ sites vs ~10⁷ particles), essentially **every SPNP that reaches the strip is captured**: y ≈ [SPNP]₀ × V × Nₐ with V = 0.10 cm³ of sample:
$$y = 2.29\times10^{-13}\ \text{mol dm}^{-3} \times 1.0\times10^{-4}\ \text{dm}^3 \times 6.022\times10^{23} = \mathbf{1.38\times10^{7}\ ABSPNP}$$
**L2 · Thought** The intended model is **inventory depletion**, not equilibrium occupancy: the strip sees the whole 0.10 cm³ sample flow past, and the antibodies are in such excess (K·σ·A/V ≫ 1) that capture is quantitative — the answer is simply "all the SPNP in one sample volume". (A Langmuir-occupancy estimate gives ~7 × 10⁸ — 50× too large — precisely because it assumes concentrations are maintained rather than depleted; this is the §4 competitive-occupancy failure boundary firing on schedule: sites shared but *inventory limited* → switch to mass balance.) The intended answer: 1.38 × 10⁷ ✓.

### (g) Minimum virus particles for a positive test
**L1 · Answer** This test deposits 1.38 × 10⁷ ABSPNP on 3 mm² → density 4.59 × 10⁶ mm⁻², from 7.1 × 10⁵ virus particles per sample. Visibility needs 3 × 10⁶ mm⁻², and deposition is proportional to viral loading:
$$N_{min} = 7.1\times10^{5} \times \frac{3\times10^{6}}{4.59\times10^{6}} = \mathbf{4.6\times10^{5}\ virus\ particles}$$
**L2 · Thought** Minimum-detectable-amount scaling (§4): threshold signal ÷ signal per unit analyte × reference amount — all in *densities* here (the 3 mm² cancels). The proportionality assumption (capture stays quantitative at lower loading) is even safer than at full loading, since the sites remain in excess. Intended value: 4.64 × 10⁵ ✓.

---

## Q5 — The smallest Chinese knot (19 marks)

### (a)(i) Structure of A
**L1 · Answer** **3-fluorophenol** (F meta to OH). Nitration then puts NO₂ para to the –OH (director of choice), giving 3-fluoro-4-nitrophenol.
### (a)(ii) The active electrophile
**L1 · Answer** The **nitronium ion, NO₂⁺** (generated from HNO₃/H₂SO₄ — exactly the Q1-2025 chemistry: 2 H₂SO₄ + HNO₃ ⇌ NO₂⁺ + H₃O⁺ + 2 HSO₄⁻).
**L2 · Thought** Mixed acid → NO₂⁺ is the stock answer; the question's phrasing "active electrophile *formed*" is asking for the ion, not the mixture. Regiochemistry note: –OH is the dominant director (para), F the weaker one — the product's substitution pattern is the evidence for which starting isomer A is.

### (b) Structure of B
**L1 · Answer** Analysis: C 51.81/12.01 = 4.314; H 3.62/1.008 = 3.591; N 10.07/14.01 = 0.7188 → ratio 6 : 5 : 1; residual mass per N = 139.1 − 91.1 = 48.0 = 3 O → **B = C₆H₅NO₃ = 4-nitrophenol** (NO₂ para to OH, as retained in the product).
**L2 · Thought** The analysis permits *only* a nitrophenol (any halogenated precursor fails the C% — check: 3-chloro-4-nitrophenol would give 41.5 % C). The para NO₂/OH relationship in the product then selects the 4-isomer. The KF/Cu step is a copper-mediated oxidative *ortho* C–H fluorination of the electron-poor phenol (KF as the F source); the two ortho positions of 4-nitrophenol are equivalent, so a single fluoro isomer results. Note the contrast with route A: A introduces NO₂ *into* a fluoroarene; B introduces F *into* a nitroarene — same target, orthogonal orders.

### (c)(i) Structure of C
**L1 · Answer** The phenol O-alkylated with 6-bromohex-1-ene (the drawn reagent): **1-(hex-5-en-1-yloxy)-3-fluoro-4-nitrobenzene** (O–CH₂CH₂CH₂CH₂CH=CH₂ at C1, F at C3, NO₂ at C4).
### (c)(ii) Structure of D
**L1 · Answer** **3-(R-amino)-4-nitrophenyl hex-5-en-1-yl ether**: RNH– replaces the aryl F.
**L2 · Thought** Site-selection: the aryl fluorine is *ortho* to NO₂ — classic activated SNAr (Meisenheimer stabilisation by the para/ortho nitro group), so the amine displaces F, not the alkyl bromide's chemistry (already used) and not the nitro group. The terminal alkene is the metathesis handle needed later (the stem says the strand ends are joined by alkene metathesis — spot it early and every ether linkage makes sense).

### (d) Compound E and reagent G
**L1 · Answer**
- **E** = the **benzimidazole-bearing bromopyridine**: 2-bromo-6-(1-R-5(6)-(hex-5-en-1-yloxy)-1H-benzimidazol-2-yl)pyridine. Formed because Na₂S₂O₄ reduces D's ArNO₂ to ArNH₂, giving an *ortho*-diamine (RNH– and –NH₂ adjacent), which condenses with the reagent's aldehyde (6-bromopyridine-2-carbaldehyde) and cyclodehydrates to the benzimidazole (R on the imidazole N, as in F).
- **G** = **2,6-dibromo-4-(dimethylamino)pyridine**: the strand's central unit is a 4-dimethylamino-pyridine flanked on both 2,6-positions by thiazolothiazoles; two molecules of F (each contributing one thiazolothiazole-pyridine-benzimidazole half) couple onto G's two bromides under the same Pd mix that coupled E's bromide with thiazolothiazole.
**L2 · Thought** Repeat-unit back-reading again: the strand is a dimer of two F halves about a central pyridine — find the *new* bonds (the two thiazolothiazole–pyridine links either side of the central NMe₂-pyridine) and the precursor of the central fragment must carry the two leaving groups: 2,6-dibromo. The NMe₂ on the central ring is read straight off the drawn strand. The same "Pd catalyst mix" twice is the hint that both steps are the same coupling (direct arylation of the thiazolothiazole C–H with an aryl bromide).

### (e) The primary amine RNH₂
**L1 · Answer** **3-methylbutan-1-amine** (isopentylamine), H₂N–CH₂–CH₂–CH(CH₃)₂.
Assignment: 3.26 ppm (2H, dt) = N–CH₂ (triplet from CH₂, doublet from NH); 1.63 (2H, dt) = middle CH₂; 1.77 (1H, m) = CH; 0.98 (6H, d) = two equivalent CH₃ on one CH.
**L2 · Thought** Read the table from the high-field end: a 6H doublet demands an isopropyl group (CH with two identical CH₃); the CH attached to it (1H, m) then two CH₂'s, one of them deshielded (3.26) by N. n+1 rule: CH₂–CH₂–CH–(CH₃)₂ gives dt/dt/m/d exactly as listed. The 3.26 "doublet of triplets" (not plain triplet) is the N–H coupling clue that places this CH₂ directly on nitrogen.

### (f) Metal ions and coordinating atoms on the strand
**L1 · Answer** Each metal ion sits in a **tridentate N₃ pocket** formed where two strands cross: per pocket, the donors are the **pyridine N, the benzimidazole imine N (the =N–), and one thiazole N of the thiazolothiazole unit**. Each metal is bound by two such pockets (one from each crossing strand) → 6 N donors in total. (Drawn as circled M at each crossing with arrows from the three N atoms of each pocket.)
**L2 · Thought** The strand's architecture is a periodic ligand: pyridine–benzimidazole–thiazolothiazole repeats — each repeat presents three convergent nitrogen lone pairs (terpyridine-like pocket). Terpyridine-type N₃ pockets + first-row divalent metal = the programmed cross-points of the weave. The dimethylamino group is a donor *base* but not part of the pocket geometry (it modifies solubility/electronics).

### (g) Coordination geometry (tick)
**L1 · Answer** **Octahedral** (6 N donors: two tridentate pockets at ~90° to each other).
**L2 · Thought** Two tridentate chelates on one metal = 6 coordinate; Fe(II)/terpyridine-type pockets give near-regular octahedra (this is also what makes the grid rigid enough to weave).

### (h) M²⁺ and X⁻
**L1 · Answer** **M²⁺ = Fe²⁺**; **X⁻ = BF₄⁻, tetrafluoroborate**, drawn tetrahedral (B centre, 4 F at corners).
Audit: NaOH → green precipitate turning brown on standing = Fe(OH)₂ oxidising to Fe(OH)₃ (the iron fingerprint); X⁻ tetrahedral, mononegative, two elements, no oxygen → BF₄⁻; mass check: Fe(BF₄)₂·6H₂O: M = 55.85 + 2(86.81) + 6(18.02) = 337.6; waters = 108.1/337.6 = **32.0 %** ✓ exactly.
**L2 · Thought** Solve by the hardest constraint first: "green → brown precipitate" is diagnostic of Fe²⁺ (no other first-row ion gives that colour sequence). Then the 32.0 % water mass loss is a pure arithmetic lock on the full formula — always convert a mass-loss clue into a formula check rather than trying to fit water counts by trial.

### (i) Which structures form from each connection pattern
**L1 · Answer** (Number the ends 1–12 clockwise around the perimeter: 1–3 = tops of the three vertical strands, 4–6 = right ends of the three horizontal strands, 7–9 = bottoms of the vertical strands (right→left), 10–12 = left ends of the horizontal strands (bottom→top). Trace components by following each strand through its connections.)
- **(i) (1,2)(3,4)(5,6)(7,8)(9,10)(11,12) → Chinese knots**: all six strands join into ONE closed serpentine component, and the closure arcs weave it into the knot (the panchang/7₄-type topology of the rope knot).
- **(ii) (1,2)(4,5)(6,7)(8,9)(10,11), 3 & 12 unjoined → individual rings + linear molecules**: the two vertical strands V1–V2 are joined at *both* ends → a closed ring; the remaining strands form one open chain (V3–H3–H2–H1) with ends 3 and 12 free → linear molecule.
- **(iii) (1,2)(3,4)(5,6)(8,9)(10,11), 7 & 12 unjoined → two interlinked rings** (plus a short open chain V3–H1): V1–V2 close into one ring, H2–H3 close into a second ring threaded through the first by the weave's over/under pattern → a 2-component link.
- **(iv) (2,3)(4,5)(6,7)(8,9)(10,11)(12,1) → individual rings**: the shifted closure also gives one closed serpentine component, but its closure arcs let it untwist to a plain ring (an unknot, not the Chinese knot).
**L2 · Thought** Method over memorisation: (1) draw the 12 ends around the perimeter; (2) trace each connection and count **components** — one closed component containing all strands is the *candidate* for the knot, two closed components is a link candidate, any free end means linear molecules; (3) only then ask about over/under: the knot requires the single component to carry the full over-under-over sequence of the weave — which is why (i) (whose closure continues the weave's own alternation) gives the knot while (iv) (whose shifted arcs cancel the twist) collapses to an unknot. The metathesis constraint "adjacent ends only" is what makes some patterns unreachable — a nice case of a *chemical* constraint (ring strain/proximity) shaping a *topological* outcome.

---

## Q6 — Storing vaccines: ensilication (12 marks)

### (a) Processes 1 and 2
**L1 · Answer**
Process 1: Si(OCH₂CH₃)₄ + 4 H₂O → Si(OH)₄ + 4 CH₃CH₂OH
Process 2: Si(OH)₄ → SiO₂ + 2 H₂O
**L2 · Thought** Hydrolysis swaps every –OEt for –OH (atom audit: Si 1=1; O 4+4 = 4+4 ✓; the ethanol takes the ethoxy groups intact — do not oxidise it). Condensation/dehydration then eliminates water to give the network oxide.

### (b) ΔH° for SiO₂ + 6 NaF + 6 HCl → H₂SiF₆ + 6 NaCl + 2 H₂O
**L1 · Answer** Target = (reaction 2) + 6 × (NaOH + HCl → NaCl + H₂O) − 6 × (NaOH + HF → H₂O + NaF):
ΔH° = −100.3 + 6(−56.7) − 6(−61.5) = **−71.5 kJ mol⁻¹**
(audit: the 6 HF and 6 NaOH cancel; waters: 2 + 6 − 6 = 2 ✓).
**L2 · Thought** Build the Hess cycle by identifying the "exchange" species: the target has NaF and HCl where the given set has HF and NaOH — the two neutralisations interconvert them. Write the target first, then hunt multipliers; verify cancellation species-by-species before trusting the number.

### (c) ΔH° and ΔS° for process 2
**L1 · Answer** K_eq = 1/[Si(OH)₄] → ln K_eq = −ln[Si(OH)₄] = −(−1680/T − 0.605) = **+1680/T + 0.605**.
Match to ln K = −ΔH°/R · 1/T + ΔS°/R:
ΔH° = −1680 × 8.314 = **−14.0 kJ mol⁻¹**; ΔS° = **+**0.605 × 8.314 = **+5.03 J K⁻¹ mol⁻¹**.
**L2 · Thought** The given ln[Si(OH)₄] expression is for the *reactant*, so negate the **whole** right-hand side to get ln K — including the intercept: −(−0.605) = **+**0.605. (The single most likely error is to flip the 1/T term but not the constant; that sign slip turns ΔS° negative, which then contradicts the data — the intercept of the *given* line is negative, so ΔS°/R = +0.605 comes out positive. Negating only half an expression is the classic sign error; write the negation with brackets before distributing.) A small positive ΔS° is chemically sensible here: dissolving one silicic-acid molecule releases its ordered hydration shell, outweighing the ordering of the solid formed — and the given linear relation is authoritative over intuition either way.

### (d) Constant A
**L1 · Answer** At t = 0 every (1 − Γt/r + Γ²t²/2r²) bracket = 1, so c₀ = 1² + A × 1² → A = 1.56744 − 1 = **0.56744**.
**L2 · Thought** Read the structure of the autocorrelation function before substituting: t = 0 collapses it to c₀ = 1 + A by inspection. No algebra needed if you see the collapse — but write the bracket evaluation once to prove it.

### (e) Slope a and intercept b
**L1 · Answer** f = (c − c₀)/(Γt) = at − b:
f₁ = (1.54289 − 1.56744)/0.170713 = −0.14381; f₂ = (1.51937 − 1.56744)/0.341426 = −0.14079
a = f₂ − f₁ = **3.02 × 10⁻³ nm⁻¹ μs⁻¹**; b = a − f₁ = **0.14683 nm⁻¹**.
**L2 · Thought** The linearisation is given (f = at − b), so this is a two-point line: slope from the difference, intercept by back-substitution. The stem's warning "sensitive to rounding" is operational: carry all 5–6 significant figures through (c₀ and the two c values differ only in the third decimal — premature rounding to 3 s.f. would zero out the signal).

### (f) Radii r₁ and r₂
**L1 · Answer** Set x₁ = 1/r₁, x₂ = 1/r₂: (i) x₁ + A x₂ = b; (ii) x₁² + A x₂² = 2a/Γ = 0.035357 nm⁻².
From (i): x₁ = 0.14683 − 0.56744 x₂; substitute into (ii):
0.88943 x₂² − 0.16664 x₂ − 0.013799 = 0 → x₂ = 0.2495 nm⁻¹ (positive root) → **r₂ = 4.0 nm** (free protein);
x₁ = 0.14683 − 0.56744 × 0.2495 = 5.27 × 10⁻³ nm⁻¹ → **r₁ = 1.9 × 10² nm** (ensilicated particle).
**L2 · Thought** The substitution xᵢ = 1/rᵢ is the given hint — use it: it turns the messy inverse-square system into a linear-plus-quadratic pair with one clean positive root (reject the negative root: radii are positive). Physical anchor: a 4 nm free protein and a ~190 nm silica-loaded particle are exactly the size contrast DLS is bought to resolve; two same-order radii would have made the two-term autocorrelation function pointless.

---

*End of Paper 4 (2022). Next: 2021 Round 1.*

---

# Paper 5 — 2021 UKChO Round 1 (53rd IChO selection)

*6 questions, 85 marks, 2 h → ≈ 1.4 min per mark. Marks: Q1 = 9, Q2 = 9, Q3 = 16, Q4 = 13, Q5 = 21, Q6 = 17.*

## Q1 — Life on Venus: phosphine (9 marks)

### (a) Shape of phosphine
**L1 · Answer** Trigonal pyramidal (like NH₃): P with three P–H bonds and one lone pair; H–P–H ≈ 94–107° (lone pair compresses the tetrahedral angle).
**L2 · Thought** VSEPR domain count (4 domains, 1 lone pair) → pyramidal molecule. Draw the lone pair explicitly — the shape word alone is the mark, but the lone pair is the reason.

### (b)(i) Oxidation states
**L1 · Answer** PH₃: P = **−3**; H₃PO₄: P = **+5**.
### (b)(ii) PH₃ + O₂
**L1 · Answer** PH₃ + 2 O₂ → H₃PO₄. (Audit: P 1=1; H 3=3; O 4=4; electron audit: P climbs 8, 2 O₂ accept 8 ✓.)
**L2 · Thought** Oxidation-state audit before balancing: P goes −3 → +5 (8 e⁻), so 2 O₂ per PH₃ — the electron count writes the equation; the atom count then confirms it.

### (c) Three phosphine preparations
**L1 · Answer**
(i) PCl₃ + 3 LiH → PH₃ + 3 LiCl (hydride as H⁻ source; audit: Cl 3=3, Li 3=3, H 3=3 ✓).
(ii) Ca₃P₂ + 6 H₂O → 2 PH₃ + 3 Ca(OH)₂ (phosphide P³⁻ protonated by water; audit ✓).
(iii) 4 H₃PO₃ → PH₃ + 3 H₃PO₄ (disproportionation: one P(+3) → P(−3), three P(+3) → P(+5); audit: P 4=4; H 12=12; O 12=12 ✓).
**L2 · Thought** For (iii), the word "disproportionation" is the instruction: same element in two oxidation states — choose the available pair (PH₃ = −3, H₃PO₄ = +5) and balance by electron count first (3 × (+5) per 1 × (−3)). For (i), LiH is H⁻ (not H⁺) — PCl₃ is reduced, and the P(−1) intermediates LiPCl₂H etc. all funnel to PH₃.

### (d) The phosphonium salt
**L1 · Answer**
(i) Anion = **SO₄²⁻**.
(ii) Cation = **[P(CH₂OH)₄]⁺**, tetrakis(hydroxymethyl)phosphonium: tetrahedral P with four identical –CH₂OH arms.
Mass audit: salt = [P(CH₂OH)₄]₂SO₄: 2 × 155.11 + 96.06 = **406.28 g mol⁻¹ ✓** (matches 406.272).
NMR audit: ¹³C one signal (four equivalent CH₂OH) ✓; ¹H two signals: CH₂ (non-exchangeable) and OH (exchanges with D₂O) ✓.
**L2 · Thought** PH₃ + methanal under acid is the classic hydroxymethylation: P–H bonds add across C=O four times (PH₃ → P(CH₂OH)₃ → [P(CH₂OH)₄]⁺ by protonation… here direct quaternisation under acid). Solve by constraints, hardest first: the single ¹³C signal demands four equivalent CH₂ groups on one central atom — [P(CH₂OH)₄]⁺ is the unique answer; the D₂O-exchangeable signal then confirms OH's. Only after the cation is fixed does the mass reveal the anion: 406.272 − 2 × 155.11 = 96.06 = SO₄²⁻ (note the salt is 2 : 1, not 1 : 1 — the mass forces that; a bisulfate 1 : 1 salt would be 252.2).

---

## Q2 — Capturing carbon: calcium looping (9 marks)

### (a) Carbonator
**L1 · Answer** CaO + CO₂ → CaCO₃.
### (b) Calciner
**L1 · Answer** CaCO₃ → CaO + CO₂.
**L2 · Thought** The loop is read straight off the diagram: carbonator consumes CO₂ from flue gas (→ CaCO₃), calciner releases pure CO₂ (→ CaO). Name the direction of carbon flow before writing equations — writing the calciner backwards is the classic slip.

### (c) H₂S combustion
**L1 · Answer** 2 H₂S + 3 O₂ → 2 SO₂ + 2 H₂O. (Audit: S 2=2; H 4=4; O 6=6 ✓.)
### (d) SO₂ + CaCO₃ + O₂
**L1 · Answer** 2 SO₂ + 2 CaCO₃ + O₂ → 2 CaSO₄ + 2 CO₂. (Audit: S 2=2; Ca 2=2; C 2=2; O 4+6+2 = 12 = 8+4 ✓.)
**L2 · Thought** "Unreactive impurity" in a limestone loop → the sulfate (CaSO₄, gypsum-like, thermally stubborn). The O₂ term is the tell that S(+4) must be oxidised to S(+6): SO₂ alone with CaCO₃ could only give CaSO₃, which is not "unreactive" enough — the oxygen in the reagent list settles it.

### (e) Pellet reactor
**L1 · Answer** K₂CO₃ + Ca(OH)₂ → CaCO₃ + 2 KOH. (Audit: K 2=2; Ca 1=1; C 1=1; O/H ✓.)
**L2 · Thought** Read the flows: K₂CO₃ enters from the contactor, Ca(OH)₂ from the slaker; CaCO₃ leaves to the calciner, KOH returns to the contactor. Metathesis (no redox) — the loop recycles KOH while the calcium carries the carbon.

### (f) ΔH° of the air contactor reaction
**L1 · Answer** Reaction: CO₂ + 2 KOH → K₂CO₃ + H₂O (printed in the diagram).
ΔH° = [ΔfH(K₂CO₃) + ΔfH(H₂O)] − [ΔfH(CO₂) + 2 ΔfH(KOH)]
= [−1151.2 + (−285.8)] − [−393.5 + 2(−424.8)] = −1437.0 + 1243.1 = **−193.9 kJ**.
**L2 · Thought** The equation is printed inside the reactor box — use it verbatim (wording audit: some will instinctively write CO₂ + KOH → KHCO₃, which the diagram forbids). CaO/CaCO₃/Ca(OH)₂ data are distractors for this part (data audit), but not for (g).

### (g) Sum of the four reactor reactions (tick)
**L1 · Answer** Tick **the statement that the sum is zero** (ΔH° = 0).
**L2 · Thought** State-function logic: the four reactions form a closed cycle — every species is produced once and consumed once (KOH, K₂CO₃, Ca(OH)₂, CaCO₃, CaO, H₂O, CO₂ all cancel), so the net equation is empty and ΔH° = 0. Numerical confirmation using (f)'s data: contactor −193.9 + pellet +80.8 + calciner +178.3 + slaker −65.2 = 0.0 kJ ✓ — the cycle audit and the arithmetic agree, which is the strongest possible check. (The net *process* moves CO₂ from air to storage, but that is physical transfer, not a chemical reaction.)

### (h) Entropy changes (tick two)
**L1 · Answer** Tick: **"The entropy change of the universe is positive"** and **"The entropy change of this direct air capture process is negative"**.
**L2 · Thought** Read the statements' *subject* before any phase accounting — the two ticks are about two different systems. (1) The universe: the DAC plant demonstrably runs (it is a working industrial process driven by the energy input to the calciner), and any feasible real process has ΔS_universe > 0 — the second law is the deciding criterion. (2) The DAC process itself: it takes CO₂ from *dilute* air (~0.04 %) and delivers it *concentrated* — gathering a dispersed gas into an ordered, captured state is a large decrease in the process's entropy. (The per-reactor sign table — calciner ΔS > 0 as CaCO₃(s) → CaO(s) + CO₂(g), contactor ΔS < 0 as CO₂(g) is absorbed, etc. — is real chemistry, but the booklet's statements are not about individual reactors; ticking by reactor answers a question that was not asked. Command-word/statements audit first, phase accounting second.)

---

## Q3 — Levulinic acid from fructose (16 marks)

### (a) Functional groups in levulinic acid (tick)
**L1 · Answer** **Ketone** and **carboxylic acid** (4-oxopentanoic acid, CH₃–CO–CH₂CH₂–COOH).
### (b) Molecular formula
**L1 · Answer** **C₅H₈O₃**.
**L2 · Thought** DBE = 2 (one C=O in the ketone, one in the acid) → C₅H₁₀O₃ minus H₂. The alcohol-looking name misleads some into adding an OH — count from the drawn skeleton.

### (c) Atoms bonded in the cyclic form (circle)
**L1 · Answer** Circle **C2 (the ketone carbonyl carbon)** and **the hydroxyl oxygen on C5** (the C5–OH), which form the hemiketal C–O bond closing the five-membered (furanose) ring.
**L2 · Thought** Ring-size filter: fructose cyclises to a five-membered ring (2,6-anhydro → furanose), so the OH must come from C5, not C6 (a C6–OH would give a six-membered pyranose — glucose's habit, not fructose's here). The cyclic structure printed beside it confirms: ring O at the top between C5 and the anomeric C2.

### (d)(i) Alkene A
**L1 · Answer** A = the **enol** of B: the furanose ring with a C1=C2 double bond — the anomeric carbon (C2, bearing the ring O) joined by a double bond to the exocyclic =CH–OH (former C1); C3, C4 still bear OH, C5 bears CH₂OH. (SMILES: `OC=C1OC(CO)C(O)C1O`.)
**L2 · Thought** The given isomerisation scheme (enol ⇌ keto: R–C(OH)=C–R′ ⇌ R–CO–CH–R′) is the map: B must be the keto form (aldehyde at C1), so A is the corresponding enol — water is lost from C2–OH and a C1–H. The ring's other OH's cannot produce an enol that isomerises to *this* B (a C3=C4 enol would tautomerise to a C3 or C4 ketone, not the C1 aldehyde in B).

### (d)(ii) Other trisubstituted alkenes
**L1 · Answer** Three more eliminations of H₂O from adjacent ring positions:
- **C3=C4 with OH remaining on C4** (lose C3–OH + C4–H);
- **C3=C4 with OH remaining on C3** (lose C4–OH + C3–H);
- **C4=C5** (lose C4–OH + C5–H; C5 bears the CH₂OH arm).
(No C2=C3 alkene is possible: the anomeric C2 has no H to eliminate.)
**L2 · Thought** Enumeration discipline: list every ring bond between two carbons that jointly carry (removable OH) + (removable H); C2–OH can only leave with a C1–H (that is A) because C2 itself is H-less. Each of these is trisubstituted (three non-H substituents on the C=C) — the check filters out the C3=C4-with-both-OH-retained impossibility (that one would be tetrasubstituted and still has both OH's, i.e. no dehydration happened at all).

### (e) Intermediates C and D
**L1 · Answer** B → E loses 2 H₂O; the two eliminations can happen in either order:
- **C**: first lose C3–OH + C2–H → C2=C3 enol-ether (C4 keeps OH): ring = O–C(CHO)=CH–CH(OH)–CH(CH₂OH).
- **D**: first lose C4–OH + C5–H → C4=C5 alkene (C3 keeps OH): ring = O–CH(CHO)–CH(OH)–CH=C(CH₂OH)–.
Each then loses the other H₂O → **E = 5-(hydroxymethyl)furfural (HMF)**: furan ring with –CHO at the 2-position and –CH₂OH at the 5-position (SMILES `O=Cc1ccc(CO)o1`).
**L2 · Thought** Count the unsaturations: E is an aromatic furan (DBE: 2 ring π + ring), so B (one ring, one C=O) must gain two C=C — hence two dehydrations at exactly the positions computed in (d)(ii)'s framework. C and D are the two orderings of those eliminations; note the anomeric C2 regains an H when A tautomerises to B, which is precisely the H spent forming C2=C3 — proton bookkeeping across the scheme is the quiet connector.

### (f) By-product F
**L1 · Answer** **Formic acid, HCOOH** (SMILES `O=CO`). E (HMF, C₆H₆O₃) + 2 H₂O → levulinic acid (C₅H₈O₃) + HCOOH (CH₂O₂): atom audit C 6 = 5+1 ✓, H 10 = 8+2 ✓, O 5 = 3+2 ✓. IR audit: broad 3500–3100 cm⁻¹ (O–H) + 1745 cm⁻¹ (C=O) = small carboxylic acid ✓.
**L2 · Thought** The classic HMF → levulinic acid + formic acid hydrolysis — but it is derivable, not memorised: the mass balance demands a one-carbon, oxygen-rich, acidic by-product; the IR (broad OH + carbonyl) confirms a carboxylic acid; C1 = formic acid is the unique fit.

### (g) Z in [RuH₂(CO)(PPh₃)₃]
**L1 · Answer** **Z = +2** (2 × H⁻, CO and PPh₃ neutral → Ru(II)).
**L2 · Thought** Ligand-charge audit: hydrides are −1 (covalent classification), so Ru = +2. Do not count PPh₃ or CO as charged — the two classic freebies.

### (h) Other stereoisomers of [RuH₂(CO)(PPh₃)₃]
**L1 · Answer** The shown isomer is cis-H₂ (H trans to CO; H trans to P; two P trans to each other). Two more:
- **trans-H₂**: the two hydrides opposite; CO cis to both hydrides; one PPh₃ trans to CO, the other two PPh₃ each trans to a hydride.
- **cis-H₂ with CO trans to PPh₃**: hydrides cis; each hydride trans to a PPh₃; the remaining PPh₃ trans to CO.
**Enantiomer ticks**: none — the shown isomer and both drawn isomers are achiral (each has a mirror plane; octahedral complexes of type MA₂BC₃ with monodentate ligands are achiral here).
**L2 · Thought** Enumerate by trans-pair inventory (three trans slots): the H's are either trans to each other (1 arrangement) or cis; when cis, the unique ligand CO is either trans to an H (shown isomer) or trans to a P (third isomer) — that exhausts MA₂BC₃. Chirality check is a mirror-plane hunt, not a vibe: each candidate has at least one plane containing Ru and two ligand positions, so no enantiomers anywhere.

### (i) ³¹P NMR of the catalyst (tick)
**L1 · Answer** Tick: **a doublet and a triplet** (2 : 1 intensity): Pˣ/Pʷ are equivalent (trans to each other, with identical ligand sets) and couple to Pʸ → doublet (2P); Pʸ couples to the two equivalent P's → triplet (1P).
**L2 · Thought** Count ³¹P environments from the structure, not from the ligand count: Pˣ (top) and Pʷ (bottom) are related by their identical environments (each trans to the other P and cis to {Pʸ, CO, Hᴶ, Hᴷ}), and the hydride multiplets in (j) confirm the equivalence (Hᴶ sees exactly two equal P couplings at 31 Hz). Equivalent nuclei do not split each other — hence doublet + triplet, not three doublets of doublets (that would be the answer for three inequivalent P's, the failure mode to check against).

### (j) Coupling-constant table
**L1 · Answer**

| pair | J / Hz | basis |
|---|---|---|
| Hᴶ–Hᴷ | 6 | the small doublet shared by both signals |
| Hᴶ–Pʷ | 31 | part of Hᴶ's triplet (cis) |
| Hᴶ–Pˣ | 31 | part of Hᴶ's triplet (cis) |
| Hᴶ–Pʸ | 15 | Hᴶ's smaller doublet (cis) |
| Hᴷ–Pʷ | 28 | part of Hᴷ's triplet (cis) |
| Hᴷ–Pˣ | 28 | part of Hᴷ's triplet (cis) |
| Hᴷ–Pʸ | 74 | Hᴷ's large doublet (**trans** to Pʸ) |

**L2 · Thought** Work from the two stated rules: trans > cis, and equivalent P's give a triplet. Hᴷ (−8.80 ppm, dtd) owns the 74 Hz doublet — the only large, trans-sized coupling, so Hᴷ is trans to the unique Pʸ; its 28 Hz triplet then covers the equivalent Pˣ/Pʷ pair, and 6 Hz is H–H. Hᴶ (−6.83 ppm, tdd) has no trans-sized coupling (its largest is 31 Hz) → Hᴶ is trans to CO (no P across), cis to all three P's: the equivalent pair at 31 Hz (triplet) and Pʸ at 15 Hz (doublet). The table self-checks: every coupling appears in exactly one multiplet pattern, and the two patterns read backwards consistently (t(31)d(15)d(6) and d(74)t(28)d(6)).

---

## Q4 — 'Social distancing' in molecules: conformations (13 marks)

### (a) E or S in the boxes (ethane rotation)
**L1 · Answer** 120° = **E**; 180° = **S**; 240° = **E**; 300° = **S**; 360° = **E**.
**L2 · Thought** Ethane's pattern is period-120°: eclipsed at 0/120/240/360, staggered at 60/180/300. The minima on the diagram sit at 60/180/300 — read off the axis before writing.

### (b) Methylbutane projections → points A–F
**L1 · Answer** **A = 2; B = 6; C = 3; D = 4; E = 1; F = 5** (A/C and D/F interchangeable — degenerate pairs).
Deciding analysis (front C = C2: 2 CH₃ + H; back C = C3: CH₃ + 2 H):
- Staggered, back-Me **anti to front-Me** (the butane-like anti form, lowest): 2 (back-Me at bottom anti to front-top-Me) and 3 (back-Me upper-left anti to front-lower-right-Me) → A (0°) and C (120°), the two equal lowest minima.
- Staggered, back-Me **anti to front-H** (all Me–Me pairs gauche, higher minimum): 1 → E (240°).
- Eclipsed with **no Me–Me eclipse** (back-Me eclipses front-H; both front-Me's eclipse back-H's): 6 → B (the lower peak, 60°).
- Eclipsed with **one Me–Me eclipse**: 4 and 5 → D (180°) and F (300°), the two equal highest peaks.
**L2 · Thought** Order the interactions before the angles: the energy of any (eclipsed) pair scales Me–Me > Me–H > H–H. Two checks keep this honest: (1) the diagram itself — A and C sit at the same depth (same conformer, rotated 120° around the C–C bond, since the two front methyls are equivalent), as do D and F; (2) the anti/gauche logic must match butane intuition — the conformer with the two methyls anti (β-type) is the lowest, *not* the one with back-Me anti to front-H. Getting α/β backwards is the classic error; anchor it with "Me–Me anti = lowest".

### (c)(i) The three equilibrium constants at 298 K
**L1 · Answer** Using ΔG° = −RT ln K:
- G₁ ⇋ AP: ΔG° = −3.63 kJ mol⁻¹ → K = exp(3630/(8.314 × 298)) = **4.33** ([AP]/[G₁]).
- AP ⇋ G₂: G₂ is the mirror of G₁ (same energy), so ΔG° = +3.63 kJ mol⁻¹ → K = **0.231** ([G₂]/[AP]).
- G₂ ⇋ G₁: identical energies → ΔG° = 0 → K = **1**.
(Cycle audit: 4.33 × 0.231 × 1 = 1.000 ✓ — the three constants multiply to 1 around the closed triangle, as they must.)
### (c)(ii) Percentage of time in AP
**L1 · Answer** [G₁] = [G₂] = x (symmetry), [AP] = 4.33x → AP fraction = 4.33/(1 + 1 + 4.33) = **68 %**.
**L2 · Thought** Two moves: (1) the two gauche forms are enantiomers, hence equal population — do not run two separate equilibria; (2) the ratio only needs one equilibrium (K₁) plus the symmetry statement. Plausibility anchor: butane is ~70 % anti at room temperature in textbooks ✓.

### (d) Equal-energy sets among 7–12 (acetylcholine)
**L1 · Answer** **(7 = 11), (8 = 10), 9, 12.**
- 9: staggered **anti** (NMe₃⁺ at 12 o'clock, OAc at 6 o'clock — dihedral 180°).
- 7 and 11: the two **gauche** staggered forms (N/OAc dihedral 60°, mirror images).
- 8 and 10: the two **eclipsed forms with OAc eclipsing a front H** (N/OAc dihedral 120°, mirror images).
- 12: the **fully eclipsed** form (OAc directly behind NMe₃⁺, dihedral 0° — the unique highest-energy form).
**L2 · Thought** Classify each projection by the NMe₃⁺–OAc dihedral alone (the two H's on each carbon are equivalent, so only the N/O positions matter): 180° → anti; 60° → gauche; 120° → eclipsed-H; 0° → eclipsed-N/OAc. Then ask which are related by a mirror plane/rotation (equal energy) rather than merely similar: 7 and 11 are mirror images; 8 and 10 are mirror images; 9 and 12 are singletons by symmetry. This is butane's six-conformation taxonomy transplanted onto N⁺–CH₂–CH₂–OAc — once you see the butane skeleton, the grouping is mechanical.

### (e) Which of 7–12 are mimicked by cyclopropanes W, X, Y, Z
**L1 · Answer** (the mapping)
- **12 (fully eclipsed, N/OAc dihedral 0°) → W and Z** (the two cis-1,2-cyclopropanes: **W** = both substituents wedged (both toward the viewer); **Z** = both dashed (both behind) — either way the substituents eclipse each other, dihedral 0°).
- **8 → X; 10 → Y** (the two mirror-image eclipsed forms with OAc eclipsing a front H, dihedral ≈ 120°: the two trans-1,2-cyclopropanes — substituents on opposite faces, an enantiomeric pair — give exactly this eclipsed arrangement with the substituents anti to the eclipsed hydrogens).
- **7, 9, 11 → None** (the *staggered* conformers — gauche 60° AND the anti 180° form — have no cyclopropane mimic at all).
**L2 · Thought** The deciding observation is a *structural* one about cyclopropane, not a dihedral-number match: every bond of a cyclopropane ring is **eclipsed** with its neighbours, so a cyclopropane can only mimic **eclipsed** Newman projections — among 7–12 those are 8, 10, 12. cis-1,2 substituents (same face) eclipse each other → conformer 12 (dihedral 0°); trans-1,2 substituents (opposite faces) eclipse the flanking C–H bonds instead → the ≈120° eclipsed forms 8 and 10 (X and Y are the two enantiomeric trans arrangements, matching the two mirror-image projections). The naive mapping "trans-cyclopropane = anti (180°) → conformer 9" is the designed trap: the anti form is *staggered*, and no cyclopropane can be staggered about a ring bond. Drug-design moral (the question's point): rigidity only pays when the locked geometry matches a *bound* conformation — here the lockable set is {0°, ~120°}, and the lowest-energy staggered conformers are precisely the ones that cannot be locked.

---

## Q5 — Hydroxychloroquine synthesis (21 marks)

### (a) IUPAC name of A
**L1 · Answer** **5-chloropentan-2-one** (CH₃–CO–CH₂–CH₂–CH₂–Cl; SMILES `CC(=O)CCCCl`). (Mark scheme confirms: five-carbon chain — the ketone gets locant 2, the chloro lands at 5.)
**L2 · Thought** Number to give the ketone the lowest locant (2, not 4); the chloro is then at 5. Count the skeletal chain carefully before naming — four carbons (4-chlorobutan-2-one) is a misread of the drawing, and the error propagates into every downstream structure (the final drug's –NH–CH(CH₃)–CH₂CH₂CH₂–N< tail needs all five).

### (b) B and C
**L1 · Answer**
- **B** = CH₃–CO–CH₂–CH₂–CH₂–N(CH₂CH₃)–CH₂CH₂OH (5-(N-ethyl-N-(2-hydroxyethyl)amino)pentan-2-one; SMILES `CC(=O)CCCN(CC)CCO`): the secondary amine does SN2 on the primary C–Cl.
- **C** = the **ketimine** CH₃–C(=NH)–CH₂–CH₂–CH₂–N(CH₂CH₃)–CH₂CH₂OH (SMILES `CC(=N)CCCN(CC)CCO`): NH₃ condenses with B's ketone (−H₂O).
**L2 · Thought** Site-selection: A offers both a ketone (reversible addition) and a primary alkyl chloride (irreversible SN2) — the secondary amine alkylates the chloride; adding ammonia to the ketone then gives the imine. The target drawn at the right of the scheme (the saturated amine) telegraphs that step (i) must reduce C=N, which is also the evidence that C is the imine rather than a hemiaminal stopped halfway.

### (c) Reagents/conditions for step (i) (tick)
**L1 · Answer** Tick **H₂ / Ni catalyst** (imine → amine hydrogenation).
**L2 · Thought** Eliminate by transformation: C=N → CH–NH is a two-electron reduction — of the list, only H₂/Ni supplies it (KMnO₄, K₂Cr₂O₇, OsO₄, O₂ are oxidants; Br₂/UV is radical halogenation; ethylamine would transiminate; H₂SO₄ hydrolyses the imine back). Process of elimination is a legitimate deciding criterion when the reagent list is finite.

### (d) D, E, F
**L1 · Answer**
- **D** = nitrobenzene (HNO₃/H₂SO₄ → NO₂⁺, the 2025-Q1 chemistry again).
- **E** = **1-chloro-3-nitrobenzene** (NO₂ is meta-directing → chlorination goes meta).
- **F** = **3-chloroaniline** (H₂/Pt reduces NO₂ → NH₂, C–Cl survives).
**L2 · Thought** The two-directional reading pays again: the drawn anil product (3-chloroaniline-derived) fixes the *meta* relationship — so E must be meta-chloro-nitrobenzene, and the directing effect of NO₂ (meta) is the mechanistic justification that makes it a *deduction*, not a guess. F's amine is the nucleophile that attacks reagent Z's electrophilic carbon next.

### (e) V⁻, W⁺, X⁺, Y, Z
**L1 · Answer**
- **V⁻** = diethyl malonate anion: ⁻CH(CO₂Et)₂ (charge on the central C, resonance onto both carbonyl O's: EtO₂C–C(=O⁻)–CO₂Et ↔).
- **W⁺** = protonated triethyl orthoformate: HC(OEt)₃H⁺ (an ethoxy oxygen protonated).
- **X⁺** = diethoxycarbenium ion: HC(OEt)₂⁺ (W⁺ loses neutral EtOH; resonance EtO–CH=OEt⁺ ↔ EtO⁺=CH–OEt).
- **Y** = (EtO₂C)₂CH–CH(OEt)₂ (V⁻'s central carbon alkylated by X⁺).
- **Z** = diethyl ethoxymethylenemalonate (EMME): (EtO₂C)₂C=CH–OEt (Y loses a second EtOH).
**L2 · Thought** This is a guided umpolung tour: the orthoformate is sequentially *activated* (protonate → ionise to a carbenium), the malonate supplies the nucleophilic carbon, and elimination of ethanol unmasks the electrophilic alkene that F's aniline will attack. Check each cation/anion's formal charge as you draw it (formal-charge audit) — W⁺ must be O-protonated (not C-protonated), because only O-protonation makes ethanol a leaving group.

### (f) G, H, I, J (final part)
**L1 · Answer** *(The final-part scheme: the anil Ar–NH–CH=C(CO₂Et)₂ (F + Z) →(high-temperature reflux, "a cyclisation")→ G →(NaOH in EtOH)→ H →(high-temperature reflux, −CO₂)→ I →(POCl₃)→ J →(+ the side-chain amine)→ hydroxychloroquine.)* Follow the arrows in order:
- **G** = the **Gould–Jacobs cyclisation product**: **ethyl 7-chloro-4-hydroxyquinoline-3-carboxylate** (drawn as its 4-oxo-1,4-dihydro tautomer is equally correct) — thermal electrocyclic ring closure of the anil onto the ring's free ortho position — `CCOC(=O)c1cnc2cc(Cl)ccc2c1O` (C₁₂H₁₀ClNO₃ ✓);
- **H** = the **carboxylic acid (or its sodium salt)**: 7-chloro-4-hydroxyquinoline-3-carboxylic acid — NaOH/EtOH hydrolyses only the ester — `O=C(O)c1cnc2cc(Cl)ccc2c1O` (C₁₀H₆ClNO₃ ✓ = G − C₂H₄);
- **I** = **7-chloroquinolin-4-ol** (4-hydroxy-7-chloroquinoline): high-temperature reflux **decarboxylates** the 3-carboxyl (the printed "−CO₂" is the instruction) — `Oc1ccnc2cc(Cl)ccc12` (C₉H₆ClNO ✓ = H − CO₂);
- **J** = **4,7-dichloroquinoline** — POCl₃ replaces the 4-OH by Cl — `Clc1ccnc2cc(Cl)ccc12` (C₉H₅Cl₂N ✓);
- J + the side-chain amine (from part (c): H₂N–CH(CH₃)–CH₂CH₂CH₂–N(Et)–CH₂CH₂OH) → **hydroxychloroquine** (S_NAr at C4; the 4-Cl is the leaving group activated by the ring N).
**L2 · Thought** Read the reagent order as the specification: the cyclisation comes first (the anil's ortho closure onto the malonate carbonyl), NaOH then *hydrolyses the ester* (the quinoline 4-OH survives), the second high-temperature step is marked "−CO₂" (decarboxylation of the 3-carboxylic acid, standard for 4-hydroxyquinoline-3-carboxylates), POCl₃ converts 4-OH → 4-Cl, and only then does the side-chain amine displace that 4-Cl. (The scheme's arrow order, not the drug's familiarity, assigns the letters; the formula audit chain closes at every letter: −C₂H₄, −CO₂, −OH + Cl.) The 7-chloro position comes from the *meta*-chloroaniline choice back in (d) — meta starting material, 7-chloro product: ring-position bookkeeping across the whole route.

---

## Q6 — Xenon fluorides (17 marks)

### (a) Formation of XeF₄
**L1 · Answer** Xe + 2 F₂ → XeF₄. (Audit: Xe 1=1; F 4=4 ✓.)
**L2 · Thought** Direct combination, Xe(0) → Xe(+4): the oxidation-state audit (Xe loses 4 e⁻, 2 F₂ gain 4 e⁻) writes the stoichiometry.

### (b) Dot-and-cross of XeF₄
**L1 · Answer** Electron budget: 8 (Xe) + 4 × 7 (F) = 36 e⁻. Draw four Xe–F single bonds (one dot–cross pair each) and **two lone pairs on Xe**; each F carries three lone pairs. (Six domains on Xe, matching the stem's "six electron pairs".)
**L2 · Thought** Count first: 36 e⁻ = 8 bonding + 28 non-bonding; after giving each F its three lone pairs (24 e⁻), 4 e⁻ remain on Xe → 2 lone pairs. If your Xe has one or three lone pairs, the budget failed — recount before drawing shapes.

### (c) Two arrangements of six pairs in XeF₄ (tick)
**L1 · Answer** Draw (i) lone pairs **trans** (opposite vertices of the octahedron) → the four F's form a **square plane** — **tick: this is the adopted arrangement**; (ii) lone pairs **cis** (adjacent) → F's form a distorted see-saw square pyramid — not adopted.
**L2 · Thought** Lone-pair/lone-pair repulsion is minimised at 180° — VSEPR's first tiebreaker. Square planar XeF₄ is the canonical textbook shape; the cis alternative would put the two lone pairs in each other's face (maximum LP–LP repulsion).

### (d) Arrangements of five pairs in XeF₂ (tick)
**L1 · Answer** Draw the trigonal-bipyramidal options: (i) all three lone pairs **equatorial** → two F's axial → **linear molecule — tick: adopted**; (ii) two lone pairs axial, one equatorial → bent/T-shaped F arrangement — not adopted.
**L2 · Thought** In a trigonal bipyramid, equatorial positions have fewer 90° neighbours (2 vs 3), so lone pairs always claim the equator first — with three lone pairs, they take all three equatorial sites and the molecule degenerates to linear (the "VSEPR degeneracy" pattern: 5 pairs → 2 bonds = linear, memorised as AX₂E₃).

### (e) Rate equation for XeF₂ formation
**L1 · Answer** Constant volume, so amounts ∝ concentrations:
- Rows 1→3: n(Xe) doubles (1.0 → 2.0), n(F₂) constant, rate doubles (3.6 → 7.2) → **first order in Xe**;
- Rows 1→2: n(F₂) doubles (5.0 → 10.0), n(Xe) constant, rate unchanged (3.6 → 3.6) → **zero order in F₂**.
**rate = k · n(Xe)** (equivalently rate = k′[Xe]).
**L2 · Thought** Vary-one-factor-at-a-time (§7.8): pick the pair of rows where only one quantity changes — never fit all three rows simultaneously. Zero-order in F₂ is the chemically interesting result (fluorine atoms come from a pre-equilibrium dissociation, consistent with the F + Xe rate-determining step introduced later — the paper rewards noticing the consistency).

### (f) k_cat/k expression
**L1 · Answer**
$$\frac{k_{cat}}{k} = \frac{A_{cat}}{A}\exp\!\left(\frac{E_a - E_{cat}}{RT}\right) = \frac{A_{cat}}{A}\exp\!\left(\frac{\Delta E}{RT}\right)$$
**L2 · Thought** Write both Arrhenius laws and divide; the sign of the exponent is the only place to slip — catalysts lower Ea, so Ea − Ecat = ΔE > 0 and the ratio exceeds 1 once ΔE is positive ✓ (direction check).

### (g) ΔE from the two temperature ratios
**L1 · Answer** With A, A_cat temperature-independent, divide the two ratio equations:
$$\frac{23}{13} = \exp\!\left[\frac{\Delta E}{R}\left(\frac{1}{373.15} - \frac{1}{393.15}\right)\right]$$
$$\Delta E = \frac{8.314 \times \ln(23/13)}{1/373.15 - 1/393.15} = \frac{8.314 \times 0.5706}{1.3635\times10^{-4}} = \mathbf{34.8\ kJ\ mol^{-1}}$$
**L2 · Thought** Two unknowns (ΔE and the prefactor ratio) need two temperatures — dividing eliminates A_cat/A without ever knowing it (hidden-calibration logic again: the data series determines both unknowns). Sign audit: the catalysed advantage *grows* as T falls (23 > 13), so ΔE must be positive ✓ — a negative answer would mean you swapped the two temperatures.

### (h) Activation energy from the refined rate law
**L1 · Answer** The refined law is k = β(T/μ)^{1/2} e^(−Ea/RT), i.e. ln(k/T^{1/2}) = const − Ea/(RT) (β, μ constant). Linearise with y = ln(k/√T) vs 1/T:

| T / °C | T / K | k | y = ln(k/√T) |
|---|---|---|---|
| 50 | 323.15 | 1.55 × 10⁻¹⁰ | −25.48 |
| 70 | 343.15 | 1.19 × 10⁻⁹ | −23.47 |
| 100 | 373.15 | 1.70 × 10⁻⁸ | −20.85 |
| 130 | 403.15 | 1.63 × 10⁻⁷ | −18.63 |
| 170 | 443.15 | 2.07 × 10⁻⁶ | −16.14 |

Least-squares slope = −1.115 × 10⁴ K → Ea = 1.115 × 10⁴ × 8.314 = **92.7 kJ mol⁻¹** (mark scheme range 92.4–93.0; neglecting the T^½ term gives 94.3 and scores nothing — the prefactor must be divided out first).
**L2 · Thought** The trap is applying the plain Arrhenius treatment (ln k vs 1/T) to a law that carries a T^{1/2} prefactor — you must divide the temperature dependence out first (declared-model linearisation, same discipline as 2023 Q4(i)'s "multiply by T first"). The spreadsheet table is written out so the method is inspectable — and every cell is checkable in isolation (e.g. 323 K: 1.55 × 10⁻¹⁰/√323.15 = 8.62 × 10⁻¹² → ln = −25.48); a table whose entries are individually wrong but whose slope is right is still wrong (the slope is protected here only because the errors were near-constant — that is luck, not method). Slope × R with the sign watched gives Ea positive ✓ (rates increase with T, as they must).

### (i) Rate constant if M(Xe) were 28 g mol⁻¹
**L1 · Answer** Only the reduced mass changes: k ∝ μ^{−1/2} (all else equal).
μ(correct) = (1/131.29 + 1/18.998)⁻¹ = 16.60; μ(28) = (1/28 + 1/18.998)⁻¹ = 11.32.
$$k_{28} = k_{131.29}\times\left(\frac{\mu_{131.29}}{\mu_{28}}\right)^{1/2} = 1.70\times10^{-8}\times\sqrt{\frac{16.60}{11.32}} = \mathbf{2.06\times10^{-8}\ dm^3\ mol^{-1}\ s^{-1}}$$
**L2 · Thought** Isolate what the question changes: with β, T, Ea fixed, k scales as μ^{−1/2} — a lighter (wrong) xenon makes the reduced mass smaller and the atom faster, so k *increases* (factor 1.21) ✓ direction check. The historical joke (Ramsay's caricature pointing at "28") is the context; the physics is a one-line ratio once the scaling law is stated before substituting (§7.5 symbol discipline).

---

*End of Paper 5 (2021). Next: 2020 Round 1.*

---

# Paper 6 — 2020 UKChO Round 1 (52nd IChO selection)

*6 questions, 86 marks, 2 h → ≈ 1.4 min per mark. Marks: Q1 = 10, Q2 = 10, Q3 = 17, Q4 = 12, Q5 = 17, Q6 = 20.*

## Q1 — Calcium carbide (10 marks)

### (a)(i) Formation of calcium carbide
**L1 · Answer** CaO + 3 C → CaC₂ + CO. (Audit: Ca 1=1; C 3 = 1+2 ✓; O 1=1 ✓; electron audit: 2 C(0) → C₂²⁻ (gain 2 e⁻), C(0) → CO (C +2, loses 2 e⁻) ✓.)
### (a)(ii) Dot-and-cross of C₂²⁻
**L1 · Answer** Electron budget: 2 × 4 + 2 = 10 e⁻ → a **triple bond** [:C≡C:]²⁻ with one lone pair on each carbon (isoelectronic with N₂).
**L2 · Thought** The 10-electron count forces the triple bond (as in N₂, CO, CN⁻) — the carbide ion is the acetylide [C≡C]²⁻, which is exactly why its protonation in (b) gives ethyne H–C≡C–H. The equation in (a)(i) is balanced by the *electron* audit first (carbon both reduced to C₂²⁻ and oxidised to CO), atom count second.

### (b) Ethyne from calcium carbide
**L1 · Answer** CaC₂ + 2 H₂O → C₂H₂↑ + Ca(OH)₂. (Audit: Ca 1=1; C 2=2; H 4 = 2+2 ✓; O 2=2 ✓.)

### (c) Percentage purity
**L1 · Answer** The Ca(OH)₂ produced is titrated:
n(HCl) = 0.250 × 34.60 × 10⁻³ = 8.650 × 10⁻³ mol in the 20.00 cm³ aliquot
n(Ca(OH)₂) in aliquot = 8.650 × 10⁻³/2 = 4.325 × 10⁻³ mol → in 50.0 cm³ total: × 2.5 = 1.081 × 10⁻² mol = n(CaC₂)
m(CaC₂) = 1.081 × 10⁻² × 64.10 = 0.6931 g → purity = 0.6931/0.752 × 100 % = **92.2 %**
**L2 · Thought** Chain-map (§ consequential-marking style): HCl → OH⁻ → Ca(OH)₂ → CaC₂, with the 20/50 aliquot factor as the silent step. The impurities "do not react" — the titration therefore measures only carbide-derived hydroxide, which is the whole design.

### (d) Atoms in the CaC₂ unit cell
**L1 · Answer** **Ca: 8 corners × ⅛ + 1 body centre = 2. C: 2 top-edge pairs + 2 bottom-edge pairs (each shared by 4 cells → 4 × ¼ = 1) + 4 on vertical edges (4 × ¼ = 1) + 2 fully inside = 4.** Net: 2 Ca and 4 C → 2 CaC₂ per cell.
**L2 · Thought** Share-count before arithmetic (skeleton 7.4 step ③): corners ⅛, edges ¼, faces ½, interior 1 — and the carbons sit as C₂ dumbbells, so counting individual C atoms (not dumbbells) avoids the factor-of-two error.

### (e) Cell parameter z
**L1 · Answer** Mass of cell = 2 × 64.10/6.022 × 10²³ = 2.129 × 10⁻²² g; V = m/ρ = 2.129 × 10⁻²²/2.20 = 9.68 × 10⁻²³ cm³ = 96.8 Å³
z = V/(xy) = 96.8/(3.88 × 3.88) = **6.43 Å**
**L2 · Thought** Density links the macroscopic and atomic scales; unit discipline: convert the volume to Å³ before dividing by Å² (or stay in cm throughout). Sanity anchor: z > x, y (CaC₂ is a tetragonally *elongated* NaCl cell because of the C≡C dumbbell axis ✓).

---

## Q2 — Hydrogen as a fuel (10 marks)

### (a) Reforming enthalpy
**L1 · Answer** CH₄(g) + 2 H₂O(l) → CO₂(g) + 4 H₂(g):
ΔH = [−393.5 + 0] − [−74.8 + 2(−285.8)] = **+252.9 kJ**
**L2 · Thought** Products minus reactants, elements (H₂) at zero. Endothermic ✓ — reforming needs energy input, which is why it is run hot.

### (b) Cathode half-reaction
**L1 · Answer** **Half reaction 2** (2 H⁺ + 2 e⁻ → H₂): cathode = reduction (gain of electrons).
**L2 · Thought** Mnemonic-free rule: cathode takes electrons *from* the external circuit, so the half-reaction with e⁻ on the *left* (as reactant) goes there.

### (c) Overall cell enthalpy
**L1 · Answer** 2 H₂O(l) → 2 H₂(g) + O₂(g): ΔH = −2 × (−285.8) = **+571.6 kJ**.

### (d) Cell potential
**L1 · Answer** ΔS° for the cell reaction = −2 ΔSf°(H₂O(l)) = −2 × (−163.0) = +326.0 J K⁻¹
ΔG° = ΔH° − TΔS° = 571.6 × 10³ − 298 × 326.0 = 4.745 × 10⁵ J
n = 4 electrons (per O₂ formed) → E° = −ΔG°/(nF) = −474 500/(4 × 96 485) = **−1.23 V**
**L2 · Thought** Two traps: (1) ΔS° comes only from the *formation* data given (ΔSf°(H₂O)) — flip its sign because the reaction *consumes* water; (2) n = 4 for the *overall* equation as written (2 H₂O → 2 H₂ + O₂), not 2. The negative E is the electrolysis voltage that must be supplied — magnitude 1.23 V is the famous water-electrolysis threshold ✓.

### (e) Standard electrode potential of half reaction 1
**L1 · Answer** **−1.23 V** (the oxidation 2 H₂O → O₂ + 4 H⁺ + 4 e⁻ carries the full cell potential; the H⁺/H₂ couple is 0 by convention).
**L2 · Thought** E(cell) = E(cathode) − E(anode) with E(cathode) = 0 → E(anode, as written for oxidation) = −E(cell)... careful with sign conventions: the question asks for the potential of the half-reaction *as written* (oxidation), which equals E(cell) here = −1.23 V since the other half is the standard hydrogen electrode.

### (f) ΔcH° of CH₄
**L1 · Answer** CH₄ + 2 O₂ → CO₂ + 2 H₂O(l): ΔcH = [−393.5 + 2(−285.8)] − [−74.8] = **−890.3 kJ mol⁻¹**.
### (g) ΔcH° of H₂
**L1 · Answer** H₂ + ½ O₂ → H₂O(l): ΔcH = **−285.8 kJ mol⁻¹** (= ΔfH°(H₂O(l))).
**L2 · Thought** (f) and (g) are designed to make you construct the combustion equations first — the given formation data cover exactly these two combustions and nothing else (data audit).

### (h) Heat-per-second ratio, H₂ vs CH₄
**L1 · Answer**
$$\frac{\text{heat(H}_2\text{)}}{\text{heat(CH}_4\text{)}} = \frac{285.8/\sqrt{2.016}}{890.3/\sqrt{16.04}} = \frac{201.3}{222.3} = \mathbf{0.906}$$
(mark scheme: 0.908 using integer M_r (2, 16) — same ratio; the inverse 1.10 is the classic wrong-way-around and scores partial credit only).
**L2 · Thought** The model penalises heavy molecules (slower effusion through the burner at equal pressure) — compute the two reduced quantities separately before the ratio to keep units visible (kJ mol⁻¹ / (g mol⁻¹)^{1/2}). Hydrogen delivers ~91 % of methane's heat per second in this model, so a hydrogen grid is *plausible* for the same appliances — the question's moral.

---

## Q3 — Sun cream: oxybenzone and octinoxate (17 marks)

### (a) Functional groups in oxybenzone (tick)
**L1 · Answer** **Ketone** (the benzophenone C=O), **phenol** (Ar–OH), **ether** (Ar–O–CH₃).
**L2 · Thought** The C=O is attached to two carbons → ketone, not aldehyde/acid; the –OH is on the ring → phenol, not alcohol; the Ar–O–Me is an ether, not an ester (no C=O on that side).

### (b) The intramolecular H-bond (circle)
**L1 · Answer** Circle **the phenolic O–H hydrogen** and **the ketone carbonyl oxygen** — the six-membered chelate O–H···O=C ring (which extends the conjugation over the benzophenone system).
**L2 · Thought** Same move as 2023 Q5(b) (lactate): the stabilising H-bond closes a strain-free 5/6-membered ring; the two atoms are donor-H and acceptor-O. Circling the two oxygens' *atoms* (not the OH group and the whole carbonyl) is what the question literally asks.

### (c) Oxybenzone synthesis: A, B, C, D
**L1 · Answer**
- **A** = benzoic acid, C₆H₅COOH (C₇H₆O₂ ✓; SOCl₂ converts COOH → COCl).
- **B** = benzoyl chloride, C₆H₅COCl.
- **C** = benzene-1,3-diol (resorcinol), C₆H₆O₂ ✓ — methylated once by dimethyl sulfate/NaOH.
- **D** = 3-methoxyphenol (resorcinol monomethyl ether), C₇H₈O₂ ✓.
(B + D + AlCl₃ → Friedel–Crafts acylation of D at the position **ortho to the phenol OH**, giving the 2-hydroxy-4-methoxybenzophenone skeleton of oxybenzone.)
**L2 · Thought** Formula audit first: A has 2 O and becomes the benzoyl half (unsubstituted phenyl ring in the product) → benzoic acid; C has 2 O and becomes the resorcinol half; dimethyl sulfate + base monomethylates one of the two equivalent OH's of resorcinol. The acylation regiochemistry (ortho to OH, giving the chelating 2-OH needed for part (b)'s H-bond) is dictated by the phenol's directing power — and confirmed by the product drawing.

### (d) Octinoxate stereoisomers
**L1 · Answer**
(i) **Enantiomer**: same (E)-cinnamate geometry, invert the 2-ethylhexyl stereocentre (swap the wedge H to dash on the CH(Et)(Bu) carbon).
(ii) **Non-enantiomer stereoisomer**: the **(Z)-cinnamate** (cis ArCH=CH–CO₂R), keeping the stereocentre as drawn — a diastereomer.
**L2 · Thought** Stereoisomer inventory: the molecule has two independent stereogenic elements — the C=C (E/Z) and the ethylhexyl stereocentre (R/S). Enantiomer = invert *all* stereogenic elements that are chiral (here: the stereocentre only; the alkene is not a chiral element); a non-enantiomer stereoisomer = flip exactly one of the two (the alkene), giving a diastereomer. Flipping *both* also gives an enantiomer, so "only the centre" for (i) and "only the alkene" for (ii) is the clean pair.

### (e) E and F
**L1 · Answer**
- **E** = **butanal**, CH₃CH₂CH₂CHO (`CCCC=O`): IR 1730 (C=O); NMR: 0.9 (3H, t, CH₃), 1.6 (2H, m, CH₂), 2.5 (2H, m, α-CH₂), 9.7 (1H, t, CHO) ✓ — the 9.7 triplet is the aldehyde fingerprint.
- **F** = **2-ethylhex-2-enal**, CH₃CH₂CH₂CH=C(CH₂CH₃)–CHO (C₈H₁₄O = 2 × C₄H₈O − H₂O ✓; IR 1628 C=C + 1687 conjugated C=O ✓): base-catalysed aldol self-condensation of butanal with dehydration.
**L2 · Thought** The condensation scheme printed above (R₁CO–CH₂–R₂ + R₃CO–R₄ → enone + H₂O) is the aldol map: E must have α-H's (the 2.5 ppm α-CH₂) and a carbonyl (the 9.7 aldehyde). Two identical E's: one enolises at its α-CH₂ and attacks the other's carbonyl, then loses water → the α-ethyl enal. Formula and the two IR bands (C=C and C=O "next to each other", as the stem requires) close the proof.

### (f) G and H
**L1 · Answer**
- **G** = **2-ethylhexan-1-ol**, CH₃CH₂CH₂CH₂CH(CH₂CH₃)–CH₂OH (H₂/Pd reduces both the C=C and the aldehyde of F).
- **H** = **2-ethylhexyl ethanoate (acetate)**, CH₃CO–O–CH₂–CH(CH₂CH₃)–(CH₂)₃CH₃ (transesterification of G with methyl acetate/NaOCH₃; methanol is the suppressed by-product).
(H + 4-methoxybenzaldehyde/NaOCH₃ then does a Claisen–Schmidt condensation at the acetate's α-CH₂ → octinoxate, 2-ethylhexyl (E)-4-methoxycinnamate.)
**L2 · Thought** Work backwards from the drawn octinoxate: its ester alkoxy group is 2-ethylhexyl (C₈, from F) and the acyl part is 4-methoxycinnamoyl (from ArCHO + an acetate enolate). So H must be the C₈ alcohol's *acetate ester* (supplying the α-CH₂ for the final condensation), and G the C₈ alcohol itself. The reagent "methyl acetate/NaOCH₃" is the transesterification signature (esters exchange alkoxy groups under alkoxide catalysis).

### (g) What all truxinate/truxillate products share (tick)
**L1 · Answer** **The same molecular formula** only.
**L2 · Thought** All are [2+2] dimers of the same monomer (C₁₈ → C₃₆H₄₄O₄… same formula whatever the regio/stereochemistry). Melting points and optical rotation differ across stereoisomers (and racemic products rotate plane-polarised light in *no* direction). This is the "isomers have the same formula" truism being tested — the other two options are precisely the properties that *distinguish* stereoisomers.

### (h) Truxinate stereoisomers (adjacent Ar, adjacent R on the cyclobutane)
**L1 · Answer**
(i) **"Four" (all four substituents wedged up): no enantiomer** — it contains four stereocentres yet is **meso (achiral)**: a mirror plane through the midpoints of the two Ar edges (and the two R edges) swaps the identical pairs, so the molecule is superimposable on its mirror image.
**"Three" (each of the two drawn isomers): has an enantiomer** — for the isomer with an Ar down: no mirror plane survives (the Ar-down/Ar-up swap breaks both candidate planes); its mirror image (one Ar up, three down, viewed from the other face as the *other* Ar-down arrangement) is non-superimposable. Same for the isomer with an R down.
(ii) **"Two" line — three structures:**
- **both Ar up** (both R down): **no enantiomer** — horizontal mirror plane swapping the two Ar (both up) and the two R (both down); note this is the same molecule as "both R up" viewed from the other face.
- **adjacent mixed pair up** (one Ar and one R on the same edge up, the other edge down): **has an enantiomer** — no improper symmetry; the mirror image is the bottom-edge-up form, non-superimposable (draw one of the pair).
- **diagonal pair up** (one Ar and one R diagonally opposite up): **has an enantiomer** — no improper symmetry; the mirror image is the other diagonal (draw one of the pair).
**L2 · Thought** The method is *improper-symmetry checking*, not stereocentre counting: for each candidate, ask for a mirror plane, inversion centre, or S-axis in the *substituted* ring. The table is a trap for "four stereocentres → must be chiral" — the all-up form has four stereocentres and is achiral, while several "two"-face isomers with the same count are chiral pairs. Also note the degeneracy discipline: viewing a structure from the other face is *not* a new isomer, but a mirror image that cannot be rotated onto the original *is* an enantiomer — that distinction is exactly what (h)(ii) tests with its "only draw one of the pair" instruction.

---

## Q4 — Silicon oxides and silicates (12 marks)

### (a)(i) Gas Y
**L1 · Answer** **CO₂.**
### (a)(ii) Anion of X
**L1 · Answer** **[SiO₄]⁴⁻**, tetrahedral: central Si with four single-bonded O's (orthosilicate; charge −4 indicated).
### (a)(iii) Equation
**L1 · Answer** SiO₂ + 2 Na₂CO₃ → Na₄SiO₄ + 2 CO₂. (Audit: Si 1=1; Na 4=4; C 2=2; O 2+6 = 4+4 ✓; the "1 : 2 ratio" of the stem is satisfied.)
**L2 · Thought** The tetrahedral, Si/O-only anion fixes orthosilicate; the 1:2 stoichiometry then writes the equation and identifies the gas as CO₂ (carbonate decomposed by the acidic oxide at 1500 °C — the classic "acidic oxide drives out weaker-acid anhydride" pattern).

### (b) CaSiO₃ + dilute HCl
**L1 · Answer** CaSiO₃ + 2 HCl + 10 H₂O → SiO₂·11H₂O + CaCl₂. (Audit: Ca 1=1; Si 1=1; Cl 2=2; H 2+20 = 22 ✓; O 3+10 = 2+11 ✓.)
**L2 · Thought** Balance by stripping it to essentials: CaSiO₃ + 2 HCl → SiO₂ + CaCl₂ + H₂O, then hydrate the silica with the remaining 10 waters of crystallisation. The given hydrate SiO₂·11H₂O fixes the water count — do not "simplify" it away.

### (c) Quartz connectivity
**L1 · Answer** **4** — every SiO₄ tetrahedron shares *all four* of its oxygens, so each tetrahedron is corner-linked to four others (a fully corner-shared 3D network).
**L2 · Thought** Count from the drawing convention: each O is shared between 2 Si; each Si has 4 O → 4 neighbours. This is the endpoint of the silicate-sharing series (0 in [SiO₄]⁴⁻, 1 in [Si₂O₇]⁶⁻, 2 in the rings below, 3 in the talc sheet, 4 in quartz).

### (d) Silicate anion structures
**L1 · Answer**
(i) **[Si₃O₉]⁶⁻**: a **cyclic trisilicate ring** — three SiO₄ tetrahedra each sharing two corners, forming a triangle with 3 bridging and 6 terminal O's (charge: 3(+4) − 3(−2) − 6(−2) = −6 ✓).
(ii) **[Si₆O₁₈]¹²⁻** (beryl): the **six-membered ring** — six tetrahedra each sharing two corners (charge: 6(+4) − 6(−2) − 12(−2) = −12 ✓).
**L2 · Thought** The formula tells you the sharing pattern: Si : O = 1 : 3 means each Si has 2 shared + 2 terminal O's (shared O counts half per Si: 4 − 2×½ = 3 effective O per Si → ring). The charge follows automatically from the count — always write it as a check, not from memory. Beryl's 6-ring is the famous beryl/emerald channel structure.

### (e) Silicate anion in talc
**L1 · Answer** **[Si₄O₁₀]⁴⁻** (talc = Mg₃Si₄O₁₀(OH)₂: 3 × Mg²⁺ = +6, 2 × OH⁻ = −2, so the sheet carries −4).
**L2 · Thought** Charge-balance accounting is the whole question: neutral mineral = cations + hydroxide + silicate sheet. The 2D-sheet statement matches each tetrahedron sharing *three* corners (4 − 3×½ = 2.5 effective O per Si... giving Si₂O₅ stoichiometry = Si₄O₁₀ ✓ — a second route to the same answer; use both and they must agree).

### (f) Talc/chrysotile molar percentages
**L1 · Answer** Per 100 g: n(Mg) = 20.32/24.31 = 0.8361 mol; n(Si) = 28.18/28.09 = 1.0034 mol.
Talc unit = Mg₃Si₄; chrysotile unit = Mg₃Si₂. Let t, c be unit amounts:
3t + 3c = 0.8361; 4t + 2c = 1.0034 → t = 0.2230, c = 0.0557
**Talc = 0.2230/0.2787 = 80.0 mol %; chrysotile = 20.0 mol %.**
**L2 · Thought** Two species, two element balances — a 2×2 linear system (§ stoichiometric linear systems, cf. 2023 Q5e). The clean 80/20 split within rounding is the self-check; if the ratio had come out at 79.3/20.7, recheck the atomic masses used before accepting.

---

## Q5 — Colourful compounds: conjugation and porphyrins (17 marks)

### (a) Skeletal structure of buta-1,3-diene
**L1 · Answer** CH₂=CH–CH=CH₂ (a 4-carbon chain with alternating double–single–double bonds).
### (b)(i) ΔE for the UV absorption
**L1 · Answer** ΔE = hc/λ = (6.626 × 10⁻³⁴ × 2.998 × 10⁸)/(210 × 10⁻⁹) = **9.46 × 10⁻¹⁹ J**.
### (b)(ii) Length L
**L1 · Answer** n = 2 double bonds:
$$L = \sqrt{\frac{(2\times2+1)h^2}{8m_e\Delta E}} = \sqrt{\frac{5 \times (6.626\times10^{-34})^2}{8 \times 9.109\times10^{-31} \times 9.46\times10^{-19}}} = \mathbf{5.64\ \text{Å}}$$
**L2 · Thought** Particle-in-a-box in disguise: longer box → smaller ΔE → longer λ. Sanity anchor: 4 sp² C–C bonds ≈ 1.4 Å each ≈ 5.6 Å ✓ — the model is embarrassingly good, which is exactly why the question then trusts it for porphyrins.

### (c) Porphine/porphyrin scaling λ = εd²
**L1 · Answer**
(i) Mg complex: d = 2 × 2.052 = 4.104 Å → ε = λ/d² = 5714 Å/(4.104 Å)² = **339.3 Å⁻¹** (work in ångströms throughout — the question wants Å⁻¹; 33.93 would be the answer in nm·Å⁻², a unit mix-up the mark scheme refuses).
(ii) Zn: d² = 5687 Å/339.3 Å⁻¹ = 16.76 Å² → d = 4.094 Å → N–Zn = d/2 = **2.047 Å**.
(iii) Porphine 1: λ = 339.3 × (4.112)² = 5737 Å = **573.7 nm**.
**L2 · Thought** One model, three tasks: calibrate ε on the Mg complex (given N–Mg), transfer it (the stem says ε is the same for 1 and 2), then predict. Note the physical consistency: N–Zn (2.047) < N–Mg (2.052) → smaller box → *blue* shift (568.7 < 571.4) ✓ — always run the direction check before writing the number.

### (d) Ea for T → T* (Arrhenius, two points)
**L1 · Answer** ln(k₄₉₃/k₃₉₃) = (Ea/R)(1/393 − 1/493):
$$E_a = \frac{8.314 \times \ln(3.31\times10^{12}/1.32\times10^{12})}{1/393 - 1/493} = \frac{8.314 \times 0.9193}{5.16\times10^{-4}} = \mathbf{14.8\ kJ\ mol^{-1}}$$
**L2 · Thought** Standard two-point Arrhenius: ratio first (k₄₉₃/k₃₉₃ = 2.508), then divide by the reciprocal-temperature gap. Watch the order of magnitude at the end — 10⁴ J = 14.8 kJ, not 148 kJ (a slipped power of ten is the classic disaster here; check the denominator 100/(393 × 493) = 5.2 × 10⁻⁴ explicitly).

### (e) Express β and γ
**L1 · Answer** Match the given k₂ = (2Ea/μ)^{1/2}(αRT/Ea) exp(−α(2 − αRT/Ea)) to k₂ = T(β/γ)^{1/2} exp(−2α + βT):
- Exponent: −2α + α²RT/Ea = −2α + βT → **β = α²R/Ea**.
- Prefactor: T·αR(2Ea/μ)^{1/2}/Ea = T(2α²R²/(μEa))^{1/2} = T(β · 2R/μ)^{1/2} → **γ = μ/(2R)**.
**L2 · Thought** Term-matching discipline: match the exponent first (it determines β), then the prefactor (it determines γ). Check units at the end: β in K⁻¹ ✓, β/γ = 2α²R²/(μEa) ✓ consistent with the prefactor — if the two derivations of β/γ disagree, the exponent match was wrong.

### (f) β from the data
**L1 · Answer** From ln(k₂/T) = βT + i, the slope is β:
$$\beta = \frac{\ln(8.74\times10^{10}/83) - \ln(6.23\times10^{10}/61)}{83 - 61} = \frac{20.775 - 20.744}{22} = \mathbf{1.39\times10^{-3}\ K^{-1}}$$
**L2 · Thought** The linearised form dictates the axes: it is ln(k₂/**T**), not ln k₂, against T — dividing k₂ by T *before* taking the log is the step that decides the answer (the printed fallback β = 9.456 × 10⁻⁴ rescues a broken chain for (g), consequential-marking style). Two points give both β and i; check i is the same from both (i = 20.66 from each ✓).

### (g) Activation energy Ea
**L1 · Answer** β = α²R/Ea →
$$E_a = \frac{\alpha^2 R}{\beta} = \frac{2.235^2 \times 8.314}{1.39\times10^{-3}} = \mathbf{29.9\ kJ\ mol^{-1}}$$
(With the fallback β = 9.456 × 10⁻⁴: Ea = 43.9 kJ mol⁻¹.)
**L2 · Thought** Consequential chain (f) → (g): one substitution. Do *not* compare this Ea to (d)'s 14.8 kJ mol⁻¹ and "correct" one of them — they belong to different pathways (k₁ via the cis-state vs the tunnelling-dominated direct k₂ with its own barrier parameter). Keeping the two kinetic models separate in your head is the physics of the question: Arrhenius behaviour at high T, tunnelling (non-Arrhenius, hence the odd functional form) at low T.

---

## Q6 — Anammox and ladderanes (20 marks)

### (a) Oxidation states of nitrogen
**L1 · Answer**
(i) N₂: **0**; NH₄⁺: **−3**.
(ii) NO₂⁻: **+3**; NH₂NH₂ (hydrazine): **−2**; NH₂OH (hydroxylamine): **−1**.
**L2 · Thought** Each is a one-line allocation; hydroxylamine is the one to slow down on (N–O pair goes to O; N–H pairs go to N; plus the lone pair → −1). These six values drive the whole question — get them wrong and every equation below inherits the error, so double-check the two extremes before proceeding.

### (b) The three steps
**L1 · Answer**
(i) **NO₂⁻ + 4 e⁻ + 5 H⁺ → NH₂OH + H₂O** (N: +3 → −1 = gain of 4 e⁻; audit: charge −1−4+5 = 0 ✓; H 5 = 3+2 ✓; O 2 = 1+1 ✓).
(ii) **NH₄⁺ + NH₂OH → N₂H₄ + H₂O + H⁺** (comproportionation: −3 and −1 → 2 × −2, no electrons; audit: N 2=2; O 1=1; H 4+3 = 4+2+1 ✓; charge +1 = +1 ✓).
(iii) **N₂H₄ → N₂ + 4 H⁺ + 4 e⁻** (N: −2 → 0 = loss of 4 e⁻; audit: H 4=4; charge 0 = 4−4 ✓).
**L2 · Thought** Balance order: oxidation-state audit first (it gives the electron count), then H₂O/H⁺ for O and H, then charge as the final cross-check. Step 1 is the trap: +3 to −1 is a *four*-electron reduction, not two — the charge balance catches any undercounting immediately (with 2 e⁻ the charge can never close: −1 − 2 + 5 = +2 ≠ 0).

### (c) Overall anammox equation
**L1 · Answer** Sum (i) + (ii) + (iii), cancelling NH₂OH, N₂H₄, and the electrons:
**NO₂⁻ + NH₄⁺ → N₂ + 2 H₂O** (audit: N 2=2; O 2=2; H 4=4 ✓; charge −1+1 = 0 ✓).
**L2 · Thought** The celebrated anammox stoichiometry — nitrite and ammonium comproportionating to N₂. Write the three steps with the shared intermediates aligned vertically so the cancellation is visible (NH₂OH and N₂H₄ cancel exactly; 4 e⁻ and the H⁺ balance closes without remainder — a built-in audit).

### (d) Ladderane synthesis: A–K and X
**L1 · Answer**
- **A** = **cyclobutane-1,2-diyldimethanol** — the cyclobutane ring with a –CH₂OH on each of two adjacent carbons (C₆H₁₂O₂ ✓): LiAlH₄ reduces the starting fused cyclic anhydride's two carbonyls all the way to primary alcohols. (A is the *diol*; the five-membered anhydride ring with ring-O and two C=O is the starting material, not A.)
- **B** = the **dimesylate** (both OH → OMs), C₈H₁₆O₆S₂ ✓ (A + 2 MsCl − 2 HCl with Et₃N as base).
- **C** = the **thiacyclopentane fused to cyclobutane** (double intramolecular SN2 by Na₂S across the two CH₂OMs arms, closing a thiolane ring).
- **D** = the **α-chloro sulfoxide**: SO₂Cl₂/pyridine chlorinates the (drawn, unlettered) sulfoxide α to the S=O — the bicyclic thiolane-S-oxide bearing one Cl on an α-carbon next to sulfur (C₆H₉ClOS; **the printed m/z 164.01 (68.3%) / 166.00 (21.8%) is D's molecular ion**: the 3 : 1 pair = exactly one Cl ✓; exact-mass audit 72.00 + 9.07 + 34.97 + 31.97 + 16.00 ≈ 164.01 ✓).
- **Anion E⁻** = D's **carbanion** (C₆H₈ClOS⁻): the strong base (KOtBu) removes the *other* α-proton (α to the sulfoxide S=O, on the carbon next to sulfur that does not carry Cl) — the anion that will displace the neighbouring C–Cl intramolecularly.
- **F** = the **fused thiirane S-oxide** (the anion closes by intramolecular SN2 onto the CHCl carbon: S plus the two α-carbons = the three-membered ring, as stated).
- **X** = **SO, sulfur monoxide** (M = 48.06 ✓; the thiirane S-oxide ejects SO — the Ramberg–Bäcklund-style elimination).
- **G** = **bicyclo[2.2.0]hex-2-ene** (cyclobutene fused to cyclobutane, C₆H₈; ¹³C NMR 141.7 (C=C), 44.1 (bridgeheads), 20.8 (CH₂'s) ✓): after SO leaves, the two α-carbons form the new C=C.
- The drawn **[5]-ladderane core** (five fused cyclobutanes, C₁₂H₁₆) = copper-catalysed [2+2] homodimerisation of two molecules of G across their cyclobutene double bonds.
- **H** = **chloro-[5]-ladderane** (Mn-catalysed C–H chlorination of the ladder).
- **I** = **[5]-ladder-ene** (tBuOK eliminates HCl, installing a ring C=C; ¹³C NMR 140.1 ✓).
- (The drawn structure between I and J — the unlettered intermediate — is the Alder–ene adduct **[5]-ladderanyl–CH₂–CH=CH–(CH₂)₄–OTBS**: I's strained ring alkene as enophile, the terminal alkene TBSO–(CH₂)₄–CH=CH₂ as ene — new C–C bond, H migration, the side-chain C=C shifted into place.)
- **J** = **[5]-ladderanyl–CH₂–CH=CH–(CH₂)₄–OH** (the **free unsaturated alcohol**: HF/pyridine removes the TBS group from the drawn intermediate; the double bond survives).
- **K** = **HO–(CH₂)₇–[5]-ladderane** (H₂/Ni then saturates the side-chain C=C).
- Final: CrO₃/H₂SO₄ oxidises K's primary alcohol → **[5]-ladderanoic acid**, HOOC–(CH₂)₇–[5]-ladderane ✓ (matches the drawn product).
(Reading note: the scheme's arrow order assigns the letters — HF/pyridine acts *before* H₂/Ni, so J still contains the double bond and K is the fully saturated alcohol; the TBS ether itself is the unlettered drawn structure.)
**L2 · Thought** The backbone of the solution is a chain of small fingerprints: the starting 5-ring's three oxygens (ring O + two C=O) mark an *anhydride*, not a diketone (which is why LAH gives a diol of exactly C₆); MsCl/Et₃N is the dimesylate signature; Na₂S closing a thiolane is the sulfur-ring signature; the 164/166 pair is the one-chlorine isotope signature (§4); M = 48.06 is SO, which identifies F as a thiirane S-oxide and the elimination as its standard alkene-forming step; and "copper-catalysed dimerisation" of a cyclobutene is read as [2+2] homodimerisation — 2 rings + 1 new ring + 2 rings = the five fused squares. The side-chain attachment is the Alder–ene signature (terminal alkene + strained alkene → new bond, shifted double bond, no by-products). Every intermediate is verified by formula or by the printed spectrum/mass — formula audit at every station, never a guess.

---

*End of Paper 6 (2020). Next: 2019 Round 1.*

---

# Paper 7 — 2019 UKChO Round 1 (51st IChO selection)

*5 questions, 80 marks, 2 h → ≈ 1.5 min per mark. Marks: Q1 = 11, Q2 = 18, Q3 = 11, Q4 = 27, Q5 = 13.*

## Q1 — Carbon dioxide (11 marks)

### (a)(i) Dot-and-cross diagrams
**L1 · Answer** CO₂: O=C=O, linear (16 e⁻: two double bonds, two lone pairs on each O). CO: :C≡O: (10 e⁻: triple bond, one lone pair on C, one on O; the carbon lone pair is what makes CO bind metals so strongly).
**L2 · Thought** Electron budget first (16 vs 10), then minimise formal charges. The two diagrams share an isoelectronic logic: CO is the C₂²⁻/N₂ pattern from 2020 Q1(a)(ii) — recognising the 10-electron motif makes the unusual carbon lone pair natural rather than alarming.
### (a)(ii) Oxidation-state difference
**L1 · Answer** C in CO₂ = +4; C in CO = +2; **difference = 2**.
**L2 · Thought** One-line allocation each (O wins every C–O bond). Note this is why CO₂ + C ⇌ 2 CO is a comproportionation — the two oxidation states sit exactly one step apart around 0 and +2/+4.

### (b) Fizzy drinks and Henry's law
**L1 · Answer**
(i) [CO₂] = kH × p = 3.3 × 10⁻² × 3.0 = **0.099 mol dm⁻³**.
(ii) mass = 0.099 × 0.250 × 44.01 = **1.1 g**.
(iii) n = 0.099 × 0.250 = 0.0248 mol → p = nRT/V = 0.0248 × 0.08206 × 298/0.250 = **2.4 atm** (mark scheme: 2.45 × 10⁵ Pa ✓ — same answer in SI).
(iv) **High pressure and low temperature** (dissolution is exothermic and favoured by pressure).
**L2 · Thought** Part (iii) is the internal-consistency check of the whole model: the dissolved gas, returned to the gas phase in the same can, should give roughly the original 3.0 atm — the result is 2.4 atm (the small shortfall is the headspace/activity approximation, worth one honest line in L2, not a silent fudge). Gas solubility always rises with p and falls with T (entropic driving: gas → liquid loses translational freedom; heating returns it).

### (c) Maximum safe storage temperature
**L1 · Answer** Safe when p(CO₂) = [CO₂]/kH(T) ≤ 7 atm → kH(T) ≥ 0.099/7 = 0.0141 mol dm⁻³ atm⁻¹. From the graph, kH = 0.0141 at **≈ 60 °C** (the accepted band is generous, **57–63 °C** — the reading tolerance exists because the lookup is graphical).
**L2 · Thought** Two moves chained: the equilibrium pressure from the *current* dissolved concentration (sealed can, so the inventory is fixed), then read the threshold off the curve backwards (from kH to T, not T to kH). The can's rating (7 atm) sets the required kH; the graph converts it to temperature — a "graphical inverse lookup" worth stating as a method, since most students default to plugging T forward.

### (d) Water-gas-shift equilibrium
**L1 · Answer** CO + H₂O ⇌ CO₂ + H₂, extent x forward:
Kp = p(CO₂)p(H₂)/p(CO)p(H₂O) = (20 + x)²/(40 − x)² = 0.64
√: (20 + x)/(40 − x) = 0.80 → 20 + x = 32 − 0.8x → x = 6.67
**CO = 33.3 mol; H₂O = 33.3 mol; CO₂ = 26.7 mol; H₂ = 26.7 mol.**
**L2 · Thought** Δn(gas) = 0, so mole fractions and total pressure cancel — Kp depends only on the mole ratios (spot this before reaching for partial pressures; it is the whole shortcut). The positive root of the squared equation is chosen physically (0.80, not −0.80); back-substitute (26.7/33.3)² = 0.64 ✓ as the audit.

### (e) Enthalpy of the WGS reaction
**L1 · Answer** ΔH = [−393.5 + 0] − [−110.5 + (−241.1)] = **−41.9 kJ**.
**L2 · Thought** One Hess line; note H₂O is *steam* (ΔfH = −241.1, gaseous) — using −285.8 (liquid) would be the silent error, and the data table is the only licence you need (data audit).

---

## Q2 — Industrial separation of precious metals (18 marks)

### (a) Electronic structures
**L1 · Answer** (i) [Kr]4d¹⁰ = **Pd** (palladium — uniquely 4d¹⁰, no s electron at all; Ag would be 4d¹⁰5s¹); (ii) [Xe]4f¹⁴5d⁹6s¹ = **Pt** (platinum, the 5d⁹6s¹ anomaly); (iii) [Xe]4f¹⁴5d⁷6s² = **Ir** (iridium).
**L2 · Thought** The audit is "group number = d + s electron count": (i) 10 → group 10 → Pd (its famous no-5s anomaly); (ii) 9 + 1 = 10 → group 10 → Pt (5d⁹6s¹, not 5d⁸6s²); (iii) 7 + 2 = 9 → **group 9** → period-6 Co-group = Ir (Os would be 5d⁶6s² — the miscount "7 + 2 = 8" lands on Os and is exactly the slip the audit exists to catch; run the count, don't pattern-match).

### (b) Aqua regia dissolutions
**L1 · Answer**
(i) Au + 3 HNO₃ + 4 HCl → HAuCl₄ + 3 NO₂↑ + 3 H₂O (Au 0 → +3; 3 × N(+5) → N(+4); audit: N 3=3; H 7=7; O 9 = 6+3 ✓; Cl 4=4 ✓).
(ii) Pt + 4 HNO₃ + 6 HCl → H₂PtCl₆ + 4 NO₂↑ + 4 H₂O (Pt 0 → +4; audit: N 4=4; H 10=10; O 12 = 8+4 ✓; Cl 6=6 ✓).
**L2 · Thought** Electron audit writes the equation: the metal's oxidation state in the chloro-complex fixes the electron count (Au 3, Pt 4), each HNO₃ accepts exactly one electron (N +5 → +4 in NO₂), and the Cl⁻ for complexation is additional, free acid. Balancing HNO₃ : HCl as (electron count) : (complexation count) keeps the two roles of aqua regia visibly separate.

### (c) AuCl₄⁻ molecular-ion cluster
**L1 · Answer** Binomial over 4 chlorines (⁷⁹Au is unique, ³⁵Cl : ³⁷Cl = 3 : 1):

| composition | m/z | intensity / % |
|---|---|---|
| all ³⁵Cl | 197 + 140 = **337** | 0.75⁴ = **31.6** |
| 3 × ³⁵ + 1 × ³⁷ | **339** | 4 × 0.75³ × 0.25 = **42.2** |
| 2 + 2 | **341** | 6 × 0.75² × 0.25² = **21.1** |
| 1 + 3 | **343** | 4 × 0.75 × 0.25³ = **4.7** |
| 4 × ³⁷Cl | **345** | 0.25⁴ = **0.4** |

(Sum = 100 ✓; the 339 peak dominates — the classic ~1 : 1.33 : 0.67 : 0.15 : 0.01 profile.)
**L2 · Thought** This is the isotope-signature move run forwards (§4): one Au (single isotope) + four Cl (3 : 1) → binomial coefficients 1 : 4 : 6 : 4 : 1 weighted by (0.75)ⁿ(0.25)⁴⁻ⁿ. Sanity: the profile peaks at the 3 : 1 composition (339), not at all-³⁵Cl, because 4 draws favour 3 hits at p = 0.75.

### (d) Chloroauric acid + FeCl₂
**L1 · Answer** HAuCl₄ + 3 FeCl₂ → Au↓ + 3 FeCl₃ + HCl. (Audit: Cl 4+6 = 10 = 9+1 ✓; H 1=1 ✓; Fe 3=3 ✓; Au(III) + 3 e⁻ → Au(0), 3 × Fe(II) → Fe(III) ✓.)
**L2 · Thought** Selective reduction: Fe²⁺ reduces Au(III) all the way to the metal but leaves Pt(IV)/Pd(II) in solution under these conditions — the separation chemistry is just oxidation-state bookkeeping, which is why the equation must show all three Fe²⁺.

### (e) Formula of compound X
**L1 · Answer** **(NH₄)₂PtCl₆** (ammonium hexachloroplatinate(IV)).
Unit-cell audit: Pt at corners + face centres = 8 × ⅛ + 6 × ½ = 4; the PtCl₆ octahedra place Cl on edges and face planes (edges 12 × ¼ = 3, faces/interior 21 → 24 Cl total = 6 × 4 ✓); NH₄⁺ in the tetrahedral holes (8 per cell) → 8 NH₄⁺ : 4 PtCl₆ = (NH₄)₂PtCl₆ with Z = 4 ✓.
**L2 · Thought** The (NH₄)₂PtCl₆ structure is the K₂PtCl₆ type: PtCl₆²⁻ octahedra on an fcc lattice, cations in every tetrahedral hole. Counting confirms the identity that the chemistry already suggested — NH₄Cl precipitating the classic yellow (NH₄)₂PtCl₆ from H₂PtCl₆ is textbook platinum-group refining. Share-count before arithmetic (corners ⅛, edges ¼, faces ½, body 1 — skeleton 7.4).

### (f) Structures of compound Y
**L1 · Answer** Analysis per 100 g: Pd 0.4727 mol; Cl 0.9450; N 0.9493; H 2.877 → ratio 1 : 2.00 : 2.01 : 6.09 → **PdCl₂(NH₃)₂** (diamminedichloropalladium(II)). Square planar → draw **cis and trans** isomers: cis-[Pd(NH₃)₂Cl₂] (two NH₃ adjacent) and trans-[Pd(NH₃)₂Cl₂] (two NH₃ opposite).
**L2 · Thought** The analysis gives the formula; "square planar" is the instruction to enumerate MA₂B₂ geometries (exactly two: cis/trans, both achiral — the improper-symmetry check from §5.5: each has a mirror plane). This is Peyrone's/Reiset's chloride chemistry — the two isomers really do crystallise separately.

### (g) Formation of Y from H₂PdCl₄
**L1 · Answer** H₂PdCl₄ + 4 NH₄OH → Pd(NH₃)₂Cl₂↓ + 2 NH₄Cl + 4 H₂O. (Audit: Pd 1=1; Cl 4 = 2+2 ✓; N 4 = 2+2 ✓; H 2+20 = 6+8+8 = 22 ✓; O 4=4 ✓.)
**L2 · Thought** Write the substitution first (two Cl⁻ replaced by two NH₃), then balance the ammonium counter-ions and waters — the 4 NH₄OH coefficient falls out of the H/O audit, which is the check that you did not "lose" the released HCl (it neutralises half the ammonia to NH₄Cl).

### (h) ¹⁹⁵Pt NMR line counts
**L1 · Answer** Lines = (2N × I) + 1:
(i) cis-[Pt(¹⁴NH₃)₂(H₂O)₂]²⁺: N = 2, I = 1 → **5 lines**;
(ii) [Pt(¹⁴NH₃)₄]²⁺: N = 4, I = 1 → **9 lines**;
(iii) [Pt(¹⁵NH₃)₄]²⁺: N = 4, I = ½ → **5 lines**.
**L2 · Thought** Direct application of the given rule; the chemistry hides in N — count only the equivalent coupling nuclei (the two H₂O ligands couple to nothing, since ¹⁶O has I = 0 and ¹H "is not seen to couple" here — the stem tells you explicitly to ignore the water protons).

### (i) Splitting-pattern intensities
**L1 · Answer** Expand (x² + xy + y²)ⁿ and read coefficients:
(i) cis, n = 2: **1 : 2 : 3 : 2 : 1** (five lines);
(ii) tetraammine, n = 4: convolve n = 3 (1 3 6 7 6 3 1) with (1 1 1): **1 : 4 : 10 : 16 : 19 : 16 : 10 : 4 : 1** (nine lines; coefficients sum to 3⁴ = 81 ✓).
**L2 · Thought** The polynomial is just a generating function for "how many ways to distribute the I = 1 spin states (−1, 0, +1) over n equivalent nuclei" — the coefficient of x^k counts arrangements with that total spin projection. The n = 4 row is built by one convolution step from n = 3, which is the technique the question is really testing (Pascal's triangle is the I = ½ special case of this machinery).

---

## Q3 — Treating nerve agent poisoning (11 marks)

### (a)(i) Molar mass of PAM
**L1 · Answer** PAM = N-methyl-2-pyridine-aldoximinium chloride, C₇H₉ClN₂O:
M = 7(12.011) + 9(1.008) + 35.45 + 2(14.007) + 15.999 = **172.61 g mol⁻¹**.
### (a)(ii) Mass for 24 h treatment
**L1 · Answer** n = 3.00 mmol kg⁻¹ h⁻¹ × 80 kg × 24 h = 5.76 mol → m = 5.76 × 172.61 = **994 g** (≈ 0.99 kg).
**L2 · Thought** The dose chain (mmol kg⁻¹ h⁻¹ × kg × h) is pure unit bookkeeping; the 3.00 mmol/kg/h is *hourly*, so × 24 for the day. ~1 kg of antidote is the deliberately shocking number — it is why oxime dosing in the field uses auto-injectors of the active salt, not the free base.

### (b) Reaction orders in PAM
**L1 · Answer**
(i) Below 0.0002 mol dm⁻³: **first order** (rate rises ~linearly with [PAM]).
(ii) Above 0.0008 mol dm⁻³: **zero order** (rate plateaus at ~17 × 10⁻¹² mol dm⁻³ s⁻¹).
**L2 · Thought** Classic saturation (Michaelis–Menten shape): order is read from the *slope*, not the value — near-linear at the origin, flat at high [PAM]. This is exactly why (c)'s two-step mechanism (binding equilibrium then chemistry) is needed: a single bimolecular step could never plateau.

### (c) Kc expression
**L1 · Answer**
$$K_c = \frac{[AChE\text{-}I\text{-}PAM]}{[AChE\text{-}I]\,[PAM]}$$

### (d) k₂ and Kc from the reciprocal plot
**L1 · Answer** Rearrange kobs = k₂[PAM]/([PAM] + 1/Kc):
$$\frac{1}{k_{obs}} = \frac{1}{k_2} + \frac{1}{k_2 K_c}\cdot\frac{1}{[PAM]}$$
The fitted line is y = 6.75 × 10⁻⁴ x + 1.58:
(i) intercept = 1/k₂ = 1.58 s → **k₂ = 0.633 s⁻¹**;
(ii) slope = 1/(k₂Kc) = 6.75 × 10⁻⁴ mol dm⁻³ s → **Kc = 1/(0.633 × 6.75 × 10⁻⁴) = 2.34 × 10³ dm³ mol⁻¹**.
**L2 · Thought** This is the Lineweaver–Burk linearisation in disguise (intercept = 1/k₂, slope/intercept = 1/Kc) — the same "declare the linearised form before fitting" discipline as 2023 Q4(i). Consistency anchor: 1/Kc = 4.27 × 10⁻⁴ mol dm⁻³ sits exactly at the half-saturation point of the original rate curve (~0.0004 mol dm⁻³ where the rate is half-maximal ✓) — the two graphs tell the same story, and noticing that is the strongest check.

### (e) (E)-1,4-dibromobut-2-ene
**L1 · Answer** BrCH₂–CH=CH–CH₂Br with the two CH₂Br groups **trans** across the double bond (E).
**L2 · Thought** Name → structure: but-2-ene backbone (4 C), Br at 1 and 4 (the termini), E geometry on the only double bond. The E form is what the tandem alkylation below needs to span the two pyridinium ends.

### (f) Number of different reactivators
**L1 · Answer** **9** (3 choices of ring position (2-, 3-, or 4-pyridyl) for the aldoxime ring × 3 for the carboxamide ring).
**L2 · Thought** Each of the two heterocycles can be substituted at the 2-, 3-, or 4-position of its pyridine; the steps are independent, so multiply. The formula anchors ([C₁₀H₁₂N₂OBr]⁺Br⁻ then [C₁₆H₁₈N₄O₂]²⁺(Br⁻)₂) confirm the building blocks (pyridine-aldoxime, then picolinamide) but not the positions — those come from the "N–R indicates either..." note.

### (g) X and Y
**L1 · Answer**
- **X** = **4-aldoxime-1-[(E)-4-bromobut-2-en-1-yl]pyridinium bromide**: the pyridine N of 4-pyridine-aldoxime quaternised by one end of the (E)-dibromobutene (SMILES `[Br-].O/N=C/c1cc[n+](C/C=C/CBr)cc1`). Its ¹³C count: the 4-substituted pyridinium ring is mirror-symmetric (C2/C6 ≡, C3/C5 ≡ → 3 ring signals) + C(H)=N (1) + butenyl chain (4) = **8 signals ✓**.
- **Y** = **the bis-quaternary reactivator with 4-aldoxime on one ring and 4-carboxamide on the other**: [4-(hydroxyiminomethyl)-1-[(E)-4-(4-carbamoylpyridin-1-ium-1-yl)but-2-en-1-yl]pyridinium] dibromide: py⁺(4-CH=NOH)–CH₂–CH=CH–CH₂–py⁺(4-CONH₂) with 2 Br⁻. Signal count: symmetric aldoxime ring (3) + CH=NOH (1) + symmetric carboxamide ring (3) + CONH₂ (1) + chain (4, ends inequivalent) = **12 signals ✓**.
**L2 · Thought** Solve by NMR signal accounting, the same symmetry-orbit method as 2022 Q3(b). The 8-signal constraint on X forces the *symmetric* 4-substituted ring (a 2- or 3-substituted pyridinium of this kind has all ring carbons inequivalent → more signals, ruled out); the 12-signal constraint on Y then forces the *second* ring to be 4-substituted as well. (Count the symmetry of the specific substitution pattern in front of you — 2- vs 3-substituted rings have different residual symmetries — rather than applying one canned number.) Note the chemistry: pyridine N's are the nucleophiles that get quaternised (that is where the two positive charges live), and the second step's reagent is picolinamide (C₆H₆N₂O, identical formula to the aldoxime — the formula list is symmetric by design).

---

## Q4 — Bees and Brexit: thiamethoxam (27 marks)

### (a) Molecular formula of thiamethoxam
**L1 · Answer** **C₈H₁₀ClN₅O₃S** (the oxadiazinane ring (O + 2 N + 2 CH₂ + 1 C) + N–CH₃ + =N–NO₂ + 2-chlorothiazol-5-yl-CH₂: C 3+1+1+3 = 8; H 4+3+2+1 = 10; N 2+2+1 = 5; O 1+2 = 3; Cl 1; S 1 ✓).
**L2 · Thought** Fragment counting with a formula audit at the end — count ring atoms, exocyclic groups, and the heteroaryl separately, then sum. This matches the known pesticide formula exactly.

### (b) A, B, B′, B″
**L1 · Answer**
- **A** = **1,2,3-trichloropropane**, ClCH₂–CHCl–CH₂Cl (all three glycerol OH's replaced by POCl₃; C₃H₅Cl₃ ✓).
- **B** = **2,3-dichloroprop-1-ene**, CH₂=C(Cl)–CH₂Cl (CaO eliminates HCl at C1–C2).
- **B′** = **(E)-1,3-dichloroprop-1-ene**, trans-CHCl=CH–CH₂Cl.
- **B″** = **(Z)-1,3-dichloroprop-1-ene**, cis-CHCl=CH–CH₂Cl (the minor geometric isomer — "much less B″ than B′" fits the less stable Z form).
**L2 · Thought** Elimination regiochemistry: CaO dehydrohalogenates the trichloride; removing HCl from C1–C2 gives the vinyl-chloride alkene (B, no E/Z possible), from C2–C3 gives 1,3-dichloropropene, which *does* have E/Z. The geometric pair must be B′/B″ (stated), so B is the one without geometrical isomers — the puzzle solves itself once you ask "which product has no cis/trans".

### (c) Thiocyanate resonance explaining C
**L1 · Answer** Draw the **N-anionic** resonance form: **S=C=N⁻** (two double bonds, negative charge on nitrogen, S=C=N linear) — the nucleophilic nitrogen explains why B alkylates on N to give the **isothiocyanate** C = CH₂=C(Cl)–CH₂–N=C=S (allyl isothiocyanate), rather than the S-alkylated thiocyanate.
**L2 · Thought** SCN⁻ has two competing resonance forms: S⁻–C≡N (charge on S → S-alkylation) and S=C=N⁻ (charge on N → N-alkylation). The drawn C in the scheme is read from its connectivity (S=C=N–CH₂–…, i.e. the isothiocyanate), so the required resonance is the N-anionic one. This is the ambident-nucleophile lesson: always check which atom of an ambident ion actually reacted before choosing the resonance that "explains" it.

### (d) The electrophile for guanidine → E
**L1 · Answer** The **nitronium ion, NO₂⁺**: linear O=N=O⁺ (from HNO₃/H₂SO₄ — the recurring 2025-Q1/2022-Q5 motif).
**L2 · Thought** Mixed acid → NO₂⁺ again; the question wants the ion *with its shape* (linear), not the nitration equation. Guanidine's NH₂ is then the nucleophile onto NO₂⁺.

### (e) E, F, G, H
**L1 · Answer**
- **E** = **nitroguanidine**: H₂N–C(=NH)–NH–NO₂.
- **F** = **N-methyl-N′-nitroguanidine**: CH₃–NH–C(=NH)–NH–NO₂ (methylamine substitutes the nitroguanidine's NH₂ → NHCH₃, with NH₃ leaving).
- **G** = **bishydroxymethylated F**: (HOCH₂)(CH₃)N–C(=N–NO₂)–NH–CH₂OH (two N–H's methylolated by 2 HCHO; C₄H₁₀N₄O₄ = C₂H₆N₄O₂ + 2 CH₂O ✓, one valid tautomer shown).
- **H** = **the oxadiazinane ring with a free N–H**: 3-methyl-1,3,5-oxadiazinan-4-ylidene(nitro)imine — the two CH₂OH groups of G condense (lose H₂O) into the –CH₂–O–CH₂– bridge, closing the six-membered O–CH₂–N(CH₃)–C(=N–NO₂)–NH–CH₂ ring.
(H + D + K₂CO₃ then N-alkylates the free ring N–H with the thiazolyl CH₂Cl → thiamethoxam.)
**L2 · Thought** Formula audit drives G: F + 2 CH₂O adds exactly C₂H₄O₂ (two hydroxymethyls, no water lost). The "dehydration" step is the tell for the ring closure: only a –CH₂–O–CH₂– bridge (from two hydroxymethyls on the two different guanidine nitrogens) gives the oxadiazinane skeleton of the target. The free N–H in H is then the alkylation site for the thiazolyl chloride — which is why thiamethoxam's ring N–CH₂–thiazolyl bond is the *last* bond formed. The tautomer drawn is free to vary (the question says so); the connectivity is what is marked.

### (f) I and J (alternative route to D)
**L1 · Answer**
- **I** = **2-bromopropanal** (α-bromopropanal), CH₃–CHBr–CHO (C₃H₅BrO ✓; acid-catalysed α-bromination of propanal).
- **J** = the **isothiouronium intermediate**: H₂N–C(=NH)–S–CH(CH₃)–CHO (C₄H₈N₂OS ✓): thiourea's sulfur does SN2 on the α-bromo carbon of I.
(J then cyclises by N–C condensation onto the aldehyde and dehydrates to K = 2-amino-5-methylthiazole, the Hantzsch thiazole product.)
**L2 · Thought** The Hantzsch thiazole synthesis maps atom-by-atom: thiourea S → SN2 on the α-carbon; guanidine N → condenses onto the aldehyde. In the product ring, the thiourea carbon becomes C2 (bearing NH₂), the aldehyde carbon becomes C4 (bearing H), and the α-carbon becomes C5 (bearing CH₃) — that mapping is what makes K = 2-amino-**5**-methylthiazole rather than the 4-methyl isomer, and it is worth writing out explicitly because the whole alternative route hangs on it.

### (g) Lowest-energy tautomer of K
**L1 · Answer** **2-amino-5-methylthiazole** drawn with explicit double bonds: ring S(1)–C(NH₂)=N–CH=C(CH₃)–S, i.e. N=C(NH₂)–S with the C4=C5 double bond — the aromatic 6π system (two ring π bonds (4e) + one sulfur lone pair (2e), benzene-like aromaticity, as the stem states).
**L2 · Thought** The amino (not imino) tautomer preserves the aromatic thiazole ring — that is the entire thermodynamic argument ("one tautomer is aromatic … hence it predominates"). Draw the two ring double bonds and the sulfur's lone pair explicitly; the 2-imino-3H form would break the 6π count and lose.

### (h) L and M
**L1 · Answer**
- **L** = **[5-methylthiazol-2-diazonium] chloride**, [2-diazonio-5-methylthiazol-2-ylium]+ Cl⁻ (NaNO₂/HCl diazotises the 2-amino group; "a chloride salt" ✓).
- **M** = **2-chloro-5-methylthiazole** (the diazonium loses N₂ on warming and is captured by chloride — Sandmeyer logic without copper, driven by the stable diazonium).
(M + CCl₄ then radical-chlorinates the 5-methyl to the 5-chloromethyl of D.)
**L2 · Thought** The 2-aminothiazole is an arylamine: NaNO₂/HCl gives the diazonium chloride; warming ejects N₂ and chloride capture gives the 2-chloro ring — the same diazotisation signature as 2025 Q3(h) (benzenediazonium chloride, [C₆H₅N₂]Cl). The CCl₄ step that follows is the radical-chain chlorination of a methyl attached to an electron-poor heteroaryl ring.

### (i) V·, W·, and Y (radical chain mechanism)
**L1 · Answer**
- **V·** = **CH₂=C(Cl)–CH₂–N=C(Cl)–S·**: the chain radical Cl· adds to the central carbon of the isothiocyanate (C = CH₂=C(Cl)–CH₂–N=C=S), placing the unpaired electron on sulfur (a thiyl radical).
- **W·** = the **cyclic thiyl-derived radical from 5-exo-trig cyclisation**: the S· attacks the internal alkene carbon and the π electrons shift to the terminal carbon — the five-membered ring closes with the radical on the exocyclic methylene: ring S–C(Cl)=N–CH₂–C(Cl)(–CH₂·)–S (2-chloro-5-(·CH₂)-2,3,4,5-tetrahydrothiazole in ring terms).
- **Y** = the ring with the methylene radical capped by chlorine: S–C(Cl)=N–CH₂–C(Cl)(CH₂Cl)–S (the vinyl Cl still on the ring carbon, CH₂Cl installed at what becomes thiazole C5).
**L2 · Thought** The mechanism is assembled by atom-tracking toward the known product (D = 2-chloro-5-(chloromethyl)thiazole): the isothiocyanate's central carbon becomes thiazole C2 (and needs a Cl — that is the ring Cl from Cl·), its sulfur becomes the ring sulfur (which must close onto the internal alkene carbon — the 5-exo closure), the thiocyanate nitrogen stays as ring N3, the allylic CH₂ becomes C4, and the vinyl chloride carbon becomes C5 — its vinyl Cl is ejected during aromatisation while its terminal =CH₂ picks up a new Cl (from X) to become the CH₂Cl substituent. Every atom's destination is thereby forced; the mechanism is *deduced*, not remembered.

### (j) Reagent X and radical Z·
**L1 · Answer** **X = Cl₂** (chlorinates the exocyclic ·CH₂ to CH₂Cl and releases Cl·); **Z· = Cl·** (the chlorine atom, regenerated in that step and re-entering the chain at V·).
**L2 · Thought** Chain logic: the radical that does the capping must be regenerated for the cycle to continue — only X = Cl₂ returns a chlorine atom on being consumed (W· + Cl₂ → Y + Cl·). CCl₄ (the other named reagent) serves as solvent/co-chlorinator, but the stoichiometric regeneration of the *same* radical pins X = Cl₂ and Z· = Cl·. This is the classic radical-chain accounting: identify the carrier by what is consumed and what comes back.

---

## Q5 — A biodegradable plastic: PLA (13 marks)

### (a) Lactic acid and its chiral centre
**L1 · Answer** CH₃–CH(OH)–COOH (2-hydroxypropanoic acid, C₃H₆O₃ ✓); the **α-carbon (the CH bearing OH) is the chiral centre** — mark it with *.
**L2 · Thought** Four different substituents on the α-C (H, CH₃, OH, COOH) — the 2ⁿ-with-meso check is trivial here (one centre). The natural monomer is one enantiomer ((S)-(+)-lactic acid), which is why PLA is crystallisable.

### (b) Polymerisation type (tick)
**L1 · Answer** **Condensation** (each ester bond forms with loss of water between the monomer's –OH and –COOH).
**L2 · Thought** The monomer carries both –OH and –COOH, so it self-condenses with water eliminated at every step — the definition of condensation polymerisation. "Addition" would need a C=C to open (absent here; note PLA made from the lactide in (c) *is* ring-opening addition — a distinction the question quietly offers for free if you spot it).

### (c) Compound A (C₆H₈O₄)
**L1 · Answer** The **lactide**: 3,6-dimethyl-1,4-dioxane-2,5-dione — the six-membered cyclic diester of two lactic acids (ring: O–C(=O)–CH(CH₃)–O–C(=O)–CH(CH₃)); audit: 2 × C₃H₆O₃ − 2 H₂O = C₆H₈O₄ ✓.
**L2 · Thought** DBE audit: C₆H₈O₄ has DBE 3 = two C=O + one ring — a cyclic diester is the unique fit for a PLA-forming C₆ precursor. Ring-opening of the lactide is the industrial route to high-MW PLA (no water to remove), which is why A exists as an alternative to the monomer.

### (d) Average molar mass of the PLA chains
**L1 · Answer** Each chain has one carboxyl end group: n(chains) = n(KOH) = 0.0400 × 6.81 × 10⁻³ = 2.724 × 10⁻⁴ mol
M = 0.1619 g / 2.724 × 10⁻⁴ mol = **594 g mol⁻¹**.
**L2 · Thought** End-group analysis in one line: titrating the single –COOH per chain counts chains directly. The assumption (one acid end per chain, complete dissolution) should be stated; a branched or cyclic fraction would break it (worth one line as the method's boundary).

### (e) Average number of monomer units
**L1 · Answer** Residue mass per lactic acid unit = 72.06 g mol⁻¹; ends = H₂O (18.02):
n = (594.3 − 18.02)/72.06 = **8 monomer units** (≈ 8.0).
**L2 · Thought** The end-group correction (subtract one H₂O for the chain's H + OH termini) is the sophistication the question is testing — without it you get 8.25 and must awkwardly round; with it, a clean 8.0 ✓ (the printed fallback 306 g mol⁻¹ for (d) is the consequential-marking parachute for those who mishandled the titration).

### (f) NaOH for complete degradation of one year's PLA
**L1 · Answer** One NaOH per ester (per monomer residue):
n(residues) = 2.86 × 10¹¹ g / 72.06 g mol⁻¹ = 3.97 × 10⁹ mol
m(NaOH) = 3.97 × 10⁹ × 40.00 = 1.59 × 10¹¹ g = **1.59 × 10⁵ tonnes (≈ 159 000 t)**.
**L2 · Thought** "Ignore end groups" is the licence to treat the polymer as pure repeating residues — one mole of NaOH saponifies one mole of ester links. The mass ladder (tonnes → grams → moles → grams → tonnes) is where unit errors breed; write it once and reuse.

### (g) Amount of acid in the sample
**L1 · Answer** n(NaOH) = 0.100 × 19.40 × 10⁻³ = 1.940 × 10⁻³ mol in the 20.00 cm³ aliquot → in the 100 cm³ stock: × 5 = **9.70 × 10⁻³ mol of carboxyl groups** (free –COOH from lactic acid monomer and from B).
**L2 · Thought** The first titration measures all *free* acid groups — at this stage each B molecule still contributes only its one free –COOH (its ester link is intact until (h)'s reflux hydrolysis). Aliquot factor 100/20 = 5 is the silent step, as always.

### (h) Structure of compound B
**L1 · Answer** The **linear dimer lactoyl-lactic acid**: HO–CH(CH₃)–C(=O)–O–CH(CH₃)–COOH (one ester link, one free OH, one free –COOH).
**L2 · Thought** "A dimer of lactic acid" that is *hydrolysed by boiling NaOH* to give two acids: an ester-linked dimer, not the cyclic lactide (that is A from part (c) — the question is testing whether you keep the two dimers apart: cyclic lactide vs linear lactoyl-lactic acid).

### (i) Masses of lactic acid and B
**L1 · Answer** Back-titration after reflux: NaOH consumed = 4.000 × 10⁻³ − 1.850 × 10⁻³ = 2.150 × 10⁻³ mol, covering the free acid (1.940 × 10⁻³ mol per aliquot, from (g)) **plus one extra NaOH per ester link hydrolysed**:
n(B) in aliquot = 2.150 × 10⁻³ − 1.940 × 10⁻³ = 0.210 × 10⁻³ mol → in the 100 cm³ stock: × 5 = 1.05 × 10⁻³ mol
mass(B) = 1.05 × 10⁻³ × 162.14 g mol⁻¹ (C₆H₁₀O₅) = **0.170 g**
n(lactic acid) = 9.70 × 10⁻³ − 1.05 × 10⁻³ = 8.65 × 10⁻³ mol → mass = 8.65 × 10⁻³ × 90.08 = **0.779 g**
(Closure audit: assigned = 0.170 + 0.779 = 0.949 g; sample was 1.044 g; the remaining 1.044 − 0.949 = **0.095 g is the inert additive fraction** the stem pre-announced ("unreactive other compounds") — not a missing piece of the calculation.)
**L2 · Thought** This is a two-titration difference method: the first titration counts free –COOH (monomer + dimer's free acid), the reflux second titration adds one NaOH per dimer ester bond. The difference isolates B, and B's molecular formula then needs only M = 2 × 90.08 − 18.02 = 162.14. The leftover mass (0.095 g) is not an error — it is the "unreactive other compounds" the stem pre-announced, and checking the books balance to within that declared remainder is the correct closing audit.

---

*End of Paper 7 (2019). Next: 2018 Round 1.*

---

# Paper 8 — 2018 UKChO Round 1 (50th IChO selection)

*5 questions, 81 marks, 2 h → ≈ 1.5 min per mark. Marks: Q1 = 10, Q2 = 12, Q3 = 21, Q4 = 25, Q5 = 13.*

## Q1 — Lithium compounds (10 marks)

### (a) Oxidation states of cobalt
**L1 · Answer** (i) Co in CoO₂ = **+4**; (ii) Co in LiCoO₂ = **+3** (Li(+1) + Co + 2(−2) = 0 → +3).
**L2 · Thought** The intercalation chemistry is a one-electron Co(IV)/Co(III) couple — the cathode half-reaction given (CoO₂ + Li⁺ + e⁻ → LiCoO₂) already contains the answer if you audit electrons: Li⁺ insertion adds the balancing electron.

### (b) Where does Li metal form on overcharge? (circle)
**L1 · Answer** **D — at the cathode, which is the graphite electrode.** (The decisive naming is for the *charging* direction.)
**L2 · Thought** Li metal forms where Li⁺ is **reduced** — during charging that is the graphite electrode, and an electrode under reduction is by definition the **cathode** *for that direction of operation*. The trap is carrying the discharge labels over: the graphite electrode is the anode on *discharge* but becomes the cathode on *charge* (the mark scheme spells this out). So: trace the direction of electron flow during *charging* (Li⁺ + e⁻ → Li at graphite), then name the electrode for that process — "anode/cathode" are process labels, not electrode hardware labels.

### (c) Structure of EC (C₃H₄O₃)
**L1 · Answer** **Ethylene carbonate (1,3-dioxolan-2-one)**: the five-membered cyclic carbonate ring O–CH₂–CH₂–O–C(=O)– (two ring oxygens + one carbonyl). Hydrolysis gives 1,2-ethanediol + CO₂ ✓.
**L2 · Thought** DBE audit: C₃H₄O₃ has DBE 2 = one C=O + one ring. A carbonate whose hydrolysis yields a *diol* must be the cyclic ester of a diol with carbonic acid — the ring is the only structure consistent with both.

### (d) Combustion of lithium (1 : 1 Li₂O : Li₂O₂)
**L1 · Answer** 8 Li + 3 O₂ → 2 Li₂O + 2 Li₂O₂. (Audit: Li 8 = 4+4 ✓; O 6 = 2+4 ✓; the 1 : 1 molar ratio of products fixes the coefficient pair.)
**L2 · Thought** Write the two products with coefficients x and y, set x = y, then scale to integers — the constraint "1 : 1 molar ratio" is an equation, not a comment; use it as the first line of the balance.

### (e) Li₂O₂ + CO₂ (air purification)
**L1 · Answer** 2 Li₂O₂ + 2 CO₂ → 2 Li₂CO₃ + O₂. (Audit: Li 4=4; C 2=2; O 4+4 = 8 = 6+2 ✓.)
**L2 · Thought** Peroxide oxygen is the redox pivot: half of it is oxidised to O₂ while the carbonate locks the CO₂ away — the same disproportionation as Na₂O₂ scrubbers. Counting oxygens last (8 = 8) catches the missing O₂ coefficient instantly.

### (f) Compound A (oxygen storage)
**L1 · Answer**
(i) Per 100 g: Li 6.52/6.94 = 0.940 mol; Cl 33.32/35.45 = 0.940 mol; O 60.16/16.00 = 3.760 mol → ratio 1 : 1 : 4 → **LiClO₄** (lithium perchlorate).
(ii) Dot-and-cross for ClO₄⁻: tetrahedral Cl with **three Cl=O double bonds and one Cl–O⁻ single bond** (formal charges: Cl = 0, single-bonded O = −1, double-bonded O's = 0 — the minimal-charge resonance set; an all-single-bond drawing (Cl +3, four O⁻) is an acceptable alternative but has full charge separation).
(iii) Shape: **tetrahedral** (four bonding domains, no lone pair on Cl).
(iv) Decomposition: **LiClO₄ → LiCl + 2 O₂↑** (all oxygen released as molecular oxygen ✓).
**L2 · Thought** The 1 : 1 : 4 ratio falls out of the cleanest empirical-formula drill (multi-component element balance, §4). For the dot-and-cross, the lesson is formal-charge minimisation: period-3 Cl may expand its octet, and the form with Cl = 0 wins — but the valence-audit line ("hypervalence is electron-count relaxation, not d-orbital bonding") belongs with it (§7.2).

### (g) Oxygen : volume ratio of LiClO₄
**L1 · Answer** Per cm³ of compound: n(LiClO₄) = 2.42/106.39 = 2.27 × 10⁻² mol → n(O₂) = 2 × that = 4.55 × 10⁻² mol
V(O₂ at RTP) = 4.55 × 10⁻² × 24.0 dm³ = 1.09 dm³ = 1.09 × 10³ cm³
**OV ≈ 1.09 × 10³ (≈ 1100 cm³ of O₂ per cm³ of compound)**
**L2 · Thought** OV is a three-link chain: density → moles of compound per cm³ → moles of O₂ (×2 from the decomposition) → gas volume at RTP (24 dm³ mol⁻¹, the stated convention). An OV of ~1100 is why perchlorate "candles" are attractive for the ISS — a thousandfold volume amplification.

---

## Q2 — Making ammonia by lithium cycling (12 marks)

### (a) Half-equations of Step 1
**L1 · Answer** Cathode (reduction): **Li⁺ + e⁻ → Li**; anode (oxidation): **4 OH⁻ → O₂ + 2 H₂O + 4 e⁻**. (Combine: 4 LiOH → 4 Li + 2 H₂O + O₂ ✓.)
**L2 · Thought** Split the printed overall equation at the redox midpoint: Li(I) → Li(0) is the reduction; the hydroxide oxygen (−2) → O₂(0) is the oxidation. Water appears because molten LiOH is H-bearing — atom audit closes it.

### (b) ΔH°, ΔS°, ΔG° for Step 1 at 750 K
**L1 · Answer** (for 4 LiOH → 4 Li + 2 H₂O + O₂)
(i) ΔH° = [4(15.0) + 2(−268) + 15.8] − [4(−446)] = −460.2 + 1784 = **+1324 kJ**;
(ii) ΔS° = [4(63.7) + 2(224) + 236] − [4(128)] = 938.8 − 512 = **+427 J K⁻¹**;
(iii) ΔG° = ΔH° − TΔS° = 1324 − 750 × 0.427 = **+1004 kJ**.
**L2 · Thought** Read the data table's temperature label before substituting (750 K values, not 298 K). The reaction is hugely endothermic with a favourable entropy (gas formed), so ΔG stays positive even at 750 K — which is why an external potential (part (c)) is mandatory.

### (c) Minimum applied potential
**L1 · Answer** n = 4 e⁻ per equation as written:
E(cell) = −ΔG°/(nF) = −1004 × 10³/(4 × 9.65 × 10⁴) = −2.60 V
minimum applied = 2.60 + 0.60 = **3.20 V**
**L2 · Thought** Two stage-setting decisions: n = 4 (the equation produces 4 Li from 4 Li⁺) — using n = 1 is the classic slip; and the overpotential (+0.60 V) is *added to the magnitude* of the decomposition voltage, because the process is non-spontaneous. Sign audit: the cell potential of a non-spontaneous cell is negative; the applied potential must exceed its magnitude.

### (d) Steps 2 and 3, and the Li : NH₃ ratio
**L1 · Answer**
Step 2: **6 Li + N₂ → 2 Li₃N** (Li 0 → +1; N₂ reduced to N³⁻; audit: Li 6 = 6 ✓; N 2 = 2 ✓).
Step 3: **Li₃N + 3 H₂O → 3 LiOH + NH₃** (metathesis; audit: Li 3=3; N 1=1; H 6+3 = 3+... H: 6 = 3+3 ✓; O 3=3 ✓).
Stoichiometric ratio: 6 Li → 2 Li₃N → 2 NH₃ → **Li : NH₃ = 3 : 1**.
**L2 · Thought** The lithium nitride route is just two clean oxidation-state steps: metal nitriding (Li⁰ → Li⁺, N⁰ → N³⁻) then hydrolysis of the nitride (N³⁻ → NH₃). The 3 : 1 ratio is the chain you must carry through (e)–(g); losing the factor of 3 is the only real error available here.

### (e) Mass of lithium generated
**L1 · Answer** Q = It = 0.200 × 1000 = 200 C → n(e⁻) = 200/96 485 = 2.07 × 10⁻³ mol
n(Li) = 2.07 × 10⁻³ × 0.885 = 1.83 × 10⁻³ mol → m = 1.83 × 10⁻³ × 6.941 = **1.27 × 10⁻² g (12.7 mg)**
**L2 · Thought** Faraday chain: charge → moles of electrons → 1 : 1 with Li⁺ → yield 88.5 % applied last (apply the yield to moles, not to charge). Two guard digits carried through — the fallback chain (f) depends on this value.

### (f) Volume of ammonia
**L1 · Answer** n(NH₃) = n(Li)/3 = 1.83 × 10⁻³/3 = 6.11 × 10⁻⁴ mol → V = 6.11 × 10⁻⁴ × 24.0 = **14.7 cm³** (at RTP).
**L2 · Thought** Consequential chain (e) → (d) → (f): moles of Li from (e) divided by the 3 : 1 stoichiometry from (d). Steps 2 and 3 at 100 % yield is the stated licence — quote it before using it.

### (g) Lithium needed for a farm-year of ammonia (no recycling)
**L1 · Answer** NH₃ needed = 130 acres × 0.0770 t acre⁻¹ = 10.01 t → n(NH₃) = 10.01 × 10⁶/17.03 = 5.88 × 10⁵ mol
n(Li) = 3 × 5.88 × 10⁵ = 1.76 × 10⁶ mol → m = 1.76 × 10⁶ × 6.941 = **1.22 × 10⁷ g ≈ 12.2 tonnes**
**L2 · Thought** Same 3 : 1 chain, scaled up; "if the LiOH was not recycled" is the instruction to carry lithium as a consumed reagent (3 Li per NH₃) rather than a catalyst. The striking tonnage (12 t of Li for 10 t of NH₃) is the question's sustainability punchline — recycling is what makes the process viable.

---

## Q3 — Enriched uranium (21 marks)

### (a) Energy released per mole of ²³⁵U
**L1 · Answer** 8.0 kilotons per 0.45 kg → per mole (235.0439 g):
E = 8.0 × 4.184 × 10¹² × (235.0439/450) = **1.75 × 10¹³ J mol⁻¹ (1.75 × 10¹⁰ kJ mol⁻¹)**
**L2 · Thought** Scale by the molar mass ratio, converting kilotons first (1 kiloton = 4.184 × 10¹² J). The 8-digit magnitude (~10¹³ J mol⁻¹) vs chemical bonds (~10⁵–10⁶ J mol⁻¹) is the entire point of nuclear energy — seven orders of magnitude, worth one line.

### (b) Isotope abundances in the crust
**L1 · Answer** Let x = fraction of ²³⁵U: 238.0289 = x(235.0439) + (1 − x)(238.0507)
x = (238.0507 − 238.0289)/(238.0507 − 235.0439) = 0.0218/3.0068 = 0.00725
**²³⁵U = 0.725 %; ²³⁸U = 99.275 %.**
**L2 · Thought** Two-component linear system on the weighted average atomic mass (§4 multi-component balance) — the small difference (238.0507 − 238.0289) against the large span (3.0068) is why the answer is < 1 %. Natural abundance is ~0.72 % ✓ — the number you should expect.

### (c) Essential fluorine property for centrifuge separation (circle)
**L1 · Answer** **B — fluorine has only one naturally occurring isotope.**
**L2 · Thought** The centrifuge separates by mass; if fluorine had two isotopes, every UF₆ molecule would already be a mass distribution and the ²³⁵/²³⁸U split would drown in isotopic noise. The one-isotope property makes each uranium isotope map onto exactly one UF₆ mass — that is the entire basis of the method. (UF₆ being a gas is necessary but not sufficient; the question asks what is *essential for the separation*.)

### (d) Is UF₆ polar? (circle)
**L1 · Answer** **No** — the octahedron of six identical F's is centrosymmetric, so the bond dipoles cancel.
**L2 · Thought** Symmetry decides polarity, not bond polarity: six U–F dipoles point to the vertices of an octahedron and sum to zero (as in SF₆).

### (e) Percentage heavier of ²³⁸UF₆
**L1 · Answer** With integer masses: ²³⁵UF₆ = 235 + 6 × 19 = 349; ²³⁸UF₆ = 352.
(352 − 349)/349 × 100 % = **0.86 %**
**L2 · Thought** The mass difference is only 3 u on a 349-u molecule — less than 1 % — which is why enrichment by physical means needs thousands of centrifuge stages. Integer masses are explicitly instructed, so 19 for F and 235/238 for U.

### (f) Back-conversion to uranium metal
**L1 · Answer**
(i) UF₆ + H₂ → UF₄ + 2 HF (U +6 → +4; audit: U 1=1; F 6 = 4+2 ✓; H 2=2 ✓).
(ii) UF₄ + 2 Mg → U + 2 MgF₂ (U +4 → 0; Mg → Mg²⁺; audit: U 1=1; F 4 = 4 ✓; Mg 2=2 ✓).
**L2 · Thought** Stepwise reduction matching reagent strength: H₂ reduces U(VI) to U(IV) but not further (fluoride lattice too stable), so the harder Mg finishes the job — the oxidation-state staircase (VI → IV → 0) written as two equations.

### (g) Oxidation states in U₃O₈
**L1 · Answer** Mean = +16/3 ≈ 5.33; with the atoms differing by:
(i) **one: +5 and +6** (2 × U(+5) + 1 × U(+6) = +16 ✓);
(ii) **two: +4 and +6** (2 × U(+6) + 1 × U(+4) = +16 ✓).
**L2 · Thought** Set up the integer equations: 2a + b = 16 with b − a = 1 or 2. The second is the textbook assignment for U₃O₈ (a mixed U(IV)/U(VI) oxide); the first is the "differ by one" alternative the question wants you to verify is also arithmetically possible.

### (h) R, T, X, Z in the U₃O₈ → UF₆ scheme
**L1 · Answer**
(i) **R = UO₂(NO₃)₂** (uranyl nitrate): cation **[O=U=O]²⁺, linear** (uranyl, U(VI) ✓); anion **NO₃⁻, trigonal planar** (three O's around N, resonance over one N=O and two N–O⁻).
(ii) **T = (NH₄)₂U₂O₇** (ammonium diuranate): two tetrahedral **NH₄⁺** cations; anionic part **U₂O₇²⁻**. Mass audit: 2 × 18.04 + (2 × 238.03 + 7 × 16.00) = 36.08 + 588.06 = **624.13 g mol⁻¹ ✓**.
(iii) **X = UO₂** (U(IV) oxide; audit: 88.1 % U: 238.03/(238.03 + 32.00) = 88.1 % ✓); **Z = UF₄** (M = 238.03 + 4 × 19.00 = **314.03 g mol⁻¹ ✓**).
**L2 · Thought** Solve by the fingerprints, hardest first: "all uranium +VI" fixes the uranyl ion; the two tetrahedral cations + 624.13 lock the diuranate; the U : O mass ratio in X gives the dioxide (and the H₂ step is just U(VI) → U(IV) reduction); the 314.02 molar mass is a dead giveaway for UF₄ — which is also what the next step (F₂ → UF₆) requires. Note the process logic matches the real nuclear fuel cycle (ADU precipitation → reduction → hydrofluorination → fluorination).

### (i) Alpha-decay equations
**L1 · Answer**
²³⁵U → ²³¹Th + ⁴He (mass 235 → 231 + 4 ✓; charge 92 → 90 + 2 ✓);
²³⁸U → ²³⁴Th + ⁴He (238 → 234 + 4 ✓; 92 → 90 + 2 ✓).
**L2 · Thought** Alpha decay: mass number −4, atomic number −2 — the two conservation laws (mass number, charge) written first, then identify the daughter element by Z (90 = thorium).

### (j) Half-lives from the graph
**L1 · Answer** (i) **²³⁵U ≈ 7 × 10⁸ years** (mass halves 24 → 12 mg at ~0.7 × 10⁹ y); (ii) **²³⁸U ≈ 4.5 × 10⁹ years** (24 → 12 mg at ~4.5 × 10⁹ y).
**L2 · Thought** Read the halving, not the endpoint: pick a clean initial mass (24 mg) and find the time at 12 mg on each curve. Both readings match the known values (0.70 and 4.47 Gyr) — use the gridlines, not the curve tails.

### (k) Age of the Earth
**L1 · Answer** With N₀(²³⁵U) = N₀(²³⁸U) at formation, today's ratio (from (b)) is 0.725/99.275 = 0.00730:
N(²³⁵U)/N(²³⁸U) = e^{−(λ₂₃₅ − λ₂₃₈)t}
t = ln(1/0.00730)/(λ₂₃₅ − λ₂₃₈) = ln(137.2)/(9.846 × 10⁻¹⁰ − 1.551 × 10⁻¹⁰ y⁻¹)
= 4.922/(8.295 × 10⁻¹⁰) = **5.9 × 10⁹ years (≈ 6 × 10⁹ y)**
**L2 · Thought** This is the "nuclear clock" method: the differential decay constant (λ₂₃₅ − λ₂₃₈) and the current isotope ratio give the elapsed time directly. State the assumption (equal initial numbers) before computing — the method overestimates the accepted 4.5 × 10⁹ y precisely because primordial ²³⁵U/²³⁸U was not exactly 1 and later production/loss processes are ignored; stating the idealisation is part of the answer, not a caveat after it.

---

## Q4 — Cough suppressants: dextromethorphan (25 marks)

### (a) The protonated atom in the salt (circle)
**L1 · Answer** The **tertiary amine nitrogen** of the morphinan (the ring N–CH₃, the only basic site in the molecule).
**L2 · Thought** Basicity audit: the molecule contains one N (a tertiary aliphatic amine) and an aryl methyl ether (non-basic). Ammonium salt formation with HBr protonates the lone pair on N — the ether oxygen is a distractor.

### (b) Molecular formula and salt molar mass
**L1 · Answer** Dextromethorphan = **C₁₈H₂₅NO** (M = 271.40). Hydrobromide monohydrate = C₁₈H₂₅NO·HBr·H₂O:
M = 271.40 + 80.91 + 18.02 = **370.33 g mol⁻¹**.
**L2 · Thought** Fragment count: morphinan C₁₇H₂₃N skeleton (4 rings, C₁₇) + OCH₃ (1C) → C₁₈. The salt's mass must include both HBr and the water of crystallisation — dropping the hydrate is the classic slip (and the question names it "monohydrate" for a reason).

### (c) A, B, C, D, E, X (first part of the synthesis)
**L1 · Answer**
- **A** = 4-methoxybenzyl chloride, 4-MeO–C₆H₄–CH₂Cl (SOCl₂ on the benzyl alcohol).
- **B** = (4-methoxyphenyl)acetic acid, 4-MeO–C₆H₄–CH₂–COOH (Mg → Grignard, CO₂, acidic work-up; IR 3100 broad + 1716 sharp = carboxylic acid ✓).
- **C** = (4-methoxyphenyl)acetyl chloride, 4-MeO–C₆H₄–CH₂–COCl (SOCl₂ again).
- **D** = **2-(cyclohexylidene)acetonitrile**: cyclohexane ring with an exocyclic =CH–CN (the Knoevenagel product (cyclohexylidene-cyanoacetic acid, ring–C=C(CN)COOH) decarboxylates on heating, losing X).
- **E** = **2-(cyclohex-1-en-1-yl)ethanamine**: ring–CH= with the C=C *inside* the ring, –CH₂CH₂NH₂ (LAH reduces C≡N → CH₂NH₂; the acidic aqueous work-up isomerises the exocyclic methylene to the more stable internal alkene — the double-bond position in E is back-inferred from the structure of F drawn downstream, not assigned arbitrarily: §4 downstream-structure arbitration).
- **X** = **CO₂** (M = 44.01 ✓, the decarboxylation gas).
**L2 · Thought** The Knoevenagel–decarboxylation sequence is the engine: cyclohexanone + cyanoacetic acid (an active-methylene C–H twice as acidic — see (d)) condenses to the alkylidene cyanoacid, which loses CO₂ to the alkylidene nitrile. The alkene position question (exocyclic in D, internal in E's product) is settled by the structure of F drawn below it — always let the downstream structure arbitrate; the acidic work-up does the isomerisation walk (cf. 2025 Q5 K→M).

### (d) Anions of cyanoacetic acid
**L1 · Answer**
(i) **Z⁻** = N≡C–CH₂–COO⁻ (the carboxylate, OH deprotonated).
(ii) **Z²⁻** = N≡C–CH(⁻)–COO⁻ (both the carboxylate and the α-carbanion: the C–H between CN and COOH is acidic enough for the second deprotonation).
**L2 · Thought** Acidity ordering: the carboxyl OH goes first (ordinary acid), the doubly-activated α-C–H second (nitrile + carboxylate both stabilise the anion). The dianion is what makes cyanoacetic acid such a strong Knoevenagel donor — and why KOH suffices for both steps.

### (e) The two carbons connected in F → G
**L1 · Answer** **C9 and C13** (the figure's numbering: the amide carbonyl carbon and the far sp² junction carbon of the cyclohexene).
**L2 · Thought** The Bischler–Napieralski logic: POCl₃ turns the amide into a nitrilium (C9≡N⁺), and the cyclohexene π-bond attacks it. Ring-size filter decides the regiochemistry: bonding C9 to the near junction would close a five-membered ring; bonding to the far junction (C13) closes the six-membered ring actually drawn in G (fused to the original cyclohexane). The cation then deprotonates to the imine with the fusion C=C, consistent with G = F − H₂O.

### (f) H and cation I⁺
**L1 · Answer**
- **H** = **1-(4-methoxybenzyl)-1,2,3,4,5,6,7,8-octahydroisoquinoline** (the fully saturated secondary amine; H₂/Ni reduces both the imine and the fusion C=C of G; C₁₇H₂₃NO ✓).
- **I⁺** = the **N-methylene iminium** [octahydroisoquinolin-2-yl=CH₂]⁺ (the secondary amine + formaldehyde/H⁺ → [N=CH₂]⁺; NaBH₄ then delivers hydride to give J, the N-methyl tertiary amine).
**L2 · Thought** HCHO/H⁺ then NaBH₄ is reductive methylation in disguise: amine + formaldehyde → iminium → reduced to N–CH₃. The cation I⁺ is the Eschenmoser iminium (N=CH₂) — drawing it as the iminium (not the carbinolamine) is what the mark is for.

### (g) Pairs of carbons that can be connected in J → M₁/M₂
**L1 · Answer** **C4–C13 and C4–C15**: the junction/cation carbon C4 can connect to **either of the two ortho carbons** of the aromatic ring (C13 or C15) — the two pairs exist because of the **symmetry of the substituted benzene ring**, not because of two different junction carbons.
**L2 · Thought** The correct mental model: the ring's mirror symmetry makes C13 and C15 equivalent-looking ortho sites, so *two* connectable pairs exist — but both closures give the *same* morphinan connectivity, and **it is NOT the case that one pair gives M1 and the other M2**. The M1/M2 difference is decided earlier and elsewhere: which *face* of the alkene in intermediate K is protonated to make carbocation L⁺ (face-selective protonation → opposite fusion stereochemistry). Lesson: when asked "which pairs can be connected", enumerate by symmetry first (here: one cation carbon × two equivalent ortho carbons = two pairs); do not conflate the connectivity question with the stereochemistry question — they live in different steps.

### (h) K, L⁺, and Y
**L1 · Answer**
- **K** = **1-(4-hydroxybenzyl)-2-methyl-1,2,3,4,5,6,7,8-octahydroisoquinoline** (the phenol form of J: the anisole O–CH₃ cleaved to phenol by hot aqueous H₃PO₄).
- **L⁺** = the **tertiary carbocation at the saturated-ring junction (C4 in the figure's numbering — the carbon shared by both connectable pairs in (g))**: the junction methine between the piperidine and cyclohexane rings that becomes the morphinan's quaternary fusion carbon.
- **Y** = **methanol, CH₃OH** (M = 32.04 ✓, from the O-demethylation).
**L2 · Thought** The mass of Y (32.04) is the fingerprint that identifies the J → K step as O-demethylation (anisole → phenol + MeOH) — solve that first, and K's identity follows. The Grewe cyclisation cation is a *junction* cation: it forms at the methine shared by the two saturated rings because that is the position that becomes quaternary in the morphinan (bonded to both saturated rings and, after closure onto the aryl ortho carbon (C13 or C15), to the aromatic ring). Phenol (not anisole) is required because only the free phenol makes the ortho position sufficiently nucleophilic for the ring closure — the demethylation is therefore mechanistically *necessary*, not cosmetic.

### (i) M₁ and M₂
**L1 · Answer** M₁ and M₂ are **dextrorphan and levorphanol** (3-hydroxymorphinan), the tetracyclic morphinan skeleton with the free phenol:
- M₁: draw the morphinan with the C13 methine junction H **wedged** (out of the plane) — the fusion stereochemistry matching dextromethorphan;
- M₂: draw the same skeleton with the C13 junction H **dashed** (behind the plane) — matching levomethorphan.
(Methylation of the phenol OH (PhNMe₃Cl) then converts M₁/M₂ to dextromethorphan/levomethorphan.)
**Type of isomers: enantiomers** — the two structures are non-superimposable mirror images (all stereocentres inverted: (9R,13R,14R) vs (9S,13S,14S)); the D-tartaric acid resolution that follows works precisely because they are enantiomers (diastereomeric salts).
**L2 · Thought** Racemic J (built by achiral reductions) cyclises from either face of the junction cation, so both morphinan enantiomers form. The classification question is the real test: M₁/M₂ are not cis/trans, not conformational, not diastereomers at one centre — they are full mirror images, which is why a *chiral* resolving agent can separate them. The wedge/dash instruction is telling you to draw the mirror relationship explicitly at every stereocentre, not just one.

---

## Q5 — The 'inert' gas helium (13 marks)

### (a) Moles of helium in the atmosphere
**L1 · Answer** m = 0.916 mg m⁻³ × 4.2 × 10⁹ km³ = 0.916 × 10⁻³ × 4.2 × 10¹⁸ g = 3.85 × 10¹⁵ g
n = 3.85 × 10¹⁵/4.003 = **9.6 × 10¹⁴ mol**
**L2 · Thought** The unit ladder is the whole battle: km³ → m³ (×10⁹) and mg → g (×10⁻³). An atmosphere-scale answer in moles should still be astronomically large — 10¹⁴–10¹⁵ mol is the right order.

### (b) Number of party balloons
**L1 · Answer** V(balloon) = (4/3)π(0.14)³ = 0.01149 m³ = 11.49 dm³ → n per balloon = 11.49/24.0 = 0.479 mol
N = 9.61 × 10¹⁴/0.479 = **2.0 × 10¹⁵ balloons**
**L2 · Thought** Two conversions: sphere volume (radius in m), then the RTP molar volume (24 dm³ mol⁻¹ — the stated convention; using 22.4 dm³ would be the silent error). Two quadrillion balloons is the rhetorical point of the question — the atmosphere's helium stock is finite but vast.

### (c) Atoms in the unit cell of X
**L1 · Answer** **He: 8 corners × ⅛ + 6 face centres × ½ = 4. Na: 8 atoms fully inside the cell (at the sub-cube centres) = 8.** Net: 8 Na and 4 He per unit cell.
**L2 · Thought** Share-count before arithmetic (corners ⅛, faces ½, interior 1 — skeleton 7.4); the "cubically within" positions are interior and count in full. This is the fluorite (CaF₂-type) lattice with He on the Ca sites and Na on the F sites — recognising it makes (d) trivial.

### (d) Formula of compound X
**L1 · Answer** **Na₂He** (8 Na : 4 He = 2 : 1).
**L2 · Thought** The count in (c) writes the formula directly — 2017's genuinely surprising helium compound (Nature Chemistry). No helium valence is violated because, as (f) explains, the He atoms are not covalently bonded at all.

### (e) Density of X
**L1 · Answer** Cell edge a = 3.95 Å → V = (3.95 × 10⁻⁸)³ = 6.16 × 10⁻²³ cm³
mass = (8 × 22.99 + 4 × 4.003)/6.022 × 10²³ = 3.32 × 10⁻²² g
ρ = 3.32 × 10⁻²²/6.16 × 10⁻²³ = **5.4 g cm⁻³**
**L2 · Thought** Density = cell mass / cell volume, with the cell content from (c) — a fully consequential chain. Sanity anchor: ~5 g cm⁻³ sits between a light metal fluoride and a heavy oxide — plausible for a compressed Na/He lattice at 300 GPa.

### (f) What is X? (circle all)
**L1 · Answer** **C (an ionic solid) and E (an insulator).**
**L2 · Thought** The stem's own evidence decides: Na⁺ ions + localised electron pairs in the lattice gaps = an electride-like *ionic* solid; localised (not delocalised) electrons → no metallic conduction → insulator, ruling out A and D. B is excluded because there is no covalent network — helium sits in the lattice essentially unbonded.

### (g) Decomposition of X
**L1 · Answer** Na₂He → 2 Na + He. (Audit: Na 2=2; He 1=1 ✓.)
**L2 · Thought** At atmospheric pressure the compound is metastable only above ~160 GPa (part (h)), so the decomposition at ambient pressure is just atomisation to the elements.

### (h) Minimum pressure for favourable formation
**L1 · Answer** **≈ 160 GPa** — where ΔdecompG crosses zero; above it, decomposition is endergonic, so formation is thermodynamically favourable.
**L2 · Thought** Sign discipline: the graph plots the *decomposition* free energy, so formation is favourable exactly where ΔdecompG > 0. Read the zero crossing (≈160 GPa), not the plateau. This matches the reported ~113–160 GPa stability window for Na₂He — the question's 300 GPa synthesis pressure sits safely above it.

---

*End of Paper 8 (2018). Next: 2017 Round 1.*

---

# Paper 9 — 2017 UKChO Round 1 (49th IChO selection)

*5 questions, 75 marks, 2 h → ≈ 1.6 min per mark. Marks: Q1 = 8, Q2 = 11, Q3 = 23, Q4 = 21, Q5 = 12.*

## Q1 — The Green Pool of Rio (8 marks)

### (a) Oxidation state of Cl in NaClO
**L1 · Answer** **+1** (Na⁺ + Cl + (−2) = 0 → Cl = +1).
**L2 · Thought** One-line allocation; the +1 state is what makes hypochlorite both an oxidant and a comproportionation partner for Cl⁻ (part (c)).

### (b) Hypochlorite–conjugate acid equilibrium
**L1 · Answer** ClO⁻ + H₂O ⇌ HClO + OH⁻.
**L2 · Thought** The conjugate acid of a base is written by proton transfer from water; the equilibrium lies further right in acid — which is why (c) works.

### (c) Chlorine from hypochlorite + HCl
**L1 · Answer** ClO⁻ + Cl⁻ + 2 H⁺ → Cl₂ + H₂O. (Audit: Cl 2=2; charge −2+2 = 0 ✓; H 2=2 ✓; O 1=1 ✓.)
**L2 · Thought** Comproportionation: Cl(+1) + Cl(−1) → 2 Cl(0) — the oxidation-state audit writes the 1 : 1 ratio before the atoms. Under acidic conditions (b) also supplies the HClO, which is the actual oxidant; the net ionic equation is the same.

### (d) H₂O₂ destroys hypochlorite
**L1 · Answer** ClO⁻ + H₂O₂ → Cl⁻ + H₂O + O₂. (Audit: Cl 1=1; H 2=2 ✓; O 1+2 = 1+2 ✓.)
**L2 · Thought** Here hydrogen peroxide acts as the *reductant* (peroxide O −1 → O₂ 0), reducing Cl(+1) to Cl(−). This is the pool story's chemistry: adding an oxidant (H₂O₂) to a chlorinated pool destroyed the disinfectant and let algae bloom — the roles of H₂O₂ as oxidant *or* reductant are decided by the partner's oxidation state, never by habit.

### (e)(i) Formation of nitrogen trichloride
**L1 · Answer** NH₃ + 3 ClO⁻ → NCl₃ + 3 OH⁻. (Audit: N 1=1; Cl 3=3; H 3=3; O 3=3 ✓.)
### (e)(ii) Structure of NCl₃
**L1 · Answer** **Trigonal pyramidal** (like NH₃: 3 bonds + 1 lone pair), Cl–N–Cl ≈ **107°** (lone pair compresses the tetrahedral angle below 109.5°).
**L2 · Thought** VSEPR domain count (4 domains, 1 lone pair) → pyramidal; NCl₃'s large Cl substituents push the angle toward the upper end of the NH₃-like range (~107°).

### (f) Hydrazine from ammonia + hypochlorite
**L1 · Answer** 2 NH₃ + ClO⁻ → H₂N–NH₂ + Cl⁻ + H₂O. (Audit: N 2=2; Cl 1=1; H 6+0 = 4+2 = 6 ✓; O 1=1 ✓.)
**L2 · Thought** This is the Raschig first step in disguise (chloramine formation then condensation with a second ammonia); the different outcome from (e) is decided by the NH₃ : ClO⁻ ratio — excess ammonia favours hydrazine, excess hypochlorite over-chlorinates to NCl₃. The balance is closed by the N–N bond (two nitrogens, one oxidised per hypochlorite).

### (g) The blue precipitate on Ryan Lochte's hair
**L1 · Answer** **Cu(OH)₂** (copper(II) hydroxide — blue, precipitates from copper(II) sulfate at the high pH of some shampoos).
**L2 · Thought** High pH + Cu²⁺ → the insoluble hydroxide (not the sulfate, which is soluble). The green hair = yellow bleached hair + blue Cu(OH)₂ deposit; the identity is decided by the pH clue, not by the copper's blue salt colour alone (CuSO₄·5H₂O is blue too, but soluble).

---

## Q2 — Atmospheric chemistry (11 marks)

### (a) H₂S + OH radical
**L1 · Answer** H₂S + ·OH → H₂O + ·SH (the hydroxyl radical abstracts a hydrogen atom in a single encounter).
**L2 · Thought** "Single encounter" is the instruction to write an atom-transfer, not a chain: ·OH takes H· from H₂S, leaving the thiyl radical ·SH — the first step of atmospheric sulfur oxidation (cf. 2024 Q5's H-abstraction move).

### (b) Laboratory generation of H₂S
**L1 · Answer** FeS + 2 HCl → FeCl₂ + H₂S↑. (Audit: Fe 1=1; S 1=1; Cl 2=2; H 2=2 ✓.)
**L2 · Thought** Metal sulfide + strong acid → weak acid gas — the standard H₂S prep; Fe(II) stays in solution.

### (c) Atmospheric [H₂S]
**L1 · Answer** Steady state: production = consumption:
7.65 × 10⁵ = k[H₂S][·OH] = 4.7 × 10⁻¹² × [H₂S] × 1.1 × 10⁶
$$[H_2S] = \frac{7.65\times10^{5}}{5.17\times10^{-6}} = \mathbf{1.48\times10^{11}\ molecules\ cm^{-3}}$$
**L2 · Thought** "Concentration constant over time" = steady state, so the emission rate IS the removal rate — one line of kinetics, no differential equations. Dimensional check: cm³ molecule⁻¹ s⁻¹ × molecules cm⁻³ × molecules cm⁻³ = molecules cm⁻³ s⁻¹ ✓.

### (d) Convert to μg m⁻³
**L1 · Answer** 1.48 × 10¹¹ molecules cm⁻³ × 34.08 g mol⁻¹/6.022 × 10²³ = 8.37 × 10⁻¹² g cm⁻³ = **8.4 μg m⁻³**.
**L2 · Thought** Unit ladder: molecules → mass (Nₐ, with M(H₂S) = 34.08), then cm⁻³ → m⁻³ (×10⁶), then g → μg (×10⁶). The two ×10⁶ factors cancel the cm³→m³ and g→μg conversions — a clean way to check the arithmetic direction.

### (e) Partial combustion and Claus chemistry
**L1 · Answer**
(i) 2 H₂S + 3 O₂ → 2 SO₂ + 2 H₂O. (Audit: S 2=2; H 4=4; O 6=6 ✓.)
(ii) 2 H₂S + SO₂ → 3 S + 2 H₂O. (Audit: S 3=3; H 4=4; O 2=2 ✓.)
**L2 · Thought** The Claus process: burn one-third of the H₂S to SO₂ (S −2 → +4), then comproportionate with the rest (S −2 and S +4 → S 0). The oxidation-state audit makes (ii) balance itself: 2 × S(−2) + 1 × S(+4) → 3 × S(0).

### (f) Half-life of 1,1,1-trichloroethane
**L1 · Answer**
(i) From the graph, the concentration halves in **t₁/₂ ≈ 3.8 years** (mark scheme accepts **3.7–3.9 years**).
(ii) t₁/₂ = 3.8 × 3.156 × 10⁷ s = **1.20 × 10⁸ s** (3.7 y → 1.168 × 10⁸; 3.9 y → 1.231 × 10⁸).
**L2 · Thought** Read the halving (not the endpoint), and check it on a *second* interval to confirm exponentiality before quoting — two consistent halvings are worth more than one lucky reading. If your reading falls outside the accepted band (3.7–3.9 y), re-check the half-life read-off before carrying it into (g) — the value feeds directly into the OH concentration.

### (g) Global OH radical concentration
**L1 · Answer** k_obs = ln 2/t₁/₂; with [·OH] constant, decay is pseudo-first-order and [·OH] = k_obs/k₂nd = 0.693/(1.0 × 10⁻¹⁴ × t₁/₂):
$$[\cdot OH] = \frac{6.93\times10^{13}}{1.20\times10^{8}\ \text{s}} = \mathbf{5.8\times10^{5}\ molecules\ cm^{-3}}$$
(5.93 / 5.78 / 5.63 × 10⁵ for t₁/₂ = 3.7 / 3.8 / 3.9 y respectively.)
**L2 · Thought** Pseudo-first-order logic: with [·OH] constant, the decay is first-order with k_obs = k₂nd[·OH] — the molecule you can measure (1,1,1-trichloroethane) becomes the reporter for the radical you cannot. The stem's note "you may not get exactly the same result as [the 1.1 × 10⁶ cm⁻³] given earlier" licenses the factor-of-2 gap: quote your value with its derivation rather than massaging the half-life toward the earlier number.

---

## Q3 — The chemistry of Iron Man (23 marks)

### (a) TiCl₄ + NH₃ for TiN films
(i) Oxidation state of Ti in TiN: **+3** (N³⁻).
(ii) **Nitrogen is oxidised** (some NH₃'s N(−3) → N₂(0)).
(iii) **Titanium is reduced** (Ti(+4) → Ti(+3)).
(iv) Balance: Ti: a = c; Cl: 4a = d; H: 3b = d; N: b = c + 2e →
$$6\,TiCl_4 + 8\,NH_3 \longrightarrow 6\,TiN + 24\,HCl + N_2$$
(Audit: Ti 6=6; Cl 24=24; H 24=24; N 8 = 6+2 ✓.)
**L2 · Thought** Balance by oxidation-state audit first: Ti gains 1 e⁻ per atom, so the N that is oxidised must supply 1 e⁻ per Ti; the N₂ product takes 2 N per molecule — solve the three conservation equations as a small linear system rather than trial-and-error. Note the redox subtlety: most of the nitride nitrogen ends up in TiN (still −3), only a fraction is oxidised to N₂.

### (b) Masses for 40 kg of Ti₃Au
**L1 · Answer** M(Ti₃Au) = 3 × 47.87 + 196.97 = 340.58 g mol⁻¹
Ti = 40 × 143.61/340.58 = **16.9 kg**; Au = 40 × 196.97/340.58 = **23.1 kg**
**L2 · Thought** Mass-fraction by formula unit — the formula is a mole ratio, so compute one unit's mass first and split by mass contribution, not by atom count.

### (c) Coordination in α-Ti₃Au (Au at corners, Ti at face centres; a = 4.15 Å)
**L1 · Answer**
(i) Each Au is surrounded by **12 Ti** (the corner touches 12 face centres at a/√2 — 3 faces per cell × 8 cells ÷ 2 (each face shared by 2 cells) = 12; a cuboctahedron).
(ii) Each Ti is surrounded by **4 Au** (the 4 corners of its own face at a/√2).
(iii) Each Ti is surrounded by **8 Ti** (the other 8 face centres at a/√2).
**L2 · Thought** This is the L1₂ (Cu₃Au-type) lattice, and the counts must satisfy the stoichiometric identity Au:Ti = 1 : 3 → (Ti per Au) : (Au per Ti) = 3 : 1 ✓ (12 : 4) — the self-consistency audit that catches the "each face counts once" error (each corner's 24 face-touches are shared between two cells).

### (d) α-Ti₃Au distances
**L1 · Answer**
(i) Ti–Au = face-diagonal half = a/√2 = 4.15/√2 = **2.93 Å**;
(ii) shortest Ti–Ti = between adjacent face centres (e.g. top face centre to front face centre) = a/√2 = **2.93 Å**.
**L2 · Thought** Both distances collapse to the same a/√2 — the L1₂ lattice has only one near-neighbour distance, which is the geometric reason the α-form is so uniformly hard. Drawing the two right triangles (corner→face-centre; face-centre→adjacent face-centre) is faster than memorising.

### (e) Coordination in β-Ti₃Au (Au at corners + body centre; Ti in face pairs; a = 5.09 Å)
**L1 · Answer**
(i) Each Au is surrounded by **12 Ti** (body-centre Au sees 2 Ti on each of 6 faces at a√5/4; corner Au sees the nearer Ti of each pair on 3 faces × 8 cells ÷ 2 = 12).
(ii) Each Ti is surrounded by **4 Au** (2 corner Au on its own face at a√5/4 + the body-centre Au above and below at a√5/4).
(iii) Ti neighbours: **2 nearest** (its partner on the same face at a/2 *and* the chain continuation in the adjacent cell at a/2 — the Ti chains run unbroken along the cell edges) and **8 next-nearest** (four within the same cell — two on the top face and one nearest-the-front on each side face — plus the four in similar positions in the cell in front: the chain-boundary continuation is what doubles the naive count of 4 — the answer is nearest 2, next-nearest 8).
**L2 · Thought** This is the A15 (Cr₃Si-type) structure: Au forms a bcc sublattice and Ti forms linear chains along the three edge directions. The "nearest neighbour" trap is forgetting that the face pair continues across the cell boundary (the chain is infinite, so each Ti has a partner on *both* sides); the next-nearest trap is counting only the four within the drawn cell — four more sit at the same distance in the adjacent cell, and only the cross-boundary count (8) is correct. The stoichiometric audit still holds (Au:Ti = 1 : 3 → 12 : 4 ✓). Next-nearest distances: pair axis ⊥ pair axis at a√6/4 — compute one explicitly ((a/4, a/2, 0) → (0, a/4, a/2)) before generalising.

### (f) β-Ti₃Au distances
**L1 · Answer**
(i) Ti–Au = a√5/4 = 5.09 × √5/4 = **2.85 Å**;
(ii) next-nearest Ti–Ti = a√6/4 = 5.09 × √6/4 = **3.12 Å** (nearest is a/2 = 2.55 Å).
**L2 · Thought** Two independent Pythagorean checks: a√5/4 comes from (a/4, a/2) in-plane components, a√6/4 from (a/4, a/4, a/2) — writing the fractional coordinates of one Ti and its neighbours before computing is the only reliable way to avoid the √5/√13 confusion (a√13/4 is the tempting wrong face-diagonal).

---

## Q4 — The molecule twistane (21 marks)

### (a) Ideal C–C–C angle vs regular hexagon
**L1 · Answer** 120° (regular hexagon) − 109.5° (tetrahedral) = **10.5°**.
**L2 · Thought** The chair's near-tetrahedral angles are precisely why it is the low-energy conformer; the question calibrates "ideal" = tetrahedral before asking you to compare.

### (b) Unique six-membered rings of adamantane
**L1 · Answer** (in the figure's numbering; the printed example -1-2-3-4-5-6- earns no credit):
**-1-2-3-9-10-7-**; **-1-6-5-8-10-7-**; **-3-4-5-8-10-9-**.
**L2 · Thought** Adamantane's carbon graph is K₄ on the four bridgeheads with a CH₂ on every edge: each K₄ triangle = one chair ring, and there are exactly 4 triangles — one is the printed example (-1-2-3-4-5-6-, bridgeheads {1,3,5}), so the answer set is the other three: {1,3,10}, {1,5,10}, {3,5,10}, each written through its connecting CH₂'s in cyclic order (and starting from its lowest number, as instructed — the scheme refuses otherwise-correct rings that start elsewhere). Method: find the four bridgeheads, list triangles of the bridgehead graph, then flesh each out with the edge CH₂'s — that ordering (graph first, atoms second) is what makes the enumeration complete and duplicate-free.

### (c) ¹³C NMR of adamantane
**L1 · Answer** **2 signals** — {1, 3, 5, 10} (the four equivalent bridgehead CH's, T_d-symmetric) and {2, 4, 6, 7, 8, 9} (the six equivalent CH₂'s).
**L2 · Thought** Symmetry-orbit counting (§7.3): the T_d tetrahedron of bridgeheads is the only argument needed — do not count "types of carbon" by inspection.

### (d) Unique six-membered rings of twistane
**L1 · Answer** (in the figure's numbering; the printed example -1-2-3-4-5-6- earns no credit):
**-1-2-3-10-9-6-**; **-1-2-7-8-5-6-**; **-3-4-5-6-9-10-**; **-2-3-4-5-8-7-**.
**L2 · Thought** Enumerate by bridge pairs around the two junction sets: in twistane the original six-ring shares its frame with two 2-atom bridges (7–8 across the top, 9–10 across the bottom), and each pairing of two routes between the same two bridgeheads that totals four internal atoms gives one six-ring — the complete credited set is the four above (the example ring itself earns nothing). Every ring is a twist-boat, as the stem promises — if a "ring" you found were a chair, it is a connectivity error. Note the numbering trap: the bottom bridge runs 3–10–9–6 in the figure (not 3–9–10–6) — read the labels off the drawing rather than assuming consecutive numbers are consecutive atoms.

### (e) ¹³C NMR of twistane
**L1 · Answer** **3 signals** — {2, 3, 5, 6} (the four equivalent bridgehead CH's), {7, 8, 9, 10} (the four equivalent bridge CH₂'s), {1, 4} (the two equivalent CH₂'s of the original boat).
**L2 · Thought** Orbit the atoms under the molecule's three C₂ axes (each swaps bridgeheads onto bridgeheads and bridge atoms onto bridge atoms): the orbits are 4 + 4 + 2, so 3 signals. If you find 2 or 4, an automorphism was missed or over-applied — check one explicit mapping (2 → 5 → 6 → 3 closes the bridgehead orbit) before committing.

### (f) Molecular formula of adamantane and twistane
**L1 · Answer** **C₁₀H₁₆** (DBE = (2 × 10 + 2 − 16)/2 = 3 = three rings, no π bonds ✓).

### (g) The 1962 twistane synthesis: A–H, J⁻, K
**L1 · Answer** (bond framework as pre-drawn in the answer booklet; functional assignments:)
- **A** = **2-(bicyclo[2.2.1]hept-5-en-2-yl)ethan-1-ol** (norbornene with –CH₂CH₂OH at C2; LiAlH₄ reduces the starting methyl ester to the primary alcohol).
- **B** = its **methanesulfonate**, ring–CH₂CH₂–OMs (C₁₀H₁₆O₃S ✓ = A + MsCl − HCl).
- **C** = **3-(bicyclo[2.2.1]hept-5-en-2-yl)propanenitrile**, ring–CH₂CH₂–CN (NaCN, SN2 — this step installs the 10th carbon).
- **D** = **3-(bicyclo[2.2.1]hept-5-en-2-yl)propanoic acid**, ring–CH₂CH₂–COOH (KOH then H⁺/H₂O hydrolyses the nitrile).
- (intermediate cation = the **bridged iodonium** over the norbornene C=C, with the propanoic acid arm intact.)
- **E** = the **iodo-lactone** (C₁₀H₁₃IO₂ = D + I₂ − HI): a δ-lactone fused to the rearranged bicyclic framework (the carboxylate O attacks the iodonium intramolecularly (−H⁺); I remains on the adjacent carbon), accompanied by Wagner–Meerwein rearrangement of the norbornane skeleton toward the twist-boat framework. (Ring size and I position as drawn in the scheme — verify against the original figure.)
- (H₂/Pt then hydrogenolyses the C–I to give the saturated δ-lactone fused to the cyclopentane, C₁₀H₁₆O₂.)
- **F** = the **diol** from LAH opening of that δ-lactone (C₁₀H₁₈O₂ = lactone + 2 H₂): the ring-junction carbon bears the tertiary/secondary –OH and the side arm is –CH₂CH₂CH₂OH.
- **G** = the **mono-mesylate**: the arm's terminal –CH₂OH converted to –CH₂OMs; the ring –OH left free (C₁₁H₂₀O₄S).
- **H** = the **keto-mesylate**: the ring –OH oxidised to C=O (Na₂Cr₂O₇/H₂SO₄), arm –CH₂CH₂CH₂–OMs intact (C₁₁H₁₈O₄S ✓).
- **J⁻** = the **enolate α to that ring ketone** (base removes the α-H, −H⁺).
- **K** = **twistan-3-one (a twistanone, C₁₀H₁₄O)**: the enolate does an intramolecular SN2 on the tether's –CH₂–OMs, closing the third ring of the twistane skeleton and ejecting CH₃SO₃⁻.
- K + H₂N–NH₂/KOH → **twistane** (Wolff–Kishner reduction of the ketone to methylene).
**L2 · Thought** The synthesis is a masterclass in reading role assignments: LAH twice (ester → alcohol; lactone → diol), MsCl twice (alcohol → leaving group, both times for an SN2 — one intermolecular (NaCN) and one intramolecular (the final ring closure)), and the two signature reactions doing the heavy lifting: iodonium formation + intramolecular capture with skeletal rearrangement (which converts the norbornane into the twist-boat framework — the whole point of the route), and Wolff–Kishner to strip the last oxygen. The carbon accounting closes the proof: 7 (norbornane) + 2 (original arm) + 1 (from NaCN) = 10 = C₁₀ ✓ for both K (C₁₀H₁₄O) and twistane (C₁₀H₁₆). "No C–C single bonds are broken" is the licence that lets you trace every carbon from start to finish — use it.

### (h) Symmetry of twistane
**L1 · Answer**
(i) Planes of symmetry: **None**;
(ii) Rotational axes of symmetry: **Two or more** (twistane has three mutually perpendicular C₂ axes);
(iii) Superimposable on its mirror image? **No** — twistane is **chiral** (point group D₂: three proper C₂ axes and *no* improper symmetry element), so it exists as an enantiomeric pair.
**L2 · Thought** The correct improper-symmetry analysis (§5.5): test every candidate mirror plane *bond-by-bond* — any plane through one bridge maps the other bridge's atoms onto non-existent positions (the two bridges are not coplanar in the twisted frame), so no plane survives; likewise no inversion centre and no S_n axis. What survives is D₂'s three *proper* C₂ axes — and proper rotations never make a molecule achiral. The "two or more rotational axes" tick and the "No" tick are then one argument: axes yes, planes no → chiral. Twistane is the textbook D₂-chiral hydrocarbon — asserting planes from the drawing's apparent balance, without the bond-by-bond test, is exactly the failure mode this question is designed to catch.

---

## Q5 — Superbases (12 marks)

### (a) Proton affinity of the methyl anion
**L1 · Answer** Build the cycle H⁺ + CH₃⁻ → CH₄:
PA = IE(H) + D(H–CH₃) − EA(CH₃)
= (2.18 × 10⁻¹⁸ × 6.022 × 10²³/10³) + 439 − 7.52 = 1313 + 439 − 7.52 = **1744 kJ mol⁻¹**
(Thermochemical loop: H⁺ + e⁻ → H· (−IE); CH₃⁻ → CH₃· + e⁻ (+EA); H· + CH₃· → CH₄ (−D); sum reversed for PA.)
**L2 · Thought** Proton affinity is not a bond enthalpy — it is the full ionic cycle: ionisation energy of H, bond enthalpy of H–CH₃, and electron affinity of CH₃·. The lithium monoxide value (1778) exceeds this (1744), which is exactly what "stronger base" means on this scale; DEB²⁻ (1843) tops both. Watch the sign of the electron-affinity term: EA enters *subtracted* (a species that holds its electron weakly is a stronger base).

### (b) The oxalate anion, P and Q
**L1 · Answer** Oxalate C₂O₄²⁻: [⁻OOC–COO]²⁻ (two carboxylate groups joined by a C–C bond).
P = **CO₂** (44); Q = **CO** (28): LiC₂O₄⁻ → LiCO₃⁻ + CO₂ → LiO⁻ + CO (mass audit: 94.96 − 44.01 = 50.95; 50.95 − 28.01 = 22.94 = LiO⁻ ✓).
**L2 · Thought** Neutral-loss bookkeeping in a mass spectrometer: match the masses first (44 → CO₂, 28 → CO), then check the residue closes to the target ion (LiO⁻ = 22.94) — the masses alone determine both molecules; no structural guesswork is needed beyond the oxalate skeleton.

### (c) The functional group in R and its structure
**L1 · Answer** Effervescence with NaHCO₃ → a **carboxylic acid**; R = **–C≡C–COOH** (prop-2-ynoic (propiolic) acid substituent, C₃HO₂): 2 × C₃HO₂ + C₆H₄ = C₁₂H₆O₄ ✓.
**L2 · Thought** Atom audit: C₁₂H₆O₄ − C₆H₄ = C₆H₂O₄ for two identical substituents → C₃HO₂ each; a 3-carbon substituent containing COOH needs one C≡C to satisfy the hydrogen count (DBE: total for A = 10; ring 4 + 2 × (C≡C + C=O) = 10 ✓). The alkyne is not decorative — it is what makes decarboxylation to a gas-phase acetylide possible in (e).

### (d) Disubstituted benzenes C₆H₄R₂ and their ¹³C counts
**L1 · Answer**
- **1,2- (ortho)**: 6 signals (ring: {C1,C2}, {C3,C6}, {C4,C5} = 3; R: 2 C≡C + 1 COOH = 3);
- **1,3- (meta)**: 7 signals (ring: {C1,C3}, {C4,C6}, C2, C5 = 4; R: 3);
- **1,4- (para)**: 5 signals (ring: {C1,C4}, {C2,C3,C5,C6} = 2; R: 3).
**L2 · Thought** Symmetry-orbit counting again (§7.3): draw each isomer's mirror plane(s) and orbit the ring carbons before counting. The ortho pattern (3 ring orbits) is what gives 6 total — and that is the count A is stated to have, so (e) knows it starts from the **ortho** isomer.

### (e) B²⁻, C²⁻, and DEB²⁻
**L1 · Answer** (A = the ortho isomer, 6 signals ✓)
- **B²⁻** = **[1,2-C₆H₄(C≡C–COO⁻)₂]²⁻** (the dipropiolate dianion of A);
- **C²⁻** = **[1,2-C₆H₄(C≡C–COO⁻)(C≡C⁻)]²⁻** (one carboxylate decarboxylated to the acetylide);
- **DEB²⁻** = **[1,2-C₆H₄(C≡C⁻)₂]²⁻** (1,2-diethynylbenzene-1,2-diide — two ortho acetylide anions, the strongest known gas-phase base, PA 1843 kJ mol⁻¹).
**L2 · Thought** The sequence is pure decarboxylation logic: each –C≡C–COO⁻ sheds CO₂ to become –C≡C⁻ (the reverse of (b)'s neutral-loss audit). The extraordinary basicity is localised: two acetylide anions on *adjacent* ring positions — the ortho arrangement is essential (mutual electrostatic + shared-proton stabilisation of the mono-protonated form), which is why the question spent (d) establishing that A is the ortho isomer.

---

*End of Paper 9 (2017). Next: 2016 Round 1.*


---

# Paper 10 — 2016 UKChO Round 1 (48th IChO selection)

**Marks / time:** Q1 12, Q2 23, Q3 31, Q4 21, Q5 13 (total 100; 2 h ⇒ ≈1.2 min per mark).
**Theme map:** Q1 thermochemistry of the sulfur–iodine cycle; Q2 tungsten chemistry + scheelite unit cell; Q3 DBE and ¹³C-NMR structure deduction (C₈H₈ isomers); Q4 synthesis of flibanserin (Addyi); Q5 radiocarbon dating of Richard III.

---

## Question 1 — Energy storage: the sulfur–iodine cycle (12 marks)

### (a) Thermodynamics of reaction (3), 2 HI(g) ⇌ H₂(g) + I₂(g)
**L1 · Answer**
- (i) ΔrH°(298) = [0 + 62.4] − [2 × 26.5] = **+9.4 kJ mol⁻¹**
- (ii) ΔrS°(298) = [131 + 261] − [2 × 207] = **−22.0 J K⁻¹ mol⁻¹**
- (iii) ΔrG°(298) = 9.4 − 298 × (−0.0220) = **+15.96 kJ mol⁻¹**
- (iv) K₂₉₈ = e^(−15956 / (8.314 × 298)) = e^(−6.44) = **1.6 × 10⁻³**
- (v) ΔrG°(723) = 9.4 − 723 × (−0.0220) = +25.31 kJ mol⁻¹; K₇₂₃ = e^(−25306 / (8.314 × 723)) = e^(−4.21) = **1.5 × 10⁻²**
**L2 · Thought** Sign audit before touching the calculator: breaking two H–I bonds with nothing new formed but the weak I–I bond ⇒ small *positive* ΔH; 2 mol gas → 2 mol gas but entropy still *falls* slightly (the heavier, more disordered HI pair gives way to lighter, more ordered H₂ + I₂). Both signs then propagate consistently: raising T makes ΔG *more* positive here (ΔS < 0), so K only creeps up from 1.6 × 10⁻³ to 1.5 × 10⁻² — the HI decomposition is meagre even at 723 K, which is precisely why the cycle needs the other two reactions to pull it along.

### (b) Overall equation
**L1 · Answer** Doubling (1) and (3) so every intermediate cancels — (1) ×2: 2 I₂ + 2 SO₂ + 4 H₂O → 2 H₂SO₄ + 4 HI; (2): 2 H₂SO₄ → 2 SO₂ + 2 H₂O + O₂; (3) ×2: 4 HI → 2 H₂ + 2 I₂ — and summing:
**2 H₂O(g) → 2 H₂(g) + O₂(g)**
**L2 · Thought** Closed-cycle audit (§7.5): every species that is not water, hydrogen or oxygen must appear on both sides of the ledger with equal stoichiometry — I₂, SO₂, H₂SO₄, HI all cancel. If any is left over, the cycle is not closed and the "storage" claim fails.

### (c) ΔrH° for reaction (1)
**L1 · Answer** From reaction (2): ΔfH°(H₂SO₄, g) − ΔfH°(SO₂, g) = ½ × (−439 + 2 × (−242)) → the difference is (−242 − 219.5) = −461.5 kJ mol⁻¹. Then
ΔrH°(1) = [ΔfH(H₂SO₄) + 2 × 26.5] − [62.4 + ΔfH(SO₂) + 2 × (−242)] = −461.5 + 53.0 − 62.4 + 484 = **+13.1 kJ mol⁻¹**
**L2 · Thought** The unknown formation enthalpies of SO₂ and H₂SO₄ never need to be known separately — reaction (2) hands you exactly their *difference*, which is all reaction (1) asks for. Spotting which combination is determined (and which is not) is the whole move.

### (d) Energy stored per mole of sulfur atoms
**L1 · Answer** One revolution stores the enthalpy of 2 H₂O → 2 H₂ + O₂ for every 2 mol of SO₂/S cycled, i.e. per mole of S: H₂O → H₂ + ½ O₂, ΔH = **+242 kJ mol⁻¹ of S**.
**L2 · Thought** The cycle is a water-splitting machine: the only things that cross the boundary are water in and hydrogen/oxygen out, so the stored energy is just −ΔfH(H₂O, g) per mole of water split. The per-mol-of-sulfur framing tests whether you track the stoichiometry (2 H₂O split per 2 S) rather than parroting 484.

---

## Question 2 — The chemistry of tungsten (23 marks)

### (a) The tungstate ion
**L1 · Answer** WO₄²⁻: tetrahedral, **O–W–O = 109.5°**, drawn with two W=O and two W–O⁻ bonds (resonance-delocalised over all four oxygens; formal charge −2 sits on the single-bonded O atoms).
**L2 · Thought** The sulfate analogy is given in the preamble — use it: W(VI) is d⁰, so the ion is a classic AX₄ tetrahedron. Drawing all four bonds as W=O would put formal charge −2 on tungsten; the 2 + 2 pattern keeps formal charges sane (W +2, two O −1 each... minimised as in sulfate).

### (b) Scheelite to tungsten metal
**L1 · Answer**
- (i) **CaWO₄(s) + Na₂CO₃(aq) → Na₂WO₄(aq) + CaCO₃(s)** (the white insoluble salt is CaCO₃ — anion metathesis driven by the least soluble product).
- (ii) **Na₂WO₄ + 2 HCl → H₂WO₄ + 2 NaCl**; tungstic acid = **(HO)₂WO₂** (tetrahedral W with two oxo and two hydroxo ligands).
- (iii) **H₂WO₄ → WO₃ + H₂O** (thermal dehydration).
- (iv) **WO₃ + 3 H₂ → W + 3 H₂O**.
**L2 · Thought** Oxidation-state audit: tungsten stays +6 through (i)–(iii) — these are metathesis/acidification/dehydration steps, no redox — and only drops to 0 in (iv). If you find yourself balancing electrons before (iv), something has gone wrong. The (HO)₂WO₂ structure is read straight off the sulfate analogy (H₂SO₄ = (HO)₂SO₂).

### (c) Oxidation state of W in LiₓWO₃
**L1 · Answer** (i) x = 1: W + 1 − 6 = 0 ⇒ **+5**. (ii) x = 0.3: W + 0.3 − 6 = 0 ⇒ **+5.7** (average; mixed W(V)/W(VI) in the bronze).
**L2 · Thought** Charge-neutrality bookkeeping: x Li⁺ plus W plus 3 × O²⁻ sums to zero. A *fractional* oxidation state is not a single atom's state — it is an average over W(V) and W(VI) sites, which is exactly why the colour appears (intervalence charge transfer) and why the window darkens.

### (d) Densities of SF₆ and WF₆ relative to air
**L1 · Answer** Taking air as N₂ (M = 28.02): SF₆ (M = 146.06): 146.06/28.02 = **5.21**; WF₆ (M = 297.85): 297.85/28.02 = **10.6**.
**L2 · Thought** Same T, p ⇒ equal molar volumes, so the density ratio *is* the molar-mass ratio — no gas-law arithmetic needed. The result dramatises the preamble: WF₆ is over ten times as dense as air, the densest known gas at rtp.

### (e) Actual density of WF₆ at 298 K, 10⁵ Pa
**L1 · Answer** ρ = pM/(RT) = (10⁵ × 297.85 × 10⁻³) / (8.314 × 298) = 12.0 kg m⁻³ = **1.20 × 10⁻² g cm⁻³**.
**L2 · Thought** Unit discipline: convert M to kg mol⁻¹ *before* multiplying by p in Pa, so the answer lands in kg m⁻³; the g cm⁻³ conversion (÷1000) is the last step, not the first. A quick sanity anchor: air ≈ 1.2 × 10⁻³ g cm⁻³, and 10.6 × that ≈ 1.2 × 10⁻² ✓ — the two parts must agree, and they do.

### (f) WF₆ + water
**L1 · Answer** **WF₆ + 4 H₂O → H₂WO₄ + 6 HF** (two products, as stated; writing WO₃ + 6 HF + H₂O is the dehydrated equivalent).
**L2 · Thought** Complete hydrolysis of a halide to the (hydr)oxide + hydrogen halide — the same pattern as SiCl₄ or PCl₅. The toxicity story is HF; the driving force is the enormous O–H/F–H and W–O bond strengths versus W–F in water.

### (g) SF₆ + 4 H₂O(g) ⇌ H₂SO₄(g) + 6 HF(g)
**L1 · Answer**
- (i) **Positive** ΔrS° (5 mol gas → 7 mol gas).
- (ii) ΔrH° = [−735 + 6 × (−273)] − [−1210 + 4 × (−242)] = −2373 − (−2178) = **−195 kJ mol⁻¹**.
- (iii) **B — kinetically stable but thermodynamically unstable.**
**L2 · Thought** With ΔH < 0 and ΔS > 0, ΔG is negative at *all* temperatures: SF₆'s hydrolysis is emphatically downhill, so its inertness can only be kinetic — six fluorines sterically shield the small sulfur and there is no low-energy pathway for water to attack. This is the textbook separation of "stable" into two independent axes; option B is the only self-consistent reading of the facts (inert in water, yet ΔG < 0).

### (h) Counting atoms in the scheelite unit cell
**L1 · Answer** **W = 4, Ca = 4, O = 16** per unit cell (i.e. 4 × CaWO₄, Z = 4).
**L2 · Thought** Share counting (§7.4): corners × ⅛, edges × ¼, faces × ½, internal × 1 — applied to each species separately from the two views. The count must come out in the ratio 1 : 1 : 4 (Ca : W : O); if it does not, the mis-shared atom is almost always a face or edge atom double-counted as internal. Reconciling to the known formula is the built-in self-check.

### (i) Density of scheelite
**L1 · Answer** V = (0.524 × 10⁻⁷)² × (1.137 × 10⁻⁷) = 3.12 × 10⁻²² cm³; m = 4 × 287.93 / 6.022 × 10²³ = 1.91 × 10⁻²¹ g; ρ = m/V = **6.13 g cm⁻³**.
**L2 · Thought** Two conversion traps, both defused by writing units at each step: nm → cm (×10⁻⁷, and remember to cube the whole product, not each factor) and "per cell" → "per mole" via Nₐ. The answer must exceed ~3 g cm⁻³ (typical silicate gangue) — "heavy stone" is the qualitative claim, and 6.1 g cm⁻³ is its quantitative receipt.

---

## Question 3 — Double Bond Equivalents, DBE (31 marks)

### (a) General formulae
**L1 · Answer** (i) alkene/cycloalkane: **CₙH₂ₙ**; (ii) alkyne: **CₙH₂ₙ₋₂**; (iii) cycloalkene: **CₙH₂ₙ₋₂**; (iv) di-alkyne: **CₙH₂ₙ₋₆**.
**L2 · Thought** Each ring or π-bond costs 2 H from CₙH₂ₙ₊₂: (iii) has one ring *and* one double bond (−4), (iv) has two triple bonds (2 × −4 = −8 ⇒ H = 2n − 6). These four lines are the entire theory the rest of the question operationalises.

### (b) Extending the DBE table
**L1 · Answer** (r = rings, d = double bonds, t = triple bonds, with r + d + 2t = DBE)
- **DBE = 3:** (3,0,0), (2,1,0), (1,2,0), (0,3,0), (1,0,1), (0,1,1)
- **DBE = 4:** (4,0,0), (3,1,0), (2,2,0), (1,3,0), (0,4,0), (2,0,1), (1,1,1), (0,2,1), (0,0,2)
**L2 · Thought** Systematic enumeration by t = 0, 1, 2 … then r descending — this ordering is what guarantees no combination is missed or duplicated. The count grows fast (6 then 9), which is exactly why spectroscopy (part d) is needed to prune the list.

### (c) DBE of specific hydrocarbons
**L1 · Answer** (i) C₅H₄: ½(12 − 4) = **4**; (ii) C₁₈H₂₀: ½(38 − 20) = **9**; (iii) C₆₀: ½(122 − 0) = **61**; (iv) benzene: **4** (1 ring + 3 π); (v) ethynylcyclopentene: **4** (1 ring + 1 π + 2 π); (vi) adamantane: **3** (three rings — the minimum-cut count: three independent cuts to open the cage).
**L2 · Thought** Two routes and they must agree: formula arithmetic (i–iii) versus structural counting (iv–vi). C₆₀ is the cautionary one — 61 DBE from the formula, yet a ball with 12 five-membered and 20 six-membered rings: the number alone tells you nothing about shape. For the cage in (vi), count cuts, not faces: adamantane's four visible cyclohexane chairs share bonds, and the independent-ring number is 3 (E − V + 1 = 13 − 10 + 1).

### (d) The C₈H₈ isomers from ¹³C NMR (all C₈H₈, DBE = 5)
**L1 · Answer** (structures verified by machine formula check, all C₈H₈)
| Spectrum | Signals | π-bond audit | Structure |
|---|---|---|---|
| **A** | 8 × 132 (CH) | 4 C=C + 1 ring | **cyclooctatetraene** — `C1=CC=CC=CC=C1` |
| **B** | 8 × 47 (CH) | 0 π + 5 rings | **cubane** — `C12C3C4C1C5C4C3C25` |
| **C** | 4 × 96 (C), 4 × 20 (CH₂) | 2 C≡C + 1 ring | **cycloocta-1,5-diyne** — `C1#CCCC#CCC1` |
| **D** | 2 × 210 (C), 134 (C), 113 (CH₂), 2 × 93 (CH), 2 × 79 (CH₂) | 2 allenes + 1 C=C, 0 rings | **4-methylidenehepta-1,2,5,6-tetraene** — `C=C=CC(=C)C=C=C` (each "2 ×" is one signal from a *pair* of equivalent carbons: the molecule's mirror swaps the two allene arms, so 8 carbons give exactly 5 environments ✓) |
| **E** | 147 (C), 2 × 138 (CH), 2 × 131 (CH), 2 × 127 (CH), 112 (CH₂) | 4 C=C + 1 ring | **styrene (phenylethene)** — `C=Cc1ccccc1` |
| **F** | 142, 136, 117, 112 (CH); 127, 120 (CH₂); 91, 89 (C) | 3 C=C + 1 C≡C, 0 rings | **octa-1,5,7-trien-3-yne** — `C=CC#CC=CC=C` |
| **G** | 2 × 146 (C), 2 × 127 (CH), 2 × 122 (CH), 2 × 30 (CH₂) | 3 C=C + 2 rings | **bicyclo[4.2.0]octa-1(6),2,4-triene** — `C12C=CC=CC=2CC1` |
| **H** | 154 (C), 151 (C), 2 × 136 (CH), 2 × 128 (CH), 2 × 37 (CH₂) | 3 C=C + 2 rings | **bicyclo[3.3.0]octa-1(5),2,7-triene** — `C12C=CCC=2CC=C1` |
| **I** | 157 (C), 101 (CH₂), 2 × 26 (CH), 4 × 19 (CH) | 1 C=C + 4 rings | **7-methylidenequadricyclane** — `C13C2C4C(C3=C)C4C12` |

**L2 · Thought** The working order that never backfires: (1) tally hydrogen types from the (CH)/(CH₂)/(C) labels — they must sum to H₈; (2) bin the shifts by region (sp³ 0–50, alkyne/allene-flank 70–100, alkene 100–160, allene-central >200) to fix the π-bond inventory; (3) rings = 5 − (π count); (4) only then sketch a skeleton whose *symmetry orbits* reproduce the multiplicities. The multiplicities are symmetry fingerprints: A and B both have one orbit (8 × CH) but the shift region separates a flat alkene ring from an sp³ cage; G versus H differ only in whether the two quaternary sp² carbons are equivalent (G has a mirror swapping them — the fusion C=C is flanked by CH₂ on both sides; in H one fusion carbon touches two vinyl CH, the other two CH₂, so they split into 154/151 while a mirror through the fusion bond still pairs the CH and CH₂ signals). Spectrum D is the trap the preamble set up on purpose: >200 ppm can *only* be allene central carbons, and two of them plus the 70–100 flanks dictate two allene units before any structure is drawn.

---

## Question 4 — The synthesis of Addyi (flibanserin) (21 marks)

### (a) Empirical formula of A
**L1 · Answer** O% = 100 − 45.70 − 10.55 − 13.32 = 30.43. Mole ratios: C 45.70/12.01 = 3.805, H 10.55/1.008 = 10.47, N 13.32/14.01 = 0.951, O 30.43/16.00 = 1.902 → ÷0.951: C 4.00 : H 11.0 : N 1 : O 2 → **C₄H₁₁NO₂**.
**L2 · Thought** The missing-element audit comes first: nitrogen and carbon are named, but oxygen is not — the 30.43% remainder must be assigned (nothing else is plausible from ethylene oxide + NH₃). Dividing through by the smallest ratio and seeing clean integers is the confirmation, not a coincidence.

### (b) Structures of A, B and C
**L1 · Answer**
- **A = diethanolamine**, HN(CH₂CH₂OH)₂ — `OCCNCCO` (C₄H₁₁NO₂ ✓): ethylene oxide + NH₃ ring-opens twice; the C₄ formula with two oxygens and one nitrogen fixes the di-adduct over mono- or tri-ethanolamine.
- **B = 3-nitrobenzotrifluoride** — `O=[N+]([O-])c1cccc(c1)C(F)(F)F`: CF₃ is strongly meta-directing, and the flibanserin target needs the future piperazine-nitrogen attachment *meta* to CF₃.
- **C = 3-aminobenzotrifluoride** — `Nc1cccc(c1)C(F)(F)F`: Pd/H₂ reduces NO₂ → NH₂.
**L2 · Thought** Two independent anchors per structure: A's formula comes from the analysis, its connectivity from the epoxide + ammonia logic (each N–H adds one oxirane across its C–O bond; two N–H on NH₃ after the first addition ⇒ di-adduct). For B, the substitution pattern is not free choice — read it off the target: flibanserin's aryl ring carries CF₃ and the piperazine N in a 1,3-relationship, and CF₃'s meta direction happily delivers exactly that.

### (c) D, E, F, G and by-product H
**L1 · Answer** (all machine-validated)
- **D** = 1-isopropenyl-3-(2-bromoethyl)benzimidazol-2-one — `C=C(C)n1c(=O)n(CCBr)c2ccccc12` (C₁₂H₁₃BrN₂O): BrCH₂CH₂Br alkylates the benzimidazolone N–H, one HBr lost; the second bromine survives for the next alkylation.
- **E** = D with Br displaced by A's nitrogen: Ar–N–CH₂CH₂–N(CH₂CH₂OH)₂ arm — `C=C(C)n1c(=O)n(CCN(CCO)CCO)c2ccccc12` (C₁₆H₂₃N₃O₃).
- **F** = the **bis-benzenesulfonate**, n = 2 — `C=C(C)n1c(=O)n(CCN(CCOS(=O)(=O)c2ccccc2)CCOS(=O)(=O)c2ccccc2)c2ccccc12` (C₂₈H₃₁N₃O₇S₂). **18 ¹³C signals ✓**: benzimidazolone 7 + isopropenyl 3 + ethylene linker 2 + N(CH₂CH₂O)₂ 2 + two equivalent PhSO₂ rings 4 = 18.
- **G** = piperazine ring closed with C: — `C=C(C)n1c(=O)n(CCN2CCN(c3cccc(C(F)(F)F)c3)CC2)c2ccccc12` (C₂₃H₂₅F₃N₄O): the aniline NH₂ of C alkylates both sulfonate arms (− 2 PhSO₃H), closing the six-membered ring with N–Ar(CF₃) on one side and N–CH₂CH₂–benzimidazolone on the other.
- **H = propanone (acetone)** — `CC(C)=O`: H₃O⁺ hydrolyses the N-isopropenyl enamine (N–C(CH₃)=CH₂ + H₂O → N–H + CH₃COCH₃), unveiling flibanserin's N–H.
**L2 · Thought** Balanced-scheme bookkeeping does the heavy lifting: "−HBr" twice tells you two SN₂ alkylations; "−n HCl with n PhSO₂Cl" asks only for n, and the 18-signal datum answers it (n = 1 gives 16 signals, n = 2 gives 18 with the two phenyl rings symmetry-equivalent — count it both ways and only n = 2 works). The piperazine ring cannot be drawn from memory of the drug alone: it assembles when C's NH₂ consumes *both* sulfonate esters in F, which is why F had to carry two leaving groups. The isopropenyl group is a masked N–H — spotting that its hydrolysis gives the smallest possible ketone (C₃H₆O = acetone) closes the mass balance and confirms the protecting-group logic.

### (d) Site of protonation in flibanserin
**L1 · Answer** Protonation on the **piperazine nitrogen bonded to the CH₂CH₂ linker** (the dialkylamino N), *not* the N bonded to the CF₃-phenyl ring.
**L2 · Thought** Rank the lone pairs by availability: the N–aryl piperazine nitrogen's lone pair is delocalised into the aniline π-system (and further deactivated by the meta-CF₃), the benzimidazolone nitrogens are amide-like, leaving the trialkylamine-like N as the only genuinely basic site — exactly the amine a medicinal chemist would salt for formulation.

### (e) Intermediate X and compound Y
**L1 · Answer**
- **X = ethyl 3-[(2-aminophenyl)amino]but-2-enoate** — `CCOC(=O)C=C(C)Nc1ccccc1N` (C₁₂H₁₆N₂O₂): one NH₂ of the diamine condenses with the *ketone* carbonyl of ethyl acetoacetate (−H₂O); drawn as the stabilised enamine tautomer (N–H conjugated with the ester).
- **Y = 4-methyl-1,5-dihydro-1,5-benzodiazepin-2-one** — `CC1=CC(=O)Nc2ccccc2N1` (C₁₀H₁₀N₂O, seven-membered ring ✓): the free ortho-NH₂ attacks the ester carbonyl, −EtOH closes the 7-ring: N–C(CH₃)=CH–C(=O)–NH spanning the two aryl positions.
- Isomerisation: Y (C₁₀H₁₀N₂O) → Z (same formula ✓), ring contraction 7 → 5: the enamine carbon attacks the amide carbonyl and C–C cleavage/rearrangement ejects the ring carbon as the N-isopropenyl substituent of the benzimidazol-2-one.
**L2 · Thought** The chain of custody is pure atom accounting: C₆H₈N₂ + C₆H₁₀O₃ − H₂O = C₁₂H₁₆N₂O₂ (X) ✓; −C₂H₆O (EtOH) = C₁₀H₁₀N₂O (Y) ✓; and since Y → Z is stated to be an *isomerisation*, Z must share that formula — a constraint that rules out every benzimidazolone except the isopropenyl one. Which carbonyl is attacked first is decided by chemoselectivity (ketone > ester towards amines) and by the product audit: ester-first condensation could never place a seven-membered ring with the right atoms.

---

## Question 5 — Dating King Richard III (13 marks)

### (a) Removing the inorganic content — circle one
**L1 · Answer** **C — wash repeatedly with dilute HCl then dilute NaOH.**
**L2 · Thought** The target to remove is hydroxyapatite, Ca₅(PO₄)₃(OH): dilute acid dissolves it (acid-soluble calcium phosphate), and dilute alkali then strips humic-acid contaminants without destroying collagen. A (water/propanone) barely touches the mineral; B (400 °C) combusts the very collagen you need to keep — the selection is about *selective* chemistry, not brute force.

### (b) Polyglycine to graphite
**L1 · Answer**
- (i) Repeat unit: **–NH–CH₂–C(=O)–** (C₂H₃NO, M = 57.05).
- (ii) Combustion (per repeat, ×4 to clear fractions): **4 (C₂H₃NO)ₙ + 9n O₂ → 8n CO₂ + 6n H₂O + 2n N₂** (atom audit: C 8n, H 12n, N 4n, O 22n both sides ✓).
- (iii) **CO₂ + 2 H₂ → C + 2 H₂O**.
- (iv) Collagen in 1.0 g bone = 0.40 g; carbon fraction in the repeat unit = 24.02/57.05 = 0.421; graphite mass = 0.40 × 0.421 = **0.168 g ≈ 0.17 g**.
**L2 · Thought** The chain is yield-last (§7.5): composition of bone → mass of protein → carbon fraction of the repeat unit → mass of graphite, with every intermediate (CO₂, H₂-reduction) assumed quantitative as stated. Note the repeat unit, not free glycine, sets the carbon fraction — polymerisation water is gone before the sample is weighed (using glycine's 24.02/75.07 would have cost the mark).

### (c) ¹⁴C decays per day at time of death
**L1 · Answer** C atoms in 2.0 mg = (2.0 × 10⁻³ / 12.01) × 6.022 × 10²³ = 1.00 × 10²⁰; ¹⁴C atoms = 1.00 × 10²⁰ × 1.215 × 10⁻¹² = 1.22 × 10⁸; λ = ln2 / 5568 y = 3.41 × 10⁻⁷ day⁻¹; decays per day = λN = 3.41 × 10⁻⁷ × 1.22 × 10⁸ = **≈ 42 day⁻¹** (mark scheme: 41.6 ≈ 42).
**L2 · Thought** Two conversions, each a classic slip point: the abundance is quoted in *percent* (1.215 × 10⁻¹⁰ % = 1.215 × 10⁻¹² as a fraction), and λ must land in day⁻¹ (divide by 365.25, not 365, if you are matching the data's precision). The point of the number is rhetorical: ~42 counts per day per 2 mg is a miserable rate — that is why part (d) switches to atom counting by mass spectrometry.

### (d) Age of the bones and date of death
**L1 · Answer** At death: ¹⁴C/¹²C = 1.215 × 10⁻¹⁰ / 98.93 = 1.228 × 10⁻¹². Now: 1.154 × 10⁻¹².
t = (t½ / ln2) × ln(N₀/N) = (5568 / 0.6931) × ln(1.228 / 1.154) = 8033 × 0.0621 = **≈ 500 years** ⇒ death ≈ 2012 − 500 = **1512** (any year 2012–2016 is acceptable as the dating-experiment baseline).
**L2 · Thought** Ratios of ¹⁴C to ¹²C decay exactly as ¹⁴C itself (¹²C is stable), so the clock needs no absolute abundances — only the fraction of ¹⁴C remaining (0.940). The 500-year answer with the given rounded data lands near 1510 rather than the true 1485; that residual gap is data rounding, not method failure — the dating is comfortably consistent with "the man killed at Bosworth, 1485" and rules out a modern burial, which is all the question asks you to conclude.

---

*End of Paper 10 (2016). Next: 2015 Round 1.*


---

# Paper 11 — 2015 UKChO Round 1 (47th IChO selection)

**Marks / time:** Q1 9, Q2 17, Q3 20, Q4 14, Q5 15 (total 75; 2 h ⇒ ≈1.6 min per mark).
**Theme map:** Q1 indium/ITO touchscreens; Q2 rotational spectroscopy of interstellar molecules; Q3 Ritalin synthesis + stereoisomers; Q4 enzyme kinetics of ethanol metabolism; Q5 solar-jet fuel from CO₂ and water (ceria cycle).

---

## Question 1 — The chemistry of touchscreens (9 marks)

### (a) Indium(III) oxide from the hydroxide
**L1 · Answer** **2 In(OH)₃ → In₂O₃ + 3 H₂O** (atom audit: In 2, O 6, H 6 both sides ✓).
**L2 · Thought** Thermal dehydration of a metal hydroxide to the oxide — no redox (In stays +3). Balance the metal first, then waters follow automatically.

### (b) Indium in the iPad screen
**L1 · Answer**
- (i) ITO is 90% In₂O₃: 27 × 0.90 = 24.3 mg; In fraction of In₂O₃ = 229.64/277.64 = 0.827; **mass of In = 24.3 × 0.827 = 20.1 mg**.
- (ii) Direct chain (recommended): ITO areal density = 700 mg In m⁻² / (0.90 × 0.827 g In per g ITO) = 0.940 g ITO m⁻²; t = areal density/ρ = 0.940 g m⁻² / 7.15 × 10⁶ g m⁻³ = **1.31 × 10⁻⁷ m (0.131 μm ≈ 131 nm)**. (Cross-check by volume ÷ area: V(screen) = 0.027 g / 7.15 g cm⁻³ = 3.78 × 10⁻³ cm³; A = 20.1 mg In / 700 mg In m⁻² = 0.0287 m² = 287 cm² — note 20.1 mg is the *indium* mass and 20.1/700 gives the screen's *area*, not an ITO mass; t = V/A = 1.32 × 10⁻⁵ cm = 1.32 × 10⁻⁷ m ✓ same.)
**L2 · Thought** The 700 mg m⁻² in the stem is the areal density of **indium**, not of ITO — and the layer is only 90 % In₂O₃. Dividing it straight by the ITO density (≈ 98 nm) is the designed unit-subject error. The clean fix is the volume ÷ area route above (everything from the screen's own totals); equivalently, convert to the ITO areal density first: 0.700 g In m⁻² / (0.90 × 0.8271 g In per g ITO) = 0.940 g ITO m⁻², then t = 0.940/7.15 × 10⁶ = 1.32 × 10⁻⁷ m ✓ — both routes agree once the *subject* of each number is respected (a §7.5 wording audit: areal density of *what*?).

### (c) Indium ions in the FCC cell
**L1 · Answer** 8 corners × ⅛ + 6 face-centres × ½ = 1 + 3 = **4 In ions**.
**L2 · Thought** Share counting (§7.4): only the corner (⅛) and face (½) fractions survive; "approximates to FCC" tells you which positions to count.

### (d) Oxide ions in the cell
**L1 · Answer** **6 O²⁻** (wholly inside the cube).
**L2 · Thought** This is pure stoichiometric closure: 4 In³⁺ per cell with the In₂O₃ formula forces 4 × 3/2 = 6 oxides. Charge audit agrees: 4 × (+3) + 6 × (−2) = 0 ✓.

### (e) Product of heating In₂O₃ in air
**L1 · Answer** 11.5% mass loss: try loss of O₂: In₂O₃ → In₂O + O₂; predicted loss = 32.00/277.64 = **11.5% ✓** ⇒ product = **In₂O** (indium(I) oxide).
**L2 · Thought** Regime analysis: "in air" and mass *loss* point to oxygen evolution, not further oxidation. Test the simplest hypothesis (one O₂ per formula unit) against the percentage before inventing exotic mixed oxides — it fits to three significant figures.

### (f) Product with ammonia at 630 °C
**L1 · Answer** **InN** (indium nitride): In₂O₃ + 2 NH₃ → 2 InN + 3 H₂O.
**L2 · Thought** "Products are water and a semiconductor" + ammonia as the only reagent ⇒ the nitrogen must end up in the solid: a nitride. InN is indeed the well-known III–V semiconductor; the equation balances only with In in the +3 state throughout (another metathesis, not redox).

---

## Question 2 — Detecting molecules in space (17 marks)

### (a) The branched nitrile and an isomer
**L1 · Answer** (i) **2-methylpropanenitrile**: (CH₃)₂CH–C≡N — `CC(C)C#N`. (ii) **butanenitrile** (the straight-chain isomer): CH₃CH₂CH₂C≡N — `CCCC#N`.
**L2 · Thought** The nitrile carbon counts in the parent chain: "propanenitrile" = NC–C–C skeleton with the methyl branch on C2. Formula audit for both: C₄H₇N ✓ — isomers must share it.

### (b) All nitriles C₅H₉N
**L1 · Answer** Four (R–C≡N with R = C₄H₉):
**pentanenitrile** `CCCCC#N`; **2-methylbutanenitrile** `CCC(C)C#N`; **3-methylbutanenitrile** `CC(C)CC#N`; **2,2-dimethylpropanenitrile** `CC(C)(C)C#N` (all machine-checked C₅H₉N ✓).
**L2 · Thought** Exhaustive enumeration by butyl-group isomerism (n, sec, iso, tert — 4 carbon skeletons); the C≡N carbon is fixed at the terminus because nitrile carbon has only one C–C bond. DBE check: C₅H₉N has DBE = ½(12 + 1 − 9) = 2 = the triple bond ✓, so no rings or C=C can appear.

### (c) Linear HC₁₁N
**L1 · Answer** **H–C≡C–C≡C–C≡C–C≡C–C≡C–C≡N** (a cyanopolyyne: five C≡C units terminated by a nitrile).
**L2 · Thought** Linear + only one H + one N ⇒ alternating-triple-bond chain; cumulated double bonds would kink and alter the hydrogen count. Count carbons in the drawing before moving on (11 ✓) — miscounting the repeat units is the only way to lose this mark.

### (d) Rotational constant of HC₁₁N
**L1 · Answer** Transition J → J−1: ΔE = hB[J(J+1) − (J−1)J] = 2hBJ ⇒ f = 2BJ.
- (i) B = 13186.853 / (2 × 39) = **169.06 MHz**.
- (ii) f(38→37) = 2 × 169.06 × 38 = **12848.7 MHz**.
**L2 · Thought** Simplify the bracket symbolically first (J(J+1) − (J−1)J = 2J) — this is where arithmetic errors breed if you substitute early. Note the transition frequency is proportional to the *upper* J, so adjacent lines are evenly spaced by 2B: (ii) must equal 13186.853 × 38/39, a 2.6% downshift, which 12848.7 satisfies.

### (e) Mass of one atom
**L1 · Answer** ¹²C: 12.00 × 10⁻³ / 6.022 × 10²³ = **1.993 × 10⁻²⁶ kg**; ¹⁶O: **2.657 × 10⁻²⁶ kg**.
**L2 · Thought** kg not g: convert the molar mass to kg mol⁻¹ first, then divide by Nₐ — the two-step order is what keeps the powers of ten honest.

### (f) Reduced mass of ¹²C¹⁶O
**L1 · Answer** μ = (12.00 × 16.00)/(12.00 + 16.00) = 6.857 g mol⁻¹ ⇒ **1.139 × 10⁻²⁶ kg** per molecule.
**L2 · Thought** The reduced mass is the harmonic-mean-like combination that is *dominated by the lighter partner* (6.86 < 12) — if your answer lands above 12 g mol⁻¹, the formula was applied upside down.

### (g) Bond length and transition assignment of CO
**L1 · Answer**
- (i) J = 1 → 0: f = 2B ⇒ B = 5.7636 × 10¹⁰ Hz. r = √[h/(8π²μB)] = √[6.626 × 10⁻³⁴ / (8π² × 1.139 × 10⁻²⁶ × 5.7636 × 10¹⁰)] = **1.13 × 10⁻¹⁰ m (113 pm)**.
- (ii) J = f/2B = 806651.719/115271.204 = 6.998 ≈ 7 ⇒ **J = 7 → 6 transition**.
**L2 · Thought** Unit audit in (i): B must be in *Hz* (not MHz) to sit inside the SI formula with h and μ in kg. The result is its own check: 113 pm is a textbook triple-bond length. For (ii), the ratio comes out within 0.03% of an integer — treat near-integer quotients as assignments, and state the selection rule (ΔJ = ±1) that licenses the rounding.

---

## Question 3 — Ritalin® (20 marks)

### (a) Compound A
**L1 · Answer** **Phenylacetonitrile**, PhCH₂C≡N — `N#CCc1ccccc1` (C₈H₇N ✓; IR 2260 cm⁻¹ = C≡N).
**L2 · Thought** SN₂ of CN⁻ on benzyl chloride; the cyanide attacks through carbon (nitrile, not isonitrile) as the IR stretch and all downstream chemistry confirm.

### (b) Anion B⁻
**L1 · Answer** **[Ph–CH⁻–C≡N ↔ Ph–CH=C=N⁻]**: the carbanion α to the nitrile (charge delocalised onto N).
**L2 · Thought** The α-CH₂ of a nitrile is acidic (conjugate base stabilised by the C≡N π-system); deprotonation here, not on the ring, is what makes the next C–C bond.

### (c) Compounds C, D, E, F
**L1 · Answer** (all machine-validated)
- **C** = **2-(pyridin-2-yl)-2-phenylacetonitrile** — `N#CC(c1ccccc1)c1ccccn1` (C₁₃H₁₀N₂; IR 2260 ✓): B⁻ displaces chloride from 2-chloropyridine (SNAr, activated by the ring N).
- **D** = **2-(pyridin-2-yl)-2-phenylacetamide** — `NC(=O)C(c1ccccc1)c1ccccn1` (**C₁₃H₁₂N₂O ✓ matches the given formula**): partial hydrolysis C≡N → CONH₂ (IR 1655 amide C=O; 3180/3390 the two N–H stretches of a primary amide).
- **E** = **2-(pyridin-2-yl)-2-phenylacetic acid** — `O=C(O)C(c1ccccc1)c1ccccn1`: full hydrolysis of the amide (1715 acid C=O; 3000 very broad acid O–H).
- **F** = **alkyl 2-(pyridin-2-yl)-2-phenylacetate** — e.g. `COC(=O)C(c1ccccc1)c1ccccn1` for R = Me: Fischer esterification (1740 ester C=O). H₂/metal then reduces the pyridine ring to piperidine → Ritalin.
**L2 · Thought** The given molecular formula C₁₃H₁₂N₂O is the arbitration point for D: C + H₂O = C₁₃H₁₂N₂O exactly — one water added across the triple bond gives the *amide*, not the acid (which would need +2 H₂O − nothing). The IR pair at 3180/3390 (two sharp N–H bands ⇒ NH₂, not NH) independently locks the primary amide. The final H₂ step reduces the *pyridine* (the only easily hydrogenated π-system present) — that is where the piperidine of Ritalin comes from.

### (d) Protonated atom in the hydrochloride
**L1 · Answer** The **piperidine nitrogen**.
**L2 · Thought** The only basic lone pair in the molecule: the ester carbonyl oxygen and the amide-like systems are far less basic; an alkyl 2° amine (piperidine N–H) protonates first — the same reasoning as flibanserin (2016 Q4(d)).

### (e) Molar mass of Ritalin and the group R
**L1 · Answer**
- (i) salt = base + HCl: M(Ritalin) = 36.46 × 8.647 / (10.00 − 8.647) = **233 g mol⁻¹** (working: 8.647 mg base corresponds to 1.353 mg HCl; scale: M = 8.647 × 36.46/1.353).
- (ii) The framework piperidin-2-yl–CH(Ph)–C(=O)O– accounts for C₁₃H₁₇NO₂ (219.3) ⇒ R = 233 − 219 ≈ 14–15 ⇒ **R = CH₃ (methyl)**; Ritalin = C₁₄H₁₉NO₂ (M = 233.3 ✓) = methyl phenidate.
**L2 · Thought** The mass-balance rearrangement M_base = M_HCl × m_base/(m_salt − m_base) is the only algebra needed — derive it from m_salt/m_base = (M + 36.46)/M rather than memorising it. Then R is found by subtraction against a structural fragment count; a hydrocarbon group of mass ~15 can only be methyl.

### (f) IR assignments
**L1 · Answer**
- (i) **1655 cm⁻¹**: amide C=O stretch (D, –CONH₂; arrow on C=O);
- (ii) **1715 cm⁻¹**: carboxylic acid C=O (E);
- (iii) **1740 cm⁻¹**: ester C=O (F);
- (iv) **2260 cm⁻¹**: C≡N stretch (A and C);
- (v) **3000 cm⁻¹ very broad**: O–H of the H-bonded carboxylic acid (E);
- (vi) **3180 & 3390 cm⁻¹ sharp**: asymmetric + symmetric N–H stretches of the primary amide NH₂ (D).
**L2 · Thought** Carbonyl frequency tracks the substituent's electron demand: amide (lowest, resonance-donated) < acid < ester? No — acid 1715 < ester 1740 here: the discriminating features are the companions, not the numbers: the acid owns the very broad 3000 O–H, the amide owns the sharp NH₂ doublet. Assign by *pattern of bands per compound*, not by memorised wavenumber tables alone.

### (g) Enantiomer pairs among 1–4
**L1 · Answer** Reading the two stereocentres (ring C2 bond; Ph-bearing α-C): 1 = (out, out), 2 = (back, out), 3 = (out, back), 4 = (back, back). Enantiomer pairs (both centres inverted): **1 ↔ 4** and **2 ↔ 3** — all four boxes are part of an enantiomeric pair.
**L2 · Thought** With two stereocentres, "enantiomer" means *both* inverted; one-centre flips give diastereomers. Map each drawing to a (+/−, +/−) signature first, then pair them mechanically — this avoids the classic error of calling 1 and 2 enantiomers.

### (h) Anion G⁻
**L1 · Answer** The **ester enolate**: (piperidin-2-yl)(phenyl)C=C(O⁻)OR, i.e. deprotonation at the α-carbon between phenyl and the ester carbonyl (charge resonance-stabilised onto the ester oxygen).
**L2 · Thought** ⁻OR is not strong enough to touch anything else: the α-C–H is the only appreciably acidic site (pKa ~25 vs amine N–H ~35). Deprotonation *destroys the α-stereocentre* — that is the entire stereochemical point.

### (i) Isomers interconvertible via G⁻
**L1 · Answer** Pairs differing only at the α-centre: **1 ⇌ 3** and **2 ⇌ 4** (tick 1, 2, 3, 4 as members of these pairs).
**L2 · Thought** The enolate is planar at the α-carbon, so reprotonation scrambles *that centre only*; the ring C2 configuration is untouched. Hence interconversion connects exactly the pairs that share the ring-centre configuration — diastereomers, not enantiomers, which is why this trick upgrades the "wrong" diastereomer into the active one.

---

## Question 4 — Hangovers (14 marks)

### (a) What happens to NAD⁺ — circle one
**L1 · Answer** **It is reduced** (NAD⁺ → NADH; ethanol is oxidised to ethanal).
**L2 · Thought** Oxidation of the substrate must be matched by reduction of the cofactor — redox bookkeeping (ethanol → aldehyde is a 2-electron oxidation, NAD⁺ accepts H⁻ equivalent).

### (b) Drink-drive limit in mol dm⁻³
**L1 · Answer** 80 mg/100 ml = 800 mg dm⁻³; 0.800/46.07 = **0.0174 mol dm⁻³**.
**L2 · Thought** Two conversions (mg → g, 100 ml → dm³) done as one line; keep 3 sf because the limit is quoted to two but the next parts compare with K_M = 1.00 × 10⁻³.

### (c) Limiting forms of the rate law
**L1 · Answer** (i) [EtOH] ≫ K_M: **rate = k_cat[AD]** (zero order in ethanol). (ii) [EtOH] ≪ K_M: **rate = (k_cat[AD]/K_M)[EtOH]** (first order in ethanol).
**L2 · Thought** Regime analysis on the denominator: drop the smaller term in each limit. These two limits are the entire content of Michaelis–Menten kinetics; (d) and (g) are both read off them.

### (d) Order at or above the drink-drive limit
**L1 · Answer** **Zero order** (17.4 × 10⁻³ ≫ 1.00 × 10⁻³ mol dm⁻³, so case (c)(i) applies).
**L2 · Thought** Compare the two concentrations numerically and *state* the comparison — the approximation must be seen to be justified, not asserted.

### (e) Rate of loss while sobering up
**L1 · Answer** The graph is linear over most of the range (zero order) — read the slope from the constant-gradient region (first ~18 h):
- (i) **≈ 17.0 (mg/100 ml) h⁻¹** (mark scheme accepts 15.5–18.5);
- (ii) = 170 mg dm⁻³ h⁻¹ = 0.170/46.07 = 3.69 × 10⁻³ mol dm⁻³ h⁻¹ = **1.03 × 10⁻⁶ mol dm⁻³ s⁻¹**.
**L2 · Thought** A straight line *is* the experimental signature of zero-order kinetics — the graph and part (d) corroborate each other. Unit ladder for (ii): mg/100 ml → g dm⁻³ → mol dm⁻³ → per second (÷3600), one conversion per step. The scheme's tolerance band absorbs graph-reading spread; everything downstream is ECF-protected (×6.04 × 10⁻⁸ per (i) unit).

### (f) Alcohol dehydrogenase concentration
**L1 · Answer** Zero-order regime: rate = k_cat[AD] ⇒ [AD] = 1.03 × 10⁻⁶ / 1.33 = **7.7 × 10⁻⁷ mol dm⁻³** (mark scheme 7.74 × 10⁻⁷).
**L2 · Thought** Only in the saturated regime can you extract [enzyme] from the slope alone — say so explicitly; this is the consequential-marking bridge from (e) (answer = (e)(ii) ÷ 1.33).

### (g) How the half-life varies — circle one
**L1 · Answer** **It decreases.**
**L2 · Thought** For zero-order decay t½ = [EtOH]₀/2k: as the concentration falls, the time to halve the *remaining* concentration shrinks proportionally — the opposite of first-order intuition (constant t½). Confusing the two is the designed trap.

### (h) Sources of the toxic metabolites
**L1 · Answer** (i) methanoic (formic) acid ← **methanol**; (ii) oxalic (ethanedioic) acid ← **ethane-1,2-diol (ethylene glycol)**.
**L2 · Thought** The enzyme oxidises each –CH₂OH to –COOH; count the carboxyls in the metabolite to find the number of hydroxymethyl groups in the poison (one → methanol; two adjacent → the diol). This is why both are treated with ethanol — competitive substrate.

### (i) Metabolism of the poisonous alcohol — tick all that apply
**L1 · Answer** Tick: **"The maximum rate of metabolism is faster for ethanol"** (k_cat 1.33 > 1.10 s⁻¹) and **"A higher concentration of the poisonous alcohol is needed for the reaction to proceed at half of its maximum rate"** (K_M 3.2 × 10⁻² > 1.00 × 10⁻³ mol dm⁻³). Unticked: same-max-rate, ethanol-needs-more, different-rate-law.
**L2 · Thought** V_max = k_cat[enzyme] and the half-max concentration *is* K_M — the two statements follow directly from comparing the constants; the rate *law* (Michaelis–Menten form) is the same for both substrates, only the parameters differ.

---

## Question 5 — "Green" jet fuel (15 marks)

### (a) CO₂ + steam → syngas + oxygen
**L1 · Answer** **CO₂ + H₂O → CO + H₂ + O₂** (atom audit: C 1, H 2, O 3 both sides ✓).
**L2 · Thought** Both reactants are reduced one notch (CO₂ → CO, H₂O → H₂) and the discarded oxygen atoms pair up as O₂ — the equation balances in one pass if O₂ is written last.

### (b) Fischer–Tropsch
**L1 · Answer**
- (i) Alkane CₙH₂ₙ₊₂: **n CO + (2n+1) H₂ → CₙH₂ₙ₊₂ + n H₂O**.
- (ii) n = 12: **CO : H₂ = 12 : 25**.
**L2 · Thought** Balance the carbon first (n CO), then oxygen forces n H₂O, then count hydrogens to fix (2n+1) H₂ — a fixed order that works for any n. The 12:25 ratio (~1:2) is why syngas plants tune H₂/CO near 2.

### (c) Ceria-mediated reductions
**L1 · Answer** (i) **CeO₂₋δ + CO₂ → CeO₂ + CO**; (ii) **CeO₂₋δ + H₂O → CeO₂ + H₂**.
**L2 · Thought** Closed-cycle audit: the oxygen vacancies created in Step 1 are exactly refilled by oxygen stripped from CO₂/H₂O in Step 2 — cerium is the oxygen shuttle, never consumed. The δ cancels on both sides, which is the point of writing it non-stoichiometrically.

### (d) δ and the predicted syngas volume
**L1 · Answer**
- (i) n(CeO₂) = 127/172.12 = 0.738 mol; n(O₂) = 367/24000 = 0.0153 mol ⇒ O atoms lost = 0.0306 mol; **δ = 0.0306/0.738 = 0.0414**.
- (ii) each O vacancy produces one molecule of CO or H₂: V = 0.0306 × 24.0 = 0.734 dm³ = **734 cm³**.
**L2 · Thought** The factor of 2 (O₂ molecules → O atoms) is the designed slip point — write "n(O atoms) = 2 n(O₂)" explicitly. (ii) is pure consequential marking from (i): vacancies out = syngas molecules out, by the equations in (c).

### (e) Actual H₂ and CO amounts
**L1 · Answer** n(total) = 747/24000 = 0.0311 mol; with H₂ : CO = 1.70 : 1:
- (i) n(H₂) = 0.0311 × 1.70/2.70 = **0.0196 mol**;
- (ii) n(CO) = 0.0311 × 1.00/2.70 = **0.0115 mol**.
**L2 · Thought** Ratio arithmetic: divide by the sum of ratio parts (2.70), not by the larger part. The small excess over the 734 cm³ prediction is real-world imperfection, not a balancing error — note it and move on.

### (f) Total solar energy used
**L1 · Answer** E = 3.60 kW × (26 × 60 s) + 0.80 kW × (34 × 60 s) = 5.616 × 10⁶ + 1.632 × 10⁶ = **7.25 × 10⁶ J (7.25 MJ)**.
**L2 · Thought** Both steps consume solar power — summing only Step 1 is the trap; W × s = J with kW × 10³ stated on the line.

### (g) Efficiency of the reactor
**L1 · Answer**
- (i) energy released = 0.0196 × 286 + 0.0115 × 283 = 5.61 + 3.26 = **8.87 kJ**;
- (ii) efficiency = 8.87 × 10³ / 7.25 × 10⁶ = **1.2 × 10⁻³ = 0.12%**.
**L2 · Thought** Mind the unit mismatch in the final division (kJ vs J) — converting the numerator to joules on the same line prevents the ×10³ error. The dismal 0.12% is the honest punchline: the chemistry works, the energy economics (yet) do not.

### (h) Combustion enthalpy of dodecane and the FT reaction enthalpy
**L1 · Answer**
- (i) increment per CH₂ = 5470 − 4816 = 654 kJ mol⁻¹ ⇒ ΔcH(C₁₂H₂₆) = −(5470 + 4 × 654) = **−8086 kJ mol⁻¹**.
- (ii) Hess cycle: ΔrH = ΣΔcH(reactants) − ΣΔcH(products) = [12 × (−283) + 25 × (−286)] − [−8086] = −10546 + 8086 = **−2460 kJ mol⁻¹** for 12 CO + 25 H₂ → C₁₂H₂₆ + 12 H₂O.
**L2 · Thought** The homologous-series increment assumes a constant CH₂ contribution — state that assumption (it is why only heptane and octane data are needed). For (ii), combusting *both* sides to the same terminus (12 CO₂ + 25 H₂O … products give 12 CO₂ + 13 H₂O — write the cycle explicitly and the sign takes care of itself: reactants' combustion is the bigger number, so the synthesis is exothermic, as a hydrogenation should be.

---

*End of Paper 11 (2015). Next: 2014 Round 1.*


---

# Paper 12 — 2014 UKChO Round 1 (46th IChO selection)

**Marks / time:** Q1 9, Q2 9, Q3 13, Q4 18, Q5 16 (total 65; 2 h ⇒ ≈1.8 min per mark).
**Theme map:** Q1 lanthanum carbonate (Fosrenol); Q2 sodium street-lamp spectrum and ionisation energy; Q3 tazarotene synthesis; Q4 bombardier-beetle spray (NMR/IR deduction); Q5 methane clathrates.

---

## Question 1 — Controlling phosphate levels (9 marks)

### (a) Lanthanum carbonate with stomach acid; phosphate precipitation
**L1 · Answer** (i) **La₂(CO₃)₃ + 6 HCl → 2 LaCl₃ + 3 H₂O + 3 CO₂**; (ii) **La³⁺(aq) + PO₄³⁻(aq) → LaPO₄(s)**.
**L2 · Thought** Both are pure metathesis — the stem says La stays +3 throughout, so no electron bookkeeping is needed, only atom and charge audits (charge audit on (ii): +3 − 3 = 0 ✓).

### (b) Precipitation of lanthanum carbonate
**L1 · Answer** **2 La(NO₃)₃ + 3 Na₂CO₃ → La₂(CO₃)₃(s) + 6 NaNO₃**.
**L2 · Thought** Balance the polyatomic ions as blocks (CO₃ as one unit, NO₃ as one unit) — nitrate is a spectator and never needs to be "balanced atom by atom."

### (c) The anhydrous carbonate route
**L1 · Answer**
- (i) trichloroethanoic acid: **Cl₃C–C(=O)–OH** (a CCl₃ group bonded to a carboxyl carbon).
- (ii) **La₂O₃ + 6 CCl₃COOH → 2 La(CCl₃COO)₃ + 3 H₂O**.
- (iii) **2 La(CCl₃COO)₃ + 3 H₂O → La₂(CO₃)₃ + 6 CHCl₃ + 3 CO₂** (audit: La 2, C 12, Cl 18, H 6, O 15 both sides ✓).
**L2 · Thought** (iii) is the interesting one: the trichloroacetate decarboxylates (CCl₃COO⁻ → CHCl₃ + CO₂ is the haloform-type fragmentation driven by the CCl₃⁻ carbanion's stability), and the released CO₂ is captured by La³⁺/water as carbonate. Balance C and Cl first — they are the busy elements — then H and O close automatically.

### (d) From lanthanum chloride and ammonium hydrogencarbonate
**L1 · Answer** **2 LaCl₃ + 6 NH₄HCO₃ → La₂(CO₃)₃(s) + 6 NH₄Cl + 3 CO₂↑ + 3 H₂O** (audit: H 30, O 18 both sides ✓).
**L2 · Thought** The hydrogencarbonate is both the carbonate source and the acid that liberates the extra CO₂: 6 HCO₃⁻ → 3 CO₃²⁻ + 3 CO₂ + 3 H₂O is the hidden disproportionation of the anion; seeing that pair (one loses CO₂, one keeps it) makes the coefficients obvious.

### (e) Tablet masses
**L1 · Answer**
- (i) n(La) = 1.000/138.91 = 7.199 × 10⁻³ mol; n(La₂(CO₃)₃·2H₂O) = 3.600 × 10⁻³ mol; M = 2(138.91) + 3(60.01) + 2(18.02) = 493.89 g mol⁻¹ ⇒ mass = **1.78 g**.
- (ii) 1 : 1 La³⁺ : PO₄³⁻ ⇒ m(PO₄³⁻) = 7.199 × 10⁻³ × 94.97 = **0.684 g (684 mg)**.
**L2 · Thought** Two traps, both defused by writing the mole chain: the "1000 mg" refers to *lanthanum ions*, not compound (so divide by 2 for the La₂ formula unit), and the hydrate water must be included in M (it is part of the weighed tablet). The 1:1 precipitation stoichiometry then converts moles of La directly into mass of phosphate.

---

## Question 2 — A sodium street lamp (9 marks)

### (a)–(b) Electronic configuration and valence electron
**L1 · Answer** (a) **1s² 2s² 2p⁶ 3s¹**; (b) **the 3s electron**.
**L2 · Thought** "Easiest to remove" = highest-energy, outermost shell — the single 3s electron is what all the spectroscopy below tracks.

### (c) Energy of the 3p → 3s transition (589.8 nm)
**L1 · Answer** (i) E = hc/λ = (6.626 × 10⁻³⁴ × 2.998 × 10⁸)/(589.8 × 10⁻⁹) = **3.368 × 10⁻¹⁹ J atom⁻¹**; (ii) × 6.022 × 10²³ = **202.8 kJ mol⁻¹**.
**L2 · Thought** Metres, not nanometres, inside hc/λ; the per-mole conversion multiplies by Nₐ (and ÷1000) — a classic two-step where a ×10³ error hides.

### (d) I.E.(nd) as n → ∞ — circle one
**L1 · Answer** **Zero.**
**L2 · Thought** I.E.(nd) = k/n²: the further the electron sits from the core, the weaker it is held; the series converges on the free electron, i.e. zero binding energy — this is the series limit of every Rydberg formula.

### (e) Expression for the transition energy
**L1 · Answer** **ΔE = I.E.(3p) − I.E.(nd)** (both ionisation energies measured from the same reference, the free ion + electron, so the transition is their difference).
**L2 · Thought** Draw the energy ladder mentally: free electron at the top (zero), 3p deeper than nd; the photon carries away the depth difference. The sign must come out positive (3p is the deeper, more-bound level).

### (f) I.E.(3p) from the graph; ground-state ionisation energy
**L1 · Answer**
- (i) With 1/λ = I.E.(3p)/(hc) − (k/hc)(1/n²), the intercept of the 1/λ vs 1/n² line (extrapolating the printed straight line to 1/n² = 0 — graphically, or equivalently by least-squares on the tabulated points) is **0.00245 nm⁻¹** ⇒ I.E.(3p) = hc × 2.450 × 10⁶ m⁻¹ = **4.87 × 10⁻¹⁹ J atom⁻¹** (293 kJ mol⁻¹).
- (ii) I.E.(3s) = I.E.(3p) + E(3p→3s photon) = 293.1 + 202.8 = **496 kJ mol⁻¹** (≈ 495.9).
**L2 · Thought** The extrapolation *is* the physics: 1/n² → 0 means the nd electron is already free, so the line's intercept corresponds to the 3p → continuum limit. Part (ii) then closes the ladder with one photon step (3s → 3p costs exactly the 589.8 nm photon energy); landing within 0.1% of the handbook value (495.8 kJ mol⁻¹) is the built-in self-check.

---

## Question 3 — Spot cream: the synthesis of tazarotene (13 marks)

### (a) Concentration of tazarotene in the cream
**L1 · Answer** Take 100 g of cream: n = 0.05/351.46 = 1.42 × 10⁻⁴ mol; V = 100/0.90 = 111 cm³ = 0.111 dm³ ⇒ c = 1.42 × 10⁻⁴/0.111 = **1.3 × 10⁻³ mol dm⁻³**.
**L2 · Thought** "0.05% by mass" fixes a 100 g basis; density then converts the *same* 100 g to volume — mixing the two bases (per gram vs per cm³) is the standard error here.

### (b) Compound A and Ester B
**L1 · Answer**
- **A = 6-chloropyridine-3-carboxylic acid** — `O=C(O)c1cnc(Cl)cc1` (KMnO₄ oxidises the ring methyl to COOH; the aryl chloride survives).
- **B = ethyl 6-chloropyridine-3-carboxylate** — `CCOC(=O)c1cnc(Cl)cc1` (Fischer esterification, EtOH/H₂SO₄).
**L2 · Thought** KMnO₄ stops at the carboxylic acid for a benzylic/heterobenzylic methyl; the chlorine at the 2-position is untouched (it is the leaving group saved for the final coupling — recognise it as a *latent* functional group from the start).

### (c) Compounds D, E, F, I and anions C⁻, G⁻
**L1 · Answer** (all machine-validated)
- **C⁻ = benzenethiolate**, PhS⁻ Na⁺.
- **D = prenyl phenyl sulfide**, PhS–CH₂–CH=C(CH₃)₂ — `S(CC=C(C)C)c1ccccc1` (C₁₁H₁₄S ✓): SN₂ of PhS⁻ on prenyl bromide.
- **E = 4,4-dimethylthiochromane** — `CC1(C)CCSc2ccccc21` (C₁₁H₁₄S ✓): Lewis acid generates the tertiary cation at CMe₂, which cyclises onto the ortho position of the ring (intramolecular Friedel–Crafts) — the "isomerisation" relabels a C–S-tethered alkene as a fused thiochromane.
- **F = 6-acetyl-4,4-dimethylthiochromane** — `CC(=O)c1ccc2c(c1)C(C)(C)CCS2` (C₁₃H₁₆OS ✓): Friedel–Crafts acylation *para to sulfur* on the aromatic ring (S is the strongest director present).
- **G⁻ = the lithium enolate of F**, [Ar–C(O⁻)=CH₂]Li⁺ (LDA removes a methyl α-proton of the acetyl group — kinetic enolate).
- **I = 6-ethynyl-4,4-dimethylthiochromane** — `C#Cc1ccc2c(c1)C(C)(C)CCS2` (C₁₃H₁₄S ✓): trapped as the enol phosphate H (the diethyl enol phosphate, C₁₃H₁₅OS–O–PO(OEt)₂ → H = C₁₇H₂₅O₅PS by construction; exact structure as drawn in the scheme — verify against it), then LDA eliminates lithium diethyl phosphate to reveal the alkyne (the products listed — diisopropylamine + Li⁺(EtO)₂PO₂⁻ — are the elimination's fingerprint; atom audit: H − (EtO)₂PO₂Li = C₁₃H₁₄S ✓).
**L2 · Thought** The enol-phosphate detour is the tell: a methyl ketone cannot be dehydrated directly to an alkyne, so it is converted enolate → vinyl phosphate → β-elimination. When a scheme shows an enol phosphate (or enol triflate) plus strong base, read "alkyne under construction." Every formula along the chain was audited (C₁₁ → C₁₁ → C₁₃ → C₁₃): the acetylation is the only carbon-adding step, exactly matching the +C₂H₂O from F's formation.

### (d) Classification of H → I — circle one
**L1 · Answer** **Elimination** (loss of (EtO)₂PO₂H equivalents across the vinyl C–C, forming the C≡C triple bond).
**L2 · Thought** Classify by net change: two bonds to leaving groups replaced by one extra π-bond — no change in oxidation state, no atoms added.

### (e) Anion J
**L1 · Answer** **The lithium acetylide of I**: Ar–C≡C⁻ Li⁺ (the terminal alkyne C–H is acidic enough for the very strong base).
**L2 · Thought** Terminal alkynes (pKₐ ≈ 25) are deprotonated by amide bases; the acetylide is then the nucleophile for the final SNAr on B's activated 2-chloropyridine — this is the standard two-step "alkyne anion + aryl halide" coupling logic in disguise.

### (f) ¹³C NMR signals of tazarotene
**L1 · Answer** **20** (C₂₁H₂₁NO₂S; the only equivalent pair is the gem-dimethyl on C4 of the thiochromane — 21 carbons, 20 environments).
**L2 · Thought** No molecular symmetry anywhere else (the pyridine and the thiochromane are both unsymmetrically substituted); count carbon *environments*, not carbons, and hunt specifically for accidental equivalence — the gem-dimethyl pair is the only one.

### (g) The active form of the pro-drug
**L1 · Answer** **Tazarotenic acid** — the carboxylic acid `O=C(O)c1cnc(cc1)C#Cc1ccc2c(c1)C(C)(C)CCS2` (C₁₉H₁₇NO₂S, M = 323.41 ✓): ester hydrolysed to acid, −C₂H₄ in mass and −2 signals (OCH₂ and CH₃ of the ethyl ester) ✓.
**L2 · Thought** Pro-drug activation = esterase hydrolysis; the two clues (ΔM = 28.05 and −2 ¹³C signals) point at exactly the ethyl ester and nothing else — checking both constraints simultaneously is what makes the assignment certain rather than plausible.

---

## Question 4 — Bombardier beetles (18 marks)

### (a) Catalase reaction
**L1 · Answer** (i) **2 H₂O₂ → 2 H₂O + O₂**; (ii) **Disproportionation**.
**L2 · Thought** Oxygen starts at −1 in H₂O₂ and finishes at −2 (water) and 0 (O₂): the same element is both oxidised and reduced — the definition of disproportionation.

### (b) Overall equation with A
**L1 · Answer** **A + H₂O₂ → B + 2 H₂O** (sum of H₂O₂ → H₂O + ½O₂ and A + ½O₂ → B + H₂O).
**L2 · Thought** Add the two given equations and cancel the ½O₂ — the peroxide's "active oxygen" ends up in B, the rest as water; atom audit: A + H₂O₂ on the left, B + 2H₂O on the right closes if B contains one more O than A.

### (c) Energy and minimum peroxide concentration
**L1 · Answer**
- (i) Q = mcΔT = 1000 g × 4.18 × 80 = **3.34 × 10⁵ J (334 kJ)** per dm³ of mixture.
- (ii) n(A) needed per dm³ of mixture = 334.4/203 = 1.65 mol; H₂O₂ reacts 1 : 1 with A, and the peroxide chamber supplies half the mixture volume ⇒ c(H₂O₂) = 1.65 × 2 = **3.3 mol dm⁻³**.
**L2 · Thought** The chain is energy → moles (via ΔH per mole of A) → concentration, with the "equal volumes" doubling applied **last** (§7.5: yield/dilution factors land on the final moles). The factor of 2 for chamber vs mixture volume is the mark most often dropped.

### (d) Counting 1,2,4-trisubstitution isomers
**L1 · Answer** (i) **6** (3! arrangements of three different substituents over three distinguishable positions); (ii) **3** (choose which of the three positions carries the odd substituent B; the two A's fill the rest).
**L2 · Thought** The 1,2,4-pattern has no residual symmetry that permutes the substituted positions (the three ring H's are all in different environments), so positions are fully distinguishable — simple counting, no quotient to divide out.

### (e) IR assignments for I and II
**L1 · Answer** **I = O–H stretch** (very broad, H-bonded phenolic O–H, ~3300 cm⁻¹); **II = C–H stretches** (the sharp cluster ~2850–3000 cm⁻¹, aliphatic/aromatic C–H of the methyl group and ring).
**L2 · Thought** Breadth is diagnostic: only H-bonded O–H gives that huge trough; the sharp multiplet beside it sits at ordinary C–H frequency. Both bonds must live in the X substituents (per the stem), which already whispers "OH + CH₃."

### (f) Identities of Xa and Xb
**L1 · Answer** (i) Xa = **–OH (hydroxyl)**: peaks III and IV (1H each, ~8.3 and ~8.2 ppm) vanish with D₂O — exchangeable protons, and two *different* such protons mean two non-equivalent OH groups; (ii) Xb = **–CH₃ (methyl)**: peak VIII, 3H singlet at ~2.1 ppm (aryl methyl).
**L2 · Thought** The D₂O test identifies exchangeable H (O–H/N–H), and there being *two* singlets that exchange (not one 2H signal) tells you the two OH groups are chemically inequivalent — an early hint the ring has no symmetry, corroborated by the ¹³C count (7 signals = all carbons distinct).

### (g) Assigning the ring protons H1–H3
**L1 · Answer** Coupling logic: H1 (C6, between ring H and X) couples only *ortho* to H2 → large doublet; H3 (C3, flanked by two X-bearing carbons) couples only *meta* to H2 → small doublet; H2 (C5) couples ortho to H1 *and* meta to H3 → doublet of doublets (four lines).
**H1 = signal V** (6.6, larger-J doublet); **H3 = signal VI** (6.5, small-J doublet); **H2 = signal VII** (6.4, dd).
**L2 · Thought** Count each signal's couplings before matching chemical shifts: the dd signal (VII) must be the middle proton (H2) — that assignment is coupling-determined, not shift-guessed; the two doublets are then distinguished by splitting width (ortho ≫ meta), with the shift order (H1 ortho to OH, most deshielded of the pair) as corroboration only.

### (h) Structures of C and A
**L1 · Answer** **C = benzene-1,4-diol (hydroquinone)** — `Oc1ccc(O)cc1` (a disubstituted benzene with only two ¹H signals: 4 equivalent aromatic H + OH); hence **A = 2-methylbenzene-1,4-diol (methylhydroquinone / toluhydroquinone)** — `Cc1cc(O)ccc1O` (C₇H₈O₂ ✓): OH at 1,4 (Xa, Xa), CH₃ at 2 (Xb).
**L2 · Thought** C is the key that turns the whole lock: a *disubstituted* benzene with just two proton signals demands the para pattern with identical substituents (para ⇒ all four ring H equivalent); since A oxidises like a hydroquinone (beetle spray = quinone chemistry), the substituents are OH, and A is then C plus one methyl. The Xa = OH assignment from (f) is confirmed, and the 1,4-relationship of the two OH groups is fixed by C.

### (i) Structures of B and D
**L1 · Answer** **B = 2-methylcyclohexa-2,5-diene-1,4-dione (toluquinone)** — `CC1=CC(=O)C=CC1=O` (C₇H₆O₂ ✓: two-electron/two-proton oxidation of the hydroquinone); **D = cyclohexa-2,5-diene-1,4-dione (1,4-benzoquinone)** — `O=C1C=CC(=O)C=C1` (single ¹H signal: all four vinylic H equivalent ✓).
**L2 · Thought** Quinone formation is the beetle's entire weapons programme (A + ½O₂ → B + H₂O adds one O net to the ring while ejecting H₂O — the hydroquinone → quinone + H₂O bookkeeping closes). D's one-signal spectrum is the final consistency proof: only the symmetric para-quinone makes all its protons equivalent.

---

## Question 5 — Fire and ice: methane clathrates (16 marks)

### (a) Combustion of methane
**L1 · Answer** **CH₄ + 2 O₂ → CO₂ + 2 H₂O**.
**L2 · Thought** Complete combustion, carbon first, hydrogen second, oxygen last — the ordering that never fails.

### (b) Formula of structure-II hydrate
**L1 · Answer**
- (i) n(CO₂) = n(CH₄) = 84.73/100.09 = 0.8466 mol; water released by burning that methane = 2 × 0.8466 × 18.02 = 30.50 g; hydrate's own water = 116.92 − 30.50 = 86.42 g = 4.798 mol. Ratio H₂O : CH₄ = 4.798/0.8466 = 5.67 = 17/3 ⇒ empirical formula **(CH₄)₃(H₂O)₁₇** (M = 354.46).
- (ii) 2835.18/354.46 = 8.00 ⇒ molecular formula **(CH₄)₂₄(H₂O)₁₃₆**.
**L2 · Thought** The combustion water is *mixed provenance* — cage water plus oxidation water — so the 2 H₂O per CH₄ must be subtracted before the ratio is taken; skipping that correction gives 5.76, not 5.67, and the clean 3 : 17 integer check (§4 multi-component balance: a clean ratio is the self-check) is lost. The ×8 multiplier in (ii) lands on the known 136-water sII cage, a good omen.

### (c) Volume of the Baikal methane at −19.0 °C
**L1 · Answer** n = 6.67 × 10¹⁴ g / 16.04 = 4.16 × 10¹³ mol; V = nRT/p = 4.16 × 10¹³ × 8.31 × 254 / 1.0 × 10⁵ = **8.8 × 10¹¹ m³**.
**L2 · Thought** Unit ladder: kg → g → mol; Celsius → kelvin (254 K, not −19!); Pa and m³ stay SI throughout so no volume conversion is needed at the end. One atmosphere is assumed (gas escaping at the surface).

### (d) Mass and volume of the hydrate
**L1 · Answer**
- (i) %CH₄ = (8 × 16.04)/957.07 = **13.4%**.
- (ii) mass of hydrate = 6.67 × 10¹¹/0.1341 = **4.97 × 10¹² kg**.
- (iii) V = m/ρ = 4.97 × 10¹² kg / 950 kg m⁻³ = **5.2 × 10⁹ m³**.
**L2 · Thought** Consequential chain (i) → (ii) → (iii); convert the density 0.95 g cm⁻³ = 950 kg m⁻³ *before* dividing, so the answer falls out directly in m³. The number is enormous but self-consistent: ~5 km³ of ice holding ~10¹² m³ of gas — the clathrate concentrates methane by ~170×.

### (e) The unit cell
**L1 · Answer**
- (i) m = 957.07/6.022 × 10²³ = **1.59 × 10⁻²¹ g**.
- (ii) V_cell = 1.589 × 10⁻²¹/0.95 = 1.67 × 10⁻²¹ cm³ ⇒ edge = (1.67 × 10⁻²¹)^⅓ = 1.19 × 10⁻⁷ cm = **1.19 nm**.
- (iii) V(CH₄) = 8 × (4π/3)(0.21)³ = **0.310 nm³**; V(H₂O) = 46 × (4π/3)(0.14)³ = **0.529 nm³**.
- (iv) occupied = (0.310 + 0.529)/1.672 = **50%** (50.2%).
**L2 · Thought** The cell edge must land near 1 nm (§7.4 order-of-magnitude check: molecular crystals have cell edges of several molecular diameters); the packing fraction near 50% is the physically sensible answer for an open hydrogen-bonded cage — ice-like water frameworks are notoriously empty, which is precisely why there is room for the methane.

### (f) Enthalpy of formation of the hydrate
**L1 · Answer** Combustion: (CH₄)₈(H₂O)₄₆ + 16 O₂ → 8 CO₂ + 62 H₂O, ΔcH = −6690.4 kJ mol⁻¹.
ΔfH(hydrate) = [8(−393.5) + 62(−285.8)] + 6690.4 = −14177.2 kJ mol⁻¹.
Formation: 8 CH₄(g) + 46 H₂O(l) → (CH₄)₈(H₂O)₄₆(s):
ΔH = −14177.2 − [8(−74.8) + 46(−285.8)] = −14177.2 + 13745.2 = **−432 kJ mol⁻¹**.
**L2 · Thought** Two Hess cycles stacked: combustion data first digs out ΔfH of the clathrate itself (note the water count on combustion is 62 = 46 cage + 16 from burning the methanes — the most common slip), then formation from CH₄ + H₂O is a plain products-minus-reactants. The modest exothermicity (≈ −9.4 kJ per water) is the physical point: the cage is held by hydrogen-bond re-organisation and van der Waals contacts, not by any strong new bond.

---

*End of Paper 12 (2014). Next: 2013 Round 1.*


---

# Paper 13 — 2013 UKChO Round 1 (45th IChO selection)

**Marks / time:** Q1 9, Q2 13, Q3 9, Q4 15, Q5 17 (total 63; 2 h ⇒ ≈1.9 min per mark).
**Theme map:** Q1 rocket fuels (hydrazine); Q2 Olympic medals + bike-tyre gases; Q3 colours + qualitative-analysis grid; Q4 diazepam/alprazolam synthesis; Q5 creatine/creatinine (¹H NMR).

---

## Question 1 — Rocket fuels (9 marks)

### (a) Hydrazine decomposing to ammonia and nitrogen
**L1 · Answer** **3 N₂H₄ → 4 NH₃ + N₂** (audit: N 6, H 12 both sides ✓).
**L2 · Thought** Disproportionation of the N–N framework: nitrogen goes from −2 to −3 (in NH₃) and to 0 (in N₂) — total rise = total fall: one N₂ released per four NH₃, which fixes the 3 : 4 : 1 coefficients.

### (b) Enthalpy of decomposition of hydrazine to its elements
**L1 · Answer** From 2 NH₃ + H₂O₂ → N₂H₄ + 2 H₂O, ΔrH° = −241.0 kJ mol⁻¹:
ΔfH°(N₂H₄, l) = [2(−46.1) + (−187.8) + (−241.0)] − [2(−285.8)] = +50.6 kJ mol⁻¹.
Decomposition N₂H₄(l) → N₂(g) + 2 H₂(g): ΔrH° = **−50.6 kJ mol⁻¹**.
**L2 · Thought** The formation equation is the target equation run backwards — once ΔfH° is isolated the decomposition is just its negative. Sign audit: hydrazine is endothermic (+50.6), which is *why* it is a good monopropellant (its decomposition releases energy).

### (c) C-Stoff / T-Stoff
**L1 · Answer**
- (i) N: **−2 in N₂H₄ → 0 in N₂** (oxidised); O: **−1 in H₂O₂ → −2 in H₂O** (reduced).
- (ii) **CH₃OH + 3 H₂O₂ → CO₂ + 5 H₂O** (audit: C 1, H 10, O 7 both sides ✓).
- (iii) n(N₂H₄) = 225 000 × 1.021/32.05 = 7.17 × 10³ mol ⇒ 7.17 × 10³ × 622.2 = 4.46 × 10⁶ kJ; n(CH₃OH) = 862 000 × 0.7918/32.04 = 2.13 × 10⁴ mol ⇒ 2.13 × 10⁴ × 726.0 = 1.55 × 10⁷ kJ; total = **1.99 × 10⁷ kJ (≈ 19.9 GJ) evolved**.
**L2 · Thought** (iii) is a three-step chain per fuel (volume → mass → moles → heat), with densities converting litres to grams (1 L = 1000 cm³ — write it). Oxidation-number bookkeeping in (i) shows peroxide is the oxidiser in both combustions; the methanol equation balances fastest by balancing O atoms last via the H₂O coefficient.

### (d) N₂H₄ / N₂O₄ hypergolic pair
**L1 · Answer** (i) **N₂ and H₂O** (e.g. 2 N₂H₄ + N₂O₄ → 3 N₂ + 4 H₂O — both products are stable gases ✓); (ii) **NO₂** (nitrogen dioxide, the brown monomer formed on warming N₂O₄).
**L2 · Thought** (i) Apply the stated design rules as a filter: "stable + gaseous" leaves only N₂ and H₂O as sinks; then balance (the N in N₂O₄ is +4, in N₂H₄ −2, both ending at 0 — a comproportionation). (ii) N₂O₄ ⇌ 2 NO₂ is the classic brown-gas equilibrium — "brown" is the give-away.

### (e) C₂H₈N₂ (Apollo fuel)
**L1 · Answer** **(CH₃)₂N–NH₂** (1,1-dimethylhydrazine, UDMH) — `CN(C)N`: two methyls on one nitrogen (same environment ✓), the two nitrogens different (NMe₂ vs NH₂ ✓).
**L2 · Thought** "Two carbons in the same environment" forces both methyls onto the *same* atom (or a symmetric arrangement); "two nitrogens different" kills the symmetric alternative CH₃–NH–NH–CH₃. Unsymmetrical substitution on N₂H₄ is the only survivor.

---

## Question 2 — Great Britain at cycling (13 marks)

### (a) Percentage of copper in the bronze medal
**L1 · Answer** From the two equations: 2 Cu²⁺ ~ 1 I₂ ~ 2 S₂O₃²⁻, so n(Cu) = n(S₂O₃²⁻).
n(thiosulfate) = 12.20 × 10⁻³ × 0.100 = 1.220 × 10⁻³ mol (aliquot) ⇒ n(Cu) total = 1.220 × 10⁻² mol (× 250.0/25.00) ⇒ m(Cu) = 0.775 g ⇒ **96.9% by mass**.
**L2 · Thought** The iodometric chain collapses to 1 : 1 Cu : thiosulfate because the factor 2 appears twice and cancels — write the mole ratio chain explicitly (Cu²⁺ → I₂ → S₂O₃²⁻) before substituting, and remember the aliquot factor (×10) *after* the titration moles, not before.

### (b) Mass of a silver medal
**L1 · Answer** V = π r²h = π × (4.25 cm)² × 0.7 cm = 39.7 cm³. The stem's rule "density varies in proportion to composition **by mass**" is a direct linear prescription: ρ = Σ wᵢρᵢ = 0.925 × 10.49 + 0.075 × 8.96 = **10.38 g cm⁻³**. Mass = 39.72 × 10.38 = **412 g**.
**L2 · Thought** Read the alloy rule as a *prescribed model* (§7.5 prescribed-rule discipline): "density ∝ mass composition" means ρ = w₁ρ₁ + w₂ρ₂, full stop — do not substitute your own favourite mixing law for the printed one (volume additivity would give 411 g: close, but not the model the stem prescribes). The numerical difference is small (412 vs 411 g) but the rule-compliance is the mark.

### (c) Composition of a gold medal
**L1 · Answer** Acid-insoluble residue = **Au: 0.067/5.000 = 1.34%**; HCl precipitate = AgCl: n = 6.144/143.32 = 0.04287 mol ⇒ m(Ag) = 0.04287 × 107.87 = 4.625 g ⇒ **Ag: 92.5%**; **Cu: 100 − 1.34 − 92.49 = 6.2%**.
**L2 · Thought** Separation logic first: conc. HNO₃ dissolves Ag and Cu but not Au (the residue); Cl⁻ then pulls Ag down as AgCl (the Cu stays in solution — never isolated, hence by difference). The precipitate is AgCl, not Ag — the M(AgCl)/M(Ag) conversion is the mark-discriminator.

### (d) Volume of a torus-shaped tyre
**L1 · Answer** r = (66 − 2.3)/2 cm = 0.3185 m (wheel diameter minus one tube diameter, halved), d = 0.023 m: V = π²rd²/2 = π² × 0.3185 × (0.023)²/2 = **8.3 × 10⁻⁴ m³**.
**L2 · Thought** The only subtlety is r: it is measured to the *centre of the tube*, so subtract one tube diameter from the wheel diameter before halving. SI units throughout (cm → m before cubing).

### (e) Gas in the tyres
**L1 · Answer** p = 120 × 6895 = 8.27 × 10⁵ Pa.
- (i) n = pV/RT = 8.27 × 10⁵ × 8.31 × 10⁻⁴/(8.31 × 298) = **0.278 mol per tyre**.
- (ii) M(air) = 0.8 × 28.02 + 0.2 × 32.00 = 28.82 g mol⁻¹; mass = 2 × 0.278 × 28.82 = **16.0 g**.
- (iii) He: 2 × 0.278 × 4.003 = 2.22 g ⇒ reduction = 16.0 − 2.2 = **13.8 g**.
- (iv) SF₆: 2 × 0.278 × 146.06 = 81.2 g ⇒ increase = 81.2 − 16.0 = **65.2 g**.
**L2 · Thought** Same n for every gas (same p, V, T) — the whole question is "same moles, different molar mass," so compute n once and rescale. The mass differences (≈14 g saved, ≈65 g added) are tiny against bike + rider, which is the physical punchline; note the premise treats 120 psi as the absolute pressure inside the tyre, as the question intends.

---

## Question 3 — Coloured compounds (9 marks)

### (a) Colour assignments
**L1 · Answer** (exactly the answer booklet's six colours):
**red = C** (Cu₂O, brick-red) alone; **orange = G** (K₂Cr₂O₇) alone; **yellow = G + H** (no single substance is yellow; dichromate + base → yellow chromate: Cr₂O₇²⁻ + 2 OH⁻ → 2 CrO₄²⁻ + H₂O); **green = F** (FeSO₄·7H₂O, pale green) alone; **blue = D + H** (no blue solid in the list; CuSO₄ + base → pale-blue Cu(OH)₂ precipitate); **violet = I** (VSO₄·7H₂O) alone.
**L2 · Thought** Inventory first: list each solid's colour from stock knowledge (anhydrous CuSO₄ is *white* — the classic trap, since everyone pictures the blue pentahydrate; B (CuO) is black; A, E, J are white), then ask what new coloured species a pairwise mixture can *generate* — hydroxide precipitates and the dichromate↔chromate shift are the only colour-producing chemistries available, which is why exactly two colours (yellow, blue) need pairs. Answer the booklet's colour list exactly — do not add extra colours (white/black) to it; the inventory belongs to the working, not the answer grid.

### (b) The T–Z mixing grid
**L1 · Answer**
**T = lead(II) nitrate; U = sodium iodide; V = barium chloride; W = silver nitrate; X = sodium carbonate; Y = iron(II) sulfate; Z = chlorine water.**
Key assignments: the brown solution (U + Z) is I₂/I₃⁻ ⇒ {U, Z} = {NaI, Cl₂}; Z + Y gives a pale-yellow solution (Fe²⁺ → Fe³⁺) ⇒ Z = Cl₂ water, Y = FeSO₄, hence U = NaI; U + T gives bright-yellow PbI₂ ⇒ T = Pb(NO₃)₂; W forms *two* precipitates that darken in daylight (with V and with Z — AgCl is photolabile) ⇒ W = AgNO₃; W + X off-white = Ag₂CO₃ ⇒ X = Na₂CO₃; V = BaCl₂ (only one left; check: V + X white BaCO₃ ✓, V + Y white BaSO₄ ✓, V + W white AgCl darkening ✓).
**L2 · Thought** Start from the two *signature* observations — "brown solution" (only I⁻ + Cl₂ can produce it) and "darkened in daylight" (only silver halides do that) — they anchor U, Z, W immediately; the off-white Ag₂CO₃ and the bright-yellow PbI₂ then fix X and T, and V falls out by elimination. Finish with a full-grid consistency pass (every cell, including the blanks) — the assignment above survives all 21 pairings.

---

## Question 4 — GPs giving out too many drugs (15 marks)

### (a) Yield and scale-up
**L1 · Answer**
- (i) overall yield = 0.87 × 0.66 × 0.81 × 0.77 × 0.90 × 0.48 × 0.86 × 0.89 × 0.91 = **10.8%**.
- (ii) dose = 5 mg × 4 × 365 × 3 = 21.9 g diazepam; n = 21.9/284.734 = 0.0769 mol; n(aniline) = 0.0769/0.1078 = 0.714 mol; mass = 0.714 × 127.57 = **91 g of 4-chloroaniline**.
**L2 · Thought** Chain yields multiply (never average); the scale-up is one mole-to-mole step divided by the *overall* fractional yield — converting each intermediate's mass would be wasted work, since only the endpoints' molar masses matter.

### (b) Intermediates A–H in the diazepam synthesis
**L1 · Answer** (all machine-validated)
- **A = 2-bromo-4-chloroaniline** — `Nc1ccc(Cl)cc1Br` (C₆H₅NClBr): Br₂ brominates the aniline *ortho* to NH₂ (the only free activated position).
- **B = N-methyl-2-bromo-4-chloroaniline** — `CNc1ccc(Cl)cc1Br` (**C₇H₇NClBr ✓ = A + CH₂ − H**): mono-N-methylation with CH₃I.
- **C = Cbz-glycine acid chloride**, ClCO–CH₂–NH–COOCH₂Ph — `O=C(Cl)CNC(=O)OCc1ccccc1` (PCl₅: COOH → COCl).
- **D = Ar–N(CH₃)–CO–CH₂–NH–Cbz** — `CN(C(=O)CNC(=O)OCc1ccccc1)c1ccc(Cl)cc1Br` (**C₁₇H₁₆O₃N₂ClBr ✓**: B + C − HCl): N-acylation of B's N–H.
- **E = Ar–N(CH₃)–CO–CH₂–NH₂** — `CN(C(=O)CN)c1ccc(Cl)cc1Br` (**C₉H₁₀N₂OClBr ✓**): HBr cleaves the Cbz group (−CO₂, −PhCH₂Br), freeing the glycine amine.
- **F = Ar–N(CH₃)–CO–CH₂–NH–COCH₃** — `CN(C(=O)CNC(C)=O)c1ccc(Cl)cc1Br` (**C₁₁H₁₂N₂O₂ClBr ✓ = E + C₂H₂O**): acetylation of the freed amine.
- (cyclisation, C₁₂H₁₁N₂O₃Cl ✓ = F + CO − HBr) = **the carbonylative cyclisation product**: N-methyl benzodiazepine trione... precisely the 7-membered ring N(CH₃)–C(=O)–CH₂–N(COCH₃)–C(=O)– fused to the aryl ring — `CN1C(=O)CN(C(C)=O)C(=O)c2cc(Cl)ccc21`: Pd-catalysed CO insertion replaces Ar–Br by Ar–C(=O)–N, closing the 7-ring.
- **G = the phenyl carbinol** — `CN1C(=O)CN(C(C)=O)C(O)(c2ccccc2)c2cc(Cl)ccc21` (**C₁₈H₁₇N₂O₃Cl ✓ = cyclic + C₆H₆**): PhMgBr adds to the newly inserted ring ketone.
- **H = the hydroxylamine adduct of diazepam's imine**, C5 bearing Ph and NHOH with N4–H free — `CN1C(=O)CNC(NO)(c2ccccc2)c2cc(Cl)ccc21` (**C₁₆H₁₆N₃O₂Cl ✓ = G + 2 NH₂OH − H₂O − CH₃CONHOH**): the first NH₂OH deacetylates N4 (as acetohydroxamic acid), the second displaces the C5–OH; NaHSO₃ then expels hydroxylamine to give the C5=N4 imine of diazepam (**C₁₆H₁₃N₂OCl ✓**).
**L2 · Thought** Every assignment here is earned by the printed molecular formulas, not by route memory: D, E, F, the cyclised product, G and H each match to the atom. The two reagent-driven leaps are the CO insertion (a carbon count +1 with Br lost — only a new C=O bridge can do that while closing a 7-ring) and the G → H → diazepam bookkeeping, where "−CH₃CONHOH" advertises hydroxylamine's role as a deacetylating agent and "H = diazepam + NH₂OH" (check: C₁₆H₁₆N₃O₂Cl − C₁₆H₁₃N₂OCl = H₃NO) tells you H is the imine's hydroxylamine adduct.

### (c) Intermediates I, J, K in the alprazolam synthesis
**L1 · Answer** (all machine-validated)
- **I = the thionolactam** (C2 = S in place of C2 = O) — `S=C1CN=C(c2ccccc2)c2cc(Cl)ccc2N1` (**C₁₅H₁₁N₂SCl ✓**): P₂S₅ swaps the amide oxygen for sulfur.
- **J = the amidrazone**, C2 = N–NH₂ — `NN=C1CN=C(c2ccccc2)c2cc(Cl)ccc2N1` (**C₁₅H₁₃N₄Cl ✓ = I + N₂H₄ − H₂S**): hydrazine displaces the sulfur.
- **K = the ethylidene hydrazone**, C(=N–N=CH–CH₃) — `CC=NN=C1CN=C(c2ccccc2)c2cc(Cl)ccc2N1` (**C₁₇H₁₅N₄Cl ✓ = J + CH₃CHO − H₂O**): acetaldehyde condenses on the terminal –NH₂.
- (L, drawn, is the cyclised dihydrotriazole: K's terminal N=CH–CH₃ carbon bonds to the benzodiazepine N1–H, isomerising to the 1-methyl dihydrotriazolobenzodiazepine; DEAD then oxidatively aromatises the triazole — alprazolam **C₁₇H₁₃N₄Cl** — `Cc1nnc2n1-c1ccc(Cl)cc1C(c1ccccc1)=NC2`.)
**L2 · Thought** The triazole ring of alprazolam must be assembled from a 2-nitrogen + 1-carbon donor: P₂S₅ → thioamide → hydrazine → amidrazone installs N–N, acetaldehyde supplies the single carbon (becoming the triazole's methyl — count it: alprazolam's methyl is acetaldehyde's), and the "isomerisation" K ⇌ L is the intramolecular N1–H addition onto the azomethine carbon. Formula audits at each letter make the sequence self-checking.

### (d) Classification of L → alprazolam — tick one
**L1 · Answer** **Oxidation.**
**L2 · Thought** L (C₁₇H₁₅N₄Cl) → alprazolam (C₁₇H₁₃N₄Cl) is a net loss of H₂ — dehydrogenation of the dihydrotriazole to the aromatic triazole; DEAD is a recognised H-acceptor (oxidant). No atoms added or swapped, so it cannot be condensation/substitution; the electron count says oxidation.

---

## Question 5 — Getting big muscles: creatine (17 marks)

### (a) Creatine monohydrate
**L1 · Answer** Creatine = C₄H₉N₃O₂ ⇒ monohydrate = **C₄H₉N₃O₂·H₂O (i.e. C₄H₁₁N₃O₃)**.
**L2 · Thought** "Monohydrate" adds one water of crystallisation to the molecular formula — the water is not part of the covalent structure.

### (b) Biosynthetic origin of each creatine carbon
**L1 · Answer** **① (amidino C) = Ⓗ** (arginine's guanidinium carbon); **② (N–CH₃) = Ⓒ** (methionine's S-methyl, via SAM); **③ (CH₂) = Ⓐ** (glycine's α-carbon); **④ (COOH) = Ⓑ** (glycine's carboxyl carbon).
**L2 · Thought** Anatomy of the known pathway: the glycine skeleton survives intact as –N–CH₂–COOH (so ③④ ← glycine ⒶⒷ), the amidino group arrives as a block transfer from arginine (① ← Ⓗ), and the N-methyl is the classic SAM methylation, SAM's methyl being methionine's S–CH₃ (② ← Ⓒ). Matching *functional groups* (amidino C, methyl C, carboxyl C) rather than positions is what makes each assignment unique.

### (c) Ionisation states of creatine
**L1 · Answer**
- (i) pH 1 (+1): **guanidinium protonated, COOH neutral**: H₂N–C(=NH₂⁺)–N(CH₃)–CH₂–COOH.
- (ii) pH 7 (neutral): **zwitterion**: H₂N–C(=NH₂⁺)–N(CH₃)–CH₂–COO⁻.
- (iii) pH 12 (−1): **guanidine neutral, carboxylate**: H₂N–C(=NH)–N(CH₃)–CH₂–COO⁻.
**L2 · Thought** Two ionisable groups with a huge basicity gap: the guanidino group (conjugate acid pKₐ ≈ 12–13) holds its proton far longer than the carboxyl (pKₐ ≈ 2–3) gives up its own — so the +1 and neutral forms differ at the *carboxyl*, the neutral and −1 forms differ at the *guanidinium*. The given overall charges dictate which group moves at each pH; draw the charge on the guanidinium, not on the tertiary N.

### (d) Signal appearance for methionine C, D, F
**L1 · Answer** **C (S–CH₃): singlet** (3H; no H within three bonds — S–CH₃ is insulated by sulfur); **D (S–CH₂–): triplet** (2H; couples to the 2 H of the adjacent CH₂, n = 2 ⇒ n + 1 = 3); **F (α-CH): triplet** (1H; couples to the 2 H of the neighbouring CH₂).
**L2 · Thought** Coupling counts only H within three bonds *and* ignores N–H/O–H (exchanged away in D₂O) — so F sees only the β-CH₂, not the NH₂; the S–CH₃ sees nothing across the sulfur. Each answer is (neighbour H count) + 1, applied mechanically.

### (e) Carbons with diastereotopic protons
**L1 · Answer** **E (methionine) and K (arginine)**. The stem defines the scope operationally: diastereotopic pairs are "most often observed where the carbon under consideration is **bonded to** an asymmetric carbon atom" — i.e. the CH₂ *directly attached* to the stereocentre (the β-CH₂ in each amino acid: E next to F in methionine; K next to the α-carbon in arginine). Glycine (no stereocentre) contributes nothing.
**L2 · Thought** Two disciplines here. (1) Apply the question's own criterion, not the most general truth: more distant CH₂'s in a chiral molecule are *also* technically diastereotopic, but the mark scheme deducts half a mark per extra letter — in a tick/letter-list item, answer inside the stem's defined scope (§7.7: the deciding criterion is the printed one). (2) The structural logic behind the printed criterion: the diastereotopic splitting is largest and most reliably observed for the CH₂ adjacent to the stereocentre; further away the two H's become effectively equivalent on the NMR timescale. So "directly bonded" is where observation lives, not just where the scheme draws the line.

### (f) Structure of creatinine
**L1 · Answer** **2-imino-1-methylimidazolidin-4-one** — `CN1CC(=O)NC1=N` (C₄H₇N₃O ✓): the carboxyl OH condenses with the terminal amidino –NH₂ (−H₂O) to close a five-membered ring: N(CH₃)–CH₂–C(=O)–NH–C(=NH)–.
**L2 · Thought** "Cyclic molecule, equilibrium with loss of water" ⇒ intramolecular amide formation; the only sensible ring size is 5 (COOH to the terminal NH₂; attacking the =NH would give a strained/less stable alternative). Formula audit: C₄H₉N₃O₂ − H₂O = C₄H₇N₃O ✓ — exactly the waste product's formula.

### (g) Equilibrium constant from the ¹H NMR integrals
**L1 · Answer** K = [creatinine]/[creatine]. Signal A (4.1 ppm) = creatinine's ring CH₂ (2H); signal B (3.9 ppm) = creatine's CH₂ (2H). Since both are 2-proton signals, the integral ratio is the mole ratio directly: measuring the integral-trace steps, A : B ≈ 76 : 18 ≈ 4.2 : 1 ⇒ **K ≈ 4** (dimensionless; signal C at 3.0 ppm is the overlapping N–CH₃ of both species, 3H + 3H, consistent with a mixture rich in creatinine).
**L2 · Thought** The design is deliberate: the two methylene singlets are isohydric (2H each), so no proton-count correction is needed — step-height ratio = concentration ratio. Use C only as a sanity check (it must equal 1.5 × (A + B) in proton count), never in the ratio itself, because it contains both species.

### (h) The lipophilic supplement
**L1 · Answer** **Creatine ethyl ester** (ethyl 2-(1-methylguanidino)acetate): H₂N–C(=NH)–N(CH₃)–CH₂–C(=O)–O–CH₂CH₃ — `CCOC(=O)CN(C)C(=N)N` (C₆H₁₃N₃O₂ ✓). Evidence: a **triplet at 1.25 ppm (3H)** and a **quartet at 4.23 ppm (2H)** — a mutually coupled CH₃/CH₂ pair, i.e. an ethyl group, and its 4.2 ppm shift places the CH₂ on oxygen (ester O–CH₂); the creatine N–CH₃ (~3.0) and N–CH₂ (~3.9) are retained.
**L2 · Thought** The ionisation clue does the structural surgery: ionised at pH 1 (guanidinium still present) but *never* ionised at pH 12 ⇒ the carboxylic acid has been removed — derivatised. The NMR then says how: the only new feature is an O–CH₂–CH₃, so the acid is masked as its **ethyl ester** — more lipophilic, still protonatable on the guanidine. Triplet–quartet pairing with a 3-bond coupling is the fingerprint; a methyl ester would show a singlet at ~3.7 ppm instead.

---

*End of Paper 13 (2013). Next: 2012 Round 1.*


---

# Paper 14 — 2012 UKChO Round 1 (44th IChO selection)

**Marks / time:** 5 questions (Q1 sulfur chemistry; Q2 hair/perm kinetics; Q3 general knowledge; Q4 Lipitor synthesis; Q5 nano-car; 2 h).
**Theme map:** Q1 sulfur rings, S₄N₄, (SN)ₓ; Q2 sulfur in hair, thioglycolate acid–base + pseudo-first-order kinetics; Q3 general knowledge; Q4 atorvastatin (Lipitor) synthesis with IR table; Q5 molecular nano-car stereochemistry and motion.

---

## Question 1 — Sulfur chemistry

### (a) Enthalpy of 8 S₇(g) → 7 S₈(g)
**L1 · Answer** Both sides have 56 S–S bonds (8 × 7 = 7 × 8): ΔH = 56 × 260.0 − 56 × 263.3 = **−184.8 kJ mol⁻¹** (per equation as written).
**L2 · Thought** Ring equilibria are bond-count problems: count bonds broken (56 in S₇) and formed (56 in S₈) — the identical count is the trap; the enthalpy comes only from the bond-strength *difference* (3.3 kJ per bond × 56).

### (b) Solution equilibrium of S₇ and S₈
**L1 · Answer**
- i) n(S₇) = 0.0076 g/224.42 = **3.39 × 10⁻⁵ mol**; n(S₈) = 0.9892/256.48 = **3.86 × 10⁻³ mol** (in 1.00 dm³, these are the concentrations).
- ii) **K = [S₈]⁷/[S₇]⁸**.
- iii) K = (3.86 × 10⁻³)⁷/(3.39 × 10⁻⁵)⁸ = **7.3 × 10¹⁸** (units mol⁻¹ dm³, from the 7 − 8 exponent).
**L2 · Thought** Convert mass percent → mass → moles using each ring's own molar mass (n × 32.06) — using 32.06 alone is the designed slip. The enormous K is a consequence of the high powers: an equilibrium written with different stoichiometric totals carries concentration units, and its magnitude is meaningless without them.

### (c) Orthorhombic vs monoclinic S₈
**L1 · Answer** i) ΔrH = ΔcH(orthorhombic) − ΔcH(monoclinic) = −296.8 − (−297.1) = **+0.3 kJ mol⁻¹** (endothermic); ii) **orthorhombic** is the more stable form at 298 K (lower enthalpy by 0.3 kJ mol⁻¹).
**L2 · Thought** Hess through the common combustion products: the form with the *less* exothermic combustion sits *lower* in enthalpy. A +0.3 kJ difference is tiny — consistent with a real phase transition not far above room temperature.

### (d) S₄N₄ without cross-links
**L1 · Answer** An 8-membered ring alternating S and N: S1–N1=S2–N2–S3–N3=S4–N4–(back to S1), i.e. the two opposite sulfurs S2 and S4 each carry **two S=N double bonds (4 bonds each)** while S1 and S3 have two single bonds (2 bonds); every nitrogen has one single and one double bond (3 bonds).
**L2 · Thought** Bond-count bookkeeping on an alternating skeleton: give the two 4-bond sulfurs two doubles each and place them opposite (maximum separation), then every nitrogen lands on 3 bonds automatically. Any placement where the two S(IV) atoms are adjacent makes the double-bond pattern collide — a quick way to discard alternatives.

### (e) The cross-linked alternative
**L1 · Answer** Same alternating ring but with **all ring bonds alternating single/double** (each S=N–S pattern, so every S already has 3 bonds) plus **two transannular S–S single bonds** linking the opposite pairs (S1–S3 and S2–S4): every S then has 4 bonds (one double, two ring singles, one cross-link), every N keeps 3.
**L2 · Thought** The constraint "every S four bonds, every N three" is a small integer problem: with two cross-links to distribute, each S gains exactly one bond over the 3-bond alternating pattern — which fixes both the cross-link positions and the single/double alternation simultaneously. (These weak transannular S···S contacts are exactly what the real cradle-shaped S₄N₄ shows.)

### (f) Poly(sulfur nitride), (SN)ₓ
**L1 · Answer** Repeat unit: **–S=N–S–N=** drawn as a zig-zag chain with alternating bond orders, e.g. ···N–S=N–S–N=S–N··· in which every other sulfur is 4-bonded (two S=N double bonds) and the others 2-bonded; every N has one single and one double bond (3 bonds).
**L2 · Thought** The clue "linear polymer, conducts electricity" plus the bond-count constraints gives an alternating π-backbone: the conduction comes from the delocalised –S=N–S=N– π-system (the same alternation logic as (d), extended into a chain rather than closed into a ring).

---

## Question 2 — Controlling your hair

### (a) Percentage of sulfur in hair
**L1 · Answer**
- i) n(BaSO₄) = 0.260/233.39 = 1.114 × 10⁻³ mol ⇒ m(S) = 1.114 × 10⁻³ × 32.06 = 0.0357 g ⇒ **3.57%**.
- ii) dissolved BaSO₄ = 2.40 mg dm⁻³ × 2.50 dm³ = 6.00 mg; total = 266 mg ⇒ n = 1.140 × 10⁻³ mol ⇒ m(S) = 0.0365 g ⇒ **3.65%**.
**L2 · Thought** The sulfate-to-sulfur conversion (32.06/233.39) is the whole calculation in (i); (ii) is a two-source correction (§4): the precipitate on the filter is not all the sulfate — add back the soluble fraction (volume × solubility) *before* converting. The 0.08% shift is small but at 3 sf it changes the answer — which is the point of asking.

### (b) Classifying cystine formation — circle one
**L1 · Answer** **(iii) Oxidation.**
**L2 · Thought** 2 R–SH → R–S–S–R + 2 H: sulfur loses hydrogen (and electron density) — the formation of a disulfide from thiols is the textbook biological oxidation, even though no oxygen appears in the equation.

### (c) Predominant forms of thioglycolic acid
**L1 · Answer** i) pH 0: **HSCH₂COOH** (fully protonated); ii) pH 7: **HSCH₂COO⁻** (mono-anion, carboxyl deprotonated, thiol intact); iii) pH 14: **⁻SCH₂COO⁻** (di-anion).
**L2 · Thought** Assign the pKₐ values first: carboxylic acids ionise near 3–4 (pKₐ 3.67 = COOH), thiols near 10 (pKₐ 10.31 = SH); then place each pH on the ladder (below both, between, above both).

### (d) Mono- vs di-anion at pH 9.0
**L1 · Answer** [di]/[mono] = 10^(pH − pKₐ₂) = 10^(9.0 − 10.31) = 0.049 ⇒ **mono-anion 95.3%, di-anion 4.7%**.
**L2 · Thought** Only the second ionisation is active at pH 9 (the first is >99.9% complete — honour the "only two species" assumption by checking it): the Henderson ratio gives 0.049, and the percentages are 1/1.049 and 0.049/1.049 — don't forget to normalise.

### (e) Overall reaction
**L1 · Answer** **Ker–S–S–Ker + 2 RS–H → R–S–S–R + 2 Ker–S–H** (Step 1 + Step 2, cancelling Ker–S–S–R).
**L2 · Thought** The intermediate (the mixed disulfide Ker–S–S–R) must cancel — add the steps and strike it; then audit sulfur (4 each side) and the thiol count.

### (f) Which line for [Ker–S–S-Ker] vs time
**L1 · Answer** **Line C** — the curve that falls steeply at first and decays asymptotically toward zero (exponential decay).
**L2 · Thought** Constant [RSH]₀ turns the second-order law into pseudo-first-order: −d[Ker]/dt = k[RSH]₀[Ker], whose solution is a pure exponential to zero — identify the line by that *shape* (integrated-form signature, §7.8): steep initial fall, asymptotic approach to zero; the linear and plateau curves are excluded by shape, and the exponential is line C.

### (g) Rate constant from the tensile-stress graph
**L1 · Answer** For the 0.16 mol dm⁻³ series (●), −ln(F/F₀) is linear in t with slope = k[RSH]₀: measured slope ≈ (0.24 − 0.00)/60 min ≈ 3.9 × 10⁻³ min⁻¹ ⇒ k = 3.9 × 10⁻³/0.16 = **≈ 0.024 dm³ mol⁻¹ min⁻¹** (≈ 4.0 × 10⁻⁴ dm³ mol⁻¹ s⁻¹).
**L2 · Thought** The axes are already linearised (−ln(F/F₀) vs t), so the job is: calibrate axes, take the slope of the *straight-line region*, then divide by [RSH]₀ — the units come from k = slope/[RSH]₀ (min⁻¹ ÷ mol dm⁻³ = dm³ mol⁻¹ min⁻¹), and forgetting that division leaves a pseudo-first-order constant instead of the second-order k requested.

### (h) Mass of ammonium thioglycolate in one bottle
**L1 · Answer** Same pH ⇒ same k, so [RSH](Olympiad)/0.16 = slope(×)/slope(●) = 0.0121/0.0039 ≈ 3.1 ⇒ [thioglycolate] ≈ **0.50 mol dm⁻³**; mass = 0.50 × 0.500 × M(NH₄⁺ ⁻SCH₂COOH, 109.15) = **≈ 27 g** (27.3 g).
**L2 · Thought** The bottle's concentration is hidden in the *second* dataset — a hidden-calibration problem (§4): at fixed pH the pseudo-first-order slope is proportional to [RSH]₀, so the ratio of slopes is the ratio of concentrations (no absolute rate fitting needed). The salt is the mono-anion form at pH 9 (cf. (d)): ammonium thioglycolate = NH₄SCH₂COOH, M = 109.15.

---

## Question 3 — Chemistry general knowledge

### (a) Order of discovery
**L1 · Answer** **S (known since antiquity) → P (1669) → O (1774) → Ar (1894) → Pu (1940)**.
**L2 · Thought** Anchor the endpoints: sulfur is ancient, plutonium synthetic (Manhattan era); the middle three fall into place by the history of air/gases (P from urine, O₂ from Priestley/Scheele, Ar from Rayleigh's nitrogen-density anomaly).

### (b) Boiling-point ranking
**L1 · Answer** 1 **C₄H₁₀** (−0.5 °C) < 2 **CH₃CHO** (20 °C) < 3 **C₂H₅OC₂H₅** (34.5 °C) < 4 **C₂H₅OH** (78 °C) < 5 **H₂O** (100 °C) < 6 **HOCH₂CH₂OH** (197 °C).
**L2 · Thought** Rank by intermolecular forces, not mass: butane (nothing) < aldehyde (dipole) < ether (dipole, but no H-bond donation) < ethanol (one OH) < water (two H-bond sites per H) < glycol (two OH groups). The classic trap is putting the ether below the aldehyde "because ethers are inert" — mass and dipole decide, and the ether is both heavier and more polarisable.

### (c) Formulas
**L1 · Answer** (i) fool's gold = **FeS₂** (iron pyrites); (ii) Epsom salts = **MgSO₄·7H₂O**; (iii) laughing gas = **N₂O**.
**L2 · Thought** Stock knowledge; note Epsom salt is the *heptahydrate* — the water of crystallisation is part of the name.

### (d) Systematic names
**L1 · Answer** (i) acetone = **propanone**; (ii) toluene = **methylbenzene**; (iii) sodium hypochlorite = **sodium chlorate(I)**.
**L2 · Thought** For (iii) the oxidation-state nomenclature is what is being tested: Cl is +1 in OCl⁻, hence chlorate(I) — not "chlorite" (that is ClO₂⁻, chlorate(III)).

### (e) Zinc oxide on heating
**L1 · Answer** **White when cold → yellow when hot** (reverting to white on cooling).
**L2 · Thought** A reversible thermochromic shift (oxygen loss on heating narrows the band gap) — "turns yellow when hot, white when cold" is the phrasing the mark scheme wants; an irreversible answer misses the point.

### (f) Tea chemistry
**L1 · Answer** i) **C** (caffeine — the trimethylxanthine); ii) **E** (paracetamol, 4-hydroxyacetanilide); iii) **B** (sucrose); iv) **A** (aspartame — the Asp–Phe methyl ester dipeptide); v) **D** (paraquat — the 1,1′-dimethyl-4,4′-bipyridinium dichloride, a lethal herbicide).
**L2 · Thought** Identify each structure by its skeleton first (xanthine ring = caffeine; two bipyridinium N⁺ with chlorides = paraquat; dipeptide methyl ester = aspartame; para-OH acetanilide = paracetamol; the two linked pyranose/furanose rings = sucrose) — the "never add to tea" slot then has only one possible tenant.

---

## Question 4 — The synthesis of Lipitor® (atorvastatin)

**IR table (completed):** ~3300 (broad) = **O–H**; **~1775** = C=O in a small ring (lactone); 2250–2275 = **C≡N**; **~3350–3380 (sharp)** = N–H; 1700–1740 = **C=O (ester/ketone/acid)**.

### (a) Compounds B–G
**L1 · Answer** (all machine-validated)
- **B = HOCH₂–CH(OH)–CH₂–C≡N** — `N#CCC(O)CO` (C₄H₇NO₂): CN⁻ does SN₂ on the primary chloride (3300 = OH; 2270 = nitrile).
- **C = HOCH₂–CH(OH)–CH₂–COOH** (3,4-dihydroxybutanoic acid) — `O=C(O)CC(O)CO` (**C₄H₈O₄ ✓**): acid hydrolysis of the nitrile (1710 = acid C=O).
- **D = 4-hydroxyoxolan-2-one** (the γ-lactone) — `O=C1CC(O)CO1` (C₄H₆O₃ ✓ = C − H₂O): the terminal CH₂OH closes onto the COOH (1775 = strained small-ring lactone C=O; the remaining CH(OH) keeps the 3300 band).
- **E = 4-bromo-3-hydroxybutanoic acid**, BrCH₂–CH(OH)–CH₂–COOH — `O=C(O)CC(O)CBr` (**C₄H₇BrO₃ ✓ = D + HBr**): HBr opens the lactone, installing Br on the terminal carbon (1720 = acid C=O returns).
- **F = ethyl 4-bromo-3-hydroxybutanoate** — `CCOC(=O)CC(O)CBr` (**C₆H₁₁BrO₃ ✓ = E + C₂H₆ − H₂O**): Fischer esterification (1736 = ester).
- **G = ethyl 4-cyano-3-hydroxybutanoate**, NC–CH₂–CH(OH)–CH₂–CO₂Et — `CCOC(=O)CC(O)CC#N` (**C₇H₁₁NO₃ ✓ = F + CN⁻ − Br⁻**, i.e. + NaCN − NaBr as species): second SN₂ with cyanide (2254 nitrile + 1736 ester).
**L2 · Thought** Read the scheme as functional-group bookkeeping against the IR boxes: the 2270/2254 bands mark where the nitrile *is* (B, G), 1775 is the lactone alarm (only D), and the 1710→1720→1736 walk is acid → acid → ester. Note the same NaCN does two different jobs: extending the chain by one carbon in A → B, and replacing Br in F → G — both primary SN₂.

### (b) Anion I
**L1 · Answer** **⁻CH₂–C(=O)–OR** (the ester enolate of H, CH₃CO₂R — negative charge on the α-carbon, resonance onto the carbonyl oxygen).
**L2 · Thought** Only the α-protons of the ester are acidic enough for "strong base"; the resulting carbon nucleophile is the classic Claisen acylation partner used next.

### (c) Compounds J, K and L
**L1 · Answer**
- **J = the β-keto ester** RO₂C–CH₂–C(=O)–CH₂–CH(OH)–CH₂–CN (**C₇H₈NO₄R ✓ = G + CH₂CO₂R − OC₂H₅**): Claisen acylation of I by G's ester (new 1716 ketone band appears alongside 1734 ester and 2253 nitrile).
- **K = the 3,5-diol** RO₂C–CH₂–CH(OH)–CH₂–CH(OH)–CH₂–CN (**C₇H₁₀NO₄R ✓ = J + 2 H**): NaBH₄ reduces only the ketone (1716 vanishes from the IR — the discriminating observation).
- **L = the acetonide**: the 1,3-diol of K protected with 2,2-dimethoxypropane as a six-membered CMe₂-dioxane ring (IR loses the 3300 OH band entirely — only 2253 and 1728 remain ✓).
**L2 · Thought** Formula arithmetic does the identification: J = G + C₂H₂O₂R − C₂H₅O⁻ (a Claisen, not an alkylation — the ethoxide leaves from G's *ester* carbonyl); K = J + H₂ exactly; L = K + C₃H₆O − 2 CH₃OH (the acetonide exchange). The 1,3-diol → acetonide → later hydrolysis pattern is the standard way of hiding a syn-diol (the statin side chain) while the nitrile is homologated at the other end.

### (d) Phenylamine and 4-fluorobenzaldehyde
**L1 · Answer** Phenylamine = **C₆H₅NH₂ (aniline)** — `Nc1ccccc1`; 4-fluorobenzaldehyde = **4-F–C₆H₄–CHO** — `O=Cc1ccc(F)cc1`.
**L2 · Thought** Trivial in isolation, but they are the sources of two Lipitor substituents — aniline's N becomes the amide of the 3-(phenylcarbamoyl) group, and the fluorobenzaldehyde's carbonyl becomes the C2-(4-fluorophenyl) of the pyrrole; knowing where atoms end up keeps (e) honest.

### (e) O, anion P, Q and S
**L1 · Answer**
- **O = 4-methyl-3-oxo-N-phenylpentanamide**, PhNH–CO–CH₂–C(=O)–CH(CH₃)₂ — `O=C(CC(=O)C(C)C)Nc1ccccc1` (**C₁₂H₁₅NO₂ ✓ = N + PhNH₂ − CH₃OH**): aniline aminolyses N's *methyl ester* (not the ketone).
- **P = the central enolate** PhNH–CO–**CH⁻**–C(=O)–CH(CH₃)₂ (deprotonation of the doubly activated CH₂ between the two carbonyls).
- **Q = the aldol adduct** PhNH–CO–CH(CO–iPr)–CH(OH)–Ph (P adds to benzaldehyde's carbonyl; weak acid protonates the alkoxide).
- **S = the enone** PhNH–CO–C(CO–iPr)=CH–Ph — `O=C(Nc1ccccc1)C(=Cc1ccccc1)C(=O)C(C)C` (C₁₉H₁₉NO₂ ✓ = Q − H₂O): dehydration to the conjugated alkene, which is exactly the Michael acceptor needed for the Stetter step.
**L2 · Thought** The given formula of O is the arbitration point: N + PhNH₂ − H₂O would be C₁₃H₁₇NO₂ (enamine) but O is C₁₂H₁₅NO₂ — one carbon and one oxygen short, which only ester-aminolysis (−CH₃OH) explains (determinable-combination logic: let the formula, not habit, choose between "amine + ketone" and "amine + ester"). S + 4-fluorobenzaldehyde + catalyst → T is then recognisably a **Stetter reaction** (umpolung 1,4-addition of the aldehyde acyl anion equivalent onto the enone), delivering the 1,4-dicarbonyl T = PhNHCO–CH(CO–iPr)–CH(Ph)–C(=O)–C₆H₄F-4 (C₂₆H₂₄FNO₃ ✓) — the exact Paal–Knorr precursor.

### (f) Compound U
**L1 · Answer** **U = the Paal–Knorr pyrrole**: M's primary amine condenses with both ketones of T (−2 H₂O) to give the N-substituted pyrrole: N1–CH₂CH₂–CH(acetonide)–CH₂–CH(acetonide)–CH₂–CO₂R on the statin side chain, with pyrrole substituents 2-(4-fluorophenyl), 3-phenyl, 4-[(phenylamino)carbonyl], 5-isopropyl (**C₃₆H₃₉FN₂O₅R ✓ = T + M − 2 H₂O**). Acidic hydrolysis then opens the acetonide (→ the β,δ-diol) and the ester (→ the carboxylic acid), giving Lipitor.
**L2 · Thought** The target structure arbitrates the mapping (§4 downstream-structure arbitration): atorvastatin's pyrrole carries N-side chain, 2-ArF, 3-Ph, 4-CONHPh, 5-iPr — and T's 1,4-dicarbonyl provides precisely the carbonyl pair that becomes C2/C5 and the two CH carbons that become C3/C4. The formula check C₂₆H₂₄FNO₃ + C₁₀H₁₉NO₄R − 2 H₂O = C₃₆H₃₉FN₂O₅R matches the printed formula of U exactly, so the Paal–Knorr reading is verified, not guessed.

---

## Question 5 — The world's smallest powered car

### (a) Combustion analysis of nano-car (C₁₃₂H₁₂₀N₂)
**L1 · Answer**
- i) **C₁₃₂H₁₂₀N₂ + 162 O₂ → 132 CO₂ + 60 H₂O + N₂** (audit: C 132, H 120, N 2, O 324 both sides ✓).
- ii) M = 132 × 12.01 + 120 × 1.008 + 2 × 14.01 = 1734.30 g mol⁻¹ ⇒ **C 91.41%, H 6.97%, N 1.62%**.
**L2 · Thought** Balance N₂ first (it is the small term), then C and H; the oxygen coefficient is computed last (and must come out integral — 162 is the self-check). For a hydrocarbon-dominated molecule the percentages must sum to ~100 with C in the low 90s — a quick order-of-magnitude check on the arithmetic.

### (b) R/S assignment of the rotor units (order: top-left, bottom-left, top-right, bottom-right)
**L1 · Answer** Reading solid wedge = CH₃ out of the page (toward the viewer) and calibrating against the pre-assigned top-left rotor (rotor order TL, BL, TR, BR; wedge state → configuration):
- **A**: TL solid, BL solid, TR solid, BR solid → **R, S, S, R**
- **B**: TL solid, BL hashed, TR hashed, BR solid → **R, R, R, R**
- **C**: TL hashed, BL hashed, TR hashed, BR hashed → **S, R, R, S**
- **D**: TL solid, BL hashed, TR solid, BR hashed → **R, R, S, S**
- **E**: TL solid, BL solid, TR hashed, BR hashed → **R, S, R, S**
- **F**: TL hashed, BL solid, TR solid, BR hashed → **S, S, S, S**
**L2 · Thought** The rule is a proper-rotation mapping, read from the given anchor: rotors on the **right** half are the left rotors turned 180° about the vertical in-plane axis (wheel stays up, chassis now points left), which **inverts** the wedge meaning (right side: solid = S, hashed = R); rotors at the **bottom** are turned 180° about the car's long axis (wheel flips down, wedge inverts: bottom: solid = S, hashed = R); bottom-right gets both inversions and reads like top-left. The single most common error is to read all four wedges with one rule — the whole question is whether you rotate the reference into each rotor's own orientation before judging.

### (c) Which cars are optical isomers
**L1 · Answer** **B and F** (the complete answer — (R,R,R,R) ↔ (S,S,S,S), a genuine pair of distinct chiral compounds).
**L2 · Thought** The configurations give two *surface* mirror pairs — A/C and B/F — but "optical isomers" must be *different compounds*: part (d) shows A and C interconvert freely once off the surface (same molecule!), so they are not a pair of isomers at all — listing them costs a mark (the scheme: "B and F" = 2 marks; "B and F; A and C" = 1 mark). D and E are not optical isomers either: each is superimposable on its own mirror image under a 180° rotation about the surface normal (§5.5 meso check, verified rotation-by-rotation). The order of operations matters: test *superposability first* (surface rotation), then *identity off-surface* (d), before calling anything a pair of enantiomers — mirror image ≠ different compound is the double trap this part plants.

### (d) Cars that are the same molecule when free from the surface
**L1 · Answer** **A, C and E** are all the same molecule.
**L2 · Thought** Free from the surface, two proper rotations become available that the surface forbids: (1) rotation about the diyne axle swaps the two right-hand rotors — A (R,S,S,R) → (R,S,R,S) = E; (2) tumbling the whole molecule 180° about its long axis (wheels-up is fine in solution) swaps the two halves — A (R,S,S,R) → (S,R,R,S) = C. R/S labels are invariant under proper rotations, so these are *identities*, not isomerisations. Hence the surface enantiomer pair "A/C" of part (c) dissolves: they are one compound, and only B/F survive (c) as a true enantiomeric pair. This is also the mechanical consistency check of (e): the directional mover E and the stationary A are the same free molecule — motion is a *surface-bound* property, exactly the Nature paper's point.

### (e) Motion of each car on copper
**L1 · Answer**
- **A: stationary** — left pair drive one way, right pair the opposite way (collinear forces cancel exactly).
- **B: spins (clockwise, viewing the car from above with its front pointing forwards)** — top pair drive +x, bottom pair −x: no net force, but a net torque.
- **C: stationary** (mirror of A's cancellation).
- **D: stationary** — drives cancel in pairs (TL/BR vs BL/TR).
- **E: moves forwards** — with (R,S,R,S), a top R-wheel and a bottom S-wheel drive the *same* direction (+x), as do a top S and bottom R… reading the configuration: top rotors R drive one way, bottom rotors S drive the *same* way — **all four wheels propel the car in one direction**.
- **F: spins (anti-clockwise, same viewpoint: from above, front forwards)** — the mirror of B's rotation.
**L2 · Thought** The mechanics reduces to one sign rule, derived once from the rolling/paddlewheel geometry with the preamble's "R turns anti-clockwise viewed from outside": for the **top** rotors an R-wheel propels the car one way (call it +x) and an S-wheel the reverse (−x); for the **bottom** rotors the same labels drive the *opposite* direction (the wheel's contact blade is approached from the other side). Forward translation needs all four pushes aligned — only E achieves it (the meso pattern, exactly the isomer the Nature paper reports as the directional mover); all-R/all-S give zero net force but maximal torque (the observed spinning forms), and everything else cancels pairwise. Work the rule out once, tabulate the four forces per car, and the table fills itself.

---

*End of Paper 14 (2012). Next: 2011 Round 1.*


---

# Paper 15 — 2011 UKChO Round 1 (43rd IChO selection)

**Marks / time:** 5 questions with mark allocations shown per part (2 h).
**Theme map:** Q1 snack-food analysis (calorimetry + Mohr titration); Q2 calcium carbide; Q3 explosives (oxygen balance); Q4 C₄H₁₀O spectroscopy puzzle; Q5 phenobarbital synthesis.

---

## Question 1 — A popular snack food

### (a) Dietary calories per bag
**L1 · Answer** Q = mcΔT = 500 × 4.18 × 20.9 = 43.7 kJ per 2.0 g ⇒ per 22 g bag: × 11 = 480.5 kJ ⇒ × 0.239 = **≈ 115 dietary calories (115 Cal)**.
**L2 · Thought** Two scale-ups, kept separate: mass basis (2.0 g → 22 g) first, then the energy-unit conversion (kJ → Cal). The calorimeter water mass (500 g) is the only heat sink counted — the stem gives no calorimeter constant, so adding one would be inventing data.

### (b) Formulas
**L1 · Answer** (i) silver nitrate(V) = **AgNO₃**; (ii) potassium chromate(VI) = **K₂CrO₄**.
**L2 · Thought** The Roman numerals fix the anion charges: nitrate(V) = NO₃⁻ (N +5), chromate(VI) = CrO₄²⁻ (Cr +6) — hence two K⁺.

### (c) Titration equation and NaCl mass
**L1 · Answer** **Ag⁺(aq) + Cl⁻(aq) → AgCl(s)**; n(Ag⁺) = 8.20 × 10⁻³ × 0.100 = 8.20 × 10⁻⁴ mol = n(Cl⁻) in 25.0 cm³ ⇒ × 10 (250 cm³ flask) = 8.20 × 10⁻³ mol ⇒ mass NaCl = 8.20 × 10⁻³ × 58.44 = **0.479 g (≈ 0.48 g)**.
**L2 · Thought** Mohr titration: 1 : 1 stoichiometry (the chromate indicator only signals the end point — it appears nowhere in the stoichiometry). The aliquot factor (×10) is applied to the *moles*, after the titration calculation, not before.

### (d) Skeletal structure of citric acid
**L1 · Answer** **HOOC–CH₂–C(OH)(COOH)–CH₂–COOH** — a central carbon bearing –OH, –COOH, and two –CH₂–COOH arms (2-hydroxypropane-1,2,3-tricarboxylic acid) — `O=C(O)CC(O)(C(=O)O)CC(=O)O` (C₆H₈O₇ ✓).
**L2 · Thought** Parse the name from the parent outwards: propane with carboxyls at 1, 2, 3 and a hydroxyl at 2 — the central carbon is C2 of the propane chain.

### (e) Chiral centres in citric acid
**L1 · Answer** **None (0)**.
**L2 · Thought** The central carbon's four substituents are –OH, –COOH, –CH₂COOH, –CH₂COOH — two are identical, so it fails the "four different groups" test. The structural symmetry of the molecule (a mirror through the central carbon) is the deeper reason, and the check takes one line.

---

## Question 2 — Calcium carbide

### (a) Dot-cross diagram of C₂²⁻
**L1 · Answer** **[∶C≡C∶]²⁻** — a triple bond (three shared pairs, e.g. crosses from one C, dots from the other) plus one lone pair on each carbon; 14 electrons total, with the 2− charge.
**L2 · Thought** Ten bonding electrons are needed to give each carbon an octet: 3 shared pairs + 1 lone pair each — the acetylide is the nitrogen molecule's charged twin.

### (b) Diatomic gases isoelectronic with C₂²⁻
**L1 · Answer** **N₂ and CO** (both 14-electron diatomics, like C₂²⁻: 2 × 6 + 2 = 14).
**L2 · Thought** Isoelectronic counting uses total electrons including the charge; "well-known diatomic gases" then selects N₂ and CO from the 14-electron family (CN⁻ would also qualify but is not a neutral gas).

### (c) Formation of calcium carbide
**L1 · Answer** **CaO + 3 C → CaC₂ + CO** (A = CO: toxic, a reducing agent ✓; audit: Ca 1, O 1, C 3 both sides ✓).
**L2 · Thought** The side-product constraints (toxic gas, reducing agent) identify CO before any balancing is needed; the carbon is both oxidised (to CO) and reduced (to C₂²⁻) — a disproportionation of coke, which is why 3 carbons are needed per CaO.

### (d) Formula of hydrocarbon C
**L1 · Answer** (i) C : H = 92.3/12.01 : 7.7/1.008 = 7.69 : 7.64 ≈ 1 : 1 ⇒ empirical **CH**; (ii) M = 26 ⇒ **C₂H₂** (ethyne/acetylene).
**L2 · Thought** The percentage gives the ratio, the molar mass the multiplier — present both steps explicitly because the empirical formula (CH) alone cannot answer (ii).

### (e) Carbide plus water
**L1 · Answer** **CaC₂ + 2 H₂O → C₂H₂↑ + Ca(OH)₂** (the white solid is Ca(OH)₂ — slightly soluble, alkaline ✓).
**L2 · Thought** Metathesis: the C₂²⁻ dianion is simply protonated twice; no redox (carbon stays at −1). The slight solubility/alkalinity of the residue is the consistency check on Ca(OH)₂ rather than CaO.

### (f) Phosphate impurity with coke
**L1 · Answer** **Ca₃(PO₄)₂ + 8 C → Ca₃P₂ + 8 CO** (B = calcium phosphide, Ca₃P₂ ✓ "simple ionic compound of calcium and phosphorus"; audit: Ca 3, P 2, O 8, C 8 ✓).
**L2 · Thought** B is fixed by its description (only Ca and P, ionic ⇒ Ca²⁺ with P³⁻ ⇒ Ca₃P₂); then the phosphate's eight oxygens must leave as 8 CO (A, identified in (c)) — the balancing is read off, not solved.

### (g) The unpleasant odour
**L1 · Answer** **PH₃ (phosphine)**: Ca₃P₂ + 6 H₂O → 3 Ca(OH)₂ + 2 PH₃↑.
**L2 · Thought** Water protonates the phosphide exactly as it protonates carbide in (e) — same metathesis logic. (Technical phosphine carries P₂H₄ traces, which is why the smell is associated with spontaneous flaring, but PH₃ is the molecule asked for.)

---

## Question 3 — Explosives

### (a) Condition on d
**L1 · Answer** For CaHbNcOd → a CO₂ + ½b H₂O + ½c N₂, oxygen balance requires **d = 2a + b/2**.
**L2 · Thought** Only the oxygen count is restrictive (C and H have fixed sinks, N goes to N₂ regardless): count oxygens needed on the right (2a + b/2) and equate.

### (b) General oxygen-balance expression
**L1 · Answer** **OB = [d − (2a + b/2)] × 16.00 / M(CaHbNcOd) × 100%**, where M = 12.01a + 1.008b + 14.01c + 16.00d.
**L2 · Thought** Translate the definition literally: surplus oxygen atoms (actual minus required) → mass of oxygen → as a percentage of the explosive's molar mass; the sign comes for free from the bracket.

### (c) Oxygen balance of RDX
**L1 · Answer** RDX = C₃H₆N₆O₆ (M = 222.12): required d = 2 × 3 + 6/2 = 9, actual 6 ⇒ OB = (6 − 9) × 16.00/222.12 × 100 = **−21.6%**.
**L2 · Thought** First get the formula from the structure (three CH₂ groups on a triazine ring, each N bearing one NO₂: C₃H₆N₆O₆) — most of the marks are in counting atoms correctly from the drawing; the arithmetic is then one line. A negative balance (oxygen-poor) is typical of powerful explosives.

### (d) Equation for the explosion of TNT
**L1 · Answer** Applying the given rules to C₇H₅N₃O₆ (6 oxygens → 6 CO + 1 C; N → 3/2 N₂; ⅓ of the CO disproportionates: 2 CO → C + CO₂; ⅙ of the CO: 1 CO + H₂ → C + H₂O):
**2 C₇H₅N₃O₆ → 6 CO + 2 CO₂ + 6 C + 2 H₂O + 3 H₂ + 3 N₂**
(audit: C 14 = 6 + 2 + 6 ✓, H 10 = 4 + 6 ✓, N 6 ✓, O 12 = 6 + 4 + 2 ✓).
**L2 · Thought** Apply the rules in the printed order and treat each as an atom-conserving micro-step: the ⅓ rule is the *disproportionation* 2 CO → C + CO₂ (per two CO, not per one — writing "2 CO₂ + 2 C" for 2 CO breaks the carbon count, as a quick audit shows); the ⅙ rule consumes one CO and one H₂ per six original CO. Double the final equation to clear the fractions and audit all four elements.

### (e) Mass of TNT per 1.0 dm³ of gas at RTP
**L1 · Answer** Gaseous products (water is liquid at RTP, excluded): per 2 TNT: 6 CO + 2 CO₂ + 3 H₂ + 3 N₂ = 14 mol ⇒ 7 mol gas per mol TNT. n(gas) = 1.0/24 = 0.0417 mol ⇒ n(TNT) = 0.0417/7 = 5.95 × 10⁻³ mol ⇒ mass = 5.95 × 10⁻³ × 227.14 = **1.35 g**.
**L2 · Thought** Two judgement calls to state, not hide: water at RTP is condensed, so it does not count toward the gas volume; and the gas total comes from the balanced equation in (d), not from any generic rule. (If the examiner's convention counted steam as gaseous, 8 mol per TNT would give 1.18 g — the equation tells you exactly where the difference arises.)

---

## Question 4 — The C₄H₁₀O spectroscopy puzzle

**L1 · Answer** (C₄H₁₀O has DBE = 0 — only alcohols and ethers are possible)
- **1 = butan-1-ol** — `CCCCO` (primary unbranched alcohol; the remaining primary alcohol after 3 is assigned).
- **2 = butan-2-ol** — `CCC(C)O` (the only C₄H₁₀O isomer with a stereocentre — C2 bears H, OH, CH₃, C₂H₅ — hence optical isomers ✓).
- **3 = 2-methylpropan-1-ol** — `CC(C)CO`: its ¹H spectrum has exactly 4 environments with intensity ratio 2 : 1 : 1 : 6 (OCH₂ : OH : CH : 2 × CH₃) ✓.
- **4 = 2-methylpropan-2-ol** — `CC(C)(C)O`: only two ¹H signals (9 H methyls + 1 H OH) and a 3300 cm⁻¹ O–H band ✓.
- **5 = ethoxyethane (diethyl ether)** — `CCOCC`: two ¹H signals, triplet 3 H at 1.21 (CH₃) coupled to quartet 2 H at 3.47 (OCH₂) ✓ — the 3 : 2 intensities and mutual 3-bond coupling fix the ethyl group, and two signals total fix the symmetric ether.
- **6 = 1-methoxypropane (methyl propyl ether)** — `CCCOC`: four distinct carbons (OCH₃, OCH₂, CH₂, CH₃) ⇒ four ¹³C signals ✓.
- **7 = 2-methoxypropane (methyl isopropyl ether)** — `CC(C)OC`: three carbon environments (OCH₃, CH, 2 × equivalent CH₃) ⇒ three ¹³C signals ✓.
**L2 · Thought** Prune in order of decisiveness (§5.3): the chirality clue singles out 2 instantly (only one C₄H₁₀O isomer is chiral); the 3300 cm⁻¹ band splits the seven into alcohols (1–4) and ethers (5–7); the NMR intensity *ratios* are environment counts, not coupling counts — 2 : 1 : 1 : 6 demands a 6-proton environment (an isopropyl pair) plus a CH₂OH, which is 3 and nothing else; within the ethers, the two-signal spectrum with triplet/quartet is the symmetric one (5), and the ¹³C counts distinguish the two unsymmetrical methyl ethers (4 signals = straight propyl chain; 3 = isopropyl with its mirror pair).

---

## Question 5 — The synthesis of phenobarbital

### (a) Molecular formula of A
**L1 · Answer**
- C: n(CO₂) = 0.178/44.01 = 4.05 × 10⁻³ mol ⇒ 0.0486 g C;
- H: n(H₂O) = 0.146/18.02 ⇒ n(H) = 1.62 × 10⁻² mol ⇒ 0.0163 g H;
- N: n(NH₃) = n(HCl) = 40.8 × 10⁻³ × 0.200 = 8.16 × 10⁻³ mol ⇒ 0.114 g N;
- O by difference: 0.250 − 0.0486 − 0.0163 − 0.114 = 0.0708 g ⇒ n(O) = 4.42 × 10⁻³ mol.
Ratio C : H : N : O = 4.05 : 16.2 : 8.16 : 4.42 (×10⁻³) ≈ 1 : 4 : 2 : 1 ⇒ CH₄N₂O (M = 60 ✓ matches the mass spectrum) ⇒ **A = CH₄N₂O, urea, CO(NH₂)₂** — `NC(N)=O` (a known urinary metabolite ✓).
**L2 · Thought** The three elements are measured by three different channels (gravimetric CO₂, gravimetric H₂O, Kjeldahl-type alkalimetric N) — total them and take oxygen by difference (§4 multi-component balance): the clean 1 : 4 : 2 : 1 ratio is the self-check, and M = 60 confirms the empirical formula is the molecular one. The barbiturate context independently demands a one-carbon, two-nitrogen donor, which only urea satisfies.

### (b) Structures of A–G
**L1 · Answer** (all machine-validated)
- **A = urea**, CO(NH₂)₂ (from (a)).
- **B = benzyl bromide**, PhCH₂Br — `BrCc1ccccc1` (**C₇H₇Br ✓**): NBS brominates the benzylic methyl of toluene radically.
- **C = phenylacetic acid**, PhCH₂COOH — `O=C(O)Cc1ccccc1` (**C₈H₈O₂ ✓**): Grignard formation, carboxylation with CO₂, acidic work-up (the chain grows by one carbon).
- **D = phenylacetyl chloride**, PhCH₂COCl — `O=C(Cl)Cc1ccccc1` (**C₈H₇ClO ✓**): SOCl₂.
- **E = ethyl phenylacetate**, PhCH₂CO₂Et — `CCOC(=O)Cc1ccccc1` (**C₁₀H₁₂O₂ ✓ = D + EtOH − HCl**).
- **F = diethyl 2-phenylpropanedioate (diethyl phenylmalonate)**, PhCH(CO₂Et)₂ — `CCOC(=O)C(C(=O)OCC)c1ccccc1` (**C₁₃H₁₆O₄ ✓**): NaOEt forms E's α-enolate, which is C-acylated by diethyl carbonate (−EtOH), installing the second ester.
- **G = diethyl 2-ethyl-2-phenylpropanedioate**, PhC(Et)(CO₂Et)₂ — `CCOC(=O)C(CC)(C(=O)OCC)c1ccccc1` (**C₁₅H₂₀O₄ ✓ = F + C₂H₄**): NaOEt deprotonates the remaining α-H and EtBr alkylates it — the quaternary C5 of the barbiturate is now complete.
- Phenobarbital: G + urea + NaOEt → double condensation (−2 EtOH) closing the pyrimidine-2,4,6-trione ring: **5-ethyl-5-phenylbarbituric acid** — `CCC1(c2ccccc2)C(=O)NC(=O)NC1=O` (C₁₂H₁₂N₂O₃ ✓; atom audit: C₁₅H₂₀O₄ + CH₄N₂O − C₁₂H₁₂N₂O₃ = 2 × C₂H₆O ✓).
**L2 · Thought** Every formula printed in the scheme is honoured: the carbon count grows +1 (B → C, the CO₂ step), +3 (E → F, a carbonate acylation — C₁₀H₁₂O₂ + C₅H₁₀O₃ − C₂H₆O = C₁₃H₁₆O₄, which is why the reagent must be diethyl *carbonate*, not oxalate), and +2 (F → G, the ethylation). The barbiturate ring itself is just bookkeeping: two nitrogens of urea against two ester carbonyls, two ethanols out — the classic malonate–urea (barbiturate) condensation.

---

*End of Paper 15 (2011). Next: 2010 Round 1.*


---

# Paper 16 — 2010 UKChO Round 1 (42nd IChO selection)

**Marks / time:** 6 questions (2 h).
**Theme map:** Q1 Ambrox synthesis from drimenol; Q2 copper complex analysis (IChO 2009 practical); Q3 halogen fluorides; Q4 road salting (chemical potential, freezing-point depression); Q5 osmium dihydroxylation stereochemistry; Q6 gold leaf / FCC unit cell.

---

## Question 1 — Ambrox from (−)-drimenol

### (a) Moles of Ambrox per year
**L1 · Answer** M(Ambrox, C₁₆H₂₈O) = 236.38 g mol⁻¹; n = 10⁷/236.38 = **4.23 × 10⁴ mol per year**.
**L2 · Thought** Ten tonnes = 10⁷ g — write the unit conversion once (t → kg → g), then the mole chain is one line.

### (b) Structures of A–D
**L1 · Answer** (all machine-validated on the drimane skeleton: fused 6,6-bicyclic frame with angular junction CH₃, CH₂OH-bearing ring carbon adjacent to the junction, ring C=C carrying a vinyl methyl, and a gem-dimethyl pair on the other ring)
- **A = drimenyl mesylate** — `CC12C(COS(C)(=O)=O)C(C)=CCC1CCC(C)(C)C2` (**C₁₆H₂₈O₃S ✓**): the –CH₂OH is converted to –CH₂–O–SO₂CH₃ by CH₃SO₂Cl/pyridine (a better leaving group; stereochemistry untouched at carbon).
- **B = drimenyl–CH₂–C≡N** — `CC12C(CC#N)C(C)=CCC1CCC(C)(C)C2` (**C₁₆H₂₅N ✓ = skeleton + CH₂CN, no O**): KCN displaces the mesylate (SN₂ on the primary carbon, chain extended by one carbon).
- **C = drimenyl–CH₂–COOH** — `CC12C(CC(=O)O)C(C)=CCC1CCC(C)(C)C2` (**C₁₆H₂₆O₂ ✓**): nitrile hydrolysis.
- **D = the diol** (arm –CH₂–CH₂OH plus a tertiary ring –OH on the carbon bearing the vinyl methyl — positions as drawn in the scheme; if the figure shows a different relative placement, the figure rules) — `CC12C(CCO)C(C)(O)CCC1CCC(C)(C)C2` (**C₁₆H₃₀O₂ ✓**): LiAlH₄ opens the γ-lactone formed in the 75% pTsOH step.
(The unlettered intermediate after C, 75%: the **γ-lactone** — the pendant COOH adds across the ring C=C (Markovnikov: O onto the vinyl-methyl-bearing, more substituted carbon) closing a five-membered lactone; pTsOH then dehydrates D's two –OH groups into the tetrahydrofuran ring of **Ambrox**, C₁₆H₂₈O = D − H₂O ✓, `CC12C(CCO3)C3(C)CCC1CCC(C)(C)C2`, rings 5,6,6 ✓.)
**L2 · Thought** The formula trail is the map: C₁₅H₂₆O → C₁₆H₂₈O₃S (+CH₂O₂S, a mesylate, not a tosylate — count the single carbon) → C₁₆H₂₅N (no oxygen left: substitution, not addition) → C₁₆H₂₆O₂ (hydrolysed nitrile) → C₁₆H₃₀O₂ (a diol — lactone cleaved, not the lactone itself). The lactone intermediate is read off the reagent and the Ambrox target: Ambrox's 5-membered O-ring with O and CH₃ on the same carbon demands that the C=C hydration/cyclisation put oxygen on the *vinyl-methyl* carbon (Markovnikov) — the whole sequence is terminal-alkyne-style homologation (OH → CN → COOH) followed by intramolecular capture of the ring alkene.

### (c) Yield and scale-up
**L1 · Answer**
- (i) 0.90 × 0.60 × 0.84 × 0.75 × 0.86 × 0.85 = **24.9%**.
- (ii) n(drimenol) = 4.23 × 10⁴/0.2487 = 1.70 × 10⁵ mol; M(C₁₅H₂₆O) = 222.36 ⇒ mass = **3.78 × 10⁷ g ≈ 38 tonnes**.
- (iii) bark = 37.8/0.005 = **7.6 × 10³ tonnes (≈ 7 600 t)**.
**L2 · Thought** One mole of drimenol maps to one mole of Ambrox (the only carbon added is the nitrile carbon, retained throughout), so the mole ratio is 1 : 1 and the yield divides the *moles*, not the masses — the molar-mass conversion happens once, at the end. Part (iii) is the punchline of natural-product feedstocks: 7 600 tonnes of bark for 10 tonnes of product.

---

## Question 2 — Analysis of a copper-containing complex

### (a) % copper
**L1 · Answer** n(EDTA) = 21.70 × 10⁻³ × 0.02000 = 4.340 × 10⁻⁴ mol = n(Cu) in 0.1000 g ⇒ m(Cu) = 4.340 × 10⁻⁴ × 63.55 = 0.02758 g ⇒ **27.58%**.
**L2 · Thought** Cu–EDTA is 1 : 1 as printed; the murexide indicator plays no stoichiometric role.

### (b) Chloride titration
**L1 · Answer** (i) **Ag⁺(aq) + Cl⁻(aq) → AgCl(s)**; (ii) n(Ag⁺) = 21.70 × 10⁻³ × 0.1000 = 2.170 × 10⁻³ mol = n(Cl) in 0.2000 g ⇒ m(Cl) = 2.170 × 10⁻³ × 35.45 = 0.07693 g ⇒ **38.46%**.
**L2 · Thought** Same aliquot discipline as ever: the volume coincidence (21.70 cm³ twice) is a deliberate red herring — the concentrations differ by 5×, so the mole counts differ by 5×.

### (c) Element ratio and the formula of the anion
**L1 · Answer**
- (i) **Oxygen** (found by difference: it accumulates every other element's error — 100 − (27.58 + 38.46 + 20.87 + 5.17 + 5.96) = 1.96%).
- (ii) Mole ratios (per 100 g): Cu 0.434 : Cl 1.085 : C 1.738 : H 5.129 : N 0.425 → ÷ 0.434 → **Cu : Cl : C : H : N = 1 : 2.5 : 4 : 12 : 1** (i.e. 4 : 10 : 16 : 48 : 4).
- (iii) C₄H₁₂N per Cu is exactly one tetramethylammonium ion per Cu; scaling to integers gives (NMe₄)₄Cu₄Cl₁₀, and charge neutrality then *requires* the ignored element: 4(+1) + 4(+2) − 10(−1) = +2, so one O²⁻ completes it: anion = **[Cu₄OCl₁₀]⁴⁻**; X = (NMe₄)₄[Cu₄OCl₁₀] (check: Cu 27.59%, Cl 38.48%, C 20.86%, H 5.25%, N 6.08% — all match).
**L2 · Thought** The 2.5 (not 2 or 3) is the fingerprint of a cluster: it forces scaling by 2, after which the C : H : N = 4 : 12 : 1 pattern identifies the counter-ion per copper. The decisive move is using charge neutrality to *recover* the element you set aside (§4 determinable-combination): the oxide ion is found by the charge audit, and the full percentage check then confirms the whole formula, including the 1.96% oxygen by difference. (The [Cu₄OCl₁₀]⁴⁻ cluster is real — a tetrahedral Cu₄O core with ten terminal/bridging chlorides.)

---

## Question 3 — Halogen fluorides

### (a) Uranium + ClF₃
**L1 · Answer** **U + 3 ClF₃ → UF₆ + 3 ClF** (F audit: 9 = 6 + 3 ✓; Cl 3 ✓).
**L2 · Thought** Count fluorine first: UF₆ needs six, each ClF (stated side-product) keeps one — 3 ClF₃ supply exactly nine.

### (b) Atoms oxidised in 2 AgCl + 2 ClF₃ → 2 AgF₂ + Cl₂ + 2 ClF — circle
**L1 · Answer** **Ag (in AgCl: +1 → +2) and Cl (in AgCl: −1 → 0 in Cl₂)**; the ClF₃ chlorine is reduced (+3 → +2 in ClF and 0? no — only to ClF and the balance) — the oxidised species are Ag and the AgCl chloride.
**L2 · Thought** Assign oxidation numbers species by species: AgF₂ contains Ag(II) (unusual but real — this is why ClF₃ is feared); Cl₂(0) can only come from Cl(−1) being oxidised. The ClF₃'s own chlorine goes +3 → +2 (ClF), i.e. it is the oxidiser.

### (c) Disproportionation of IF, IF₃, IF₅
**L1 · Answer**
- (i) **3 IF → I₂ + IF₃**; **5 IF₃ → I₂ + 3 IF₅**; **7 IF₅ → I₂ + 5 IF₇** (the rule: I₂ plus the *next*-higher fluoride — IF(+1) → IF₃, IF₃ → IF₅, IF₅ → IF₇).
- (ii) ΔrH°: for 3 IF → I₂ + IF₃: ΔfH(IF₃) − 3ΔfH(IF) = −486 − 3(−95.4) = **−199.8 kJ mol⁻¹**; for 5 IF₃ → I₂ + 3 IF₅: 3ΔfH(IF₅) − 5ΔfH(IF₃) = 3(−843) − 5(−486) = **−99 kJ mol⁻¹**; for 7 IF₅ → I₂ + 5 IF₇: 5ΔfH(IF₇) − 7ΔfH(IF₅) = 5(−962.5) − 7(−843) = **+1088.5 kJ mol⁻¹**.
- (iii) **IF₅** is the one that does not disproportionate (ΔrH° > 0).
**L2 · Thought** The stated rule fixes the products — "the next-highest fluoride" means the *next* one (IF → IF₃, not a jump to IF₅); the balancing is I-then-F and the atom audit closes each line. The enthalpy sign audit: climbing from +1/+3 towards +5 releases energy (both −199.8 and −99 kJ), but from +5 to +7 the balance flips positive (+1088.5) — the single endothermic case is the answer to (iii), and the three enthalpies are computed with the same products-minus-reactants sign convention throughout (write the convention once, then all three lines).

---

## Question 4 — Salting roads in winter

### (a) The chemical-potential sketch
**L1 · Answer** (i) **A (steepest) = gas; B = liquid; C (shallowest) = solid** — the slope is −S, and S(gas) ≫ S(liquid) > S(solid). (ii) The two exactly known temperatures: **273 K (0 °C)** where the solid and liquid lines cross, and **373 K (100 °C)** where liquid and gas cross (standard pressure).
**L2 · Thought** dμ/dT = −S is the only theory needed; the steeper the entropy, the faster μ falls. The crossings are the phase transitions, which is why the two temperatures are "known exactly."

### (b) Effect of the salt
**L1 · Answer** (i) The solution line lies **below the pure-liquid line** (RT ln x_w < 0 since x_w < 1), roughly parallel to it, crossing the solid line at a *lower* temperature and the gas line at a *higher* temperature; (ii) boiling point: **higher than water**.
**L2 · Thought** Lowering the liquid's μ moves both intersections outward along the liquid line: freezing down, boiling up — the two effects are one phenomenon, which is why the sketch must be drawn before the numbers.

### (c) Water concentration and ion mole fraction
**L1 · Answer** (i) 1000 g dm⁻³/18.02 = **55.5 mol dm⁻³**; (ii) per dm³: 3.00 Na⁺ + 3.00 Cl⁻ = 6.00 mol ions; x_i = 6.00/(55.5 + 6.00) = **0.0976**.
**L2 · Thought** The trap is counting NaCl as one particle — the formula given counts anions + cations separately (6, not 3); the denominator includes everything.

### (d) Freezing point of 3.00 M NaCl and the solubility limit
**L1 · Answer** (i) ΔT = x_i R T_m²/Δ_mH = 0.0976 × 8.314 × 273²/6010 = **10.1 K ⇒ freezing point ≈ −10.1 °C**; (ii) x_i = 21.1/103.1 = 0.205 ⇒ 2c/(55.5 + 2c) = 0.205 ⇒ 2c = 0.205(55.5 + 2c) ⇒ 1.59c = 11.38 ⇒ **c ≈ 7.16 mol dm⁻³** (the practical limit of the method).
**L2 · Thought** Evaluate the constant R T_m²/Δ_mH once (103 K) and reuse it — the whole question is then proportional reasoning on x_i. Part (ii) inverts the same relation and then the same mole-fraction definition; solving 2c/(55.5 + 2c) = x_i for c (not assuming c ≪ 55.5) is the algebraic discipline being tested.

### (e) 3.00 M CaCl₂ with bound water
**L1 · Answer** per dm³: ions = 3 Ca²⁺ + 6 Cl⁻ = 9 mol; bound water = 3 × 9 = 27 mol; free water = 55.5 − 27 = 28.5 mol; x_i = 9/(28.5 + 9) = 0.240 ⇒ ΔT = 0.240 × 103.1 = **24.7 K ⇒ freezing point ≈ −24.7 °C**.
**L2 · Thought** Two adjustments stack: CaCl₂ gives 3 ions per formula unit (not 2), and the coordination shell removes 27 of the 55.5 mol of water from the denominator — miss either and the answer collapses to the NaCl value. The physical reading: binding water is *why* CaCl₂ works at Siberian temperatures where NaCl fails.

---

## Question 5 — Osmium in organic reactions

### (a) Oxidation numbers
**L1 · Answer** i) OsO₂: **+4**; ii) OsO₄: **+8**; iii) OsO₄²⁻: **+6**.
**L2 · Thought** Oxygen is −2 throughout; the charge on the ion enters the sum for (iii).

### (b) Classify alkene → vicinal diol — circle one
**L1 · Answer** **Oxidation.**
**L2 · Thought** Each alkene carbon gains a C–O bond (its oxidation level rises) with no C–H change — addition of two oxygens across a π-bond is an oxidation even though no O₂ appears.

### (c) Which osmium species catalyses it
**L1 · Answer** **OsO₄** (the +8 species).
**L2 · Thought** If the substrate is oxidised, the metal must be *reduced* in the cycle, so the active form starts at the top of the oxidation ladder (+8) and descends to +6 in the osmate ester — the classification in (b) dictates the choice in (c), not memory.

### (d) Oxidation number in the cyclic species
**L1 · Answer** **+6** (the cyclic osmate ester: Os(VI)).
**L2 · Thought** Adding the alkene across two Os=O bonds transfers electron density from the π-bond to the metal (Os +8 → +6) — the same 2-electron reduction that oxidises the alkene; the electron count must close between (b) and (d).

### (e) The four stereoisomers of pentane-2,3-diol — required alkenes
**L1 · Answer** Syn addition pins alkene geometry to relative configuration:
- **i) (2R,3R)** ← **(E)-pent-2-ene**, osmate attack on one specified face;
- **ii) (2S,3R)** ← **(Z)-pent-2-ene**, one face;
- **iii) (2R,3S)** ← **(Z)-pent-2-ene**, the other face;
- **iv) (2S,3S)** ← **(E)-pent-2-ene**, the other face.
**L2 · Thought** Syn dihydroxylation is stereospecific: the (E)-alkene can only give the threo/(R,R)+(S,S) pair and the (Z)-alkene only the erythro/(R,S)+(S,R) pair; the two faces of one alkene give the two enantiomers. The one-line justification to write is the mapping rule, then each drawing is read off.

### (f) Hexane-3,4-diol
**L1 · Answer** (i) **3** (circle 3): (3R,4R), (3S,4S), and the meso form (3R,4S). (ii) (3R,4R) and (3S,4S) come from the two faces of **(E)-hex-3-ene**; the meso form comes from **(Z)-hex-3-ene** (either face gives the same achiral diol).
**L2 · Thought** The 2ⁿ budget with meso correction (§5.5): the molecule is constitutionally symmetric (CH₃CH₂ at both ends), so the (3R,4S) form has an internal mirror — count 3, not 4. Note the complement to (e): there the ends differ, so all four are distinct.

### (g) The sixteen cyclic-ether stereoisomers
**L1 · Answer** **Stereoisomers 5, 8, 9 and 12 can be formed** (using the paper's numbering of the sixteen structures).
**L2 · Thought** Treat the two double bonds as independent stereochemical modules: syn addition on the first fixes the *relative* configuration of its pair (the carbinol –OH and the adjacent ring –O must end up on the **same face**: both-out or both-in — 2 options), and syn on the second likewise (2 options) — 2 × 2 = 4 survivors out of the 2⁴ = 16 drawings. The survivors are 5, 8, 9 and 12 — exactly the four "both pairs syn-consistent" combinations. The working is a per-structure face audit (read each wedge/hash at the four centres and test both pairs independently), not a guess at "which look right" — the modular stereo-constraint filtering of §5.5 applied to a reaction-outcome filter; and since the mark scheme deducts half a mark per extra number, report exactly the four.

---

## Question 6 — Gold leaf

### (a) Mass of one gold atom
**L1 · Answer** m = 197/6.02 × 10²³ = **3.27 × 10⁻²² g**.
**L2 · Thought** One isotope only, so the relative mass is the molar mass per mole; divide by Nₐ.

### (b) Atoms in the unit cell
**L1 · Answer** 8 corners × ⅛ + 6 face-centres × ½ = **4 atoms** (FCC).
**L2 · Thought** Share counting (§7.4): corners ⅛, faces ½ — the face-centred result 4 is the check on every later step.

### (c) Cell dimensions in terms of r
**L1 · Answer** i) face diagonal = 4r = a√2 ⇒ **a = 2√2 r**; ii) **V = a³ = 16√2 r³**; iii) body diagonal = a√3 = **2√6 r**.
**L2 · Thought** Contact is along the *face* diagonal in FCC (not the edge, not the body diagonal) — picture the corner atom touching the face-centre atom; the body diagonal enters only through Pythagoras in (iii).

### (d) Molar volume
**L1 · Answer** V_m = 197/19.3 = **10.2 cm³ mol⁻¹**.
**L2 · Thought** Density divides molar mass directly; keep 3 sf to feed (f).

### (e) Packing fraction
**L1 · Answer** occupied = 4 × (4π/3)r³; fraction = (16π/3)r³/(16√2 r³) = **π/(3√2) = 0.740 (74.0%)**.
**L2 · Thought** The radius cancels — the packing fraction of FCC is geometry alone; deriving it (rather than quoting 74%) is the point of the question.

### (f) Radius of a gold atom
**L1 · Answer** V_cell = 4 × (197/19.3)/6.02 × 10²³ = 6.78 × 10⁻²³ cm³ ⇒ a = (6.78 × 10⁻²³)⅓ = 4.08 × 10⁻⁸ cm ⇒ r = a/(2√2) = **1.44 × 10⁻⁸ cm (144 pm)**.
**L2 · Thought** Chain: molar volume → cell volume (÷ Nₐ, × 4 atoms) → edge (cube root) → radius (÷ 2√2). The 144 pm result is the order-of-magnitude self-check (metallic radii are 1–2 × 10⁻⁸ cm).

### (g) The Dome of the Rock
**L1 · Answer**
- i) V(Au) = 80 000/19.3 = 4145 cm³; A(hemisphere) = 2πr² = 2π × (1050)² = 6.93 × 10⁶ cm² ⇒ thickness = V/A = **6.0 × 10⁻⁴ cm (≈ 6 μm)**.
- ii) layer thickness = (2√6 r)/3 = 2.35 × 10⁻⁸ cm ⇒ layers = 6.0 × 10⁻⁴/2.35 × 10⁻⁸ = **≈ 2.5 × 10⁴ layers (25 000)**.
**L2 · Thought** Hemisphere, not sphere: use 2πr² (the curved surface only — the diameter 21 m gives r = 10.5 m, and converting to cm before dividing is the unit discipline). The 80 kg spread over ~700 m² to 6 μm is the whole reason gold leaf exists as a technology; the layer count converts macroscopic thinness back into the atomic scale of parts (c)–(f).

---

*End of Paper 16 (2010). Next: 2009 Round 1.*


---

# Paper 17 — 2009 UKChO Round 1 (41st IChO selection)

**Marks / time:** 6 questions (2 h).
**Theme map:** Q1 nitrogen-rich firework fuels; Q2 CO₂ from patio heaters and the Olympic flame; Q3 matches (P₄S₃/KClO₃) and ³¹P NMR of phosphorus sulfides; Q4 loperamide synthesis; Q5 arsenic (Marsh test, adsorption kinetics); Q6 XRF of the hidden van Gogh.

---

## Question 1 — Environmentally friendly fireworks

### (a) Dihydrazinotetrazine
**L1 · Answer**
- i) The tetrazine ring is a planar, fully conjugated 6-π-electron system (Hückel 4n + 2 with n = 1) — **aromatic** — with the hydrazine N–H lone pairs delocalised into the ring; aromatic delocalisation is what tames a molecule that is 80% nitrogen.
- ii) **4 signals**: ring nitrogens fall into two symmetry-related pairs (N1 ≡ N4, N2 ≡ N5 under the mirror through C3–C6), plus the hydrazine –NH– (linker) and the terminal –NH₂ — 2 + 2 = 4 environments.
- iii) C₂H₆N₈ + 3½ O₂ → **2 CO₂ + 3 H₂O + 4 N₂** (×2 for integers: 2 C₂H₆N₈ + 7 O₂ → 4 CO₂ + 6 H₂O + 8 N₂; audit: C 4, H 12, N 16, O 14 ✓).
**L2 · Thought** (i) asks for the bonding reason, so "stable because strong bonds" earns nothing — the answer must name aromatic delocalisation in the ring (the same stabilisation that makes benzene tame). For (ii), orbit the ring nitrogens under the molecule's mirror before counting (§7.3) — the formula C₂H₆N₈ (counted: ring C₂N₄ + 2 × NHNH₂) then feeds (iii), where "two other substances" besides N₂ are identified as CO₂ and H₂O before any balancing.

### (b) Octanitrocubane
**L1 · Answer** i) cubane C–C–C = 90°, alkane C–C–C = 109.5° ⇒ **19.5° smaller**; ii) **C₈N₈O₁₆ → 8 CO₂ + 4 N₂** (audit: C 8, N 8, O 16 ✓ — the molecule carries exactly its own oxidant).
**L2 · Thought** The cube forces 90° angles (the strain quoted in the stem); the self-oxidation check is an atom audit showing the 16 nitro-oxygens exactly oxidise the 8 carbons — that is the whole selling point of a zero-oxygen-balance explosive (cf. 2011 Q3).

### (c) Nitrocellulose
**L1 · Answer** Empirical formula **C₆H₇N₃O₁₁** (glucose unit C₆H₁₀O₅ with three –OH nitrated: + 3 HNO₃ − 3 H₂O). Combustion (oxygen balance is negative — the molecule's 11 O's leave 4.5 O per formula unit to be supplied externally, i.e. 2.25 O₂): **2 C₆H₇N₃O₁₁ + 4.5 O₂ → 12 CO₂ + 7 H₂O + 3 N₂**, or in integers **4 C₆H₇N₃O₁₁ + 9 O₂ → 24 CO₂ + 14 H₂O + 6 N₂** (audit: C 24, H 28, N 12, O: 44 + 18 = 62 = 48 + 14 ✓).
**L2 · Thought** Count the three –ONO₂ groups off the drawn repeat unit first (two on the ring, one on the exocyclic –CH₂–), then build the formula by difference from cellulose. The O₂ coefficient is taken last from the oxygen count — per 2 mol of nitrocellulose only **4.5 mol O₂** are needed (writing 9 O₂ against 2 mol is the audit-catching slip: 2 × 11 + 18 = 40 on the left vs 31 on the right fails immediately). This is the same equation as 2025 Q1(d) — worth noticing when the same molecule returns twenty years later.

---

## Question 2 — The unnecessary production of carbon dioxide

### (a) The patio heater
**L1 · Answer**
- i) n = 13 000/44.10 = **295 mol** (294.8).
- ii) n(CO₂) = 3 × 294.8 = 884 mol ⇒ mass = 884 × 44.01 = **38.9 kg**.
- iii) Q = 294.8 × 2220 = **6.54 × 10⁵ kJ** (654 MJ).
- iv) rate = 15 kJ s⁻¹/2220 kJ mol⁻¹ = 6.76 × 10⁻³ mol s⁻¹ × 24 dm³ mol⁻¹ = **0.162 dm³ s⁻¹ ≈ 162 cm³ s⁻¹**.
- v) **≈ 9.5 atm (140 psi) — essentially unchanged**: the cylinder holds liquid + vapour in equilibrium, so the pressure is the saturated vapour pressure of propane at that temperature, which does not depend on how much liquid remains (until the liquid runs out).
**L2 · Thought** (iv) is a unit chain: kJ s⁻¹ → mol s⁻¹ → dm³ s⁻¹, one conversion per step. (v) is the conceptual mark: "half full" refers to the *amount of propane*, but while any liquid remains the vapour above it is saturated — pressure is set by temperature, not fill level. The 87% fill detail is a distractor for exactly this point (§7.5 data audit).

### (b) The odorant
**L1 · Answer**
- i) CH₃–CH₂–SH, with **two As–H... C–S–H and C–C–S angles ≈ 96°** (bent at sulfur: two bonds + two lone pairs, like H₂S — accept anything in the low-to-mid 90s° up to ~109°).
- ii) n(thiol) = 294.8 × 0.02 × 10⁻⁹ = 5.9 × 10⁻⁹ mol ⇒ mass = 5.9 × 10⁻⁹ × 62.13 = **3.7 × 10⁻⁷ g** (about a third of a microgram).
**L2 · Thought** The shape at sulfur is VSEPR with two lone pairs — the angle must come out *below* tetrahedral, not above. For (ii), "0.02 per billion" is a mole ratio — apply it to the moles of propane, not to mass, or the answer is out by ~14×.

### (c) The Olympic flame
**L1 · Answer** V(CH₄) = 6000 m³ h⁻¹ × 16 × 24 h = 2.304 × 10⁶ m³; n = 2.304 × 10⁹ dm³/24 = 9.6 × 10⁷ mol; m(CO₂) = 9.6 × 10⁷ × 44.01 = 4.2 × 10⁹ g = **4.2 × 10⁶ kg (≈ 4 200 tonnes)**.
**L2 · Thought** CH₄ + 2 O₂ → CO₂ + 2 H₂O is 1 : 1 in CO₂; the m³ → dm³ conversion (×10³) is the slip point — write the unit ladder once and the rest is a two-line calculation.

---

## Question 3 — The chemistry of matches

### (a) The match-head reaction
**L1 · Answer**
- i) **P₄S₃ + 8 O₂ → P₄O₁₀ + 3 SO₂** (audit: P 4, S 3, O 16 ✓).
- ii) **2 KClO₃ → 2 KCl + 3 O₂**.
- iii) LCM of 8 and 1.5 O₂ = 24: **3 P₄S₃ + 16 KClO₃ → 3 P₄O₁₀ + 9 SO₂ + 16 KCl** (audit: P 12, S 9, K 16, Cl 16, O 48 ✓).
- iv) mass ratio P₄S₃ : KClO₃ = 3 × 220.06 : 16 × 122.55 = 660 : 1961 = **1 : 2.97**.
- v) ΔrH° = [3(−2948) + 9(−296.8) + 16(−436.7)] − [3(−154.0) + 16(−397.7)] = −18 502 + 6 825 = **−1.17 × 10⁴ kJ** (per equation as written, i.e. per 3 mol P₄S₃).
**L2 · Thought** (iii) is where the marks leak: combine via the oxygen requirement (8 O₂ per P₄S₃; 1.5 O₂ per KClO₃), scale to integers, and audit every element — do not just add (i) and (ii) with arbitrary coefficients. For (v), say what the number refers to: "per 3 mol P₄S₃", because the stoichiometric equation is the amount basis.

### (b) ³¹P NMR peak counts
**L1 · Answer** i) P₄S₄: **3 peaks** (apical P, central P, and the mirror-paired two basal P's); ii) P₄S₅: **4 peaks** (the terminal =S on one basal phosphorus destroys the mirror — all four P environments are distinct); iii) P₄S₆: **3 peaks** ({left P}, {P=S right P}, and the automorphism pair {centre P, bottom P}: on the scheme's drawn structure the centre and bottom P's interchange under a symmetry operation — S-bridges and the P–P bond map onto each other; this equivalence is a property of that drawn connectivity — if the figure is drawn differently, its symmetry rules).
**L2 · Thought** Orbit the P atoms under each cage's automorphisms (§7.3 whole-molecule test): in P₄S₄ the mirror through the apex and the bottom S-bridge swaps the two basal P's; in P₄S₅ nothing swaps anything; in P₄S₆ the bottom and centre P's swap (their bridge partners map L→L, R→R), which is the non-obvious equivalence — checking the *partners* of each bridge, not just bond counts, is what decides it.

### (c) The one-peak isomer of P₄S₄
**L1 · Answer** A structure with all four P equivalent: the **P₄ tetrahedron with one terminal =S on each phosphorus** — each P then has three P–P bonds plus one P=S (P(V), Td-symmetric ⇒ a single ³¹P environment). (An alternating (P–S)₄ eight-membered ring with alternating single/double bonds satisfies the same constraint and would also be credited.)
**L2 · Thought** The constraint "one peak" is a symmetry specification: find a connectivity in which an automorphism cycles all four P's. The P₄ tetrahedron's full permutation symmetry does it as soon as every P carries the same substituent (one =S each) — the constraint is met by construction, and the 1-peak prediction then verifies itself.

---

## Question 4 — Loperamide (anti-diarrhoea)

### (a) Protonated atom
**L1 · Answer** The **piperidine nitrogen** (the tertiary ring amine), not the dimethylamide N.
**L2 · Thought** Basicity ranking again: the amide nitrogen's lone pair is tied up in the carbonyl, while the piperidine N is an ordinary tertiary amine — the same call as in 2015/2016 (Ritalin, flibanserin).

### (b) Ester A and anion B
**L1 · Answer**
- i) Ester A = ethyl 2,2-diphenylacetate ⇒ **diphenylacetic acid (Ph₂CH–COOH) + ethanol**.
- ii) A = **Ph₂CH–CO₂CH₂CH₃** — `CCOC(=O)C(c1ccccc1)c1ccccc1` (C₁₆H₁₆O₂ ✓); the base removes **the single α-proton** (the methine H between the two phenyls and the carbonyl) ⇒ anion B = **Ph₂C⁻–CO₂Et**.
**L2 · Thought** Ester cleavage on paper: OR' comes from the alcohol, RCO from the acid. The deprotonation site is unique — only one α-H exists (both phenyls stabilise the carbanion); there is no other candidate.

### (c) Anion C and cyclic ester D
**L1 · Answer**
- **C = Ph₂C(CO₂Et)–CH₂–CH₂–O⁻** (B opens epoxyethane by SN₂; the alkoxide is the product) — `[O-]CCC(C(=O)OCC)(c1ccccc1)c1ccccc1` (C₁₈H₁₉O₃⁻ ✓).
- **D = 3,3-diphenyloxolan-2-one** (the γ-lactone) — `O=C1OCCC1(c1ccccc1)c1ccccc1` (**C₁₆H₁₄O₂ ✓**): the alkoxide O at the end of the two-carbon arm closes back onto the ester carbonyl, expelling C₂H₅O⁻, giving the **five-membered** lactone ring (O–CH₂–CH₂–CPh₂–C(=O)–).
**L2 · Thought** Count the ring atoms before naming the lactone: the arm is –CPh₂–CH₂–CH₂–O, so closure onto the ester gives a *five*-membered γ-lactone, not a β-lactone. The atom audit confirms it: anion C (C₁₈H₁₉O₃⁻) − C₂H₅O⁻ = C₁₆H₁₄O₂ exactly, and the five-membered ring is the one that makes the chain count work — ethoxide's leaving-group ability does the rest. The audit, not memory or habit, decides ring size.

### (d) E and F
**L1 · Answer**
- **E = 4-bromo-2,2-diphenylbutanoic acid**, HOOC–CPh₂–CH₂–CH₂Br — `O=C(O)C(CCBr)(c1ccccc1)c1ccccc1` (C₁₆H₁₅BrO₂ ✓): bromide opens the β-lactone at its CH₂–O bond (SN₂), releasing the carboxylate, protonated on work-up.
- **F = the acyl chloride** BrCH₂CH₂CPh₂–COCl — `O=C(Cl)C(CCBr)(c1ccccc1)c1ccccc1` (**C₁₆H₁₄BrClO ✓ = E − OH + Cl**): SOCl₂.
**L2 · Thought** β-Lactone strain makes the CH₂–O bond the weak point; bromide opens it like an epoxide. The F formula printed in the scheme confirms the −OH → −Cl swap atom-for-atom.

### (e) The two forms of G
**L1 · Answer**
- (i) **open-chain amide**: BrCH₂CH₂CPh₂–C(=O)–N(CH₃)₂ — `CN(C)C(=O)C(CCBr)(c1ccccc1)c1ccccc1` (**C₁₈H₂₀BrNO ✓ = F + NHMe₂ − HCl**).
- (ii) **cyclic bromide salt**: the dimethylamide nitrogen attacks the terminal CH₂–Br intramolecularly, closing a five-membered ring — the **1,1-dimethyl-4,4-diphenyl-... cyclic acylammonium bromide** (a five-membered iminium lactam salt): ring N⁺(CH₃)₂–CH₂–CH₂–CPh₂–C(=O)–, bromide counter-ion — `[Br-].C[N+]1(C)CCC(c2ccccc2)(c2ccccc2)C1=O` (C₁₈H₂₀BrNO ✓). **10 ¹³C signals ✓**: the two N–CH₃ groups become inequivalent on the quaternary ring nitrogen (4 Ph signals + 2 CH₂ + CPh₂ + C=O + 2 × NMe = 10), whereas the open-chain amide shows 9 (equivalent NMe₂ and equivalent phenyls).
**L2 · Thought** The ¹³C count is the arbiter between the two forms: in the open chain the two N-methyls and the two phenyls are pairwise equivalent (9 environments); cyclisation makes the N⁺ stereogenic-in-context (two different ring paths), splitting the NMe signal — exactly the stated 10. Count it both ways before choosing; the given number then selects, it does not merely decorate.

---

## Question 5 — Arsenic

### (a) Arsine
**L1 · Answer**
- i) **Trigonal pyramidal** (like NH₃), H–As–H ≈ 92° (lone pair + three bonds).
- ii) In the Marsh test the mirror forms by **oxygen-starved combustion**: **4 AsH₃ + 3 O₂ → 4 As + 6 H₂O** (enough O₂ to burn the hydrogen but not the arsenic; audit: As 4, H 12, O 6 ✓). In excess air the arsenic itself would oxidise further (As₂O₃) — the deposit of the *element* is the signature of oxygen deficit.
**L2 · Thought** The product named in the stem (a deposit of *arsenic*) decides the stoichiometric regime: supply exactly the oxygen that the hydrogen can consume (3 O₂ per 4 AsH₃), leaving elemental As — writing either free pyrolysis (2 AsH₃ → 2 As + 3 H₂, no O₂ at all) or full combustion (→ As₂O₃) misreads "limited air": the first ignores the flame, the second contradicts the observed mirror. Balance by allocating O₂ to hydrogen first, then audit the leftover element.

### (b) Generating arsine
**L1 · Answer** i) **As₂O₃**; ii) **As₂O₃ + 6 Zn + 6 H₂SO₄ → 2 AsH₃ + 6 ZnSO₄ + 3 H₂O** (audit: As 2, Zn 6, S 6, H 12, O 27 ✓).
**L2 · Thought** As goes +3 → −3 (6 e⁻ per As, 12 total), Zn 0 → +2 (2 e⁻ each, needs 6) — the electron audit fixes the zinc coefficient and everything else follows (H₂O from the leftover H⁺/O).

### (c) HAsO₄²⁻
**L1 · Answer** i) **+5** (1 + x − 8 = −2); ii) **tetrahedral** — central As bonded to four oxygens (one protonated, the negative charge delocalised over the other three), exactly like HPO₄²⁻.
**L2 · Thought** Period-4 analogy: As sits under P, so the arsenate geometry is the phosphate geometry; draw one As–OH and three As–O⁻ with resonance noted.

### (d) Adsorption kinetics
**L1 · Answer**
- i) From the graph the concentration halves in about **8 min** (constant half-life ⇒ first order ✓; mark scheme accepts t½ = 7–9 min) ⇒ k = ln 2/8 = **0.087 min⁻¹** (accept 0.08–0.10 min⁻¹; ≈ 1.4 × 10⁻³ s⁻¹).
- ii) 10 = [A]₀ e^(−0.087 × 55) ⇒ [A]₀ = 10 × e^4.8 = **≈ 1.2 × 10³ μg dm⁻³** (mark scheme central 1400 μg dm⁻³ with k = 0.09; accepted range 800–2400 μg dm⁻³ across the k band — quote your k with the answer, ECF-style).
**L2 · Thought** First-order means the half-life is the whole measurement: read two successive halvings off the curve to confirm constancy before computing k (integrated-form signature, §7.8), and keep the reading inside the accepted 7–9 min band — it is the single point of leverage, because (ii) inherits it directly. Part (ii) is the same exponential run backwards — the safe level (10 μg dm⁻³) is the endpoint, not the start; the answer scales as e^(55k), so it is ferociously sensitive to k (that is why the scheme grades (ii) as a band, not a point).

### (e) Equilibrium adsorption
**L1 · Answer** K = [adsorbed]/[aqueous] = 186, with mass balance [aq] + [ads] = 30 ⇒ [aq] = 30/(1 + 186) = **0.16 μg dm⁻³**.
**L2 · Thought** K partitions the total arsenic 186 : 1 between surface and water; the "1 +" in the denominator is the mass balance — forgetting it and writing 30/186 = 0.161 gets the same digits by luck but for the wrong reason; write the balance explicitly.

---

## Question 6 — The hidden van Gogh (XRF)

### (a) Hydrogen levels
**L1 · Answer** i) E₁ = −R_H/1² = **−13.6 eV**; ii) the energy **tends to zero** (the continuum); iii) IE = 13.6 × 1.6022 × 10⁻¹⁹ × 6.022 × 10²³ = 1.312 × 10⁶ J mol⁻¹ = **1312 kJ mol⁻¹**.
**L2 · Thought** The negative sign is the physics (bound states below zero); ionisation means reaching zero from −13.6 eV, hence the positive 1312 kJ mol⁻¹ — sign audit at each step.

### (b) Z_eff for sodium
**L1 · Answer** 495.8 kJ mol⁻¹ = 5.14 eV atom⁻¹; valence shell n = 3: 5.14 = 13.6 × Z_eff²/3² ⇒ Z_eff = √(5.14 × 9/13.6) = **1.84**.
**L2 · Thought** Convert kJ mol⁻¹ to eV atom⁻¹ *before* using the Rydberg form (÷ 96.5); the valence electron is n = 3 (3s), not n = 1 — the result (less than Z = 11, more than 1) is the physical picture of the ten core electrons shielding imperfectly.

### (c) Element A from Kα(A) (≈ 8000 eV)
**L1 · Answer** Kα: ΔE = 13.6 × (Z − 1)² × (1 − ¼) = 10.2(Z − 1)² eV ⇒ (Z − 1)² = 8000/10.2 = 784 ⇒ Z − 1 = 28 ⇒ **Z = 29, A = Cu** (check: 10.2 × 28² = 7997 eV ✓).
**L2 · Thought** The transition factor is (1/1² − 1/2²) = ¾ — fold it into the constant (10.2 eV) once and reuse for every Kα. The near-integer Z from the square root is the assignment licence (quantum-ladder move).

### (d) Element B from Lα(B) (≈ 10 000 eV)
**L1 · Answer** Lα (3d → 2p, S = 7.4): ΔE = 13.6 × (Z − 7.4)² × (1/4 − 1/9) = 1.89(Z − 7.4)² eV ⇒ (Z − 7.4)² = 5300 ⇒ Z ≈ 80 ⇒ **B = Hg** (check: 1.89 × 72.6² = 9.96 keV ✓). ii) the red sulfide pigment at the lips = **HgS (vermilion/cinnabar)**.
**L2 · Thought** The Lα constant (13.6 × 5/36 = 1.89 eV) and its shielding (7.4) are given — the only work is the square root. (ii) then follows from "red sulfide + Hg": vermilion is the canonical red lip pigment of the period.

### (e) The 10 500 eV peak
**L1 · Answer** i) Kα: (Z − 1)² = 10 500/10.2 = 1029 ⇒ Z = **33, C = As**; Lα: (Z − 7.4)² = 10 500/1.89 = 5560 ⇒ Z = **82, D = Pb**. ii) Scheele's green with A = Cu and C = As(+3): **CuHAsO₃** (copper(II) hydrogen arsenite(III): Cu²⁺ + H⁺ + AsO₃³⁻ — charge audit 0 ✓).
**L2 · Thought** One peak, two assignments — the overlap is the point of the question (two ladders through the same energy); each ladder resolves cleanly to an integer Z. (ii) is assembled from the two identified elements plus the stated +3 arsenic: CuHAsO₃ is the only neutral (A C H Oₓ) combination with Cu²⁺ and arsenite.

### (f) Kα of antimony
**L1 · Answer** ΔE = 10.2 × (51 − 1)² = **25 500 eV (25.5 keV)** (consistent with the peak near 26 keV in the spectrum ✓).
**L2 · Thought** Same constant as (c): (Z − 1)² with Z = 51 → 2500 × 10.2 — the spectrum's own peak confirms the calibration.

### (g) Oxidation state of D in Naples yellow, D₂Sb₂O₇
**L1 · Answer** D = Pb; Sb is stated to be in its highest oxidation state (+5): 2x + 2 × 5 − 14 = 0 ⇒ **x = +2 (Pb(II))**.
**L2 · Thought** Charge neutrality with the Sb fixed by the previous sentence — a one-line audit; Pb(II) in Pb₂Sb₂O₇ (lead antimonate) is the sane result.

---

*End of Paper 17 (2009). Next: 2008 Round 1.*


---

# Paper 18 — 2008 UKChO Round 1 (40th IChO selection)

**Marks / time:** 6 questions (2 h).
**Theme map:** Q1 silicon purification (zone refining); Q2 vitamin D kinetics in mushrooms; Q3 mercury fulminate and cyanuric acid; Q4 aluminium phosphide clusters; Q5 cone-snail toxin sequencing; Q6 fexofenadine synthesis.

---

## Question 1 — Pure silicon for solar cells

### (a) Quartz + carbon
**L1 · Answer** **SiO₂ + 2 C → Si + 2 CO** (audit: Si 1, O 2, C 2 ✓). (The equally credited alternative is SiO₂ + C → Si + CO₂.)
**L2 · Thought** At furnace temperatures carbon is oxidised only to CO (the thermodynamically preferred product above ~1700 °C); both the CO and CO₂ forms are accepted answers, so the balance (2 C for CO) is what matters — writing the audit line is the mark-securing habit either way.

### (b) Silane and trichlorosilane
**L1 · Answer** i) **109.5°** (SiH₄ is tetrahedral, like CH₄); ii) **SiHCl₃ + H₂ → Si + 3 HCl** (audit: Si 1, H 4, Cl 3 ✓).
**L2 · Thought** VSEPR with four identical bonds is a one-line answer; the reduction is metathesis of Cl for H — the same H₂ appears on both sides of the process (Si + 3 HCl → SiHCl₃ + H₂ is the forward step), so the closed-cycle audit is satisfied.

### (c) The ethanol route
**L1 · Answer** i) **4 SiH(OCH₂CH₃)₃ → SiH₄ + 3 Si(OCH₂CH₃)₄** (audit: Si 4, H 28, C 24, O 12 ✓); ii) **SiH₄ + 2 O₂ → SiO₂ + 2 H₂O**.
**L2 · Thought** Disproportionation bookkeeping: silicon goes from +2 to 0 (SiH₄) and +4 (Si(OEt)₄) — one in four molecules is reduced, three oxidised, and the ethoxy groups are spectators. Silane's pyrophoricity (ii) is its total oxidation: every bond ends as Si–O or O–H.

### (d) Zone refining
**L1 · Answer**
- i) C(x) = kC₀(1 − x)^(k−1) rises monotonically in x (k < 1), so the maximum in the kept region is at x = 0.95: C = 2.00 × 10⁻³ × 3300 × (0.05)^(−0.998) = 6.6 × 19.9 = **≈ 131 ppm** (131–132 ppm at this precision; quote 131 ppm).
- ii) 10 = 8.00 × 10⁻⁶ × 1300 × (1 − x)^(−0.999992) ⇒ (1 − x)^(−0.999992) = 961.5 ⇒ 1 − x = 1.04 × 10⁻³ ⇒ **discard the last ≈ 0.104% (about 0.1%) of the bar**.
**L2 · Thought** Two different questions hide in one formula: (i) asks for the *worst point kept* (evaluate at the boundary x = 0.95 — note the concentration only grows along the bar when k < 1), (ii) asks for the *boundary position itself* (solve for 1 − x, then read the answer as the discarded tail, not the kept fraction — the exponent k − 1 ≈ −1 means the impurity piles up almost as 1/(1 − x), so a tiny tail suffices).

---

## Question 2 — Vitamin D production in mushrooms

### (a) Chiral centres of ergosterol
**L1 · Answer** **Nine**: C3 (bearing OH), the four ring-junction/ring carbons C8, C9, C10, C13, C14, C17, and the two side-chain centres C20 and C24 (the C22=C23 double bond is planar and not a centre; the C25 carbon has two identical methyls).
**L2 · Thought** Work along the skeleton once, testing each sp³ carbon for four different substituents (§5.5): ring-junction carbons are easily missed, and C25 is the designed false positive (two –CH₃).

### (b) Destination of the transferred hydrogen
**L1 · Answer** The hydrogen from the indicated (angular C19) methyl ends up on **C9** — the carbon at the former A/B-ring junction in vitamin D2 (the secosteroid's new sp³ junction below the diene system).
**L2 · Thought** The photochemistry is electrocyclic B-ring opening followed by a [1,7]-sigmatropic hydrogen shift: the H travels from the C19 methyl across the conjugated triene to C9 — identifying it is atom-tracking backwards from the product (which carbon gained an H relative to the steroid precursor).

### (c) Observed order a — circle one
**L1 · Answer** **Zero** (a = 0).
**L2 · Thought** Both graphs are *straight lines* of product vs time — a constant rate independent of how much ergosterol remains is the integrated-form signature of zero order (§7.8); the photochemistry is photon-limited, not substrate-limited.

### (d) Rate constant for oyster mushrooms
**L1 · Answer** Zero order ⇒ k = the slope: from the graph, (42 − 7) μg g⁻¹ over 40 min ⇒ **k ≈ 0.88 μg g⁻¹ min⁻¹** (0.875 with clean endpoints; units μg g⁻¹ min⁻¹, i.e. concentration per time, as zero order requires).
**L2 · Thought** The units are the second mark: for a = 0, rate = k exactly, so k carries the rate's units — stating mol dm⁻³ s⁻¹ or min⁻¹ alone would contradict the order just established. Read the slope from the line's own endpoints (§7.8: calibrate both axes first).

### (e) Vitamin D2 in 10 g of button mushrooms after 1 h
**L1 · Answer** Button line: intercept ≈ 3 μg g⁻¹, slope ≈ (14 − 3)/40 = 0.275 μg g⁻¹ min⁻¹ ⇒ at 60 min: 3 + 0.275 × 60 = 19.5 μg g⁻¹ ⇒ in 10 g: **≈ 195 μg (≈ 0.20 mg)**.
**L2 · Thought** Read the line, do not invent it: intercept plus slope × time (the line does not pass through the origin — there is pre-formed vitamin even at t = 0), then scale by the 10 g sample last.

### (f) Activation energy from k(35 °C) = 2 k(25 °C)
**L1 · Answer** ln(k₂/k₁) = (Ea/R)(1/T₁ − 1/T₂) ⇒ ln 2 = (Ea/8.314) × (1/298 − 1/308) = (Ea/8.314) × 1.089 × 10⁻⁴ ⇒ Ea = 0.693 × 8.314/1.089 × 10⁻⁴ = **≈ 53 kJ mol⁻¹ (52.9 kJ mol⁻¹)**.
**L2 · Thought** The ratio form eliminates the pre-exponential factor A — write it before substituting; kelvin conversion (298/308, not 25/35) is the only slip available.

---

## Question 3 — Mercury fulminate

### (a) Detonation equation
**L1 · Answer** **HgC₂N₂O₂ → Hg + N₂ + 2 CO** (audit: Hg 1, C 2, N 2, O 2 ✓; two gases — N₂ and CO — and two elements — Hg and N₂ ✓).
**L2 · Thought** "Two gases, two elements" is a constraint set: N₂ is both an element and a gas, mercury is the other element, and the leftover C/O can only be CO (CO₂ would leave the oxygen count unable to close with elemental products). Balance against those constraints, not by trial.

### (b) Enthalpy of detonation
**L1 · Answer** ΔrH° = [0 + 0 + 2 × (−111)] − [+386] = **−608 kJ mol⁻¹**.
**L2 · Thought** Elements (Hg, N₂) are zero by definition — say so on the page; the unused data (HgO, CO₂, NO, NO₂) are deliberate distractors (§7.5 data audit: name them as unused rather than forcing them in).

### (c) Structure of mercury(II) fulminate
**L1 · Answer** **Hg–C≡N⁺–O⁻ (two per Hg²⁺): Hg(CNO)₂ with Hg–C bonds** — each fulminate ion is ⁻C≡N⁺–O⁻ (a C≡N triple bond, formal charges −1 on C and +1 on N, single N–O bond bearing the negative end); mercury(II) bound to carbon (organometallic ✓, triple-bond IR stretch ✓).
**L2 · Thought** The constraints fix the connectivity: organometallic ⇒ Hg–C; triple-bond stretch ⇒ C≡N; a −1 triatomic with the octet satisfied gives ⁻C≡N⁺–O⁻ as the dominant Lewis form — the atom bonded to Hg is the carbanionic carbon.

### (d) Structure of mercury(II) cyanate
**L1 · Answer** **Hg–O–C≡N (two per Hg²⁺): Hg(OCN)₂** — each cyanate ion is ⁻O–C≡N (N≡C triple bond, charge on oxygen); mercury bonded through **oxygen** (not organometallic ✓, triple-bond stretch retained ✓).
**L2 · Thought** The ambident-ion logic (§4 polarity analysis): the same CNO⁻ atoms connect through the other end — fulminate binds via C, cyanate via O; "not organometallic" is the instruction to move the Hg bond from C to O while keeping the triple bond that the IR demands.

### (e) The two forms of cyanuric acid
**L1 · Answer**
- **Keto form**: a six-membered ring of alternating N–H and C=O groups (1,3,5-triazinane-2,4,6-trione: three –NH–C(=O)– repeats, fully symmetric);
- **Enol (aromatic) form**: 1,3,5-triazine-2,4,6-triol — an aromatic triazine ring (three ring C=N and three ring C–N alternating, 6 π-electrons) with an –OH on each carbon.
**L2 · Thought** "Three atoms of each element symmetrically equivalent" forces the 1,3,5-alternating ring in both cases; the two forms are the amide↔imidic-acid tautomers, and only the enol is aromatic (the keto ring is saturated in the π sense — each carbonyl is exocyclic). This is the amide–imidol tautomerism of HNCO trimerised, drawn symmetrically on purpose.

---

## Question 4 — Aluminium chemistry and rat poison

### (a) Electrons around Al in covalent AlCl₃
**L1 · Answer** **6** (three single bonds; electron-deficient, octet incomplete).
**L2 · Thought** This is the whole reason AlCl₃ dimerises and is Lewis-acidic — the electron count is the explanation, not a coincidence.

### (b) Vapour-phase molecule A (M_r = 266.66)
**L1 · Answer** i) **Al₂Cl₆** (266.66 = 2 × 133.33); ii) **Cl₂Al(μ-Cl)₂AlCl₂** — a four-membered Al–Cl–Al–Cl ring with two bridging chlorines (3-centre bonds) and two terminal Cl on each Al; iii) **8 electrons around each Al** (four bonds each).
**L2 · Thought** The molar mass doubles the empirical unit, and the dimer's structure is driven by the deficit found in (a): each Al completes its octet by accepting a lone pair from a bridging Cl — bridging, not Al–Al bonding, is the answer (watch the electron count go 6 → 8 to verify).

### (c) Hydrolysis of AlP
**L1 · Answer** **AlP + 3 H₂O → Al(OH)₃ + PH₃↑** (audit: Al 1, P 1, H 6, O 3 ✓).
**L2 · Thought** Same metathesis as CaC₂/Ca₃P₂ hydrolyses (2011 Q2): the P³⁻ anion is protonated to PH₃; no redox (P stays −3).

### (d) Electrons around Al in iBu₂AlH
**L1 · Answer** **6** (three covalent bonds: 2 × iBu + H).
**L2 · Thought** Same deficit as AlCl₃ — the molecule is a Lewis acid looking for a fourth bond, which is exactly what happens next.

### (e) Compound B (m/z max 864)
**L1 · Answer**
- i) B = **[iBu₂Al(μ-PH–SiPh₃)]₂** — a dimer with a four-membered Al–P–Al–P ring: two iBu on each Al, one SiPh₃ on each P, H retained on each bridging P (monomer unit [iBu₂Al–PH–SiPh₃] = 432; 864 = 2 × 432 ✓ — the dimerisation follows the Al₂Cl₆ guide of part (b)).
- ii) geometric isomers: **cis and trans** — the two SiPh₃ groups on the same face vs opposite faces of the Al₂P₂ ring plane (draw one with both SiPh₃ up, one with one up/one down).
**L2 · Thought** The assembly is read off the data: iBu₂AlH + Ph₃SiPH₂ → H₂ + [iBu₂Al–PH–SiPh₃] unit (Al–P bond formed, the second P–H retained for the bridge), and "use (b) as a guide" is a direct instruction to dimerise through P-bridges. The m/z ceiling fixes n = 2, and the ring's two P substituents then generate cis/trans pairs — geometric isomerism about the 4-ring is the only kind available.

### (f) Compound C
**L1 · Answer** **An Al₄P₄ cube** (cubane skeleton, alternating Al and P vertices): each Al bears one iBu, each P bears one SiPh₃ — [iBuAl(PSiPh₃)]₄, i.e. 2 B units with four iBuH (methylpropane) eliminated.
**L2 · Thought** The clues assemble uniquely: 4 Al + 4 P with *equal* iBu and Ph₃Si counts (one each per vertex), a *single* ³¹P environment (a perfect alternating cube makes all four P equivalent), and methylpropane evolution = loss of one iBu as iBuH per Al–P pair (the P–H and one Al–iBu reductively eliminate). The Al₄P₄ cube is the only structure satisfying all four constraints simultaneously — and it is the natural precursor to AlP (all Al–P bonds pre-formed).

### (g) Gas D
**L1 · Answer** **2-methylpropene (isobutene, (CH₃)₂C=CH₂)** — β-hydride elimination of the remaining isobutyl groups (while the P–SiPh₃ groups leave as Ph₃SiH).
**L2 · Thought** Thermolysis of metal alkyls without other outlets goes β-hydride elimination: iBu on Al → isobutene + Al–H, and the hydrides then collapse the cluster to AlP. Identifying D completes the atom account: C − 4 Ph₃SiH − Al₄P₄ leaves exactly 4 × C₄H₈.

---

## Question 5 — Toxins from cone snails (mass-spec sequencing)

### (a) Ile–Leu–Gly
**L1 · Answer** i) mass = (131 + 131 + 75) − 2 × 18 = **301**; ii) Ion 1 (the Ile acylium H₂N–CHR–CO⁺) = 131 − 17 = **114**; iii) Ion 2 (the Ile–Leu b₂ acylium) = 131 + 131 − 18 − 17 = **227**.
**L2 · Thought** Two mass bookkeepings, kept distinct: the *peptide* loses (n − 1) waters (one per amide bond); an *acylium fragment ion* additionally loses OH (17) from its C-terminus. The b-ion ladder used in (c) is exactly the Ion 1/Ion 2 pattern extended.

### (b) Number of unique sequences
**L1 · Answer** 9 residues with cysteine duplicated: 9!/2! = **181 440**.
**L2 · Thought** Permutations of a multiset — divide by the factorial of each repeat count (here just the two Cys); everything else is distinct.

### (c) Sequence of the first 7 amino acids
**L1 · Answer** Read the b-ion ladder (consecutive differences = residue masses):
| ion | m/z | Δ | residue |
|---|---|---|---|
| 1 | 104 | — | Cys (104 + 17 = 121) |
| 2 | 217 | 113 | 131 → Ile or Leu |
| 3 | 330 | 113 | 131 → Leu or Ile |
| 4 | 458 | 128 | 146 → Gln |
| 5 | 573 | 115 | 133 → Asp |
| 6 | 676 | 103 | 121 → Cys |
| 7 | 773 | 97 | 115 → Pro |
The ¹H NMR of residue 3 shows a single 6-H signal (two equivalent CH₃ of an isopropyl group), a 1-H and a 2-H overlapping pair, and a 1-H signal — **leucine** (–CH₂–CH(CH₃)₂), not isoleucine (which would give *two separate* 3-H methyl signals, a triplet and a doublet). ⇒ **sequence: Cys–Ile–Leu–Gln–Asp–Cys–Pro**(–Glu–Gly). (Total mass check: Σ residues − 8 × 18 = 976 ✓.)
**L2 · Thought** The b₁ ion carries the +17 offset (104 + 17 = 121), every later step is a clean residue mass — the ladder reads itself once the first rung is anchored. The composition list then arbitrates: two consecutive 131s are only possible because the mixture contains *both* Ile and Leu. The NMR is the classic Ile/Leu discriminator — count the methyl environments (one 6-H signal vs two 3-H signals), and the whole sequence clicks; the given Glu–Gly tail and the 976 total are the final audit.

---

## Question 6 — The synthesis of fexofenadine

### (a) The salt, the molar mass, and the group R
**L1 · Answer**
- i) Protonated: the **piperidine nitrogen** (the tertiary ring amine; the carboxylic acid stays as –COOH in the HCl salt).
- ii) M = 36.46 × 112.00/(120.14 − 112.00) = **501.7 g mol⁻¹** (501.66; fexofenadine = C₃₂H₃₉NO₄ ✓).
- iii) **R = phenyl (C₆H₅–)**: the tertiary alcohol at piperidine C4 is –C(OH)(C₆H₅)₂ (the hydroxydiphenylmethyl group); with R = Ph the drug's formula closes to C₃₂H₃₉NO₄, M = 501.67 ✓.
**L2 · Thought** (ii) is the same salt-balance rearrangement as 2015 Q3e (M = M_HCl × m_base/(m_salt − m_base)); (iii) then lets the molecular mass arbitrate — C₃₂H₃₉NO₄ minus the drawn skeleton leaves exactly C₁₂H₁₀ = two phenyls, so R = Ph is forced, and the Grignard steps in the scheme (RMgBr, twice) corroborate it.

### (b) Starting material X and the base's targets
**L1 · Answer** X = **benzyl cyanide (phenylacetonitrile), Ph–CH₂–C≡N** — `N#CCc1ccccc1` (C₈H₇N ✓); the base removes the **two benzylic α-hydrogens** (the CH₂ protons next to the nitrile), one in each methylation step.
**L2 · Thought** The nitrile's α-CH₂ is the only acidic C–H present (pKₐ ≈ 21) — two successive deprotonation/methylation cycles install the two methyls that become the drug's α,α-dimethyl group.

### (c) Structures of A–G
**L1 · Answer** (all machine-validated)
- **A = 2-phenylpropanenitrile**, Ph–CH(CH₃)–CN — `CC(C#N)c1ccccc1` (**C₉H₉N ✓ = X + CH₂ − H**).
- **B = 2-methyl-2-phenylpropanenitrile**, Ph–C(CH₃)₂–CN — `CC(C)(C#N)c1ccccc1` (**C₁₀H₁₁N ✓**, second α-methylation).
- **C = 4-(2-cyanopropan-2-yl)phenyl 4-chlorobutyl ketone**, p-(NC–CMe₂)–C₆H₄–CO–(CH₂)₃Cl — `CC(C)(C#N)c1ccc(C(=O)CCCCl)cc1` (**C₁₄H₁₆ClNO ✓ = B + C₄H₅ClO**): AlCl₃-catalysed Friedel–Crafts acylation *para* to the bulky cyanodimethylmethyl group.
- **D = the secondary alcohol** p-(NC–CMe₂)–C₆H₄–CH(OH)–(CH₂)₃Cl — `CC(C)(C#N)c1ccc(C(O)CCCCl)cc1` (**C₁₄H₁₈ClNO ✓ = C + 2 H**): NaBH₄ reduces only the ketone (nitrile untouched).
- **E = piperidin-4-yl phenyl ketone (4-benzoylpiperidine)** — `O=C(c1ccccc1)C1CCNCC1` (**C₆H₁₀NOR with R = Ph ✓**): one PhMgBr converts the methyl ester to the ketone (the methoxide leaves).
- **F = 4-(hydroxydiphenylmethyl)piperidine** — `OC(c1ccccc1)(c1ccccc1)C1CCNCC1` (**C₆H₁₁NOR₂ with R = Ph ✓**): the second PhMgBr adds to E's carbonyl; dilute acid work-up gives the tertiary alcohol.
- **G = D's chloride linked to F's piperidine nitrogen** — `CC(C)(C#N)c1ccc(C(O)CCCN2CCC(C(O)(c3ccccc3)c3ccccc3)CC2)cc1` (**= C₃₂H₃₈N₂O₂ with R = Ph**, i.e. D (C₁₄H₁₈ClNO) + F (C₁₈H₂₁NO) − HCl ✓): N-alkylation (SN₂) at the terminal CH₂Cl; heating with dilute acid then hydrolyses the nitrile (–CMe₂–CN → –CMe₂–COOH, −NH₃) to fexofenadine.
**L2 · Thought** The formula trail is complete at every step: methylations add CH₂ each time; acylation adds C₄H₅ClO (read the acid chloride as 4-chlorobutyryl chloride from its drawing); reduction adds H₂; the ester → ketone → tertiary alcohol sequence is the standard double-Grignard on an ester (the first RMgBr gives a ketone because the ketone is less electrophilic than the ester only in the exam's simplified frame — state the ester→ketone→alcohol ladder plainly). The drug's two halves meet in the most obvious way (amine + alkyl chloride), and the masked carboxylic acid travels the whole route as a nitrile — the same protection strategy as 2016 Q4 (isopropenyl benzimidazolone).

---

*End of Paper 18 (2008). Next: 2007 Round 1.*


---

# Paper 19 — 2007 UKChO Round 1 (39th IChO selection)

**Marks / time:** 6 questions (2 h).
**Theme map:** Q1 space-shuttle propellants; Q2 phosphorus geometry (P₄ to molybdophosphate); Q3 phosphate in the environment (molybdophosphate titration, Ksp); Q4 flame-retardant cation (THP⁺); Q5 Tamiflu synthesis (Rohloff route); Q6 chlorine dioxide.

---

## Question 1 — Launching the space shuttle

### (a) Hydrogen and oxygen
**L1 · Answer** **2 H₂ + O₂ → 2 H₂O**.
**L2 · Thought** The workhorse equation; the 1 : 8 mass ratio it implies (4 : 32) is what (b) uses.

### (b) Stoichiometric masses in the external tank
**L1 · Answer** Propellant = 745 − 27 = 718 t; H₂ : O₂ = 1 : 8 by mass ⇒ **H₂ = 718/9 = 79.8 t; O₂ = 638.2 t**.
**L2 · Thought** The "correct stoichiometric proportions" phrase licenses the 1 : 8 split — the tank's tare mass (27 t) must be subtracted *first*, not prorated.

### (c) Actual volumes and tank capacity
**L1 · Answer** V(H₂) = 104 × 10⁶ g/0.0708 = 1.469 × 10⁹ cm³ = **1469 m³**; V(O₂) = 614 × 10⁶/1.141 = 5.38 × 10⁸ cm³ = **538 m³**; total ≈ **2.01 × 10³ m³ (≈ 2007 m³)**.
**L2 · Thought** Mass → volume via density with tonnes → grams written out (×10⁶); the striking physical point is that 90% of the mass is oxygen but 73% of the *volume* is hydrogen — the tank is sized by the density extreme.

### (d) Enthalpy of the booster reaction
**L1 · Answer** ΔrH° = [4(−1675.7) + 2(−704.2) + 12(−285.8) + 0] − [0 + 6(−295.3)] = −11 540.8 + 1 771.8 = **−9769 kJ** (per equation as written, i.e. per 10 mol Al).
**L2 · Thought** Elements (Al, N₂) are zero — state it; say what the number refers to (per 10 Al), because part (e) divides by exactly that.

### (e) Energy from 450 tonnes of propellant
**L1 · Answer** n(Al) = 450 × 10⁶ × 0.16/26.98 = 2.67 × 10⁶ mol; energy = (2.67 × 10⁶/10) × 9769 = **2.6 × 10⁹ kJ (≈ 2.6 TJ)**.
**L2 · Thought** Chain: propellant → Al mass (16%) → moles → ÷ 10 (the equation's basis) → × enthalpy; the "limiting reagent" clause justifies ignoring the perchlorate in the energy count.

---

## Question 2 — Geometric shapes in chemistry

### (a)–(b) White phosphorus P₄
**L1 · Answer** (a) Four P atoms at the vertices of a regular tetrahedron, **every pair of P atoms bonded** (6 P–P bonds, 60° angles); (b) **6 edges**.
**L2 · Thought** "Each P at a vertex, bonded to the other three" — the 60° bond angle is the source of white phosphorus's strain and reactivity; the edge count (C(4,2) = 6) feeds every later atom audit in this question.

### (c) The two oxides
**L1 · Answer** i) **P₄ + 3 O₂ → P₄O₆**; ii) **P₄ + 5 O₂ → P₄O₁₀**.
**L2 · Thought** The tetrahedral cage is retained (given in (d)); the equations balance by O count with the molecular formulas named by oxidation state — P(III) gives P₄O₆, P(V) P₄O₁₀.

### (d) Phosphorus(III) oxide
**L1 · Answer** A P₄ tetrahedron with **an oxygen bridging each of the six edges** (P–O–P on every former P–P bond) — P₄O₆.
**L2 · Thought** "No longer bonded to each other, joined by bridging oxygens" is a literal instruction: insert one O into each of the 6 edges — 6 oxygens, matching the name.

### (e) Phosphorus(V) oxide
**L1 · Answer** P₄O₆ **plus one terminal oxygen on each P vertex** (each P: three bridging O + one terminal P=O) — P₄O₁₀.
**L2 · Thought** 6 bridging + 4 terminal = 10 ✓ — the terminal oxygens are what take P from +3 to +5 (each P's bond count rises from 3 to 4).

### (f)–(g) Phosphoric(V) acid
**L1 · Answer** (f) **(HO)₃P=O** — tetrahedral P with one P=O and three P–OH; (g) **P₄O₁₀ + 6 H₂O → 4 H₃PO₄** (audit: P 4, O 16, H 12 ✓).
**L2 · Thought** The acid's structure is read off the oxide's terminal oxygen (it becomes the P=O) plus hydrolysed bridges; the hydration equation balances P first, then waters.

### (h)–(k) The molybdophosphate ion
**L1 · Answer**
- (h) Mo in (NH₄)₂MoO₄: **+6**.
- (i) Cuboctahedron: **12 vertices, 24 edges**.
- (j) i) **12 Mo** (one per vertex); ii) **40 O** (24 edge-bridges + 12 vertex-terminal + 4 central phosphate O).
- (k) charge = 12 × 6 + 5 − 80 = **3−** ⇒ **[PMo₁₂O₄₀]³⁻**, so ammonium molybdophosphate = **(NH₄)₃[PMo₁₂O₄₀]**.
**L2 · Thought** The whole question is one atom-counting exercise (§7.4 share counting transposed to a polyhedron): vertices → Mo, edges → bridging O, "a further oxygen per vertex" → 12 more, and the central PO₄'s four oxygens are *additional* (not edge/vertex atoms) — the classic slip is to double-count them as vertex atoms or to forget them entirely. The charge audit in (k) then determines the ammonium count with no further information.

---

## Question 3 — Phosphate levels in our environment

### (a) Why 23 moles of NaOH per mole of precipitate — circle two
**L1 · Answer** **C** (the molybdenum-containing species is acidic) and **E** (the molybdophosphate ion contains many molybdenums).
**L2 · Thought** The stoichiometry is read off the ion's structure: [PMo₁₂O₄₀]³⁻ + 23 OH⁻ → PO₄³⁻ + 12 MoO₄²⁻ (+ water/ammonia) — each of the 12 Mo(VI) centres consumes hydroxide as it is broken down to molybdate(VI), so the *multiplicity of Mo* (E) and the *acidity of the Mo species* (C) are the two explanations; A is false (NaOH is strong), B confuses mass with moles, D is backwards (phosphate is basic).

### (b) Phosphate in the serum
**L1 · Answer** n(NaOH) = 17.25 × 10⁻³ × 0.0100 = 1.725 × 10⁻⁴ mol; n(PO₄) = 1.725 × 10⁻⁴/23 = 7.50 × 10⁻⁶ mol in 10.0 cm³ ⇒ **7.50 × 10⁻⁴ mol dm⁻³ (0.750 mmol dm⁻³)** — within the <1.8 mmol dm⁻³ safe level ✓.
**L2 · Thought** The 23 : 1 factor is stated in the stem — the only discipline is applying it to the *moles* before scaling the aliquot (10.0 cm³ → per dm³). Comparing with the safe level is the built-in conclusion line.

### (c) Prevalent phosphate form at pH 7.4
**L1 · Answer** The active equilibrium is the second (pKa₂ = 7.21): [HPO₄²⁻]/[H₂PO₄⁻] = Ka₂/[H⁺] = 6.2 × 10⁻⁸/10⁻⁷·⁴ = 1.56 ⇒ **HPO₄²⁻ predominates (≈ 61%)**.
**L2 · Thought** Pick the pKa nearest the pH (the first and third are >2 pH units away, so those species are negligible — say so); then the ratio, then normalise.

### (d) Lanthanum carbonate + stomach acid
**L1 · Answer** **La₂(CO₃)₃ + 6 HCl → 2 LaCl₃ + 3 H₂O + 3 CO₂**.
**L2 · Thought** Identical chemistry to 2014 Q1(a) — carbonate metathesis, La stays +3.

### (e) Saturated LaPO₄ concentration
**L1 · Answer** Ksp = s² ⇒ s = √(7.08 × 10⁻²⁷) = **8.4 × 10⁻¹⁴ mol dm⁻³**.
**L2 · Thought** For a 1 : 1 salt, [La³⁺] = [PO₄³⁻] = s and Ksp = s² — the 1 : 1 stoichiometry must be stated, since it is what makes the square root valid.

### (f) Which phosphate precipitates first
**L1 · Answer** **LaPO₄** (Ksp 7.08 × 10⁻²⁷ ≪ 9.84 × 10⁻²¹ for AlPO₄).
**L2 · Thought** Same 1 : 1 stoichiometry in both salts ⇒ directly comparable Ksp values: the smaller Ksp needs the lower [PO₄³⁻] to exceed its ion product, so it comes down first as phosphate is added — the comparison only works because both salts share the 1 : 1 form, which is worth one line of justification.

---

## Question 4 — The flame-retardant cation (THP⁺)

### (a) Phosphine and methanal geometries
**L1 · Answer** PH₃: **trigonal pyramidal**, H–P–H ≈ 93–94° (lone pair + 3 bonds); methanal HCHO: **trigonal planar**, H–C–H and H–C–O ≈ 120° (C=O double bond).
**L2 · Thought** VSEPR with explicit lone-pair bookkeeping: P has 3 bonds + 1 lone pair (bent like NH₃ but with a smaller angle), C has 3 σ-bonds and no lone pairs (planar).

### (b) Hydrogen environments in X⁺
**L1 · Answer** **2 environments, ratio 1 : 2 (OH : CH₂)** — i.e. 4 OH protons : 8 CH₂ protons (the mark scheme quotes 1 : 2; the same pair as 2 : 1 written the other way — state which is which either way).
**L2 · Thought** With one carbon environment (given), the four CH₂OH arms are all equivalent; the ¹H spectrum then splits only into CH₂ (~4.8 ppm) and OH (6.25 ppm) — the integration ratio 8 : 4 = 2 : 1 is the headcount.

### (c) The D₂O-labile signal at 6.25 ppm
**L1 · Answer** **–OH (hydroxyl groups)** — exchangeable protons, replaced by D (invisible in ¹H NMR).
**L2 · Thought** The D₂O test again: only O–H/N–H exchange; combined with (b), the molecule carries four equivalent CH₂OH units.

### (d) ³¹P coupling
**L1 · Answer** **8 hydrogen nuclei** (the eight CH₂ protons of the four equivalent arms ⇒ the multiplet is a nonet).
**L2 · Thought** One carbon environment ⇒ all four arms equivalent ⇒ P sees all 8 CH₂ protons identically (²JPH); the (2nI + 1) rule with I = ½ then gives 9 lines.

### (e) The mass spectrum
**L1 · Answer**
- i) The 30-unit loss = **CH₂O** (formaldehyde, 12 + 2 + 16).
- ii) X⁺ = **[P(CH₂OH)₄]⁺** (m/z = 31 + 4 × 31 = **155** ✓ the molecular ion).
- iii) In D₂O the four –OH become –OD: 155 + 4 = **m/z 159**.
**L2 · Thought** The ladder anchors itself (§7.3 fragment-ladder): 155 − 30 − 30 − 30 = 65, and each step is one formaldehyde molecule leaving an arm; the D₂O shift counts the exchangeable protons (4 × 1 = +4) — a one-number confirmation of four –OH groups.

### (f) Structures
**L1 · Answer**
- i) **[P(CH₂OH)₄]⁺** — tetrahedral P (four single P–C bonds, like PH₄⁺/NH₄⁺): tetrakis(hydroxymethyl)phosphonium, formed as PH₃ + 4 HCHO + H⁺ → [P(CH₂OH)₄]⁺.
- ii) m/z 65 = **[PH₃(CH₂OH)]⁺** (31 + 3 + 31 = 65 ✓): the phosphonium core after three CH₂O losses — protonated hydroxymethylphosphine, P still tetrahedral-ish with three P–H bonds.
**L2 · Thought** Assembly logic: 155 = 31 + 4 × 31 exactly, and 31 = CH₂OH — the ion is built from one P and four identical arms; the "acid" in the preparation supplies the H⁺ that quaternises phosphorus. For (ii), anchor on the ladder (125, 95, 65) and let the mass decide the remaining arm count — a structure like [H₃P(CH₂OH)]⁺ is what the mass, not guesswork, returns.

---

## Question 5 — The synthesis of Tamiflu (Rohloff route)

### (a) Protonated atom in the phosphate salt
**L1 · Answer** The **primary amine –NH₂ at C5** (the acetamide N is amide-like and not basic).
**L2 · Thought** Same basicity ranking as every other drug-salt question: the free aliphatic NH₂ outcompetes the amide by ~10¹⁰ in basicity.

### (b) Chiral centres and stereoisomer count
**L1 · Answer** i) **3 chiral centres**: C3 (O–pentyl), C4 (NHAc), C5 (NH₂) — the pentan-3-yloxy central CH bears two identical ethyl groups and is *not* a centre, and the two sp² alkene carbons are not either; ii) **2³ = 8** stereoisomers.
**L2 · Thought** The 2ⁿ budget with the meso check (no internal symmetry here, so all 8 are real); the –CH(CH₂CH₃)₂ carbon is the designed false positive (§5.5: two identical ethyls).

### (c) Compounds B, C, D, E, F and by-product H (quinic acid route)
**L1 · Answer**
- **B = the ethyl ester of acetonide A** (acid-catalysed esterification of the free –COOH only; the acetonide and the two remaining OH's untouched, C₁₂H₂₀O₆).
- **C = B's C5-mesylate** (MsCl on the most reactive free secondary OH: **C₁₃H₂₂O₈S ✓ = B + CH₂O₂S − H**).
- **F = the C1-chloride** (SO₂Cl₂ substitutes the tertiary C1–OH: **C₁₃H₂₁ClO₇S ✓ = C − OH + Cl**, the "left over intermediate").
- **D = the C1=C2 alkene** (base eliminates HCl from F: **major product**, because this alkene is conjugated with the ester carbonyl — the shikimic framework: C₁₃H₂₀O₇S, acetonide + 5-OMs intact).
- **E = the regioisomeric C1=C6 alkene** (elimination toward C6 instead — unconjugated, the **unwanted isomer**, same formula).
- **H = propanone (acetone, C₃H₆O ✓)**: D + pentan-3-one/H⁺ swaps the ketal (transketalisation: CMe₂ acetonide → CEt₂ ketal, G = C₁₅H₂₄O₇S ✓ = D + C₂H₄), ejecting acetone.
**L2 · Thought** The roles sort themselves by thermodynamics and downstream need: the transketalisation replaces acetone (volatile, driven off) by the heavier pentan-3-one — and the pentylidene ketal is not decoration, it is the *source of the drug's pentan-3-yloxy group* (see (f)). D vs E is settled by conjugation with the ester (the more stable alkene is wanted and is also the one that matches shikimic acid, which is how the two routes converge on the same G). Stereochemistry is inherited unchanged from quinic acid until F (SO₂Cl₂ proceeds with retention of the framework; only C1's OH is replaced), and the ketal oxygens stay behind the ring throughout.

### (d) I, J, K (shikimic acid route)
**L1 · Answer**
- **I = shikimoyl chloride** (SOCl₂ converts only the –COOH to –COCl; the three ring OH's and the C1=C2 alkene untouched).
- **J = ethyl shikimate** (I + ethanol: the ethyl ester, stereochemistry retained).
- **K = the 3,4-(pentan-3-ylidene) ketal of J** (pentan-3-one/H⁺ protects the cis 3,4-diol; the C5–OH stays free — it is the next step's target), which MsCl then converts to **G** (the C5 mesylate) — the same G as the quinic route ✓.
**L2 · Thought** The whole point of printing both routes: they converge on G, so the shikimic route's K must be D's ketal-exchanged twin — a useful cross-check on every structure drawn in (c). SOCl₂ is specified to touch the acid only (the question's "inorganic by-products not shown" covers SO₂/HCl).

### (e) The most acidic proton in L
**L1 · Answer** The **C4 hydroxyl proton** (the free secondary alcohol's O–H).
**L2 · Thought** The base's job is to make the C4 alkoxide that will close the epoxide onto the C5 mesylate — the ester α-protons are not acidic enough at this pH regime, and deprotonating the alcohol is the only step that leads anywhere productive; identifying the *role* of the base finds the proton.

### (f) M, N, O, P, Q and R
**L1 · Answer** (formulas machine-validated)
- **M = the 4,5-epoxide** — `CCOC(=O)C1=CC2OC2C(OC(CC)CC)C1` (**C₁₄H₂₂O₄ ✓ = L − CH₃SO₃H? no: L − MsOH after alkoxide formation**: the C4 alkoxide displaces the C5 mesylate intramolecularly, inverting C5 — a 3-membered ring as stated).
- **N = 5-azido-4-hydroxy ester** (main) — `CCOC(=O)C1=CC(O)C(N=[N+]=[N-])C(OC(CC)CC)C1`, and **O = the 4-azido-5-hydroxy regioisomer** (**C₁₄H₂₃N₃O₄ ✓ = M + HN₃**): azide opens the epoxide at either carbon (mix of isomers, backside attack).
- **P = the 4,5-aziridine** — `CCOC(=O)C1=CC2NC2C(OC(CC)CC)C1` (**C₁₄H₂₃NO₃ ✓ = azido-alcohol − N₂ − O**): PMe₃ converts the azide to an iminophosphorane whose nitrogen closes onto the neighbouring carbon, expelling the remaining OH's oxygen as O=PMe₃ — the *same* aziridine from either N or O, exactly as the stem says.
- **Q = 5-azido-4-amine** — `CCOC(=O)C1=CC(N)C(N=[N+]=[N-])C(OC(CC)CC)C1` (**C₁₄H₂₄N₄O₃ ✓ = P + HN₃**): azide opens the aziridine mainly at C5, putting N₃ on C5 and freeing the ring nitrogen as the C4 amine.
- **R = 4-acetamido-5-azide** — `CCOC(=O)C1=CC(NC(C)=O)C(N=[N+]=[N-])C(OC(CC)CC)C1` (**C₁₆H₂₆N₄O₄ ✓ = Q + C₂H₂O**): acylation of the C4 amine only; H₂/Ni then reduces the C5 azide to NH₂ (−N₂, +2 H) giving Tamiflu (**C₁₆H₂₈N₂O₄ ✓**).
**L2 · Thought** The nitrogen choreography is the whole endgame, and the formulas track it: azide (N₃) in, iminophosphorane/aziridine (N) around, second azide (N₃) in, acetyl on the amine, azide out as N₂ — at every letter the formula accounts for the nitrogens (N: 0→3→1→4→4→2), which is why N and O *must* converge on the same aziridine (the azide nitrogen becomes the ring nitrogen in both regioisomers). The acylation/hydrogenation order is not arbitrary: acetylating before reducing protects the C4 amine as its amide while the C5 azide is reduced to the free –NH₂ of the drug — acylate after reduction and you could not keep the two nitrogens apart. The pentan-3-yloxy group, remember, arrived in L by reductive ketal opening of G (ketal C–O cleaved to the ether at C3 + free C4–OH: G + H₂ → L, C₁₅H₂₆O₇S ✓) — the ketal was a protecting group that pays off as a structural feature.

---

## Question 6 — Chlorine dioxide

### (a) ClO₂ dot-cross diagram and angle
**L1 · Answer** ClO₂ (19 valence electrons, an odd-electron molecule): **O–Cl–O with two Cl–O bonds of order ~1.5** (a 3-electron bond shared: one σ pair plus a delocalised 3-electron π system; one lone electron and two lone pairs on Cl) — the radical sits largely on Cl; **angle ≈ 117°** (bent; between the 120° of NO₂-type sp² and 109° — accept 115–120°).
**L2 · Thought** Count the electrons first (7 + 12 = 19): an odd total forces either an expanded octet or an odd-electron bond — the honest drawing is the ~1.5-order delocalised one with the unpaired electron on chlorine, and the angle follows from sp²-plus-one-electron geometry (lone electron repels less than a pair, so the angle stays above 109° but below 120°… i.e. ~117°).

### (b) Davy's disproportionation
**L1 · Answer**
- i) ClO₂: **+4**; HClO₃: **+5**; HClO₄: **+7**.
- ii) **3 HClO₃ → 2 ClO₂ + HClO₄ + H₂O** (audit: Cl 3 = 2 + 1 ✓, H 3 ✓, O 9 = 8 + 1 ✓; chlorine: 3 × +5 → 2 × +4 + 1 × +7, electron balance −2 + 2 ✓).
- iii) HClO₄: **(HO)Cl(=O)₃** — tetrahedral Cl with one O–H; the perchlorate ion ClO₄⁻ is **tetrahedral, 109.5°**.
**L2 · Thought** The oxidation-state ladder tells you the split (the only even-numbered rungs around +5 are +4 and +7 — the products are given), and the electron audit then fixes 3:2:1. Structure of the acid: three oxo + one hydroxo on tetrahedral chlorine, like H₂SO₄ minus one OH.

### (c) NaClO₃ + SO₂ in sulfuric acid
**L1 · Answer** **2 NaClO₃ + SO₂ → 2 ClO₂ + Na₂SO₄** (audit: Cl 2, S 1, Na 2, O 6+2 = 8 = 4+4 ✓; chlorine +5 → +4, sulfur +4 → +6, 2 e⁻ each side ✓).
**L2 · Thought** Chlorine +5 → +4 (1 e⁻ each, 2 total), sulfur +4 → +6 (2 e⁻) — the electron audit pairs one SO₂ with two chlorates; the "one other product" clause forces a single sodium sulfate. (In the acidic medium NaHSO₄ is the plausible protonated form, but the printed minimal form is Na₂SO₄ with no H₂SO₄ in the equation — write the minimal form; the redox core 2 ClO₃⁻ + SO₂ → 2 ClO₂ + SO₄²⁻ is identical either way.)

### (d) NaClO₃ + oxalic acid
**L1 · Answer** **2 NaClO₃ + (COOH)₂ + H₂SO₄ → 2 ClO₂ + 2 CO₂ + Na₂SO₄ + 2 H₂O** (audit: Cl 2, C 2, Na 2, S 1, H 4, O: 6+4+4 = 14 → 4+4+4+2 = 14 ✓).
**L2 · Thought** Oxalate is oxidised to 2 CO₂ (+3 → +4, 2 e⁻ total), again reducing two Cl(+5) to Cl(+4); the CO₂ by-product is exactly the "dilution" the stem mentions — check the equation contains it before moving on.

### (e) Chlorine oxidation of sodium chlorate(III)
**L1 · Answer** i) **NaClO₂** (sodium chlorite, Cl +3); ii) **Cl₂ + 2 NaClO₂ → 2 ClO₂ + 2 NaCl** (audit: Cl 2+2 = 4 ✓ on both sides, Na 2 ✓; chlorate(III) chlorine +3 → +4, chlorine gas 0 → −1 ✓).
**L2 · Thought** This is a comproportionation in reverse (disproportionation of roles): Cl₂ is the *oxidant* here despite being the usual product of chloride oxidations — the +3 → +4 climb of the chlorite drives it; two ClO₂ per Cl₂ keeps the electron count closed.

---

*End of Paper 19 (2007). Next: 2006 Round 1.*


---

# Paper 20 — 2006 UKChO Round 1 (38th IChO selection)

**Marks / time:** 7 questions (2 h).
**Theme map:** Q1 sherbet lemons (sucrose, tartaric/citric acid stereochemistry); Q2 vehicle-exhaust redox; Q3 acyl chlorides; Q4 CuSO₄ thermogravimetry; Q5 emergency oxygen; Q6 sildenafil synthesis; Q7 haloalkane MS/NMR.

---

## Question 1 — Sherbet lemons

### (a)–(c) Sucrose combustion and daily calories
**L1 · Answer**
- (a) **C₁₂H₂₂O₁₁ + 12 O₂ → 12 CO₂ + 11 H₂O** (audit: C 12, H 22, O 35 ✓).
- (b) n = 6.70/342.30 = 0.0196 mol ⇒ Q = 0.0196 × 5644 = **110 kJ (110.5)**.
- (c) 2500 Cal = 2500/0.239 = 10 460 kJ; 10 460/110.5 = **≈ 95 sweets**.
**L2 · Thought** Standard chain: mass → moles → molar enthalpy → energy; then unit-convert (kJ → Cal) before dividing. The absurd answer (95 sweets) is the health-warning punchline — sanity checks can be qualitative as well as numerical.

### (d) Tartaric acid and NaHCO₃ for 6.00 cm³ of CO₂
**L1 · Answer** n(CO₂) = 6.00 × 10⁻³/24.0 = 2.50 × 10⁻⁴ mol; tartaric acid is *diprotic* (2 CO₂ per molecule): n(acid) = 1.25 × 10⁻⁴ mol ⇒ **m(tartaric acid) = 1.25 × 10⁻⁴ × 150.09 = 18.8 mg**; n(NaHCO₃) = 2.50 × 10⁻⁴ mol ⇒ **m(NaHCO₃) = 2.50 × 10⁻⁴ × 84.01 = 21.0 mg**.
**L2 · Thought** The stoichiometric heart of the question is "two –COOH groups, two CO₂" — the acid count is halved, not the bicarbonate's. Minimum masses mean complete reaction of both, so the equation (2 NaHCO₃ + H₂ tart → 2 CO₂ + 2 H₂O + Na₂ tart) should be written, even though not requested.

### (e) Stereoisomers of tartaric acid
**L1 · Answer** **Three**: (2R,3R) and (2S,3S) — an **enantiomeric pair** — and the **meso form (2R,3S)**, which is superimposable on its own mirror image (internal mirror plane through the C2–C3 midpoint) and is *not* an enantiomer of itself or of the pair (it is a diastereomer of them).
**L2 · Thought** The 2ⁿ budget with meso correction (§5.5): 2² = 4 candidate configurations, but (2R,3S) and (2S,3R) are the same achiral molecule counted twice — verify the internal mirror bond-by-bond rather than asserting it. This is the textbook case the stem's "some stereoisomers may be superimposable on their mirror images" was written for.

### (f) Asymmetric carbons in citric acid
**L1 · Answer** **None (0)** — the central carbon carries two identical –CH₂COOH groups.
**L2 · Thought** Same check as 2011 Q1e: "four *different* groups" fails at the central carbon, and no other carbon is sp³ with four attachments.

---

## Question 2 — Redox chemistry of vehicle pollution

### (a) Complete combustion of octane
**L1 · Answer** **2 C₈H₁₈ + 25 O₂ → 16 CO₂ + 18 H₂O** (audit: C 16, H 36, O 50 ✓).
**L2 · Thought** Balance C, then H, then O (halve 25/2 if fractions bother you — doubling at the end is cleaner).

### (b) Oxidation of CO
**L1 · Answer** i) **2 CO + O₂ → 2 CO₂**; ii) **CO + H₂O → CO₂ + H₂** (the water-gas shift).
**L2 · Thought** In (ii) water is the *oxidant* — H(+1) is reduced to H₂ while C(+2) climbs to +4; recognising water as an oxidising agent here is the conceptual point.

### (c) Reduction of NO
**L1 · Answer** i) **2 NO + 2 CO → N₂ + 2 CO₂**; ii) **2 NO + 2 H₂ → N₂ + 2 H₂O**.
**L2 · Thought** Nitrogen +2 → 0 in both; the reductant's element (C or H) rises correspondingly — 2-electron reductants, 2 NO each.

### (d) The ceria oxygen-storage equilibrium
**L1 · Answer** **4 CeO₂ ⇌ 2 Ce₂O₃ + O₂** (Ce(IV) ⇌ Ce(III); audit: Ce 4, O 8 = 6 + 2 ✓).
**L2 · Thought** "Equilibrium mixture of cerium(III) and cerium(IV) oxides" names both partners (CeO₂ and Ce₂O₃); oxygen gas is the only other species the atom audit allows. In oxygen-rich exhaust it stores O₂ (right-to-left), in fuel-rich it donates (left-to-right) — that is what "oxygen storage" means chemically.

### (e) Carbon + NO₂
**L1 · Answer** **C + 2 NO₂ → CO₂ + 2 NO** (audit: C 1, N 2, O 4 = 2 + 2 ✓).
**L2 · Thought** The stem gives the products (CO₂ and NO); carbon 0 → +4, nitrogen +4 → +2 — two NO₂ per carbon closes the electron count.

### (f) Urea structure and bond angles
**L1 · Answer** **O=C(NH₂)₂**: trigonal-planar carbon — **N–C–O ≈ 120°, H–N–H ≈ 120°** (each N is ~planar by conjugation with the carbonyl).
**L2 · Thought** The carbonyl's π-delocalisation flattens the nitrogens too (amide conjugation), so both angles answer "≈120°" rather than 109.5°/107° — saying *why* (lone pair delocalised into C=O) is the mark-worthy line.

### (g) Urea + water → ammonia
**L1 · Answer** **(NH₂)₂CO + H₂O → 2 NH₃ + CO₂** (audit: C 1, N 2, H 6, O 2 ✓).
**L2 · Thought** Hydrolysis of the carbamide: the carbon is ejected as CO₂ (in practice via carbamic acid), no redox.

### (h) NH₃ with NO and NO₂
**L1 · Answer** i) **4 NH₃ + 6 NO → 5 N₂ + 6 H₂O**; ii) **8 NH₃ + 6 NO₂ → 7 N₂ + 12 H₂O** (audit both: N, H, O ✓).
**L2 · Thought** Comproportionation (NH₃'s N at −3 meets NOₓ's N at +2/+4 at 0): balance the electrons first — NO gains 2 e⁻, NO₂ 4 e⁻, each NH₃ loses 3 e⁻ — then set NH₃ : NOₓ = 2 : 3 (i) or 4 : 3 (ii) and clear fractions.

### (i) Underlining oxidised (single) and reduced (double) atoms
**L1 · Answer** (b) **C in CO oxidised**; (c) **C in CO / H in H₂ oxidised; N in NO reduced**; (d) **Ce(+4) reduced to Ce(+3), lattice O(−2) oxidised to O₂**; (e) **C(s) oxidised; N in NO₂ reduced**; (h) **N in NH₃ oxidised; N in NO/NO₂ reduced**.
**L2 · Thought** Run the oxidation-state audit equation by equation and underline *atoms*, not compounds — in (d) note both an oxidation and a reduction happen within one compound's lattice (the Ce drops, the oxide ion climbs out as O₂).

---

## Question 3 — Acyl chlorides and related oxochlorides

### (a)–(b) Acyl chloride reactions
**L1 · Answer** (a) **CH₃COCl + H₂O → CH₃COOH + HCl**; (b) **C₂H₅COCl + C₂H₅OH → C₂H₅CO₂C₂H₅ + HCl**.
**L2 · Thought** Nucleophilic acyl substitution: the nucleophile's O takes the acyl group, its H leaves with Cl as HCl — one line each, with HCl as the stoichiometric signature.

### (c) Compound A (Carbaryl route)
**L1 · Answer** **A = 1-naphthyl chloroformate** (1-naphthyl-O–C(=O)–Cl) — `O=C(Cl)Oc1cccc2ccccc12` (**C₁₁H₇O₂Cl ✓**): phosgene converts the naphthol's OH into –OCOCl; CH₃NH₂ then substitutes Cl to give the methylcarbamate (Carbaryl, 1-naphthyl-O–CONHCH₃).
**L2 · Thought** Formula audit: A = naphthol (C₁₀H₈O) + COCl₂ − HCl = C₁₁H₇O₂Cl ✓ — the chlorine survives into A and leaves only in the second step, which is why phosgene can play "diacyl chloride" twice.

### (d) POCl₃ and SOCl₂ structures and oxidation states
**L1 · Answer** POCl₃: **tetrahedral** (P with three Cl and one =O), **P = +5**; SOCl₂: **trigonal pyramidal** (S with two Cl, one =O, one lone pair), **S = +4**.
**L2 · Thought** Count the electron pairs around the central atom (P: 4 domains, no lone pair; S: 3 domains + 1 lone pair) before naming the shape; the oxidation states fall out of the same count (Cl −1, O −2).

### (e) Thionyl chloride + water
**L1 · Answer** **SOCl₂ + H₂O → SO₂ + 2 HCl** (audit: S 1, O 2 = 1 + 1... 2 HCl, S 1, O 2 = 2 ✓ H 2 ✓).
**L2 · Thought** Sulfur stays +4 (metathesis, no redox): the two Cl are replaced by the double-bonded O of SO₂ — the acid-chloride-of-sulfurous-acid logic.

### (f) Phosphate esters from POCl₃ + methanol
**L1 · Answer** i) 1 : 1 → **CH₃O–P(=O)Cl₂** (methyl phosphorodichloridate); ii) 1 : 2 → **(CH₃O)₂P(=O)Cl** (dimethyl phosphorochloridate).
**L2 · Thought** Successive substitution of Cl by OMe (one per methanol, one HCl lost per substitution) — the third chlorine would need a third methanol; count them off.

### (g) Acid B and its formation
**L1 · Answer** The precipitate's analysis gives Ag : P : O = 71.3/107.87 : 10.2/30.97 : 18.5/16.00 = 2.01 : 1 : 3.51 ≈ **4 : 2 : 7 → Ag₄P₂O₇** (silver pyrophosphate ✓ 71.3% Ag, 10.2% P ✓), so **B = pyrophosphoric acid, H₄P₂O₇** — (HO)₂P(=O)–O–P(=O)(OH)₂ (two tetrahedral P sharing one bridging O). Formation (with HCl the only other product): **5 H₃PO₄ + POCl₃ → 3 H₄P₂O₇ + 3 HCl** (audit: P 6, H 15, Cl 3, O 21 ✓).
**L2 · Thought** The precipitate analysis identifies B *before* any equation is written (Ag : P = 2 : 1 only fits the pyrophosphate among simple silver phosphates — verify the percentages rather than assuming). For the equation, the honest construction is a two-step cycle: 2 H₃PO₄ → H₄P₂O₇ + H₂O (condensation) with POCl₃ + 3 H₂O → H₃PO₄ + 3 HCl consuming the water (as the stem states); combining three condensations with one hydrolysis gives the printed 5 : 1 : 3 : 3 balance — check all four elements, because the intermediate H₃PO₄ produced by POCl₃'s hydrolysis cancels against the feed.

---

## Question 4 — Thermal decomposition of copper(II) sulfate

### (a) Formulae of A, B and C
**L1 · Answer** Mass losses of the pentahydrate (M = 249.68): each H₂O = 7.2%; A (≈ 14% loss) = **CuSO₄·3H₂O** (−2 H₂O); B (≈ 29% loss) = **CuSO₄·H₂O** (−4 H₂O); C (≈ 36% loss) = **CuSO₄** (all five waters gone, 36.1% ✓).
**L2 · Thought** Anchor the stoichiometry on the waters: 5 H₂O = 36.1% of the pentahydrate's mass, so each step of ~7–14% is one or two waters — match the plateaux to integer hydration numbers rather than to arbitrary compositions (§4 capacity/audit: the clean integers are the self-check).

### (b) E → F redox
**L1 · Answer** **E = CuO, F = Cu₂O**: **4 CuO → 2 Cu₂O + O₂** (Cu +2 → +1, oxide −2 → 0; mass loss to 71.3% total ✓).
**L2 · Thought** After the sulfate has gone (C → CuO by SO₃ loss at ~68%), further mass loss can only come from oxygen itself — a redox decomposition with O₂ evolved, the only remaining light product; the mass audit (CuO 68.1%, Cu₂O 71.3%) confirms the assignment.

### (c) Empirical formula of D
**L1 · Answer** **Cu₂SO₅** (i.e. CuO·CuSO₄ — copper(II) oxosulfate): exactly half of the CuSO₄ has become CuO, so the bulk composition is (CuSO₄ + CuO)/2 = Cu₂SO₅ (mass loss ≈ 52%, matching D's plateau ✓).
**L2 · Thought** "Exactly half decomposed" is a bulk-composition instruction, not a molecular one: average the reactant and product formulas 1 : 1, then reduce to integers; the mass-loss check (~52%) is the confirmation that D is this oxosulfate rather than a guess like CuSO₃.

---

## Question 5 — Emergency oxygen supplies

### (a) Decomposition of sodium chlorate(V)
**L1 · Answer** **2 NaClO₃ → 2 NaCl + 3 O₂** (audit: Na 2, Cl 2, O 6 ✓).
**L2 · Thought** Chlorate(V) to chloride: all six oxygens leave as 3 O₂ — the classic oxygen-candle reaction.

### (b) Barium peroxide scavenging
**L1 · Answer** i) **BaO₂ + Cl₂ → BaCl₂ + O₂**; ii) **2 BaO₂ + 4 HClO → 2 BaCl₂ + 2 H₂O + 3 O₂** (audit both: Ba, Cl, H, O ✓).
**L2 · Thought** Peroxide as both base and oxidant: in (i) the peroxide O₂²⁻ is itself oxidised to O₂ while chlorine is captured as chloride (Cl₂ + O₂²⁻ → 2 Cl⁻ + O₂, a comproportionation to 0 and −1); in (ii) HClO's Cl(+1) is reduced to Cl⁻ and the peroxide again ends as O₂ — write the ionic electron balance first if the coefficients resist you.

### (c) Total oxygen volume from the flow graph
**L1 · Answer** Integrate the flow curve (rectangle-by-rectangle): the plateau plus the long decay tail sum to **≈ 15 dm³** per canister.
**L2 · Thought** An estimate question: state the integration method (plateau rectangle + trapezoids on the decay), not just the number — and take the exponential tail all the way out: truncating it early under-reads the total by ~30 %; the full tail is what brings the total to ≈ 15 dm³. Part (d) then shows the graph was always meant as an estimate (it asks for *60 dm³* from several such generators in practice).

### (d) NaClO₃ for 60 dm³ of O₂
**L1 · Answer** n(O₂) = 60/24.0 = 2.50 mol ⇒ n(NaClO₃) = 2.50 × 2/3 = 1.67 mol ⇒ mass = 1.67 × 106.44 = **177 g**.
**L2 · Thought** The 2 : 3 stoichiometry from (a) applied to moles of *product* — gas volume to moles first (24 dm³), stoichiometric ratio second, molar mass last.

### (e) Oxidation states of oxygen
**L1 · Answer** i) CO₂: **−2**; ii) BaO₂ (peroxide): **−1**; iii) KO₂ (superoxide): **−½**.
**L2 · Thought** The O–O bond is the tell: peroxide and superoxide keep an O–O linkage, so the average oxidation state is fractional — compute from the cation charge (Ba²⁺, K⁺) rather than writing −2 by reflex.

### (f) Potassium superoxide chemistry
**L1 · Answer** i) **4 KO₂ + 2 H₂O → 4 KOH + 3 O₂** (audit: K 4, O 8 + 2 = 10 → 4 + 6 = 10 ✓ H 4 ✓); ii) **KOH + CO₂ → KHCO₃** (the by-product absorbing CO₂; alternatively 2 KOH + CO₂ → K₂CO₃ + H₂O).
**L2 · Thought** In (i) the superoxide both disproportionates (O(−½) → O(−2) in KOH and O(0) in O₂) — 4 KO₂ give 3 O₂ + 4 OH⁻; the KOH by-product is then the CO₂ scrubber, which is the elegant dual role (more O₂ released *and* CO₂ removed) that the question wants you to notice.

---

## Question 6 — The synthesis of Viagra (sildenafil)

### (a) Intermediates B, D, E, F, G, I, J
**L1 · Answer** (all machine-validated)
- **B = ethyl 1-methyl-3-n-propylpyrazole-5-carboxylate** — `CCOC(=O)c1cc(CCC)n(C)n1` (**C₁₀H₁₆N₂O₂ ✓ = A + CH₂**): (CH₃)₂SO₄ methylates the pyrazole N–H.
- **D = 1-methyl-3-n-propyl-4-nitropyrazole-5-carboxylic acid** — `O=C(O)c1c([N+](=O)[O-])c(CCC)n(C)n1` (**C₈H₁₁N₃O₄ ✓ = C + NO₂ − H**): conc. HNO₃/H₂SO₄ nitrates the pyrazole's only free ring position (C4).
- **E = the acyl chloride** — `O=C(Cl)c1c([N+](=O)[O-])c(CCC)n(C)n1` (**C₈H₁₀N₃O₃Cl ✓ = D − OH + Cl**): SOCl₂.
- **F = the 4-nitro-carboxamide** — `NC(=O)c1c([N+](=O)[O-])c(CCC)n(C)n1` (**C₈H₁₂N₄O₃ ✓ = E + NH₃ − HCl**).
- **G = the 4-amino-carboxamide** — `NC(=O)c1c(N)c(CCC)n(C)n1` (**C₈H₁₄N₄O ✓ = F + 3 H₂ − 2 H₂O**): H₂/Pd reduces only the nitro group.
- **I = 5-(2-ethoxyphenyl)-1-methyl-3-n-propyl-1,6-dihydropyrazolo[4,3-d]pyrimidin-7-one** — `O=c1[nH]c(-c2ccccc2OCC)nc2c1c(CCC)n(C)n2` (**C₁₇H₂₀N₄O₂ ✓ = H − H₂O**): NaOH-mediated cyclodehydration of the 4-(2-ethoxybenzamido)-5-carboxamide H (G + 2-ethoxybenzoyl chloride, C₁₇H₂₂N₄O₃ ✓).
- **J = the 4′-(chlorosulfonyl) derivative** (chlorosulfonation *para* to the ethoxy group on the pendant phenyl ring: I + ClSO₃H − H₂O = **C₁₇H₁₉ClN₄O₄S ✓**), which N-methylpiperazine converts to sildenafil (**C₂₂H₃₀N₆O₄S ✓**).
**L2 · Thought** The whole sequence is heterocycle bookkeeping on the pyrazole: methylate N1 (B), free the acid (C), nitrate C4 (D), activate the acid (E), make the amide (F), unmask the 4-amine (G), acylate it (H), then let the two amides condense into the fused pyrimidinone (I). Every printed formula closes on these assignments (B → C is a hydrolysis: −C₂H₄ exactly; H → I is −H₂O exactly). The pendant phenyl ring arrives as 2-ethoxybenzoyl chloride at G → H, and its para position is sulfonated last — blocking-group-free route, so regiochemistry (C4 for nitro, para for sulfonyl) is the only judgement required.

### (b) Reagents for B → C and E → F
**L1 · Answer** i) B → C: **HCl(aq)** (aqueous acid hydrolysis of the ester — heating with dilute hydrochloric acid; aqueous NaOH then acidic work-up achieves the same net change and is a creditable alternative); ii) E → F: **concentrated aqueous ammonia (NH₃)** (aminolysis of the acyl chloride).
**L2 · Thought** Match the reagent class to the bond change: ester → acid can be driven by aqueous acid (HCl(aq)) or base-then-work-up; acyl chloride → amide is ammonia (the HCl is mopped up by excess NH₃ as NH₄Cl).

### (c) The hydrogen removed by NaOH (H → I)
**L1 · Answer** **An N–H of the pyrazole-5-carboxamide (the –CONH₂ group)**.
**L2 · Thought** The ring-closing nucleophile must be the 5-carboxamide's nitrogen (it attacks the 2-ethoxybenzamide carbonyl carbon intramolecularly); deprotonating *its* N–H creates that nucleophile, and dehydration then ejects the carbonyl oxygen as water. Deprotonating the benzamide N–H would make the wrong nitrogen nucleophilic and could not close this ring.

### (d) N-methylpiperazine
**L1 · Answer** A six-membered ring with two nitrogens at 1,4-positions, one bearing methyl: **CN1CCNCC1** (C₅H₁₂N₂ ✓) — the free N–H is what sulfonylates J.
**L2 · Thought** Read the target backwards (§4 repeat-unit/back-reading logic): sildenafil's –SO₂–N(CH₃)–(CH₂CH₂)₂NH ring = an N-methylated piperazine joined through the *other* nitrogen — cleave the S–N bond mentally, restore the N–H, and the reagent appears.

### (e) Hydrazine and reagent K
**L1 · Answer** i) **H₂N–NH₂** (each N pyramidal, one lone pair); ii) **K = ethyl 2,4-dioxooctanoate** (ethyl pentanoylpyruvate), EtO₂C–CO–CH₂–CO–CH₂CH₂CH₃ — `CCOC(=O)C(=O)CC(=O)CCC` (C₉H₁₄O₄ ✓): the 1,3-diketo portion (C4 ketone + C2 ketone) condenses with hydrazine's two nitrogens (2 × −H₂O), closing the pyrazole with the n-propyl group at C3 and the ester at C5.
**L2 · Thought** Back-read the pyrazole (§4 repeat-unit logic): A + 2 H₂O − N₂H₄ = C₉H₁₄O₄, so K is a nine-carbon tetravalent dicarbonyl with an ester; placing the n-propyl on the ring's C3 and the ester on C5 fixes which end is which — then the two water losses fall out as the two C=O/N–H condensations.

---

## Question 7 — Spectra of haloalkanes

### (a) Molecular ions of CFC-12 (CCl₂F₂)
**L1 · Answer** Peaks at **m/z 120, 122, 124** (¹²C + 2 × ¹⁹F + ³⁵Cl₂ / ³⁵Cl³⁷Cl / ³⁷Cl₂) with intensities **9 : 6 : 1** ((¾)² : 2 × ¾ × ¼ : (¼)²).
**L2 · Thought** Binomial convolution of the two chlorines' 3 : 1 ratio (§4 isotope-signature): the fluorines and carbon are silent (single isotopes), so the whole pattern is the Cl₂ expansion.

### (b) Molecular-ion sketch for Halon 1211 (CBrClF₂)
**L1 · Answer** Four ion compositions: 164 (⁷⁹Br³⁵Cl, 37.5%), 166 (⁷⁹Br³⁷Cl, 12.5%), 166 (⁸¹Br³⁵Cl, 37.5%), 168 (⁸¹Br³⁷Cl, 12.5%) ⇒ **three peaks at 164 : 166 : 168 with intensities 3 : 4 : 1** (the 166 peak merges two compositions).
**L2 · Thought** Two independent coin flips (Br 1 : 1, Cl 3 : 1) multiplied out: (½ × ¾) : (½ × ¼ + ½ × ¾) : (½ × ¼) = 3 : 4 : 1 — the merged middle peak is the instructive part: same m/z can hide two different isotopic compositions.

### (c) CH₂Br₂/CHDBr₂/CD₂Br₂ mixture (half of all H = D)
**L1 · Answer** With 50 % D at each position, the molecular species are CH₂Br₂ : CHDBr₂ : CD₂Br₂ = 1 : 2 : 1 (0.25 : 0.50 : 0.25), and Br₂ splits ⁷⁹Br₂ : ⁷⁹Br⁸¹Br : ⁸¹Br₂ = 1 : 2 : 1. Convolving:
**172 : 173 : 174 : 175 : 176 : 177 : 178 = 1 : 2 : 3 : 4 : 3 : 2 : 1**
(172 = CH₂⁷⁹Br₂; 173 = CHD⁷⁹Br₂; 174 = CD₂⁷⁹Br₂ + CH₂⁷⁹Br⁸¹Br; 175 = CHD⁷⁹Br⁸¹Br; 176 = CD₂⁷⁹Br⁸¹Br + CH₂⁸¹Br₂; 177 = CHD⁸¹Br₂; 178 = CD₂⁸¹Br₂).
**L2 · Thought** Two independent binomials (H/D at 1 : 2 : 1, Br/Br at 1 : 2 : 1) convolve into the symmetric 1 : 2 : 3 : 4 : 3 : 2 : 1 — compute the composition grid, then sum diagonals of equal mass; the seven-peak envelope is the product, and its symmetry is the self-check.

### (d) Number of ¹⁹F environments
**L1 · Answer** **A: 2** (CF and CF₂); **B: 1**; **C: 2** (CF₃ and CH₂F); **D: 1**; **E: 1**; **F: 1**; **G: 1**.
**L2 · Thought** Environment counting on small molecules (§7.3): only A and C have two kinds of carbon, so only they can have two fluorine environments — the single-carbon compounds (D–G) are all-equivalent by default.

### (e) Halothane, C₂HBrClF₃, one ¹⁹F signal
**L1 · Answer** One signal ⇒ all three F on the same carbon: **CF₃–CHBrCl (2-bromo-2-chloro-1,1,1-trifluoroethane)**, which has one stereocentre — the two 3D structures are the **(R)- and (S)-enantiomers** (draw both with the CF₃ in the plane and Br/Cl/H wedged and dashed, mirror images).
**L2 · Thought** The one-signal constraint places the CF₃ group uniquely; the molecule is then chiral (four different groups on C2: CF₃, Br, Cl, H), and "two possible structures" = the enantiomeric pair — the anaesthetic is indeed used as the racemate.

### (f) Intensity ratios
**L1 · Answer** A: **1 : 2** (CF : CF₂); C: **3 : 1** (CF₃ : CH₂F).
**L2 · Thought** Signal intensity counts nuclei, not environments — read the ratio straight off the group sizes.

### (g) The ¹⁹F NMR shown (X at −67.8, Y at −71.9)
**L1 · Answer** The compound is **CFC-113 (A), Cl₂FC–CClF₂**: **X = the two CF₂ fluorines** (the stronger **doublet** at −67.8 ppm — split by the single neighbouring F, n = 1); **Y = the single CF fluorine** (the weaker **triplet** at −71.9 ppm — split by the two neighbouring F's, n = 2).
**L2 · Thought** Splitting and intensity cross-check each other (§7.3): the 2-F group is split by 1 F (doublet) and integrates twice as much; the 1-F group is split by 2 F (triplet) and integrates half as much — X's doublet is taller than Y's triplet in the printed spectrum, exactly as required. Of the table's compounds, only A has two mutually coupled fluorine environments within three bonds (F–C–C–F), so the assignment is unique before any shift comparison.

---

*End of Paper 20 (2006). Next: 2005 Round 1.*

---

# Paper 21 — 2005 UKChO Round 1 (37th IChO selection)

**Marks / time:** 6 questions (2 h).
**Theme map:** Q1 oxides of carbon; Q2 I₂O₅ and CO detection; Q3 ant-sting methanoic acid; Q4 ¹³C/¹H NMR of NanoBalletDancer; Q5 breathalyser redox; Q6 rimonabant synthesis.

---

## Question 1 — Carbon oxides

### (a)(i) Calcium carbonate + hydrochloric acid
**L1 · Answer** **CaCO₃ + 2 HCl → CaCl₂ + H₂O + CO₂**
**L2 · Thought** Acid + carbonate → salt + carbonic acid, which falls apart to CO₂ + H₂O; balance Ca first, then Cl (2 HCl), and the O/H follow automatically.

### (a)(ii) Structure of carbonic acid
**L1 · Answer** **O=C(OH)₂** — a central carbon double-bonded to one O and single-bonded to two –OH groups (trigonal-planar carbon, like a "hydroxy-aldehyde hydrate").
**L2 · Thought** Carbonic acid is just CO₂ with a water added across one C=O π-bond: carbon keeps valence 4 with one C=O and two C–OH.

### (b)(i) Dehydration of methanoic acid
**L1 · Answer** **HCOOH —(conc. H₂SO₄, ~140 °C)→ CO + H₂O** (sulfuric acid is the dehydrating agent, written over the arrow; it is not consumed).
**L2 · Thought** "Dehydrating" means remove the elements of water: from HCOOH take the –OH and the carbonyl H... rather, take O + 2 H as H₂O, leaving CO. Counting atoms on each side (C 1, H 2, O 2 → C 1, O 1 + H₂O) confirms the bookkeeping.

### (b)(ii) Dot-and-cross structure of CO
**L1 · Answer** **:C≡O:** — three shared pairs (six electrons) between C and O, with one lone pair left on carbon and one on oxygen; one of the three bonding pairs is dative (both electrons donated by O), giving formal charges C⁻–O⁺. Ten valence electrons in total (4 from C + 6 from O).
**L2 · Thought** Count valence electrons first (10), then satisfy octets: only a triple bond leaves both atoms with complete octets — exactly the N₂ pattern, since CO is isoelectronic with N₂.

### (b)(iii) Bond order in CO
**L1 · Answer** **Triple bond.**
**L2 · Thought** Follows directly from the dot-and-cross picture: three shared pairs. (Experiment backs it: the C–O bond in CO is shorter and stronger than any C=O double bond.)

### (c) PdCl₂ test for CO
**L1 · Answer** **PdCl₂ + CO + H₂O → Pd + CO₂ + 2 HCl**
**L2 · Thought** CO is oxidised to CO₂ (C: +2 → +4, releasing 2 e⁻); Pd²⁺ is reduced to Pd(0) (accepting 2 e⁻) — a 1 : 1 redox couple. Oxygen balance needs one H₂O on the left, which then delivers 2 HCl on the right; check: Pd 1=1, Cl 2=2, C 1=1, O 1+1=2, H 2=2. ✓

### (d)(i) Propan-1,3-dioic acid → carbon suboxide
**L1 · Answer** Structure: **HOOC–CH₂–COOH** (malonic acid, a CH₂ flanked by two carboxyls). Equation: **CH₂(COOH)₂ → C₃O₂ + 2 H₂O**.
**L2 · Thought** "Fully dehydrating" means strip every removable water: two –COOH groups lose 2 × H₂O in total (the two acidic H's plus one O from each –OH... precisely: C₃H₄O₄ − 2 H₂O = C₃O₂). Atom count: C 3=3, H 4 = 2×2, O 4 = 2 + 2. ✓

### (d)(ii) Structure of carbon suboxide
**L1 · Answer** **O=C=C=C=O** — a linear chain of three carbons joined by cumulated double bonds, capped by an oxygen at each end.
**L2 · Thought** Carbon valence 4 with no H left: cumulene logic (like CO₂ extended by one carbon). Each terminal C is satisfied by =O and =C; the central C takes two double bonds. Linear at every carbon (sp).

### (e) Mellitic acid and C₁₂O₉
**L1 · Answer** Benzene hexacarboxylic acid: **a benzene ring bearing six –COOH groups, one on every ring carbon, C₆(COOH)₆**. C₁₂O₉ is **mellitic trianhydride**: the same benzene core with each *pair of adjacent* –COOH groups cyclised into a five-membered anhydride ring (three anhydride bridges, positions 1,2 / 3,4 / 5,6) — SMILES `O=c1oc(=O)c2c3c(=O)oc(=O)c3c3c(=O)oc(=O)c3c12` (validator: C₁₂O₉, rings 5,5,5,6 ✓).
**L2 · Thought** Dehydration budget: C₆(COOH)₆ = C₁₂H₆O₁₂; losing 6 H₂O would give C₁₂O₆ — too far; losing **3 H₂O** (one per adjacent acid pair, the standard anhydride condensation) gives C₁₂H₀O₉ = C₁₂O₉ ✓. So exactly three –CO–O–CO– bridges form, each consuming two neighbouring carboxyls: 3 × 2 = 6 carboxyls, all accounted for. Anhydride rings are 5-membered (O–CO–C–C–CO), the maleic-anhydride pattern fused onto all six edges... onto three alternate edges of the ring.

---

## Question 2 — Diiodine pentoxide

### (a) I₂O₅ + CO
**L1 · Answer** **I₂O₅ + 5 CO → I₂ + 5 CO₂**
**L2 · Thought** Iodine goes from +5 to 0 (gains 5 e⁻ per I, 10 per I₂O₅); each CO → CO₂ donates 2 e⁻, so 5 CO per I₂O₅. The five oxygens transfer one-for-one onto the five CO molecules — "I₂O₅ is a stored oxidant delivering five O atoms" is the cleanest way to see the stoichiometry.

### (b) Percentage of CO in the gas sample
**L1 · Answer** n(Na₂S₂O₃) = 8.00 × 10⁻³ dm³ × 0.100 mol dm⁻³ = 8.00 × 10⁻⁴ mol → n(I₂) = ½ × 8.00 × 10⁻⁴ = 4.00 × 10⁻⁴ mol → n(CO) = 5 × n(I₂) = 2.00 × 10⁻³ mol → V(CO) = 2.00 × 10⁻³ × 24.0 dm³ = 48.0 cm³ → **48.0 / 150 = 32.0 % CO by volume**.
**L2 · Thought** Chain the mole ratios through the two reactions (thiosulfate : I₂ = 2 : 1; I₂ : CO = 1 : 5) before touching volumes — the factor 5 from part (a) is the pivot, and forgetting it is the classic error here. Gas volumes at the same r.t.p. convert moles straight into percentages.

### (c) The hydrated form
**L1 · Answer** M(I₂O₅) = 2(126.90) + 5(16.00) = 333.80 g mol⁻¹. Let the hydrate be I₂O₅·xH₂O: mass loss = 18.02x / (333.80 + 18.02x) = 0.01766 → 18.02x = 6.00 → x = 0.333 = ⅓. So the hydrate is **3 I₂O₅·H₂O, empirical formula HI₃O₈**; dehydration: **2 HI₃O₈ → 3 I₂O₅ + H₂O**.
**L2 · Thought** Work per mole of I₂O₅ and let x be fractional — 1.766 % is a tiny mass loss, so x must be small; x = ⅓ drops out cleanly (0.9823 × 18.02x = 5.895). Multiply through by 3 to get whole-number formulas, and note the check: 2 HI₃O₈ = H₂I₆O₁₆ → 3 I₂O₅ + H₂O balances exactly (I 6=6, O 16 = 15+1, H 2=2).

### (d) Parent acid of I₂O₅
**L1 · Answer** **I₂O₅ + H₂O → 2 HIO₃** (parent acid = iodic acid, **HIO₃**). Oxidation state of iodine in I₂O₅: 2x + 5(−2) = 0 → **x = +5**.
**L2 · Thought** The ethanoic-anhydride analogy tells you what to do: anhydride + water → 2 × acid, i.e. split I₂O₅ symmetrically and add H₂O across the I–O–I bridge. The oxidation state is unchanged by hydration — anhydride and acid always share it.

### (e) Structures of HIO₃ and I₂O₅
**L1 · Answer** HIO₃: **HO–I(=O)₂** — iodine with one –OH, two terminal I=O bonds and one lone pair (pyramidal iodine, like chloric acid). I₂O₅: **O₂I–O–IO₂** — two IO₂ units joined by a single bridging oxygen (the anhydride link I–O–I), each iodine keeping its lone pair.
**L2 · Thought** Build the acid first (I needs an octet: OH + 2 oxo + lone pair), then form the anhydride by removing H₂O from two acid molecules across two –OH groups — the surviving I–O–I bridge is exactly what part (d)'s hydration reverses.

### (f) I₂ + Cl₂ + H₂O
**L1 · Answer** **I₂ + 5 Cl₂ + 6 H₂O → 2 HIO₃ + 10 HCl**
**L2 · Thought** Iodine: 0 → +5, so each I₂ releases 10 e⁻; each Cl₂ accepts 2 e⁻ → 5 Cl₂. Then balance O with 6 H₂O on the left (2 HIO₃ needs 6 O) and H follows: 12 H left = 2 (HIO₃) + 10 (HCl) right. ✓ Chlorine is the oxidant, water supplies the oxygen.

---

## Question 3 — Ants and methanoic acid

### (a)(i) Total acid in one ant
**L1 · Answer** Pure acid injected = 50 % × 6.0 × 10⁻³ cm³ = 3.0 × 10⁻³ cm³; that is 80 % of the ant's stock → total = 3.0 × 10⁻³ / 0.80 = **3.75 × 10⁻³ cm³** (3.8 × 10⁻³ cm³ to 2 s.f.).
**L2 · Thought** Two percentage operations in sequence — apply the 50 % (composition) and the 80 % (fraction injected) to *different* bases and keep them in the right order: volume of pure acid first, then scale up for the reserve.

### (a)(ii) Ants per litre
**L1 · Answer** 1.0 dm³ = 1000 cm³; 1000 / 3.75 × 10⁻³ = **2.7 × 10⁵ ants** (≈ 270 000).
**L2 · Thought** Simple scaling — the number sounds absurd, which is exactly the point of the question (nobody really distilled ants by the litre... they did).

### (b)(i) Neutralising the sting
**L1 · Answer** **NaHCO₃ + HCOOH → HCOONa + H₂O + CO₂**
**L2 · Thought** Carbonate/bicarbonate + acid always gives salt + water + CO₂; 1 : 1 here because HCOOH is monoprotic.

### (b)(ii) Moles of acid injected
**L1 · Answer** mass = 3.0 × 10⁻³ cm³ × 1.2 g cm⁻³ = 3.6 × 10⁻³ g; n = 3.6 × 10⁻³ / 46.03 = **7.8 × 10⁻⁵ mol**.
**L2 · Thought** Density converts the *pure-acid* volume (from (a)(i), before dividing by 0.8 — only the injected amount matters) to mass; M(HCOOH) = 46.03.

### (b)(iii) Mass of NaHCO₃
**L1 · Answer** 1 : 1 ratio → n(NaHCO₃) = 7.8 × 10⁻⁵ mol; mass = 7.8 × 10⁻⁵ × 84.01 = 6.6 × 10⁻³ g = **6.6 mg**.
**L2 · Thought** Carry the unrounded mole value through (7.82 × 10⁻⁵ × 84.01 = 6.57 mg → 6.6 mg) and only round at the end.

### (c) Concentration in the body
**L1 · Answer** c = 7.8 × 10⁻⁵ mol / 1.0 × 10⁻³ dm³ = **0.078 mol dm⁻³**.
**L2 · Thought** The acid dilutes into 1.0 cm³ of body water (its own volume ignored, as instructed) — convert cm³ → dm³ (×10⁻³) before dividing.

### (d) [H⁺] from pH
**L1 · Answer** [H⁺] = 10⁻²·⁴³ = **3.7 × 10⁻³ mol dm⁻³**.
**L2 · Thought** Straight inversion of the given definition; keep 2 s.f. to match the pH's two decimal places.

### (e) Percentage ionised
**L1 · Answer** fraction ionised = [H⁺]/c = 3.7 × 10⁻³ / 0.078 = **4.7 %** (4.75 % before rounding; mark scheme prints 4.8 % from its own rounding — same quantity).
**L2 · Thought** Each ionised molecule gives exactly one H⁺, so [H⁺] counts the ionised molecules directly — divide by the analytical concentration. "Weak acid" in one number: ≈ 95 % of the molecules stay intact.

### (f) Ka of methanoic acid
**L1 · Answer** Ka = [HCOO⁻][H⁺]/[HCOOH] = (3.72 × 10⁻³)² / (0.078 − 0.0037) = 1.38 × 10⁻⁵ / 0.0743 = **1.9 × 10⁻⁴ mol dm⁻³** (mark scheme: 1.8 × 10⁻⁴ from rounded inputs, accepts 1.9 × 10⁻⁴ ✓; pKa = 3.73).
**L2 · Thought** The 1 : 1 dissociation makes numerator = [H⁺]², and the denominator is the *unionised* acid (c − [H⁺]), not c itself — with 4.7 % ionised the correction is small but it is what the question is testing. (Literature Ka ≈ 1.8 × 10⁻⁴ — a nice consistency check.)

---

## Question 4 — NMR spectra of NanoBalletDancer (C₄₁H₅₀O₂)

*Structure used throughout (consistent with the paper's numbering; validator: `CCCC#Cc1cc(C#CCCC)cc(Cc2cc(C#CC(C)(C)C)c(C3OCC(C)(C)CO3)c(C#CC(C)(C)C)c2)c1` → C₄₁H₅₀O₂ ✓):*
- *Ring 1 (atoms 6–11, the "hips"): 1,3,5-trisubstituted benzene — at 6 and 8 two identical legs –C≡C–CH₂–CH₂–CH₃ (atoms 5,4,3,2,1 and 12,13,14,15,16), at 10 the linker –CH₂– (atom 17).*
- *Linker: atom 17 = CH₂ joining C10 to C18 of ring 2.*
- *Ring 2 (atoms 18–23, the "chest"): 1,2,4,5-tetrasubstituted benzene — at 20 and 22 two identical arms –C≡C–C(CH₃)₃ (24,25,26,27,28,29 and 30,31,32,33,34,35), at 18 the linker CH₂, at 21 the head.*
- *Head: 2-aryl-5,5-dimethyl-1,3-dioxane — 36 = acetal CH between the two oxygens, 37 ≡ 39 = the two ring OCH₂ carbons, 38 = quaternary C5, 40 and 41 = its two methyls.*

### (a) Equivalent benzene-ring carbons
**L1 · Answer** **6 ≡ 8 and 9 ≡ 11** (ring 1: mirror through C7–C10 swaps the two identical legs); **19 ≡ 23 and 20 ≡ 22** (ring 2: mirror through C18–C21 swaps the two identical arms). Distinct signals: ring 1 → 4 ({6,8}, 7, {9,11}, 10); ring 2 → 4 (18, {19,23}, {20,22}, 21) ⇒ **8 benzene-ring signals in total**.
**L2 · Thought** Find each ring's symmetry plane by its substitution *pattern*, not by looking at the drawing: ring 1 has two identical substituents at 6, 8 and a different one at 10 (a mirror through 7 and 10); ring 2 has identical arms at 20, 22 with two different substituents at 18, 21 (a mirror through 18 and 21). Carbons lying on the mirror (7, 10, 18, 21) stay unique; off-axis atoms pair up.

### (b) Equivalent triple-bond carbons
**L1 · Answer** **4 ≡ 13 and 5 ≡ 12** (the two legs); **24 ≡ 30 and 25 ≡ 31** (the two arms) ⇒ **4 alkyne-carbon signals in total**.
**L2 · Thought** The legs are interchangeable as whole units (via ring 1's mirror) and likewise the arms (via ring 2's mirror); within one –C≡C– the two carbons are *not* equivalent (one touches the ring, the other touches CH₂/C(CH₃)₃), so each triple bond contributes two signals: 4 triple bonds × 2 ÷ 2 (pairwise equivalence) = 4.

### (c) Methyl groups
**L1 · Answer** Ten methyls in **4 environments**: **1 ≡ 16** (the two leg-terminal CH₃); **27 ≡ 28 ≡ 29 ≡ 33 ≡ 34 ≡ 35** (the six tert-butyl methyls of the two equivalent arms); **40** (unique); **41** (unique).
**L2 · Thought** The tert-butyl methyls are equivalent by free rotation about C–C and by the arm-swap mirror — all six collapse into one signal. The surprise is the head: 40 and 41 sit on the same carbon (38) yet are **not** equivalent — on the chair-shaped 1,3-dioxane one is axial and one equatorial, ring flip is frozen on the NMR timescale, and no symmetry operation swaps them (the mirror through C36–C38 swaps 37 ≡ 39 but leaves 40 and 41 each in place). "Same carbon" ≠ "same environment" is the lesson of the whole question.

### (d) Total ¹³C environments
**L1 · Answer** benzene 8 + alkynes 4 + methyls 4 + OCH₂ (37 ≡ 39) 1 + acetal CH (36) 1 + quaternary C38 1 + quaternary C26 ≡ C32 1 + linker CH₂ (17) 1 + leg CH₂'s (2 ≡ 15, 3 ≡ 14) 2 = **23 signals**.
**L2 · Thought** Inventory audit (§7.3): count by *class*, then add. Every one of the 41 carbons must appear in exactly one bucket: 12 ring C → 8, 8 alkyne C → 4, 10 methyl C → 4, and the remaining 11 C (2 CH₂ legs ×2, linker, 26, 32, 36, 37, 38, 39) → 7. 8 + 4 + 4 + 7 = 23 ✓.

### (e) Coupling to 5 hydrogens
**L1 · Answer** n = 5 → (n + 1) = **6 peaks**, ratio **1 : 5 : 10 : 10 : 5 : 1** (the sixth row of Pascal's triangle).
**L2 · Thought** Extend the triangle one row beyond those printed: each entry is the sum of the two above it (1, 5, 10, 10, 5, 1 — symmetric by construction).

### (f) Assigning the ¹H spectrum (A–M)
**L1 · Answer**

| signal | H's | atoms | region / identity |
|---|---|---|---|
| A | 1H | **7** | aromatic H between the two legs (ring 1) |
| B | 2H | **19, 23** | aromatic pair on ring 2 |
| C | 2H | **9, 11** | aromatic pair flanking the linker on ring 1 |
| D | 1H | **36** | acetal methine O–CH(Ar)–O (~6 ppm) |
| E | 2H | **17** | linker CH₂ between the two rings |
| F | 2H | **37 and 39** | one H from each ring OCH₂ (diastereotopic pair) |
| G | 2H | **37 and 39** | the other H from each ring OCH₂ |
| H | 4H | **3, 14** | propargylic CH₂'s next to the leg triple bonds |
| I | 4H | **2, 15** | middle CH₂'s of the legs |
| J | 3H | **40 or 41** | one of the head methyls (axial/equatorial) |
| K | 18H | **27, 28, 29, 33, 34, 35** | the two tert-butyl "hands" |
| L | 6H | **1, 16** | terminal CH₃'s of the legs |
| M | 3H | **41 or 40** | the other head methyl |

Check: 1+2+2+1+2+2+2+4+4+3+18+6+3 = 50 H ✓ (matches C₄₁H₅₀O₂).

**L2 · Thought** Assign by elimination using integration × shift logic (§7.3), in decreasing order of certainty: (1) K = 18H can only be the six t-Bu methyls — nothing else holds 18 H; (2) L = 6H next: the two leg CH₃'s (the only remaining 6-H pool); (3) the aromatic band (~7.0–7.4 ppm) holds exactly 5 H: A (1H) must be the *unique* aromatic position 7, and B, C (2H each) are the two symmetry pairs — B was given as 19, 23, so C = 9, 11; (4) D (1H, ~6 ppm) can only be the acetal methine 36, the single CH between two oxygens; (5) E (2H) = the lone linker CH₂, atom 17; (6) F and G (2H each) are the four OCH₂ protons of 37 ≡ 39, split 2 + 2 because the two protons on each CH₂ are diastereotopic (axial vs equatorial) — the signal count forces "37 and 39" for *both* letters; (7) H, I (4H each) are the two leg CH₂ pairs — the propargylic pair 3, 14 (deshielded by the triple bond) lies downfield of 2, 15; (8) J and M (3H each) are 40 and 41, distinct as established in (c), and the paper itself allows "40 or 41" since no spectrum feature tells axial from equatorial. When two assignments are genuinely interchangeable, commit with the hedged "... or ..." form rather than re-deriving.

---

## Question 5 — The Breathalyser

### (a)(i) Oxidation of ethanol
**L1 · Answer** **CH₃CH₂OH + H₂O → CH₃CO₂H + 4 H⁺ + 4 e⁻**
**L2 · Thought** Ethanol → ethanoic acid adds one O and removes 2 H net... do it by the standard algorithm: balance O with H₂O (one on the left), then H with H⁺ (4 on the right: 6 H left vs 4 H right in acid + the 2 extra... precisely: left H = 6+2 = 8, right H = 4 + x → x = 4), then charge with e⁻ (right side +4 → 4 e⁻). ✓

### (a)(ii) Reduction of dichromate
**L1 · Answer** **Cr₂O₇²⁻ + 6 e⁻ + 14 H⁺ → 2 Cr³⁺ + 7 H₂O**
**L2 · Thought** The half-equation to memorise cold: Cr +6 → +3 is 3 e⁻ per Cr, so 6 e⁻ per dichromate; 7 O's need 14 H⁺ to become 7 H₂O; charge check: −2 − 6 + 14 = +6 = 2 × (+3). ✓

### (a)(iii) Overall equation
**L1 · Answer** LCM of 4 and 6 electrons = 12: 3 × oxidation + 2 × reduction:
**2 Cr₂O₇²⁻ + 3 CH₃CH₂OH + 16 H⁺ → 4 Cr³⁺ + 3 CH₃CO₂H + 11 H₂O**
**L2 · Thought** Cross-multiply the electron counts (3 × 4 e⁻ = 2 × 6 e⁻ = 12), add, and cancel: 28 H⁺ − 12 H⁺... precisely 3 H₂O cancel from the left and 28 − 12 = 16 H⁺ survive; final audit: Cr 4, C 6, H 34, O 49 = 49, charge +16 − 4 = +12 = 4 × 3. ✓

### (a)(iv) With potassium and sulfuric acid
**L1 · Answer** **2 K₂Cr₂O₇ + 3 CH₃CH₂OH + 8 H₂SO₄ → 2 K₂SO₄ + 2 Cr₂(SO₄)₃ + 3 CH₃CO₂H + 11 H₂O**
**L2 · Thought** Dress the ionic equation with spectators: 4 K⁺ and 16 H⁺ need 8 SO₄²⁻ on the left; on the right pair them up as 2 K₂SO₄ + 2 Cr₂(SO₄)₃ (sulfate: 2 + 6 = 8 ✓). Never leave K⁺ or SO₄²⁻ floating in a "molecular" equation.

### (b)(i) Breath concentration at the legal limit
**L1 · Answer** Blood: 80 mg per 100 cm³ = 800 mg per 1000 cm³. Breath = blood / 2300 → 800 / 2300 = 0.348 mg = **348 µg per 1000 cm³ of breath**.
**L2 · Thought** One division by the partition factor — but get the direction right: breath is *more dilute*, so divide. Convert mg → µg (×1000) only at the end.

### (b)(ii) Mass of K₂Cr₂O₇ for 3× the limit
**L1 · Answer** Ethanol to detect: 3 × 348 µg = 1044 µg = 1.044 × 10⁻³ g → n = 1.044 × 10⁻³ / 46.07 = 2.266 × 10⁻⁵ mol. Dichromate : ethanol = 2 : 3 → n(K₂Cr₂O₇) = ⅔ × 2.266 × 10⁻⁵ = 1.510 × 10⁻⁵ mol → mass = 1.510 × 10⁻⁵ × 294.19 = 4.44 × 10⁻³ g ≈ **4.45 mg**.
**L2 · Thought** Three multipliers to keep straight: the ×3 safety factor, the 2 : 3 redox ratio from (a)(iii), and M(K₂Cr₂O₇) = 294.19. Carry full precision (348 → 347.8...) and round at the end: 3 × 347.8 / 46.07 × ⅔ × 294.19 = 4.44 mg ≈ 4.45 mg ✓.

### (b)(iii) Colour change
**L1 · Answer** **Orange → green** (dichromate Cr(VI) is orange; the Cr³⁺ product is green).
**L2 · Thought** The colour IS the assay: each ethanol molecule reduces its share of orange Cr₂O₇²⁻ to green Cr³⁺, so the length of green stain gauges the dose.

---

## Question 6 — The synthesis of rimonabant

**L1 · Answers (structures; all SMILES machine-validated)**

| species | structure | SMILES |
|---|---|---|
| chlorobenzene | C₆H₅Cl | `Clc1ccccc1` |
| propanoyl chloride | CH₃CH₂COCl | `CCC(=O)Cl` |
| **A** | 1-(4-chlorophenyl)propan-1-one (4-chloropropiophenone), C₉H₉ClO | `CCC(=O)c1ccc(Cl)cc1` |
| **B** | lithium enolate of A, C₉H₈ClO⁻ Li⁺ | `CC=C([O-])c1ccc(Cl)cc1.[Li+]` |
| **C** | ethyl 4-(4-chlorophenyl)-3-methyl-2,4-dioxobutanoate, C₁₃H₁₃ClO₄ | `CCOC(=O)C(=O)C(C)C(=O)c1ccc(Cl)cc1` |
| **D** | ethyl 5-(4-chlorophenyl)-1-(2,4-dichlorophenyl)-4-methylpyrazole-3-carboxylate, C₁₉H₁₅Cl₃N₂O₂ | `CCOC(=O)c1nn(-c2ccc(Cl)cc2Cl)c(-c2ccc(Cl)cc2)c1C` |
| **E** | the carboxylic acid, C₁₇H₁₁Cl₃N₂O₂ | `O=C(O)c1nn(-c2ccc(Cl)cc2Cl)c(-c2ccc(Cl)cc2)c1C` |
| **F** | the acyl chloride, C₁₇H₁₀Cl₄N₂O | `O=C(Cl)c1nn(-c2ccc(Cl)cc2Cl)c(-c2ccc(Cl)cc2)c1C` |
| rimonabant | N-(piperidin-1-yl) amide, C₂₂H₂₁Cl₃N₄O | `O=C(NN1CCCCC1)c1nn(-c2ccc(Cl)cc2Cl)c(-c2ccc(Cl)cc2)c1C` |

**L2 · Thought** Walk the scheme by functional-group logic, using each printed by-product as a constraint:
- **A**: AlCl₃ + acyl chloride = Friedel–Crafts acylation; the printed HCl confirms electrophilic aromatic substitution, and Cl directs *para* (sterics beat the small ortho effect) → 4-chloropropiophenone.
- **B**: "strong lithium base −H" and the printed formula C₉H₈ClO⁻Li⁺ say exactly one α-H is removed → the kinetic enolate; the formula is the checksum (A minus H, plus Li).
- **C**: B + diethyl oxalate → printed LiOC₂H₅ means the enolate carbon has attacked an oxalate carbonyl and expelled ethoxide: a Claisen acylation installing –CO–CO₂Et on the α-carbon → ArCO–CH(CH₃)–CO–CO₂Et.
- **D**: C + 2,4-dichlorophenylhydrazine, **minus 2 H₂O** — two condensations must occur. The arylhydrazine's –NH₂ condenses at the ketone next to the aryl (C4) and the ring closes onto the central keto carbon (C2), expelling the second water; the ester survives untouched and becomes the pyrazole 3-substituent, the methyl lands at C4, the 4-chlorophenyl at C5, and the hydrazine's aryl on N1 — exactly rimonabant's substitution pattern. The "−2 H₂O" printed in the scheme is what forces a *double* condensation (pyrazole), not a simple hydrazone.
- **E**: KOH/MeOH then dilute HCl, with printed C₂H₅OH + KCl — saponification of the ethyl ester followed by acidic work-up → carboxylic acid. (The KCl comes from neutralising any potassium salts... precisely from the HCl work-up of the carboxylate/phenolate-free mixture.)
- **F**: SOCl₂ with printed SO₂ + HCl — the classic acid → acyl chloride conversion.
- **F → rimonabant**: the reagent drawn is 1-aminopiperidine, H₂N–N(CH₂)₅; its free –NH₂ attacks the acyl chloride, HCl is printed as the by-product, and the product is the N–N-linked amide: pyrazole-3-C(=O)–NH–N(piperidine). The hydrazide-style C(=O)NH–N< linkage is rimonabant's signature — check the final formula C₂₂H₂₁Cl₃N₄O against the validator ✓.

---

*End of Paper 21 (2005). Next: 2004 Round 1.*

---

# Paper 22 — 2004 UKChO Round 1 (36th IChO selection)

**Marks / time:** 7 questions (2 h).
**Theme map:** Q1 redox half-equations; Q2 marble erosion and barium conservation; Q3 Winkler dissolved-oxygen method; Q4 Agent Orange / 2,4,5-T synthesis and dioxin; Q5 tin pest thermodynamics; Q6 hydrogen-like ions in a supernova; Q7 asparagus-pee sulfur compounds.

---

## Question 1 — Redox half-equations (in aqueous acid)

**L1 · Answers**

| | half-equation | type |
|---|---|---|
| (a) | Fe³⁺ + e⁻ → Fe²⁺ | **reduction** (Fe +3 → +2) |
| (b) | 2 H⁺ + 2 e⁻ → H₂ | **reduction** (H +1 → 0) |
| (c) | MnO₄²⁻ → MnO₄⁻ + e⁻ | **oxidation** (Mn +6 → +7) |
| (d) | 2 SO₄²⁻ → S₂O₈²⁻ + 2 e⁻ | **oxidation** (peroxodisulfate forms; electrons leave) |
| (e) | NO₃⁻ + 2 H⁺ + e⁻ → NO₂ + H₂O | **reduction** (N +5 → +4) |
| (f) | H₂O₂ → O₂ + 2 H⁺ + 2 e⁻ | **oxidation** (O −1 → 0) |
| (g) | Cr₂O₇²⁻ + 14 H⁺ + 6 e⁻ → 2 Cr³⁺ + 7 H₂O | **reduction** (Cr +6 → +3) |

**L2 · Thought** One algorithm for all seven (§7.5 prescribed order): ① balance the element that changes oxidation state; ② balance O with H₂O; ③ balance H with H⁺ (acid solution); ④ balance charge with e⁻; ⑤ the side the electrons land on decides the label — electrons on the *left* (consumed) = reduction, on the *right* (released) = oxidation. The oxidation-state arithmetic decides electron count before any balancing: (c) and (d) are the traps — both are oxidations even though no obvious "oxidant" is named; in (d) two sulfates link through a peroxide –O–O– bridge, so 2 e⁻ must be expelled. Audit of (e): charge −1 + 2 − 1 = 0 ✓; of (g): −2 + 14 − 6 = +6 = 2 × (+3) ✓.

---

## Question 2 — Pollution and the Taj Mahal

### (a) CaCO₃ + carbonic acid
**L1 · Answer** **CaCO₃(s) + H₂CO₃(aq) → Ca(HCO₃)₂(aq)** (calcium hydrogencarbonate, which is soluble).
**L2 · Thought** Carbonic acid converts the insoluble carbonate into the soluble bicarbonate — erosion in one equation: solid → solution.

### (b)(i) CaCO₃ + sulfuric acid
**L1 · Answer** **CaCO₃ + H₂SO₄ → CaSO₄ + H₂O + CO₂**
**L2 · Thought** Strong acid displaces the weak-acid anion as CO₂ + H₂O; the sulfate is left as a solid deposit.

### (b)(ii) Why the conversion accelerates erosion
**L1 · Answer** CaSO₄ is about **350 times more soluble** than CaCO₃ (4.5 × 10⁻² vs 1.3 × 10⁻⁴ mol dm⁻³), so the sulfate layer dissolves in rain and is washed away, continually exposing fresh marble to attack.
**L2 · Thought** Use the supplied solubility table as the argument — the numbers are given precisely so the comparison is quantitative, not vague: the stone loses material whenever the reaction product can leave.

### (c) Hydrolysis of urea
**L1 · Answer** **CO(NH₂)₂ + H₂O → 2 NH₃ + CO₂**
**L2 · Thought** The stem dictates the products (ammonia and carbon dioxide); the water splits the C–N bonds, and the balance then writes itself (C 1, O 2 = 2, N 2, H 6 = 6 ✓).

### (d)(i) Ba(OH)₂ + CO₂
**L1 · Answer** **Ba(OH)₂ + CO₂ → BaCO₃ + H₂O**
**L2 · Thought** Base + acidic oxide → carbonate + water, 1 : 1 — same pattern as limewater.

### (d)(ii) Why BaCO₃ slows erosion
**L1 · Answer** BaCO₃ is **even less soluble than CaCO₃** (9.1 × 10⁻⁵ vs 1.3 × 10⁻⁴ mol dm⁻³), so it precipitates inside the pores and on the surface as a coherent, insoluble mineral layer that binds the stone and shields it from acidic rainwater.
**L2 · Thought** Same solubility-table logic as (b)(ii), run in reverse: depositing something *less* soluble than the substrate protects; depositing something *more* soluble destroys.

### (e)(i) BaCO₃ + SO₂ + O₂
**L1 · Answer** **2 BaCO₃ + 2 SO₂ + O₂ → 2 BaSO₄ + 2 CO₂**
**L2 · Thought** Sulfur is oxidised +4 → +6, so atmospheric O₂ must appear as the oxidant (the stem says "in the presence of oxygen"): each O₂ accepts the 4 e⁻ from two SO₂. Audit: Ba 2, C 2, S 2, O 6 + 4 + 2 = 12 = 8 + 4 ✓.

### (e)(ii) Speed up or slow down?
**L1 · Answer** **Slow down.** BaSO₄ is the least soluble substance in the whole table (9.4 × 10⁻⁶ mol dm⁻³, ~14 × less soluble than even CaCO₃), so the sulfate crust is a tough, insoluble, chemically resistant skin that keeps acid rain away from the stone beneath.
**L2 · Thought** The question trains a single judgement — *fate of the reaction product decides the rate of material loss* — applied three times with three different solubilities. BaSO₄ is so insoluble it is essentially permanent (it is the basis of the "barium meal" precisely because it neither dissolves nor reacts).

---

## Question 3 — Dissolved oxygen (the Winkler method)

### (a)(i) Oxidation of Mn(OH)₂ by O₂
**L1 · Answer** **4 Mn(OH)₂ + O₂ + 2 H₂O → 4 Mn(OH)₃**
**L2 · Thought** Mn²⁺ → Mn³⁺ releases 1 e⁻ per Mn; O₂ → hydroxide takes 4 e⁻ (O₂ + 2 H₂O + 4 e⁻ → 4 OH⁻), hence 4 Mn per O₂. Audit: Mn 4, O 8 + 2 + 2 = 12 = 12, H 8 + 4 = 12 ✓.

### (a)(ii) Oxidation of KI by Mn(OH)₃
**L1 · Answer** **2 Mn(OH)₃ + 2 KI → 2 Mn(OH)₂ + I₂ + 2 KOH**
**L2 · Thought** Each Mn³⁺ takes 1 e⁻ back down to Mn²⁺; two I⁻ give 2 e⁻ to become I₂ — so 2 Mn(OH)₃ per I₂. Write it with the K⁺/OH⁻ spectators balanced as compounds, then audit: Mn 2, I 2, K 2, O 6 = 4 + 2, H 6 = 4 + 2 ✓.

### (b) Indicator
**L1 · Answer** **Starch solution** — deep blue-black with iodine, turning colourless at the end-point (added near the end, when the iodine colour has faded to pale straw).
**L2 · Thought** The standard indicator for any iodine/thiosulfate titration; the intense starch–triiodide complex gives a sharp endpoint at very low residual I₂.

### (c) Dissolved oxygen concentration
**L1 · Answer** n(S₂O₃²⁻) = 25.0 × 10⁻³ dm³ × 0.00100 mol dm⁻³ = 2.50 × 10⁻⁵ mol → n(I₂) = 1.25 × 10⁻⁵ mol (2 : 1) → n(O₂) = n(I₂) / 2 = 6.25 × 10⁻⁶ mol in 25.0 cm³ (each O₂ generates 4 Mn³⁺, which liberate 2 I₂) → c(O₂) = 6.25 × 10⁻⁶ / 0.0250 = 2.50 × 10⁻⁴ mol dm⁻³ → × 32.00 g mol⁻¹ = 8.00 × 10⁻³ g dm⁻³ = **8.00 mg dm⁻³** (above the 5 mg dm⁻³ fish-survival threshold).
**L2 · Thought** Chain the mole ratios through all three reactions before touching volumes (§7.5): O₂ : Mn(OH)₃ : I₂ : S₂O₃²⁻ = 1 : 4 : 2 : 4, i.e. n(O₂) = n(S₂O₃²⁻)/4. The whole titration is an amplifier — one O₂ molecule ultimately consumes four thiosulfates — which is exactly why the method is "one of the most accurate".

### (d) The colourless gas
**L1 · Answer** **NO** (nitrogen monoxide); in air: **2 NO + O₂ → 2 NO₂** (brown nitrogen dioxide).
**L2 · Thought** "Colourless gas turning brown in air" is the fingerprint of NO — nothing else common does it; the brown product is NO₂.

### (e) Iodide + nitrate(III)
**L1 · Answer** **2 NO₂⁻ + 2 I⁻ + 4 H⁺ → 2 NO + I₂ + 2 H₂O**
**L2 · Thought** N goes +3 → +2 (1 e⁻ each, 2 total) matching 2 I⁻ → I₂ + 2 e⁻; then the standard algorithm: O balanced by 2 H₂O, H by 4 H⁺, charge −2 − 2 + 4 = 0 ✓. The NO product is consistent with part (d)'s observation — use the observation as the product constraint, not as an afterthought.

### (f) Nitrate(III) + azide
**L1 · Answer** **NO₂⁻ + N₃⁻ + 2 H⁺ → N₂ + N₂O + H₂O**
**L2 · Thought** The two gaseous products are given, so this is a balance-by-construction with an oxidation-state checksum: N in NO₂⁻ is +3, the azide nitrogens average −⅓, total +2 on the left; N₂ contributes 0 and N₂O contributes 2 × (+1) = +2 on the right ✓ (a comproportionation — the two nitrogen species meet in the middle). Atoms: N 4 = 4, O 2 = 2, H 2 = 2; charge −1 − 1 + 2 = 0 ✓. This scavenges the NO₂⁻ before it can liberate iodine.

---

## Question 4 — Agent Orange

### (a) 1,2,4,5-tetrachlorobenzene
**L1 · Answer** Benzene ring with **Cl on positions 1, 2, 4, 5** and H on 3 and 6 (`Clc1cc(Cl)c(Cl)cc1Cl`, C₆H₂Cl₄ ✓). The two H's are related by the ring's mirror/C₂ symmetry → one 2H singlet, exactly as the printed spectrum shows.
**L2 · Thought** Read the spectrum backwards: a single 2H aromatic signal demands two *equivalent* ring hydrogens, which only the 1,2,4,5-pattern supplies among tetrachlorobenzenes (§7.3 orbit counting).

### (b) Intermediate X
**L1 · Answer** **2,4,5-trichlorophenol** (`Oc1cc(Cl)c(Cl)cc1Cl`, C₆H₃Cl₃O ✓): hot NaOH substitutes **one** ring Cl by OH (nucleophilic aromatic substitution); acidification protonates the phenoxide.
**L2 · Thought** Evidence chain: X's spectrum shows three 1H signals — two aromatic (the formerly equivalent H's are now distinct, so substitution happened) plus the 5.8 ppm signal that vanishes on D₃O⁺ treatment → an exchangeable O–H (phenol). Only one Cl is replaced (three Cl's survive into 2,4,5-T), and OH lands where a Cl was.

### (c) Systematic name of X
**L1 · Answer** **2,4,5-trichlorophenol** (phenol C1 = OH carbon; chlorines at 2, 4, 5).
**L2 · Thought** Phenol is the parent (OH outranks Cl); number from the OH carbon to give the lowest locant set {2,4,5} rather than {3,4,6}.

### (d) X after D₃O⁺ work-up
**L1 · Answer** The same molecule with **O–D instead of O–H**: 2,4,5-trichlorophenol-O-d (`Oc1cc(Cl)c(Cl)cc1Cl` with the hydroxyl proton replaced by ²H).
**L2 · Thought** The acidic D₃O⁺ exchanges the labile phenolic proton only — the ring C–H bonds are untouched — which is precisely why the 5.8 ppm signal disappears (²H is silent in a ¹H spectrum).

### (e) Chloroethanoic acid
**L1 · Answer** **ClCH₂COOH** (`O=C(O)CCl`, C₂H₃ClO₂ ✓).
**L2 · Thought** "Ethanoic acid" = two carbons; "chloro" on the only available carbon (the methyl) — no ambiguity possible.

### (f) 2,4,5-T
**L1 · Answer** **(2,4,5-trichlorophenoxy)ethanoic acid**: 2,4,5-Cl₃C₆H₂–O–CH₂–COOH (`O=C(O)COc1cc(Cl)c(Cl)cc1Cl`, C₈H₅Cl₃O₃ ✓) — the phenoxide does a Williamson S_N2 on ClCH₂COOH, installing the –O–CH₂–COOH side chain.
**L2 · Thought** NaOH deprotonates the phenol (phenoxide is a far better nucleophile), the phenoxide displaces chloride from the chloroacid's CH₂, and the second acidification restores the carboxylic acid. The NMR confirms: the OH signal is gone, a 2H signal appears (~4.8 ppm, O–CH₂), two aromatic 1H signals remain, and a far-downfield 1H (COOH) appears in DMSO.

### (g) Signal assignments in 2,4,5-T
**L1 · Answer** **D (2H) = the O–CH₂ group** (the only 2H signal; deshielded by the oxygen); **A (1H, furthest downfield) = COOH**; **B and C (1H each) = the two aromatic H's** — B (downfield) = H-3, flanked by two chlorines; C (upfield) = H-6, next to the ether oxygen. (B and C are the honest residual ambiguity; both are singlets because the two ring protons are *para*-related and do not couple observably.)
**L2 · Thought** Integration disposes of D and A immediately (2H and far-downfield-acid are unique). For the aromatic pair, coupling topology gives nothing (para H–H coupling ≈ 0 → two singlets), so only the shift argument remains: the proton between the two chlorines sits further downfield than the proton beside the oxygen. State the assignment with the hedge — "as far as you are able" licenses exactly this.

### (h) Dioxin
**L1 · Answer** **2,3,7,8-tetrachlorodibenzo-1,4-dioxin (TCDD)**: two 2,4,5-trichlorophenol units joined head-to-head by **two oxygen bridges** between their C1 oxygens and each other's ortho (C2) positions — a central 1,4-dioxin ring fused to two benzene rings, with Cl at 2, 3, 7, 8 (`Clc1cc2c(cc1Cl)Oc1cc(Cl)c(Cl)cc1O2`, C₁₂H₄Cl₄O₂ ✓, three 6-rings ✓).
**L2 · Thought** Balance-first structure determination (§7.3): 2 C₆H₃Cl₃O + 2 NaOH − 2 NaCl − 2 H₂O = C₁₂H₄Cl₄O₂ — the product has lost **2 Cl and 2 H** from the pair, i.e. two SNAr events in which each phenoxide oxygen displaces the *ortho*-chlorine of the other ring, closing the six-membered O–C–C–O–C–C central ring. The single 7.2 ppm ¹H signal then decides the symmetry: all four remaining aromatic H's (positions 1, 4, 6, 9) must be equivalent, which only the symmetric 2,3,7,8-pattern delivers (two mirror planes). The molecule is the infamous "dioxin" — flat, symmetric, and extraordinarily toxic.

---

## Question 5 — Tin pest

### (a) ΔrH for white → grey
**L1 · Answer** ΔrH = ΔfH(grey) − ΔfH(white) = −2.09 − 0 = **−2.09 kJ mol⁻¹**.
**L2 · Thought** Products minus reactants; the element's reference form (white tin) is zero by definition.

### (b) ΔrS
**L1 · Answer** ΔrS = S(grey) − S(white) = 44.1 − 51.4 = **−7.3 J K⁻¹ mol⁻¹**.
**L2 · Thought** Same products-minus-reactants pattern applied to absolute entropies (the stem explicitly invites it); a negative value makes sense — the denser... rather, the more ordered covalent diamond-type lattice has lower entropy than the metal.

### (c) ΔrG at 25 °C
**L1 · Answer** ΔrG = ΔrH − TΔrS = −2090 − 298 × (−7.3) = −2090 + 2175 = **+85 J mol⁻¹ (+0.085 kJ mol⁻¹)**.
**L2 · Thought** Watch the units (kJ vs J — convert ΔH to joules or ΔS to kJ before mixing) and the double negative: −TΔrS with ΔrS < 0 is a *positive*, destabilising term that grows with T.

### (d) Stable allotrope at room temperature
**L1 · Answer** **White tin.** ΔrG for white → grey is positive (+85 J mol⁻¹) at 298 K, so the conversion cannot take place; white tin is the stable form at 25 °C.
**L2 · Thought** Direct application of the stem's feasibility rule: ΔrG > 0 ⇒ process cannot occur. (The margin is tiny — which is why tin pest is a real phenomenon only in cold churches and polar expeditions.)

### (e) Critical temperature Tc
**L1 · Answer** Equilibrium ⇔ ΔrG = 0: Tc = ΔrH / ΔrS = (−2090 J mol⁻¹)/(−7.3 J K⁻¹ mol⁻¹) = **286 K (13 °C)**. Below Tc the negative ΔH wins and grey tin becomes the stable form.
**L2 · Thought** Both ΔH and ΔS are negative, so the ratio is positive and meaningful; the sign logic tells you the direction of the switch: cooling favours the exothermic direction (white → grey) — the classic entropy-vs-enthalpy crossover.

### (f) Percentage volume increase
**L1 · Answer** For a fixed mass, V ∝ 1/ρ: V_grey/V_white = ρ_white/ρ_grey = 7.31/5.75 = 1.271 → **volume increases by 27 %** (27.1 %).
**L2 · Thought** Density converts with the *reciprocal* — the common slip is computing 5.75/7.31 (which would give a shrinkage, contradicting the premise of "warts" bursting the surface). The ~27 % expansion is what cracks organ pipes.

### (g) Greater coordination number
**L1 · Answer** **White tin.** Its atoms pack at a *longer* nearest-neighbour distance (302 pm vs 280 pm) yet give a *higher* density (7.31 vs 5.75 g cm⁻³) — only possible if each atom has **more neighbours** (metallic close-type packing, CN = 6 in distorted form). Grey tin has the diamond structure: four short, strong covalent bonds (CN = 4, 280 pm) in an open, low-density lattice.
**L2 · Thought** The two data columns argue together: grey tin's shorter distance reflects fewer, stronger, directional covalent bonds; white tin's longer distance with higher density implies a higher coordination number — density = (mass per atom × atoms per volume), so more neighbours at slightly longer range wins. Coordination number is counted, not guessed from bond length alone.

---

## Question 6 — A supernova (hydrogen-like ions)

### (a) Energy of the 2p electron in H
**L1 · Answer** E₂ = −R_H × Z²/n² = −2.179 × 10⁻¹⁸ × 1/4 = **−5.45 × 10⁻¹⁹ J** (−5.448 × 10⁻¹⁹ J).
**L2 · Thought** Direct substitution with Z = 1, n = 2 (2p means n = 2); keep the minus sign — bound states are below the zero of the free electron.

### (b) Promotion energy 1s → 2p
**L1 · Answer** ΔE = E₂ − E₁ = (−R_H/4) − (−R_H) = ¾ R_H = **1.63 × 10⁻¹⁸ J** (1.634 × 10⁻¹⁸ J).
**L2 · Thought** Energy *needed* = final minus initial; the ¾ factor (1 − 1/4) is the Lyman-series fingerprint and recurs in (d)–(f).

### (c) Ionisation energy of He⁺
**L1 · Answer** He⁺ has Z = 2, one electron, n = 1: IE = R_H × 2²/1² = 4 × 2.179 × 10⁻¹⁸ = **8.72 × 10⁻¹⁸ J** (per ion).
**L2 · Thought** Ionisation = promotion to n = ∞, where E = 0, so IE = |E₁|; the Z² scaling quadruples hydrogen's value.

### (d) Hydrogen Lyman-α frequency
**L1 · Answer** f = ΔE/h = 1.634 × 10⁻¹⁸ / 6.626 × 10⁻³⁴ = **2.47 × 10¹⁵ Hz** (2.466 × 10¹⁵ Hz).
**L2 · Thought** Reuse part (b)'s ΔE unchanged (emission energy = absorption energy for the same gap) — one division by h. This is the ultraviolet Lyman-α line.

### (e) O⁷⁺ Lyman-α frequency
**L1 · Answer** O⁷⁺: one electron left, Z = 8. ΔE scales by Z² = 64: ΔE = 48 R_H = 1.046 × 10⁻¹⁶ J; f = 1.046 × 10⁻¹⁶ / 6.626 × 10⁻³⁴ = **1.58 × 10¹⁷ Hz**.
**L2 · Thought** Same ¾ factor, new Z: f(O⁷⁺) = 64 × f(H) = 64 × 2.466 × 10¹⁵ = 1.58 × 10¹⁷ Hz — X-ray frequencies, detectable by Chandra exactly as the stem's photograph caption says. Scaling an already-computed transition by Z² is faster and less error-prone than recomputing from scratch.

### (f) Element with Lyman-α at 2.471 × 10¹⁷ Hz
**L1 · Answer** ΔE = hf = 6.626 × 10⁻³⁴ × 2.471 × 10¹⁷ = 1.637 × 10⁻¹⁶ J. Z² = ΔE/(¾ R_H) = 1.637 × 10⁻¹⁶ / 1.634 × 10⁻¹⁸ = 100.2 ≈ 100 → Z = 10 → **neon (Ne⁹⁺)**.
**L2 · Thought** Invert the same relation: the ¾ R_H unit is the universal Lyman-α yardstick, so the quotient is Z² directly. 100.2 lands within 0.2 % of a perfect square — the near-integer check (§4 quantum-ladder spectroscopy) confirms the identification rather than merely suggesting it.

---

## Question 7 — Asparagus-pee

### (a) Role of DCC
**L1 · Answer** **iii) dehydrating agent** — DCC couples the carboxylic acid and the thiol into a thioester by removing the elements of water, itself becoming the printed urea by-product R–NH–CO–NH–R (dicyclohexylurea).
**L2 · Thought** The by-product drawn beside every DCC step is the evidence: R–NH–CO–NH–R is DCC plus H₂O, so DCC must have absorbed water from the coupling partners — the definition of a dehydrating (coupling) agent.

### (b) Structures (all SMILES machine-validated)

| | structure | SMILES | formula / M |
|---|---|---|---|
| **A** | S-methyl prop-2-enethioate, CH₂=CH–C(=O)–S–CH₃ | `C=CC(=O)SC` | C₄H₆OS, **102** ✓ |
| **W** | 3-sulfanylpropanoic acid, HS–CH₂CH₂–COOH | `O=C(O)CCS` | C₃H₆O₂S |
| **X** | 3-(methylthio)propanoic acid, CH₃S–CH₂CH₂–COOH | `CSCCC(=O)O` | C₄H₈O₂S |
| **B** | S-methyl 3-(methylthio)propanethioate, CH₃S–CH₂CH₂–C(=O)–S–CH₃ | `CSCCC(=O)SC` | C₅H₁₀OS₂, **150** ✓ |
| **Y** | S-methyl 3-bromopropanethioate, Br–CH₂CH₂–C(=O)–S–CH₃ | `O=C(SC)CCBr` | C₄H₇BrOS, **182/184** ✓ |
| **Z1 / Z2** | (R)- and (S)-S-methyl 2,3-dibromopropanethioate, BrCH₂–CHBr–C(=O)–S–CH₃ | `O=C(SC)C(Br)CBr` | C₄H₆Br₂OS, **260/262/264** ✓ |

**L2 · Thought** Mass-led decoding, one step at a time:
- **A**: propenoic acid (72) + CH₃SH (48) − H₂O (DCC!) = 102 = M⁺ exactly → a **thioester**, CH₂=CH–C(=O)–SCH₃. The DCC by-product confirms a dehydration, and the surviving C=C is needed for the later HBr/Br₂ additions.
- **W**: H₂S adds across acrylic acid's C=C (Michael-style conjugate addition, S to the β-carbon) → HS–CH₂CH₂–COOH.
- **X**: CH₃I methylates the thiol sulfur (the most nucleophilic site) → CH₃S–CH₂CH₂–COOH.
- **B**: X (120) + CH₃SH (48) − H₂O = 150 = M⁺ exactly → the second DCC thioesterification, now of X's carboxyl group → CH₃S–CH₂CH₂–C(=O)–SCH₃. Two different sulfur environments (thioether and thioester), one formula checksum.
- **Y**: A + HBr (81) = 183 → one Br (the 1 : 1 M⁺ doublet at 182/184). HBr adds to the C=C; of the two regioisomers only **BrCH₂CH₂–C(=O)–SCH₃ has no stereocentre**, matching "Y is not optically active" (conjugate addition puts Br on the terminal β-carbon; the alternative CH₃–CHBr– product would be chiral).
- **Z1/Z2**: A + Br₂ (160) = 262 → two Br's (the 1 : 2 : 1 triplet at 260/262/264, the classic Br₂ binomial envelope). Addition across the C=C gives BrCH₂–CHBr–C(=O)–SCH₃ with **exactly one stereocentre** (C2: H, Br, CH₂Br, C(=O)SCH₃) → a pair of enantiomers, (R) and (S) = Z1 and Z2, formed as the racemate. The isotope pattern and the stereochemistry cross-validate the same structure.

### (c) Hydrolysis equations
**L1 · Answer**
**A: CH₂=CH–C(=O)–SCH₃ + H₂O → CH₂=CH–COOH + CH₃SH**
**B: CH₃S–CH₂CH₂–C(=O)–SCH₃ + H₂O → CH₃S–CH₂CH₂–COOH + CH₃SH**
(the mark scheme also accepts the double hydrolysis B + 2 H₂O → HS–CH₂CH₂–COOH + 2 CH₃SH — both sulfurs cleaved; the single thioester cleavage above is the primary answer).
**L2 · Thought** Thioesters hydrolyse by acyl–sulfur cleavage: water's OH takes the acyl carbon (→ carboxylic acid) and its H takes the sulfur (→ free thiol). In B only the *thioester* S–Me is cleaved under the mild reading — the thioether S–Me further down the chain is inert — so one methanethiol is released per molecule in each case, matching the stem's "releasing methanethiol" (the scheme's "OR" variant drives both S–Me groups off; note it, but write the clean one). Atom audit for B: left C₅H₁₂O₂S₂; right C₄H₈O₂S + CH₄S = C₅H₁₂O₂S₂ ✓.

---

*End of Paper 22 (2004). Next: 2003 Round 1.*

---

# Paper 23 — 2003 UKChO Round 1 (35th IChO selection)

**Marks / time:** 8 questions (2 h).
**Theme map:** Q1 self-heating coffee can (CaO hydration); Q2 Reinecke's salt composition; Q3 green chemistry / atom economy; Q4 redox equations; Q5 historical combining proportions; Q6 hydroxylamine–Fe³⁺ titration; Q7 flunitrazepam (Rohypnol) synthesis; Q8 polonium radioactivity and simple-cubic structure.

---

## Question 1 — Heating a cup of coffee

### (a) CaO + water
**L1 · Answer** **CaO + H₂O → Ca(OH)₂**
**L2 · Thought** Basic oxide + water → hydroxide ("slaking"); 1 : 1 : 1 with nothing left over.

### (b) Rate vs pH (fastest first)
**L1 · Answer** **acidic, neutral, basic** (fastest first).
**L2 · Thought** The rate asked about is the rate of the *heating reaction* of CaO with the solution. In acid the oxide/hydroxide surface is attacked directly and dissolved as fast as it forms (CaO + 2 H⁺ → Ca²⁺ + H₂O is diffusion-limited fast, keeping fresh surface exposed), so heat release is fastest; in neutral water the plain hydration runs at its intrinsic rate; in base the common-ion hydroxide suppresses the dissolution step of the hydration (the Ca(OH)₂ surface layer sits undisturbed and passivates), so the observed heating is slowest. Note the can's dilute NaOH/KOH is the *control* medium — chosen precisely because base gives a manageable, slowed rate. (An "OH⁻-catalysis" intuition suggests the reverse order; the observed order acidic > neutral > basic is the consistent reading of the surface chemistry — acid keeps the surface clean, base passivates it.)

### (c) ΔrH of the reaction
**L1 · Answer** ΔrH = ΔfH(Ca(OH)₂) − [ΔfH(CaO) + ΔfH(H₂O)] = −1003 − (−635 − 286) = **−82 kJ mol⁻¹**.
**L2 · Thought** Products minus reactants with the three supplied formation enthalpies; the negative sign (exothermic) is the sanity check — the can exists precisely because this reaction releases heat.

### (d) Energy to warm the coffee
**L1 · Answer** Q = mcΔT = 210 g × 4.18 J K⁻¹ g⁻¹ × 40 K = 35 112 J ≈ **35.1 kJ** (35 kJ).
**L2 · Thought** 210 cm³ of water-based coffee = 210 g (density 1 g cm⁻³, implicit in "heat capacity as for water"); Q = mcΔT in one line.

### (e) Minimum mass of CaO
**L1 · Answer** n(CaO) = 35.112 kJ / 82 kJ mol⁻¹ = 0.428 mol → mass = 0.428 × 56.08 = **24 g**.
**L2 · Thought** "Minimum" = 100 % heat-transfer efficiency assumed; divide energy by molar enthalpy to get moles, then × M(CaO) = 56.08. Carry 82 exactly (not 82.0-rounded mid-values) and round only at the end.

---

## Question 2 — Reinecke's salt, NH₄[Cr(SCN)ₓ(NH₃)ᵧ]

### (a) x and y
**L1 · Answer** Per 100 g: n(Cr) = 15.5/52.00 = 0.298; n(S) = 38.15/32.06 = 1.190; n(N) = 29.2/14.01 = 2.084. Ratios: S/Cr = 3.99 ≈ 4 → **x = 4**; N/Cr = 6.99 ≈ 7, and the formula already contains 1 N (NH₄⁺) + 4 N (4 SCN) = 5 → y = 7 − 5 = **2**. Salt: **NH₄[Cr(SCN)₄(NH₃)₂]**; check: M = 336.4 → Cr 15.46 %, S 38.12 %, N 29.15 % ✓ against all three data.
**L2 · Thought** Percentage-to-ratio in one pass (§7.5), then the subtlety: the nitrogen total counts *three* sources (counter-ion, thiocyanates, ammines) — subtract the known ones before reading off y. Close with the full percentage back-check on the proposed formula, which here matches to better than 0.05 % on every element.

### (b) Oxidation number of chromium
**L1 · Answer** Anion charge = −1 (balances NH₄⁺): Cr + 4(−1) + 2(0) = −1 → **Cr = +3**.
**L2 · Thought** SCN⁻ is −1, NH₃ is neutral; the counter-ion fixes the anion's total charge before any algebra.

### (c) Shape of the anion
**L1 · Answer** **Octahedral** — six monodentate ligands (4 SCN⁻ + 2 NH₃) around Cr(III), a d³ ion with no Jahn–Teller ambiguity.
**L2 · Thought** Coordination number first (6), then the geometry is automatic for six identical-typed donor atoms.

### (d) Two structures + isomerism
**L1 · Answer** **cis- and trans-[Cr(SCN)₄(NH₃)₂]⁻**: the two NH₃ ligands adjacent (90° apart) vs opposite (180° apart) on the octahedron. This is **geometrical (cis–trans) isomerism**.
**L2 · Thought** With formula MA₄B₂ on an octahedron there are exactly two arrangements (the 1,2- and 1,6-positions); the four SCN fill the rest identically in both. (Linkage isomers NCS vs SCN also exist in principle, but the formula given fixes SCN throughout — the cis/trans pair is the intended answer.)

---

## Question 3 — Green chemistry

### (a)(i) Overall chlorohydrin-route equation
**L1 · Answer** Adding the two steps and cancelling ClCH₂CH₂OH, HCl and one H₂O:
**C₂H₄ + Cl₂ + Ca(OH)₂ → C₂H₄O + CaCl₂ + H₂O**
**L2 · Thought** Add step equations, cancel species appearing on both sides (ClCH₂CH₂OH and HCl cancel completely; one of the two waters survives on the right). Audit: C 2, H 6 = 4 + 2, O 2 = 2, Cl 2, Ca 1 ✓.

### (a)(ii) Atom economy of the chlorohydrin route
**L1 · Answer** AE = M(C₂H₄O) / M(all products) × 100 = 44.05 / (44.05 + 110.98 + 18.02) × 100 = 44.05/173.05 × 100 = **25 %** (25.5 %).
**L2 · Thought** The denominator is ALL products of the *overall* equation (not the reactants — equivalent by mass conservation, but the definition printed uses products): CaCl₂ (110.98) is the dead weight here, four-fifths of the mass ending as waste.

### (b) Atom economy of the petrochemical route
**L1 · Answer** **100 %** — the only product is C₂H₄O; every atom of C₂H₄ and ½ O₂ ends up in it.
**L2 · Thought** Addition/oxidation with no co-product is the ideal the chlorohydrin route fails to reach; no arithmetic needed beyond noticing a single product.

### (c) The BHC ibuprofen process
**L1 · Answer**
i) Overall: isobutylbenzene (C₁₀H₁₄) + (CH₃CO)₂O + H₂ + CO → ibuprofen (C₁₃H₁₈O₂) + CH₃CO₂H. Atom audit: C 15 = 15, H 22 = 22, O 4 = 4 ✓. AE = 206.28 / (206.28 + 60.05) × 100 = **77 %** (77.5 %).
ii) **HF is the catalyst** for step 1 — the strong-acid catalyst of the Friedel–Crafts acylation of isobutylbenzene by ethanoic anhydride (it is not consumed; para-acylation gives the 4-isobutylacetophenone shown).
iii) **If the ethanoic acid is recovered and reused (to make more anhydride), the atom economy rises towards ~100 %** — the sole by-product is recycled back into the process, so effectively every atom ends up in ibuprofen.
**L2 · Thought** Build the overall equation from the three step schemes (acylation → H₂/Ni reduction of the ketone to the secondary alcohol → Pd-catalysed carbonylation inserting CO between the carbinol carbon and OH... precisely: the benzylic alcohol + CO → arylpropionic acid), then the atom-economy formula once. The HF question tests whether "catalyst" is distinguished from "reagent": it appears above the arrow and in no product. Part (iii) shows atom economy is a *process* property, not a reaction property — recycling the by-product stream is what made BHC's route famous.

---

## Question 4 — Redox equations (half-equation method)

**L1 · Answers**
(a) **Zn + Cu²⁺ → Zn²⁺ + Cu** (Zn + CuSO₄ → ZnSO₄ + Cu)
(b) **Cl₂ + 2 Br⁻ → 2 Cl⁻ + Br₂** (Cl₂ + 2 NaBr → 2 NaCl + Br₂)
(c) **Mg + 2 HCl → MgCl₂ + H₂**
(d) **MnO₂ + 4 HCl → MnCl₂ + Cl₂ + 2 H₂O**
(e) **5 SO₃²⁻ + 2 MnO₄⁻ + 6 H⁺ → 5 SO₄²⁻ + 2 Mn²⁺ + 3 H₂O**
(f) **3 Sn²⁺ + Cr₂O₇²⁻ + 14 H⁺ → 3 Sn⁴⁺ + 2 Cr³⁺ + 7 H₂O**
(g) **5 FeC₂O₄ + 3 MnO₄⁻ + 24 H⁺ → 5 Fe³⁺ + 10 CO₂ + 3 Mn²⁺ + 12 H₂O**

**L2 · Thought** One workflow for all seven: write the two half-equations, scale to the LCM of the electron counts, add, audit atoms + charge.
- (a)–(c) are one- or two-electron metatheses of displacement: Zn → Zn²⁺ + 2 e⁻ with Cu²⁺ + 2 e⁻ → Cu; Cl₂ + 2 e⁻ → 2 Cl⁻ with 2 Br⁻ → Br₂ + 2 e⁻; Mg → Mg²⁺ + 2 e⁻ with 2 H⁺ + 2 e⁻ → H₂. The observations are the checksums: copper plates out / solution pales; bromine's orange appears; hydrogen effervesces.
- (d) Mn(IV) → Mn(II) takes 2 e⁻; 2 Cl⁻ → Cl₂ + 2 e⁻ supplies them; the yellow-green gas (Cl₂) confirms which half runs as oxidation. Balance O with 2 H₂O, H with 4 H⁺ → 4 HCl total.
- (e) S +4 → +6 (2 e⁻ per sulfite) vs Mn +7 → +2 (5 e⁻): LCM 10 → 5 SO₃²⁻ : 2 MnO₄⁻; charge audit −6 = −6 ✓.
- (f) Sn²⁺ → Sn⁴⁺ (2 e⁻) vs Cr₂O₇²⁻ + 14 H⁺ + 6 e⁻ → 2 Cr³⁺ + 7 H₂O: LCM 6 → 3 : 1; the green Cr³⁺ confirms the product side.
- (g) The trap: **iron(II) ethanedioate is oxidised at BOTH centres** — Fe²⁺ → Fe³⁺ (1 e⁻) and C₂O₄²⁻ → 2 CO₂ (2 e⁻) = 3 e⁻ per formula unit; LCM with 5 e⁻ (MnO₄⁻) = 15 → 5 : 3. Forgetting the oxalate oxidation (using 1 e⁻) is the designed error; the full audit catches it: charge +21 = +21, O 32 = 32 ✓.

---

## Question 5 — Combining proportions of the elements

### (a) Formula of the antimony calx
**L1 · Answer** 12 grains Sb → 14.4 grains calx (theoretical) ⇒ oxygen taken up = 2.4 grains. n(Sb) : n(O) = 12/121.75 : 2.4/16.00 = 0.0986 : 0.150 = 1 : 1.52 ≈ 2 : 3 → **Sb₂O₃**.
**L2 · Thought** Mass gain IS the oxygen mass — the whole Lavoisier insight; divide each by its atomic mass and hunt the simple ratio (1.5 = 3/2 → double to integers).

### (b) Theoretical mass of zinc calx
**L1 · Answer** 1 Drachm = 60 grains Zn; ZnO mass = 60 × M(ZnO)/M(Zn) = 60 × 81.37/65.37 = **74.7 grains**.
**L2 · Thought** All the zinc ends up in the product, so scale by the molar-mass ratio ZnO/Zn — the gain (14.7 grains) is the oxygen that 60 grains of Zn can hold.

### (c) The fraction α converted
**L1 · Answer** Mass gained = 6 grains = mass of O in the ZnO formed = α × 60 × (16.00/65.37) grains → α = 6 / 14.69 = **0.41** (0.409). Hence: **zinc oxide = α × 74.7 = 30.5 grains; unreacted zinc = 60 × (1 − α) = 35.5 grains** (total 66.0 = 60 + 6 ✓). (Mark scheme, with Zn = 65.4: α = 0.412, ZnO = 30.7 grains, Zn left = 35.3 grains — same answers at the data's precision.)
**L2 · Thought** Anchor on the *measured* quantity — the 6-grain gain is oxygen alone, so equate it to α × (oxygen capacity of 60 grains of Zn). The closure check (oxide + metal = initial + gain) is built in and must reproduce 66 grains exactly.

---

## Question 6 — Hydroxylamine and iron(III)

### (a) Structure of NH₃OH⁺ Cl⁻
**L1 · Answer** **[H₃N–OH]⁺ Cl⁻**: nitrogen with four σ-bonds (3 × N–H, 1 × N–O) and no lone pair — **tetrahedral at N, all H–N–H and H–N–O angles ≈ 109.5°** (≈107°); oxygen with two bonds and two lone pairs — **bent at O, N–O–H ≈ 109.5°** (≈104–107°), drawn with the Cl⁻ nearby as the counter-ion.
**L2 · Thought** Count electron domains, not atoms: protonated N has 4 domains (0 lone pairs) → tetrahedral; O has 4 domains (2 lone pairs) → bent. The proton goes on N (the more basic site — ammonia-like, not water-like), which is what "hydroxylammonium" says.

### (b) Mole ratio Fe³⁺ : hydroxylammonium chloride
**L1 · Answer** n(NH₃OH⁺Cl⁻) in the aliquot = (1.00 g / 69.49 g mol⁻¹) × (25.0/250) = 1.439 × 10⁻³ mol. n(MnO₄⁻) = 28.9 × 10⁻³ × 0.0200 = 5.78 × 10⁻⁴ mol → n(Fe²⁺) titrated = 5 × 5.78 × 10⁻⁴ = 2.89 × 10⁻³ mol = n(Fe³⁺) that had reacted. Ratio = 2.89 × 10⁻³ / 1.439 × 10⁻³ = **2.01 ≈ 2 : 1**.
**L2 · Thought** Chain the titration backwards (§7.5): MnO₄⁻ takes 5 e⁻ (Mn +7 → +2), Fe²⁺ gives 1 e⁻ each, so moles of iron = 5 × moles of manganate; the aliquot factor (1/10) must be applied to the hydroxylammonium side. The near-integer 2.008 is the self-check that the whole chain is right.

### (c) Oxidation numbers of nitrogen
**L1 · Answer** In NH₃OH⁺: N + 3(+1) + (−2) + (+1) = +1 → **N = −1**. Each hydroxylammonium reduces 2 Fe³⁺, so it loses 2 e⁻ → **N = +1 in the product**.
**L2 · Thought** Oxidation-state bookkeeping with H = +1, O = −2 and the ion's overall +1 charge; the electron count from (b) then dictates the product's oxidation state — 2 electrons out means +2 on the single nitrogen atom.

### (d) The nitrogen product
**L1 · Answer** **N₂O** — the only option with nitrogen at +1 (average). (N₂ = 0, NO = +2, N₂O₄ = +4, NH₃ = −3.)
**L2 · Thought** Match the required oxidation state (+1) to the list; N₂O's two nitrogens average +1 — and two hydroxylammonium nitrogens (−1 each) comproportionating to (+1, +1) inside one N₂O is atom-economical, which the equation in (e) confirms.

### (e) Balanced equation
**L1 · Answer** **2 NH₃OH⁺ + 4 Fe³⁺ → N₂O + 4 Fe²⁺ + H₂O + 6 H⁺**
(chloride spectator: 2 NH₃OH⁺Cl⁻ + 4 Fe³⁺ → N₂O + 4 Fe²⁺ + H₂O + 6 H⁺ + 2 Cl⁻.)
**L2 · Thought** Construct from the two fixed points: 2 N needed for N₂O (so 2 hydroxylammonium), 4 e⁻ released (so 4 Fe³⁺). Then O: 2 left → 1 in N₂O + 1 H₂O; H: 8 left → 2 (H₂O) + 6 H⁺; charge: +2 + 12 = +14 = +8 + 6 ✓ — every audit line closes.

---

## Question 7 — The synthesis of Rohypnol (flunitrazepam)

**L1 · Answers (all SMILES machine-validated against the printed formulas)**

| | structure | SMILES | formula check |
|---|---|---|---|
| phenylhydrazine | Ph–NH–NH₂ | `NNc1ccccc1` | C₆H₈N₂ ✓ |
| **A** | 2-fluorobenzyl bromide (radical bromination of CH₃) | `Fc1ccccc1CBr` | C₇H₆BrF ✓ |
| **B** | 2-fluorophenylacetonitrile (ArCH₂CN) | `Fc1ccccc1CC#N` | C₈H₆FN ✓ |
| **C** | 2-fluorophenylacetic acid (ArCH₂COOH) | `Fc1ccccc1CC(=O)O` | C₈H₇FO₂ ✓ |
| **D** | 2-fluorophenylacetyl chloride (ArCH₂COCl) | `Fc1ccccc1CC(=O)Cl` | C₈H₆ClFO ✓ |
| **E** | 2-(2-fluorophenyl)-1-phenylethanone, 2-FC₆H₄CH₂COPh | `O=C(Cc1ccccc1F)c2ccccc2` | C₁₄H₁₁FO ✓ |
| (hydrazone) | the phenylhydrazone of E, 2-FC₆H₄CH₂C(=N–NHPh)Ph | `Fc1ccccc1CC(=NNc2ccccc2)c3ccccc3` | C₂₀H₁₇FN₂ ✓ |
| (indole) | 3-(2-fluorophenyl)-2-phenyl-1H-indole | `[nH]1c(-c2ccccc2)c(-c2ccccc2F)c3ccccc13` | C₂₀H₁₄FN ✓ |
| (ozonolysis product) | N-[2-(2-fluorobenzoyl)phenyl]benzamide, 2-(PhCONH)–C₆H₄–CO–(2-FC₆H₄) | `O=C(c1ccccc1)Nc1ccccc1C(=O)c1ccccc1F` | C₂₀H₁₄FNO₂ ✓ |
| **G** | benzoic acid (by-product) | `O=C(O)c1ccccc1` | C₇H₆O₂ ✓ |
| **H** | 2-amino-2'-fluorobenzophenone, 2-NH₂–C₆H₄–CO–(2-FC₆H₄) | `Nc1ccccc1C(=O)c1ccccc1F` | C₁₃H₁₀FNO ✓ |
| **I** | N-[2-(2-fluorobenzoyl)phenyl]-2-bromoacetamide, 2-(BrCH₂CONH)–C₆H₄–CO–ArF | `O=C(CBr)Nc1ccccc1C(=O)c1ccccc1F` | C₁₅H₁₁BrFNO₂ ✓ |
| **J** | the glycinamide, 2-(H₂NCH₂CONH)–C₆H₄–CO–ArF | `NCC(=O)Nc1ccccc1C(=O)c1ccccc1F` | C₁₅H₁₃FN₂O₂ ✓ |
| **K** | 5-(2-fluorophenyl)-1,3-dihydro-2H-1,4-benzodiazepin-2-one (7-membered ring closed, −H₂O) | `O=C1CN=C(c2ccccc2F)c2ccccc2N1` | C₁₅H₁₁FN₂O ✓ |
| **L** | the 7-nitro derivative of K | `O=C1CN=C(c2ccccc2F)c2cc([N+](=O)[O-])ccc2N1` | C₁₅H₁₀FN₃O₃ ✓ |
| flunitrazepam | N1-methyl-L (Rohypnol) | `CN1C(=O)CN=C(c2ccccc2F)c2cc([N+](=O)[O-])ccc21` | C₁₆H₁₂FN₃O₃ ✓ |

**L2 · Thought** Read the scheme as a sequence of formula-audited transformations (§4 by-product fingerprinting + formula audit at every letter):
- **A**: Br₂/UV/reflux = radical side-chain bromination — Br lands on the methyl, not the ring (the formula C₇H₆BrF = toluene −H +Br confirms one Br, side chain).
- **B**: NaCN = S_N2 on the benzyl bromide, +1 carbon as C≡N (C₈ ✓).
- **C**: aqueous H₂SO₄ hydrolyses the nitrile all the way to the carboxylic acid (+O₂, +H, C₈H₇FO₂ ✓).
- **D**: SOCl₂ → acyl chloride (the OH → Cl swap is the whole story; C₈H₆ClFO ✓).
- **E**: benzene/AlCl₃ = Friedel–Crafts acylation: ArCH₂COCl + C₆H₆ → ArCH₂COPh + HCl; C₁₄H₁₁FO = D + C₆H₆ − HCl ✓. This ketone is the linchpin of the whole route.
- **E → hydrazone (C₂₀H₁₇FN₂)**: + PhNHNH₂ − H₂O exactly (H: 11 + 8 − 2 = 17 ✓, O gone ✓) — a condensation, stopping at the phenylhydrazone.
- **hydrazone → indole (C₂₀H₁₄FN), −NH₃**: the Fischer indole synthesis closes the five-membered N-ring onto the hydrazine's benzene ortho position, ejecting NH₃ (the terminal –NH₂ nitrogen leaves; the aniline N stays as the indole NH). Regiochemistry: the carbonyl carbon's substituent (Ph) becomes the indole C2 substituent, the α-carbon's (2-FC₆H₄) becomes the C3 substituent → 2-phenyl-3-(2-fluorophenyl)indole; formula −NH₃ ✓ and ring count 5+6+6+6 ✓.
- **Ozonolysis (C₂₀H₁₄FNO₂)**: the stem defines it — "oxidises alkene carbons to carbonyls". The indole C2=C3 bond is cleaved: C2 → C(=O)–Ph flanked by N (a benzanilide), C3 → C(=O)–ArF fused ortho on the aniline ring: the anilide 2-(PhCONH)–C₆H₄–CO–ArF. +2 O, H and N counts unchanged ✓; the five-membered ring is gone (three 6-rings only) ✓ — the ring-count check is what proves the ring *opened* rather than oxidised in place.
- **H₂SO₄(aq) → G + H**: anilide hydrolysis splits PhCO– off as benzoic acid (**G**, C₇H₆O₂ ✓ — the "by-product" label confirms something must leave), freeing the amine **H** = 2-amino-2'-fluorobenzophenone (C₁₃H₁₀FNO = C₂₀H₁₄FNO₂ + H₂O − C₇H₆O₂ ✓).
- **H → I**: the reagent drawn is bromoethanoyl bromide, BrCH₂COBr; the aniline NH₂ is acylated (−HBr): I = bromoacetamide (+C₂H₂BrO − HBr → C₁₅H₁₁BrFNO₂ ✓).
- **I → J**: NH₃ substitutes Br (S_N2 on the α-bromo amide, −HBr): glycinamide J (N: 1 → 2 ✓).
- **J → K, −H₂O**: intramolecular condensation — the new –NH₂ attacks the benzophenone carbonyl and dehydrates to the cyclic imine, closing the **seven-membered 1,4-benzodiazepin-2-one** ring (the ring audit shows 6, 6, **7** ✓; formula −H₂O ✓). This is the benzodiazepine pharmacophore.
- **K → L**: conc. H₂SO₄/HNO₃ = nitration of the activated anilide ring at C7 (+NO₂ −H ✓).
- **L → flunitrazepam**: CH₃I methylates the remaining amide N1 (+CH₂ ✓). The final validator check C₁₆H₁₂FN₃O₃ with rings 6, 6, 7 matches the drawn drug exactly.

---

## Question 8 — Polonium

### (a) Electronic configuration
**L1 · Answer** Po (Z = 84): **[Xe] 4f¹⁴ 5d¹⁰ 6s² 6p⁴** (full: 1s² 2s²2p⁶ 3s²3p⁶3d¹⁰ 4s²4p⁶4d¹⁰4f¹⁴ 5s²5p⁶5d¹⁰ 6s²6p⁴).
**L2 · Thought** Build from xenon (54): + 4f¹⁴ (68) + 5d¹⁰ (78) + 6s² (80) + 6p⁴ (84); group 16 ⇒ …s²p⁴ outer shell, like O, S, Se, Te above it.

### (b) Alpha-decay product of ²¹⁰Po
**L1 · Answer** **²¹⁰₈₄Po → ²⁰⁶₈₂Pb + ⁴₂α** — lead-206.
**L2 · Thought** α emission removes 4 mass units and 2 charge units: 210 − 4 = 206, 84 − 2 = 82 = Pb. (The decay chain of ²¹⁰Po indeed terminates at stable ²⁰⁶Pb.)

### (c) Power output after 1 year
**L1 · Answer** P = P₀ × (½)^(t/t½) = 141 W × (½)^(365/138) = 141 × 0.160 = **22.5 W** (per gram).
**L2 · Thought** Activity (and hence heating power) decays with the same exponential as the atom count: 365/138 = 2.64 half-lives, so the power falls to (½)^2·⁶⁴ ≈ 16 % — Po's furious specific power is paid for with a fast fade.

### (d) Half-life of ²³⁸Pu
**L1 · Answer** (½)^(5/t½) = 0.96 → t½ = 5 × ln 2 / (−ln 0.96) = 5 × 0.6931/0.0408 = **≈ 85 years**.
**L2 · Thought** Invert the same decay law; a 4 % drop over 5 years means 5 y is only 0.059 of a half-life → t½ ≈ 85 y (literature 87.7 y — the "approximately 96 %" input justifies the estimate). Contrast with (c): 45× longer half-life, 250× lower specific power — the isotope trade-off in one line.

### (e) Atomic radius of polonium
**L1 · Answer** Simple cubic = 1 atom per unit cell (8 corners × ⅛): a³ = M/(ρN_A) = 209.98 / (9.142 × 6.022 × 10²³) = 3.81 × 10⁻²³ cm³ → a = 3.37 × 10⁻⁸ cm (337 pm). Atoms touch along the cube edge, so r = a/2 = **1.68 × 10⁻⁸ cm (168 pm)**.
**L2 · Thought** Three links in order (§7.4): cell contents (1 atom) → cell volume from density (ρ = mass per cell / a³) → geometry converting edge to radius. The last step is structure-specific: simple cubic touches along the *edge* (r = a/2) — a body-centred cell would touch along the body diagonal (r = √3 a/4), so state which contact line you are using. Magnitude check: ~10⁻⁸ cm is the right order for an atomic radius.

---

*End of Paper 23 (2003). This completes all 23 UKChO Round 1 papers, 2003–2025.*
