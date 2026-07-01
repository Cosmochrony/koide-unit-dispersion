# KUD — The Charged-Lepton Koide Relation as a Unit-Dispersion Constraint

J. Beau, Independent Researcher, France

## Status

Preprint, v1.0. Concept DOI: [10.5281/zenodo.21109812](https://doi.org/10.5281/zenodo.21109812)

Source note (reconnaissance): it fixes a target invariant for the charged-lepton mass sector; it does
not derive the masses.

## Abstract

Writing the square-root mass vector $r_\ell = (\sqrt{m_e}, \sqrt{m_\mu}, \sqrt{m_\tau})$ with mean
$\bar r$ and standard deviation $\sigma_r$, the Koide quotient is exactly

$$ Q_\ell = \frac{1 + \mathrm{CV}(r_\ell)^2}{3}, \qquad \mathrm{CV}(r_\ell) = \sigma_r/\bar r, $$

so that

$$ Q_\ell = 2/3 \iff \mathrm{CV}(r_\ell) = 1 \iff \sigma_r = \bar r. $$

The charged-lepton square-root masses have unit relative dispersion (checked: $\mathrm{CV} = 0.99999$).
This is the sharpest scale-free statement of the relation, and it separates the intrinsic dispersion
target from the concrete hierarchy.

## Results

1. **Unit-dispersion identity.** $Q_\ell = (1 + \mathrm{CV}(r_\ell)^2)/3$; Koide $\iff \mathrm{CV} = 1$.

2. **Dispersion versus hierarchy.** In the cyclic form $r_g = \bar r(1 + \sqrt2\cos(\delta + 2\pi g/3))$,
   $Q_\ell = 2/3$ fixes the amplitude $\sqrt2$ for every $\delta$; $\delta$ places one generation near a
   node of the square-root profile, which is what produces the large hierarchy. The two targets — the
   dispersion $\mathrm{CV} = 1$ and the node placement — are independent, the node placement being the
   harder, exponentially sensitive residue.

3. **Cascade-ladder obstruction.** The pinned ladder $(1, \tfrac12 + u, \tfrac12 - u)$ has
   $\mathrm{CV} \le 1/\sqrt2$ ($Q \le 1/2$); the committed Yukawa carrier $H_\Pi^{1/2}$ gives
   $\mathrm{CV}(r_\ell) \in [0.09, 0.37]$, with the single norm $\lambda_Y$ cancelling in $\mathrm{CV}$.
   The maximum-entropy carrier of $\mathrm{CV} = 1$ cannot be the square root of the level ladder.

4. **Maximum-entropy reading (open test).** $\mathrm{CV} = 1$ is the unit dispersion of the exponential
   (maximum entropy on $\mathbb{R}_+$ at fixed mean). The crux is the constraint — only a first-moment
   condition on $\sqrt m$ gives $\mathrm{CV} = 1$ (the natural quadratic norm gives $0.756$) — and, one
   level below, the discrete-to-continuous bridge: three discrete masses do not inherit the continuous
   unit dispersion (the discrete-weight extremum is uniform, $\mathrm{CV} = 0$). A forced continuous
   generation coordinate with forced three-point realisations of discrete $\mathrm{CV} = 1$ is required.

## Position in the programme

This note belongs to the **fermionic matter sub-programme**. It is downstream of the **Projected Yukawa
Line** (PYL) and **Projected Yukawa Operator** (PYO) notes, whose generation-level ladder it shows to
under-disperse, and it points the entropic reading at the projection entropy of the non-injective
projection (ENI). It records a target invariant, not a mass formula.

## Build

```bash
cd tex
pdflatex -output-directory=../out KoideUnitDispersion.tex
cd ../out && bibtex KoideUnitDispersion && cd ../tex
pdflatex -output-directory=../out KoideUnitDispersion.tex
pdflatex -output-directory=../out KoideUnitDispersion.tex
```
