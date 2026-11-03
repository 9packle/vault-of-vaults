# Part II — Trinity College Cambridge 面试题汇编（14 Problems）

> **Source.** 全部题目取自 Trinity College Cambridge NST Admissions Guidance paper（源编码 T1-xx），按 Physics / Chemistry / Mathematics 分类，题目原文与完整解答均保持原样，未作任何删改。

---

## Physics (T1-03, T1-05, T1-07, T1-08, T1-09, T1-10, T1-18)

#### P1 — Perfume Diffusion in a Sealed Room (Source: T1-03 · Trinity College Cambridge, NST Admissions Guidance paper)

How long before the perfume reaches the wall?


**Problem.** A compact cloud of perfume molecules is released at the centre of an isolated 5 m spherical room (T = 300 K, molecular number density 2.5×10²⁵ m⁻³). Roughly how long before the scent reaches the walls?

**Thought.** *Route 1* opens Fick's laws and solves the diffusion equation — beyond A-Level. *Route 2*, kept here, is the dimensional-analysis-first estimate the problem itself recommends: the diffusion coefficient can only be built from a length (the mean free path) times a speed (the thermal speed), both of which A-Level kinetic theory supplies (physics §3: r.m.s. and mean molecular speeds, the pressure formula derivation with its mean-free-path reasoning); the diffusion time then follows from the one-dimensional random-walk relation t ~ R²/2D, whose structure (variance growing linearly in time) is variance growing *linearly* with time — the unmistakable signature of a diffusive process (contrast exponential relaxation, in which a quantity decays by equal fractions in equal times: different mathematics, different physics). The only flagged step is the precise numerical factor ⅓ in D = λv̄/3 — quoted as given, like any data-booklet constant. Everything else — the collision cross-section estimate, the thermal speed, the final weeks-long answer, and the five-orders-of-magnitude convection punchline — is school physics with its assumptions spoken aloud.

**1. Statement & Symbols.** R = 5 m, T = 300 K, n = 2.5×10²⁵ m⁻³; perfume m = 250 u = 4.15×10⁻²⁵ kg — a typical large-organic-molecule scale, a reasonable stand-in for a scent molecule. Estimate t.

**2. Governing Principles.** Kinetic theory: mean free path λ = 1/(√2 nσ) with molecular diameter d ≈ 3×10⁻¹⁰ m (the √2 counts the relative motion of the colliding molecules — the target molecules are not stationary); thermal speed v̄ = √(8k_BT/πm) (physics §3); Dimensional analysis: D = (1/3)λv̄ (given); diffusion as a random walk: x_rms = √(2Dt), so t ≈ R²/(2D) (physics §1 estimation; mathematics §15 separable intuition).

**3. Derivation.**

*Step 1 — mean free path.* σ = πd² ≈ 3×10⁻¹⁹ m²; λ = 1/(√2 × 2.5×10²⁵ × 3×10⁻¹⁹) ≈ 1×10⁻⁷ m.

*Step 2 — thermal speed of the perfume molecule.* v̄ = √(8 × 1.381×10⁻²³ × 300/(π × 4.15×10⁻²⁵)) ≈ √(2.54×10⁴) ≈ 160 m s⁻¹.

*Step 3 — diffusion coefficient.* D = (1/3)λv̄ ≈ (1/3)(10⁻⁷)(160) ≈ 5×10⁻⁶ m² s⁻¹.

*Step 4 — diffusion time.* t ≈ R²/(2D) = 25/(10⁻⁵) ≈ 2.5×10⁶ s ≈ **one month**. (The three-dimensional radial version, r² = 6Dt, changes this to ≈ 8×10⁵ s — the same order; the honest headline is 10⁶ s, weeks. Strictly, 'time to reach the wall' is a first-passage problem whose prefactor depends on geometry — the R²/D scaling is the robust content of any such estimate.)

**4. Numerical Result.** t ≈ 2.5×10⁶ s ≈ 1 month (order 10⁶ s).

**5. Verification.** Cross-check D against air's own value ≈ 2×10⁻⁵ m² s⁻¹ at 300 K: the heavier, slower perfume molecule differs by a factor of a few ✓. Every step is an estimate with its assumption stated (d, the ⅓ factor, the one-dimensional geometry).

**6. Conclusion & Discussion.** Weeks by pure diffusion. *Flagged datum:* the ⅓ in D = λv̄/3. *The real lesson:* a non-isolated room convects — draughts at 0.1 m s⁻¹ cross 5 m in ~50 s, five orders of magnitude faster; smell travels by convection, and the isolated-room premise is what makes the diffusion calculation the right one.


#### P2 — Molecular Separation in Air at STP (Source: T1-05 · Trinity College Cambridge, NST Admissions Guidance paper)

> "C5. What is the average separation between atoms or molecules in a gas at 1 atm and 273 K?"

**Thought.** One cube root of the volume per molecule gives the spacing; distinguishing it from the mean free path (an order of magnitude larger) is exactly the follow-up the examiner wants.


**1. Statement & Symbols.**
P = 1 atm, T = 273 K. Find the mean intermolecular spacing ℓ = (V/N)^(1/3).

**2. Governing Principles.**
Each molecule occupies on average a cube of volume V/N; the molar volume at STP is 22.4 L.

**3. Derivation.**
*Step 1 — Volume per molecule.* V_m = 22.4×10⁻³ m³/mol; V/N = 22.4×10⁻³/6.022×10²³ = 3.72×10⁻²⁶ m³.
*Step 2 — Cube root.* ℓ = (3.72×10⁻²⁶)^(1/3) = 3.3×10⁻⁹ m ≈ **3.3 nm**.

**4. Numerical Result.**
ℓ ≈ 3 nm (30 Å).

**5. Verification.**
Cross-check via ideal gas law: n = P/(kT) = 1.01×10⁵/(1.381×10⁻²³×273) = 2.69×10²⁵ m⁻³; (1/n)^(1/3) = (3.72×10⁻²⁶)^(1/3) = 3.3 nm ✓ identical.

**6. Conclusion & Discussion.**
ℓ ≈ 3 nm, about ten times a molecular diameter (~0.3 nm): each molecule is a tiny island in mostly empty space — precisely why gases are ideal to first order and why the mean free path (P2-adjacent, ℓ²/d² ~ 100× smaller) is the collision length, not ℓ. Distinguishing "separation" from "mean free path" is the examiner's follow-up.


#### P3 — The Golfer's Drive (Source: T1-07 · Trinity College Cambridge, NST Admissions Guidance paper)

> "P1. A golfer driving from the tee swings his club so that the head completes a (virtually) complete circle in 0.5 s. Make a reasoned estimate of the maximum distance he could hit the ball."

**Thought.** The yardage is not the answer; the audit trail is. Each assumption — swing radius from body geometry, elastic transfer, no drag — should be stated with its direction of error.


**1. Statement & Symbols.**
Club head completes a near-circle of radius r in T = 0.5 s. Estimate the drive range.

**2. Governing Principles.**
Uniform circular motion (v = ωr), collision physics (light ball struck by heavy club head), projectile range R = v²sin2θ/g with optimal elevation 45°.

**3. Derivation.**
*Step 1 — Club head speed.* Angular speed ω = 2π/T = 2π/0.5 = 12.6 rad/s. Radius of the swing circle ≈ arm (0.7 m) + club shaft (1.1 m) ≈ 1.8 m. Head speed v_h = ωr = 12.6×1.8 ≈ 23 m/s.
*Step 2 — Ball exit speed.* Model the impact as a one-dimensional elastic collision between a heavy club head (M ≈ 1 kg effective) moving at v_h and a light ball (m ≈ 50 g) initially at rest. Momentum: Mv_h = Mu + mv_b. Energy: Mv_h² = Mu² + mv_b² (halves cancel). The two equations imply reversal of the relative velocity, v_b − u = v_h; solving simultaneously gives v_b = 2Mv_h/(M + m) = 2v_h/(1 + m/M). With m/M = 0.05: v_b = 2×23/1.05 ≈ **44 m/s**. (Assumption audit: M ≫ m and elasticity are generous, while the rigid shaft and neglected aerodynamic drag are losses — real drives fly farther, thanks to shaft whip; the simple model brackets the truth from below.)
*Step 3 — Range at 45°.* R = v_b²/g = 44²/9.81 = 1936/9.81 ≈ **200 m**. Order 10² m.

**4. Numerical Result.**
Maximum drive ≈ 200 m (order 10² m); the official expectation is the assumption list, not the number.

**5. Verification.**
Dimensions ✓. Real professional drives reach 250–350 m thanks to the whip effect of shaft flexing — our rigid-model 200 m sits sensibly just below ✓.

**6. Conclusion & Discussion.**
The mark-bearing content is the explicit assumption chain: swing radius from body geometry, speed from ωr, exit speed from the elastic heavy-on-light collision, 45° launch, no drag. Interviewers score the audit trail, not the yardage.


#### P4 — Charging Two Cans by Induction (Source: T1-08 · Trinity College Cambridge, NST Admissions Guidance paper)

> "P2. You are provided with a positively charged ball suspended by an insulating thread and two uncharged metal cans. Describe the sequence of operations you would carry out to charge one can positively and the other can negatively."

**Thought.** The physics is entirely in the sequence: induce, separate, then remove. Violate the order and the separated charge relaxes away — a protocol with causal annotations is what is being examined.


**1. Statement & Symbols.**
A positively charged ball on an insulating thread; two uncharged metal cans (conducting, insulated from ground). Goal: one can +, one can −.

**2. Governing Principles.**
Electrostatic induction: a nearby charge polarises a conductor; charge separation vanishes if the polarised conductor is re-neutralised after removal of the external charge — the sequence (induce → separate → remove) is what freezes the separated charge.

**3. Derivation (the operation sequence, with the physics of each step).**
*Step 1 — Touch the cans together* so the pair forms a single conductor.
*Step 2 — Bring the positive ball close to can A (do not touch).* Free electrons in the combined conductor are attracted toward the ball: can A acquires induced negative charge, can B an equal induced positive charge (charge conservation: the pair is still neutral overall).
*Step 3 — While holding the ball in place, separate the cans.* The mobile charge can no longer redistribute between them: A carries net negative, B net positive, frozen in place.
*Step 4 — Remove the ball.* The induced distribution relaxes into surface distributions, but each can now retains its net charge: A negative, B positive. Note the polarity is opposite to the inducing ball on the near can — induction, not conduction.

**4. Numerical Result.**
Sequence: contact → induce (ball near A) → separate (ball held) → remove ball. Result: can A negative, can B positive — equal and opposite net charges set by the induced separation of Step 2. The magnitude grows with the ball's charge, the can geometry and the closeness of approach, roughly linearly in the ball's charge as long as it stays below the discharge threshold (a small charge already suffices, but the result is not independent of the ball's total charge).

**5. Verification.**
Charge conservation at every stage: total charge of the two-can system is 0 before and after ✓. Grounding check: if instead of separating first you removed the ball, both cans would return to neutral — the temporal order is the entire point.

**6. Conclusion & Discussion.**
This is the induction-charging cycle (the same physics as the electrophorus). The tested skill is describing an *ordered protocol with causal annotations* — each step justified by what the charge would do if the order were violated.


#### P5 — Newton's Law of Cooling: A Suspicious Constant (Source: T1-09 · Trinity College Cambridge, NST Admissions Guidance paper)

> "P3. According to Newton's law of cooling, the temperature of an object decreases at a rate proportional to the difference between its temperature and that of the surroundings. If the constant of proportionality is 100 s-1, estimate the time it takes for a freshly brewed cup of coffee to become drinkable."

**Thought.** Compute with the given constant, watch the answer violate experience (six milliseconds), and say so. Parameter auditing, not integration, is the tested skill.


**1. Statement & Symbols.**
Ṫ = −k(T − T_s), k = 100 s⁻¹ (as stated), coffee from ~90 °C to drinkable ~60 °C, room T_s = 20 °C. Estimate t.

**2. Governing Principles.tt**
Newton's cooling integrates to T − T_s = ΔT₀e^(−kt); the characteristic time is 1/k.

**3. Derivation.**
*Step 1 — Solve.* T(t) = T_s + (T₀ − T_s)e^(−kt).
*Step 2 — Substitute the stated constant.* Time to cool from 90 to 60: (60−20)/(90−20) = 40/70 = e^(−100t) ⟹ t = ln(70/40)/100 = ln(1.75)/100 = 0.560/100 = 5.6×10⁻³ s.
*Step 3 — Flag the absurdity.* A coffee cooling in 6 ms is physically impossible — the stated k is at least five orders of magnitude too large. (The correct order for a mug is k ~ 10⁻³–10⁻⁴ s⁻¹, dominated by evaporation and convection.) The honest response: "with k = 100 s⁻¹ the model gives 6 ms, contradicting experience; I suspect the intended value was ~10⁻³ s⁻¹; with that, t = ln(1.75)/10⁻³ ≈ 560 s ≈ 9 minutes."
*Step 4 — Redo with the corrected constant.* t = ln(ΔT₀/ΔT)/k = 0.56/10⁻³ ≈ 5.6×10² s ≈ 10 min ✓ matches experience.

**4. Numerical Result.**
As stated: t ≈ 6 ms (absurd, flag it); with a realistic k ≈ 10⁻³ s⁻¹: t ≈ 10 minutes.

**5. Verification.**
Dimension: k in s⁻¹ makes kt dimensionless ✓. The sanity check (coffee stays hot for minutes, not milliseconds) is the controlling evidence.

**6. Conclusion & Discussion.**
This is a parameter-audit problem disguised as a plug-in exercise. The examiner's own guidance invites "thinking about the limitations of an approach": compute with the given number, demonstrate the contradiction, and repair the model. The formula, the flag, and the corrected estimate together form the full answer.


#### P6 — Earth–Sun Density Ratio from Angular Diameters (Source: T1-10 · Trinity College Cambridge, NST Admissions Guidance paper)

> "P4. Seen from the Moon, the Earth has 3.6 times the angular diameter of the Sun. What is the ratio of densities of the Sun and the Earth?"

**Thought.** Two different physical regimes supply the two masses: local surface gravity for the Earth, orbital dynamics for the Sun. Choosing which tool produces which quantity is the whole problem.


**1. Statement & Symbols.**
From the Moon: angular diameter of Earth = 3.6 × that of the Sun. Need ρ_E/ρ_S. Distances (from common knowledge): Earth–Moon d = 3.84×10⁸ m; Sun–Earth D = 1.50×10¹¹ m.

**2. Governing Principles.**
Angular diameter ≈ 2R/distance; g = GM/R² at a surface; Earth's g measured at its surface, Sun's mass from Earth's orbital period (Kepler III).

**3. Derivation.**
*Step 1 — Radii ratio.* 2R_E/d = 3.6×(2R_S/D) ⟹ R_E/R_S = 3.6d/D = 3.6×3.84×10⁸/1.50×10¹¹ = 3.6×2.56×10⁻³ = 9.2×10⁻³.
*Step 2 — Masses.* Earth: M_E = gR_E²/G (its surface gravity is known locally). Sun: from Earth's orbit, M_S = 4π²D³/(GT²) with T = 1 yr = 3.16×10⁷ s. (Only the 3.6 angular ratio is problem-given; d, D, g and T are common-knowledge data — declaring which is which is part of the answer.)
*Step 3 — Density ratio.* ρ_E/ρ_S = (M_E/R_E³)/(M_S/R_S³) = [gR_E²/G × GT²/(4π²D³)] × (R_S/R_E)³ = gT²/(4π²D³) × R_S³/R_E.
Substituting R_S = R_E/(9.2×10⁻³) and grouping into two bracketed factors,
ρ_E/ρ_S = [gT²/(4π²D³)] × [R_E²/(9.2×10⁻³)³],
with units m⁻² × m² = dimensionless. Numerically: gT² = 9.81×(3.16×10⁷)² = 9.80×10¹⁵ m; 4π²D³ = 39.5×(1.50×10¹¹)³ = 1.333×10³⁵ m³; first factor = 7.35×10⁻²⁰ m⁻². Then R_E² = (6.37×10⁶)² = 4.06×10¹³ m² and (9.2×10⁻³)³ = 7.79×10⁻⁷. Product: 7.35×10⁻²⁰ × 4.06×10¹³ / 7.79×10⁻⁷ = 2.98×10⁻⁶/7.79×10⁻⁷ ≈ **3.8**.

**4. Numerical Result.**
ρ_E : ρ_S ≈ 3.8 : 1 (accepted values 5514 vs 1410 kg/m³ give 3.9 — our single-figure data reproduce it).

**5. Verification.**
Each input was independently sourced (g, orbital period, two distances); the chain uses only one geometric datum (the 3.6 ratio) beyond constants of common knowledge ✓.

**6. Conclusion & Discussion.**
A five-step chain: angular ratio → radii ratio → two mass determinations (local gravity vs orbital dynamics) → densities. The lesson: different physical regimes (surface gravity, orbital mechanics) provide the two masses — recognising which tool gives which is the real test.


#### P7 — Blue Skies, White Clouds, Blue Copper Sulphate (Source: T1-18 · Trinity College Cambridge, NST Admissions Guidance paper — cross-disciplinary physics/chemistry)

Blue sky, white clouds, blue copper sulphate


**Problem.** Why is a clear sky blue and a cloudy sky white? Why is hydrated copper sulphate blue but anhydrous white?

**Thought.** *Route 1* derives Rayleigh scattering from the driven-oscillator model — one step beyond the syllabus (Larmor). *Route 2*, kept here, splits the question exactly at its natural seam: the **physics half** uses the Rayleigh law as given (as any data-booklet law), extracting the blue/red ratio and all three companion phenomena; the **chemistry half** is pure A-Level — d–d transitions in the octahedral aqua complex, their disappearance when the water ligands are removed (chemistry §14), the complement rule. The one non-A-Level step in the whole question — the microscopic origin of λ⁻⁴ — is quarantined in the Discussion, where it is further decomposed so the reader sees precisely which sub-step (forced oscillation, A-Level; Larmor power, not) crosses the boundary. Two disciplines, one meta-question ("what wavelength-dependent mechanism removes photons?"), zero boundary violations in the core.

**1. Statement & Symbols.** Given: I_scatter ∝ 1/λ⁴ for particles ≪ λ (Rayleigh law, as data). λ_blue ≈ 450 nm, λ_red ≈ 650 nm.

**2. Governing Principles.** The given Rayleigh law; E = hf (physics §7); ligand splitting of d-orbitals and d–d absorption (chemistry §14); complementary colours.

**3. Derivation.**

*Step 1 — the sky.* I_blue/I_red = (650/450)⁴ ≈ 4.4: scattered light away from the Sun is blue-dominated.

*Step 2 — companions.* Clouds: droplets ~10 µm ≫ λ scatter all wavelengths alike → white. Sunset: long path removes short wavelengths from the direct beam → red. Not violet: weak solar violet, low eye sensitivity, ozone absorption.

*Step 3 — the copper half.* In CuSO₄·5H₂O, octahedral water ligands split the Cu²⁺ (3d⁹) levels; the d–d absorption is broad (~600–900 nm, peaking near 800 nm in the NIR) and removes the orange-red end, leaving the complement — blue. Anhydrous CuSO₄: sulfate is a weak-field ligand, so the gap is smaller and the absorption moves to longer wavelengths — out of the visible → nothing absorbed → white.

**4. Numerical Result.** Blue/red scattering ratio 4.4; sky blue, clouds white, sunsets red; blue Cu²⁺(aq) by d–d absorption, white when the field changes.

**5. Verification.** ω → 0: static field polarises but does not scatter — consistent with the law ✓. The two halves share one logic — identify the wavelength-dependent absorber — and both conclusions are checkable against everyday observation.

**6. Conclusion & Discussion.** One given law answers the sky; A-Level coordination chemistry answers the copper. *The quarantined step:* the microscopic λ⁻⁴ chain is identical to P15's — cross-reference, not repetition: forced oscillation of the bound electron (A-Level SHM language); far below resonance the amplitude is essentially frequency-independent, so a = −ω²x gives a ∝ ω², and with the single non-A-Level input (radiated power ∝ a²) I ∝ a² ∝ ω⁴ ∝ λ⁻⁴; the free-electron limit gives frequency-independent Thomson scattering, the trap the question sets.


---

## Chemistry (T1-01, T1-02, T1-04, T1-06)

#### C1 — Three Kinds of Chlorine Interaction (Source: T1-01 · Trinity College Cambridge, NST Admissions Guidance paper)

> "C1. Discuss the nature of the interaction between (a) the chlorine atoms in the molecule Cl2; (b) two chlorine ions in NaCl; and (c) two chlorine molecules."

**Thought.** Classify the interaction type before rating its strength — shared electrons, Coulomb lattice, fluctuating dipoles — and the three answers order themselves.


**1. Topic Analysis.**
One element, three binding regimes: intra-molecular covalent, ionic lattice, and inter-molecular dispersion. The examiner is testing whether "bond" and "force" are kept conceptually separate.

**2. Key Concepts.**
Shared-electron-pair covalent bond (overlap of half-filled 3p orbitals); Coulombic ionic lattice (non-directional, long-range); London dispersion (instantaneous dipole–induced dipole, universal, weak).

**3. Step-by-Step Reasoning.**
(i) **Cl atoms within Cl₂:** each Cl (3s²3p⁵) contributes its unpaired 3p electron to a shared pair: a single covalent σ bond (3p–3p overlap), bond length ~199 pm, bond enthalpy ~243 kJ/mol. Directional, short-ranged, saturating (one bond per partner; satisfied by one bond plus three lone pairs).
(ii) **Cl⁻ ions in NaCl:** Na has transferred its 3s electron to Cl, giving closed-shell Na⁺ and Cl⁻. The interaction is the Coulomb attraction q⁺q⁻/(4πε₀r) — non-directional and long-ranged, so each ion binds to *all* oppositely charged neighbours: an extended lattice (rock-salt structure), not a molecule. Lattice enthalpy ~787 kJ/mol — far larger than a covalent bond *per formula unit*, though per ion-pair-contact it is comparable (~300–400 kJ/mol·contact counting several neighbours).
(iii) **Two Cl₂ molecules:** closed-shell molecules with no permanent dipole (Cl₂ is non-polar). Only London dispersion acts: instantaneous fluctuations polarise the neighbour; the attraction scales with polarisability (larger, heavier molecules disperse more strongly) and falls as ~1/r⁶. For Cl₂ the boiling point is −34 °C — a few kJ/mol, two orders below the covalent bond.

**4. Conclusion.**
Same element, three physics: shared electrons (covalent, strong, directional), Coulomb lattice (strong, non-directional, extended), fluctuating dipoles (weak, universal). The word "interaction" is doing the work — the candidate's first move should be to classify *what kind* before citing *how strong*.

**5. Common Errors & Marking Points.**
✗ Calling the NaCl interaction "a bond between two ions" (it is a lattice). ✗ Rating dispersion as negligible *because* Cl₂ is non-polar (non-polar is exactly when dispersion dominates). Marks: orbital description of the covalent bond; lattice vs molecule for NaCl; the dispersion mechanism and its r⁻⁶ scaling.


#### C2 — Molar Enthalpy of Combustion from a Bomb Calorimeter (Source: T1-02 · Trinity College Cambridge, NST Admissions Guidance paper)

Molar enthalpy of combustion from a bomb calorimeter


**Problem.** A 1.00 g benzoic-acid tablet raises the calorimeter temperature 1.76 K (ΔH_c = 26.454 kJ g⁻¹). A 2.00 g tartaric-acid tablet raises it 1.0264 K. Find the molar enthalpy of combustion of tartaric acid.

**Thought.** *Route 1* completes the thermodynamic bookkeeping with ΔH = ΔU + Δn_gasRT — the exact route, but the relation is not on the A-Level list. *Route 2*, kept here, notices what the question's own numbers already guarantee: combustion of C₄H₆O₆ consumes 2.5 mol O₂ and produces 4 mol CO₂, so Δn_gas = +1.5 — small — and the correction ΔnRT ≈ +3.7 kJ mol⁻¹ against a ΔU of 1158 kJ mol⁻¹ is 0.3%. The A-Level solution therefore reports ΔU from the calorimeter and states the correction's *direction and size* with its formula quoted as given, exactly as a data-booklet relation would be used. The calibration logic itself — the apparatus constant transferred from a standard to an unknown — is the A-Level core, and it is executed with the assumptions the question demands listed at the end, as instructed. Nothing is hidden; the one beyond-syllabus symbol is flagged and quantified.

**1. Topic Analysis.** Calibration transfer, then the constant-volume versus constant-pressure distinction and its size.

**2. Key Concepts.** q = C_cal·ΔT (chemistry §6 calorimetry); complete combustion to CO₂ and H₂O; the ΔH–ΔU relation ΔH = ΔU + Δn_gasRT (quoted as given).

**3. Step-by-Step Reasoning.**

*Step 1 — calibrate.* C_cal = (1.00 g × 26.454 kJ g⁻¹)/1.76 K = 15.03 kJ K⁻¹. (The tabulated benzoic-acid figure is a constant-volume value, as a bomb calorimeter requires; had a ΔH been supplied instead, a ΔnRT conversion of ≈ 0.01 kJ g⁻¹ — negligible here — would precede the calibration.)

*Step 2 — the unknown run.* q = 15.03 × 1.0264 = 15.43 kJ for 2.00 g → 7.715 kJ g⁻¹; molar mass of C₄H₆O₆ = 150.09 g mol⁻¹ → ΔU_c = −7.715 × 150.09 ≈ −1158 kJ mol⁻¹.

*Step 3 — the correction, quoted and sized.* Δn_gas = (gas out) − (gas in) = 4 − 2.5 = +1.5 (water liquid; unreactive N₂ not counted); ΔH = ΔU + Δn_gasRT = −1158 + 1.5 × 8.314 × 298×10⁻³ ≈ **−1154 kJ mol⁻¹** — a 0.3% shift, direction (less exothermic) noted. Formula quoted as given.

*Step 4 — assumptions, as the question demands.* Complete combustion (balance: C₄H₆O₆ + 2.5O₂ → 4CO₂ + 3H₂O); water liquid; adiabatic calorimeter; identical assembly between runs; negligible ignition energy; ΔH effectively temperature-independent across the ≈ 1 K rise.

**4. Conclusion.** ΔU_c ≈ −1158 kJ mol⁻¹; ΔH_c ≈ −1154 kJ mol⁻¹ with the ΔnRT correction quoted as given and sized at 0.3%.

**5. Discussion.** *The beyond-syllabus symbol:* the ΔH–ΔU relation itself — derived in university thermodynamics from H = U + pV. At the precision of school data the distinction is optional; naming it, sizing it, and stating its direction is the complete A-Level-honest treatment.


#### C3 — Three Isomers of C₃H₄ (Source: T1-04 · Trinity College Cambridge, NST Admissions Guidance paper)

> "C4. Three isomeric compounds have the molecular formula C3H4. Draw possible structures showing how the atoms are arranged in space and comment on the bonding in each compound."

**Thought.** DBE equals 2 is a budget to be spent three ways; each purchase teaches one bonding concept — orthogonal pi bonds, cumulated dienes, ring strain.


**1. Topic Analysis.**
DBE = 3 + 1 − 4/2 = 2: the budget of two π-bonds/rings must be spent in three different architectures. The instruction "arranged in space" demands three-dimensional thinking from the first line.

**2. Key Concepts.**
Degrees of unsaturation; sp/sp²/sp³ hybridisation geometry; cumulated double bonds (allene) with perpendicular π systems; ring strain in cyclopropene.

**3. Step-by-Step Reasoning.**
(i) **Propyne (methylacetylene), CH₃–C≡CH.** sp³ methyl carbon, two sp carbons joined by one σ + two π bonds (a triple bond, linear at both sp centres: 180° angles). The π bonds are orthogonal (in the two perpendicular planes containing the axis), cylindrical π-symmetry overall.
(ii) **Propadiene (allene), H₂C=C=CH₂.** Cumulated double bonds: the central carbon is sp-hybridised (two σ bonds at 180°), the two terminal carbons are sp² (120° planes). Crucially the two π bonds occupy *perpendicular* planes — so the two CH₂ groups lie in perpendicular planes; an allene with different substituents at each end (abC=C=Ccd) is chiral (axial chirality), though C₃H₄ itself has a mirror plane. Bonding: the central sp carbon's two unhybridised p orbitals (p_x, p_y) each overlap with one terminal carbon's p orbital.
(iii) **Cyclopropene, C₃H₄ (one C=C in a three-membered ring, one CH₂).** One sp² CH (double bond), one sp³ CH₂; the ring forces 60° C–C–C angles against the sp²-preferred 120° — severe angle strain (~115 kJ/mol total strain energy), explaining cyclopropene's high reactivity (the π bond is weakened, polymerisation easy).

**4. Conclusion.**
Same formula, three chemistries: a linear alkyne (sp, orthogonal π bonds), a cumulated diene with perpendicular π systems and axial chirality lurking, and a strained cyclic alkene whose ring bends the rules of hybridisation geometry.

**5. Common Errors & Marking Points.**
✗ Missing the allene's perpendicular π planes (the spatial point of the question). ✗ Omitting ring-strain commentary for cyclopropene. Marks: correct DBE use, hybridisation assignment per carbon, the allene geometry (including the chirality remark), ring-strain reasoning.


#### C4 — Electroplating Chromium but Not Sodium; Two Solubility Paradoxes (Source: T1-06 · Trinity College Cambridge, NST Admissions Guidance paper)

> "C6. Comment on the following statements. (a) An electrolytic cell can be set up with chromium as the anode and an object we wish to electroplate as the cathode in a CrCl3 electrolyte solution. However, the analogous process with sodium is not feasible. (b) Calcium carbonate is poorly soluble in water and its solubility decreases as the temperature increases. Dissolving ammonium nitrate in water is an endothermic process, and yet ammonium nitrate is readily soluble."

**Thought.** Water's potential window decides the electroplating half; the Gibbs free-energy equation resolves the solubility paradox. Two different thermodynamic criteria, both needed.


**1. Topic Analysis.**
"Comment on" invites verification, mechanism, and boundary analysis in both halves: aqueous electrochemistry's water window; and the enthalpy–entropy partition of ΔG in dissolution.

**2. Key Concepts.**
Reduction potentials vs the water window (H⁺/H₂ and O₂/H₂O); kinetic overpotential enabling Cr deposition; ΔG = ΔH − TΔS governing spontaneity; Le Chatelier on solubility with temperature.

**3. Step-by-Step Reasoning.**
(i) **(a) Chromium yes, sodium no.** In aqueous CrCl₃ the cathode faces two possible reductions: Cr³⁺ + 3e⁻ → Cr (E° = −0.74 V) and 2H⁺ + 2e⁻ → H₂ (E° = 0 V). On paper hydrogen wins; in practice a large hydrogen *overpotential* on the chromium surface kinetically suppresses H₂ evolution, and Cr³⁺ reduction proceeds — chromium electroplating is an industrial reality. (Industrial practice actually uses a CrO₃-based bath rather than CrCl₃; the problem's cell is a simplified model, and the potential-window argument is unaffected.) Sodium's analogue requires Na⁺ + e⁻ → Na at E° = −2.71 V, far below the water-reduction potential at every accessible pH: water is reduced first, always, so aqueous sodium electroplating is impossible (molten NaCl is used instead — the Downs process).
(ii) **(b) CaCO₃ solubility falling with T.** Decreasing solubility with rising temperature signals an exothermic dissolution (ΔH_sol < 0); heat acts as a product, and Le Chatelier pushes the equilibrium toward solid. (Consistent with its retrograde solubility and the scaling it causes in kettles.)
(iii) **(b) Endothermic yet readily soluble NH₄NO₃.** Spontaneity is decided by ΔG = ΔH − TΔS, not by ΔH alone. Dissolution of an ionic crystal into mobile, hydrated ions is a large positive-entropy process: the ordered lattice and its organised hydration become dispersed aqueous ions. For NH₄NO₃, TΔS > ΔH (> 0), so ΔG < 0 and the salt dissolves *while cooling its own solution* — the basis of instant cold packs. The two clauses of (b) are therefore not in conflict: the first reports an enthalpy signature, the second a free-energy outcome.

**4. Conclusion.**
(a) is a competition between kinetics (overpotential) and thermodynamics (potential window): Cr wins kinetically, Na loses thermodynamically. (b) contrasts enthalpic and entropic control of two different dissolutions.

**5. Common Errors & Marking Points.**
✗ "Sodium is too reactive" as the whole answer (the point is the potential window of *water*). ✗ Treating endothermicity as an argument against spontaneity. Marks: the −2.71 V vs water argument; overpotential named for Cr; the ΔG = ΔH − TΔS resolution with the entropy argument.


---

## Mathematics (T1-15, T1-16, T1-17)

#### M1 — The Area of Region R (Source: T1-15 · Trinity College Cambridge, NST Admissions Guidance paper)

> "G1. A region R of the (x, y) plane is defined as follows. It has x > 0 and y > 0. Its boundary consists of finite sections of the following three curves: the y axis, the curve y = x^2 and a circle of radius sqrt(2) centred on the origin. What is the area of R?"

**Thought.** The universal area workflow: intersections, a one-point top-versus-bottom test, then a standard integral. Nothing beyond the arcsin evaluation separates this from routine.


**1. Statement & Symbols.**
R is bounded by x = 0 (y-axis), y = x², and x² + y² = 2, in the first quadrant. Find area(R).

**2. Governing Principles.**
Find the intersection points of the bounding curves, then integrate (upper boundary − lower boundary) dx between the appropriate limits.

**3. Derivation.**
*Step 1 — Intersections.* Parabola meets circle where x² + (x²)² = 2: writing u = x², u + u² = 2 ⟹ u² + u − 2 = 0 ⟹ (u+2)(u−1) = 0 ⟹ u = 1 (reject u = −2) ⟹ x = 1, y = 1. Circle meets y-axis at (0, √2); parabola meets y-axis at (0, 0).
*Step 2 — Identify top and bottom curves on [0, 1].* For 0 < x < 1: the circle's upper branch y = √(2 − x²) lies above the parabola y = x² (check at x = 0: √2 > 0 ✓; they meet at x = 1).
*Step 3 — Set up the integral.* Area = ∫₀¹ [√(2 − x²) − x²] dx.
*Step 4 — Evaluate each piece.* Standard integral ∫√(a² − x²) dx = (x/2)√(a² − x²) + (a²/2)arcsin(x/a). With a = √2:
∫₀¹ √(2 − x²) dx = [(x/2)√(2 − x²) + arcsin(x/√2)]₀¹ = (1/2)(1) + arcsin(1/√2) − 0 = 1/2 + π/4.
And ∫₀¹ x² dx = 1/3.
*Step 5 — Combine.* Area = (1/2 + π/4) − 1/3 = **π/4 + 1/6** ≈ 0.7854 + 0.1667 = 0.952.

**4. Numerical Result.**
Area = π/4 + 1/6 ≈ 0.952 square units.

**5. Verification.**
Upper estimate: the quarter-disc of radius √2 has area π(√2)²/4 = π/2 ≈ 1.57; R is visibly about 60% of it ✓. Lower: the area under the parabola alone is 1/3; R exceeds it by the circular cap ✓ consistent.

**6. Conclusion & Discussion.**
The workflow — intersections → top/bottom decision (with one test point) → standard integral — is the universal pattern for area-between-curves problems; the only content beyond it is the arcsin(1/√2) = π/4 evaluation.


#### M2 — The arctan(x) + arctan(1/x) Trap (Source: T1-16 · Trinity College Cambridge, NST Admissions Guidance paper)

> "G2. Sketch the graph of f(x) = arctan(x) + arctan(1/x)."

**Thought.** The addition formula degenerates — division by zero — and that degeneration is the signal to check quadrants. The identity is only half true, and the question punishes those who quote it whole.


**1. Statement & Symbols.**
Sketch f(x) = arctan x + arctan(1/x), noting the domain excludes x = 0.

**2. Governing Principles.**
Either differentiate and integrate the constant back with interval-wise constants, or apply the addition formula with explicit quadrant control. Domain discipline: f is undefined at 0 and the two branches are separate objects.

**3. Derivation.**
*Step 1 — Domain.* x ≠ 0 (1/x undefined). The function is odd: f(−x) = arctan(−x) + arctan(−1/x) = −f(x) (both branches odd) — so study x > 0 and reflect.
*Step 2 — The addition formula with quadrant care.* tan(A + B) = (tan A + tan B)/(1 − tan A tan B) with A = arctan x, B = arctan(1/x): numerator x + 1/x, denominator 1 − x·(1/x) = 0: the formula degenerates — tan is undefined, so A + B is an **odd multiple of π/2**. For x > 0 both A, B ∈ (0, π/2), so A + B ∈ (0, π) and the only possibility is A + B = **π/2**. For x < 0 both terms are negative: A + B = **−π/2**.
*Step 3 — The constant check (why the identity can't be global).* The identity "arctan x + arctan(1/x) = π/2" holds only for x > 0; extending it across zero would force a jump from −π/2 to +π/2 through a point where f is undefined — the two constants belong to two separate branches.
*Step 4 — Sketch.* Two horizontal half-lines: f = π/2 for x > 0; f = −π/2 for x < 0. Jump discontinuity at x = 0 (left limit −π/2, right limit +π/2; f(0) undefined). (Optional derivative view: f′(x) = 1/(1+x²) − 1/(1+x²) = 0 on each branch — constant on each, but the constants differ.)

**4. Numerical Result.**
f(x) = π/2 (x > 0); −π/2 (x < 0); jump discontinuity at 0.

**5. Verification.**
x = 1: arctan 1 + arctan 1 = π/4 + π/4 = π/2 ✓. x = −1: −π/4 − π/4 = −π/2 ✓. x = 2: arctan 2 + arctan(1/2) = 1.107 + 0.464 = 1.571 = π/2 ✓.

**6. Conclusion & Discussion.**
The question is Trinity's own showcase for "the actual aim might be different from what it seems": the formula-fond candidate draws one horizontal line and is wrong; the careful one asks *where* the identity holds and finds two half-lines and a jump. Blind formula application is the target, not the tool.


#### M3 — A Medical Screening Test (Source: T1-17 · Trinity College Cambridge, NST Admissions Guidance paper)

> "G3. A certain medical condition affects one in a thousand of the population. A screening procedure is developed that is 95% accurate. Discuss the probability that you have the condition if the screening procedure says that you do."

**Thought.** Bayes' theorem is one line; the discipline is questioning 'accurate' and auditing the base rate with a frequency table. The two-percent answer against ninety-five-percent intuition is the lesson.


**1. Statement & Symbols.**
Prevalence P(D) = 0.001; test "95% accurate". Interpret as sensitivity = specificity = 0.95 (the natural reading — and worth stating as an assumption, since "accurate" is ambiguous). Find P(D|+).

**2. Governing Principles.**
Bayes' theorem; the base-rate fallacy as the phenomenon to expose.

**3. Derivation.**
*Step 1 — State the ingredients.* P(+|D) = 0.95 (sensitivity); P(−|¬D) = 0.95, so P(+|¬D) = 0.05 (false-positive rate); P(D) = 0.001, P(¬D) = 0.999.
*Step 2 — Bayes.*
P(D|+) = P(+|D)P(D) / [P(+|D)P(D) + P(+|¬D)P(¬D)]
= (0.95×0.001)/[(0.95×0.001) + (0.05×0.999)]
= 0.00095/(0.00095 + 0.04995) = 0.00095/0.05090 = **0.0187 ≈ 2%**.
*Step 3 — The intuitive cross-check (counts per 100,000).* Diseased: 100 people, of whom 95 test positive. Healthy: 99,900 people, of whom 5% = 4,995 test positive. Total positives = 5,090; true positives among them = 95; 95/5090 = 1.9% ✓.
*Step 4 — The "discuss" layer.* (i) Ambiguity of "accurate": sensitivity and specificity differ in general; the answer depends on both. (ii) The paradox is the base rate: with a 1/1000 condition, even a 95% test is dominated by false positives. (iii) Remedies: repeat testing (a second positive on an independent test raises P(D|++) to ≈ 27% by the same formula), or enriching the tested population (testing only symptomatic patients raises the prior).

**4. Numerical Result.**
P(D|+) ≈ 2% under the symmetric-95% reading.

**5. Verification.**
The frequency table and the formula agree to 3 s.f. ✓. Limit check: as prevalence → 50%, P(D|+) → 95% — recovering the naive intuition that "95% accurate" should mean something ✓.

**6. Conclusion & Discussion.**
A one-line Bayes formula plus a 100,000-person frequency audit: the arithmetic is trivial, the discipline is questioning "accurate" and respecting the base rate. The examiner's verb is "discuss" — the discussion, not the number, is the answer.
