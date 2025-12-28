https://wessengetachew.github.io/2025/

All of 2025 work by Wessen

# Möbius Shell Sieve

**A Comprehensive Interactive Platform for Exploring Number Theory & the Riemann Hypothesis**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Plotly](https://img.shields.io/badge/Plotly-3F4F75?logo=plotly&logoColor=white)](https://plotly.com/javascript/)

---

## Overview

The **Möbius Shell Sieve** is a single-file, browser-based research platform integrating **65 interactive visualization tools** for exploring number theory—from lattice point counting and the Basel problem to the Riemann Hypothesis and random matrix theory.

Every tab features:
- 🎛️ **Interactive Controls** — Sliders, dropdowns, and input fields with real-time updates
- 📊 **Live Statistics Dashboard** — Big-number cards with mathematical metrics
- 📈 **Multiple Plotly Charts** — Interactive, zoomable visualizations
- 📚 **Theory Panels** — Mathematical background and key formulas
- 🎯 **Preset Examples** — One-click configurations for notable cases
- 📥 **Export Options** — CSV data, PNG screenshots, complete tab exports
- 🌓 **Dark/Light Mode** — Toggleable theme that persists across sessions

---

## Quick Start

```bash
# Clone the repository
git clone https://github.com/wessengetachew/mobius-shell-sieve.git

# Open in browser (no server required)
open mobius-full.html
# or
xdg-open mobius-full.html  # Linux
start mobius-full.html     # Windows
```

The entire application is contained in a single HTML file (~17,000 lines). No build process, no dependencies to install—just open and explore.

---

## Features by Category

### 🔷 Lattice & Geometry (Tabs 1–3)

| Tab | Description |
|-----|-------------|
| **2D Lattice** | Gauss circle problem, primitive points, Basel density 6/π² ≈ 0.608 |
| **3D Ball** | 3D lattice visualization, Apéry's constant 1/ζ(3) ≈ 0.832 |
| **Möbius μ(n)** | Möbius function visualization, Mertens function M(x) |

### 🔷 Modular Arithmetic (Tabs 4–7)

| Tab | Description |
|-----|-------------|
| **Modular Rings** | Residue class geometry, multi-modulus and Farey channel views |
| **Cayley ℍ** | Cayley transform disk↔half-plane, Ford circles, hyperbolic geodesics |
| **Farey** | Farey sequences F_n, mediant property, Ford circle visualization |
| **Primitive Roots** | Generators of (ℤ/nℤ)×, discrete logarithm visualization |

### 🔷 Analysis & Error (Tabs 8–10)

| Tab | Description |
|-----|-------------|
| **Error Analysis** | E(R) = V(R) − 6R²/π², normalized error, RH connection |
| **Dimensions** | Primitive density 1/ζ(k) across dimensions k = 2 to 8 |
| **Shells** | GCD layer decomposition, Möbius shell contributions |

### 🔷 Classical Problems (Tabs 11–14)

| Tab | Description |
|-----|-------------|
| **GCD Analysis** | Statistical GCD distribution, mean ≈ ζ(2) |
| **Gaussian ℤ[i]** | Gaussian integers, primes, norms, units {±1, ±i} |
| **Circle Problem** | N(R) = πR² + E(R), error exponent analysis |
| **Density 1/ζ** | Empirical verification of primitive density convergence |

### 🔷 Characters & Primes (Tabs 15–17)

| Tab | Description |
|-----|-------------|
| **Dirichlet χ** | Dirichlet characters mod q, L-function visualization |
| **Twin Primes** | (p, p+2) pairs, Brun's constant B₂ ≈ 1.902, Hardy-Littlewood |
| **Prime Counting π(x)** | π(x) vs x/ln(x) vs Li(x), prime number theorem |

### 🔷 Advanced Topics (Tabs 18–26)

| Tab | Description |
|-----|-------------|
| **Composite Channels** | Residue projection onto Farey channels |
| **Coprime Pairs** | V(R) counting, error term E(R), RH equivalence |
| **Sierpiński** | Uncovered integers in 6ab ± a ± b representation |
| **k-Free** | Squarefree/cubefree density 1/ζ(k) |
| **Euler ∏** | Compute π and ζ(2n) via Euler product |
| **Chord CV** | Prime detection heuristic via chord uniformity |
| **Goldbach** | Even = p + q partitions, Goldbach comet |
| **Prime Gaps** | g_n = p_{n+1} − p_n, Cramér's conjecture |
| **Sophie Germain** | Primes p where 2p+1 also prime, safe primes |

### 🔷 RH Connection (Tabs 27–29)

| Tab | Description |
|-----|-------------|
| **Mertens M(x)** | M(x) = Σμ(n), RH ⟺ M(x) = O(x^{1/2+ε}) |
| **Chebyshev ψ** | ψ(x) = Σ Λ(n), θ(x) = Σ log p, explicit formula |
| **Li(x)** | Logarithmic integral, Skewes number, sign changes |

### 🔷 Arithmetic Functions (Tabs 30–32)

| Tab | Description |
|-----|-------------|
| **Divisor d(n)** | τ(n) counts, σ(n) sums, Robin's inequality |
| **Liouville λ** | λ(n) = (−1)^{Ω(n)}, Pólya conjecture |
| **Mangoldt Λ** | Λ(n) = log p if n = p^k, prime power weights |

### 🔷 Visual Patterns (Tabs 33–35)

| Tab | Description |
|-----|-------------|
| **Ramanujan c_q** | Ramanujan sums, always integers, heatmap view |
| **Ulam Spiral** | Square spiral with prime diagonals |
| **Sacks Spiral** | Archimedean spiral, parabolic prime arms |

### 🔷 Critical Line (Tabs 36–41)

| Tab | Description |
|-----|-------------|
| **Hardy Z(t)** | Real-valued Z(t), sign changes = zeros |
| **Gram Points** | θ(g_n) = nπ, Gram's law, Lehmer pairs |
| **Explicit π(x)** | Build π(x) from zeta zeros, animated |
| **N(T) Zeros** | Zero counting function, Riemann-von Mangoldt |
| **ζ(s) Argand** | Domain coloring of ζ(s) in complex plane |
| **ζ(s) Real** | Zeta on real axis, pole at s=1, trivial zeros |

### 🔷 Zero Statistics (Tabs 42–43)

| Tab | Description |
|-----|-------------|
| **Montgomery** | Pair correlation R₂(x) = 1 − (sin πx/πx)² |
| **GUE Stats** | Gaussian Unitary Ensemble, Wigner surmise |

### 🔷 Prime Races & L-Functions (Tabs 44–46)

| Tab | Description |
|-----|-------------|
| **Prime Races** | Chebyshev bias, π(x;4,3) vs π(x;4,1) |
| **L-functions** | L(s,χ) visualization, principal vs non-principal |
| **L-func Zeros** | GRH zeros, low-lying zero distribution |

### 🔷 Quantum Connection (Tab 47)

| Tab | Description |
|-----|-------------|
| **Quantum Orbitals** | ψ_{nlm} wavefunctions, radial nodes ↔ zeta zeros |

### 🔷 Prime Patterns (Tabs 48–50)

| Tab | Description |
|-----|-------------|
| **Prime k-Tuples** | Triplets, quadruplets, Hardy-Littlewood conjecture |
| **Carmichael** | Pseudoprimes, Korselt's criterion, 561 = 3·11·17 |
| **Mersenne** | 2^p − 1 primes, Lucas-Lehmer test, GIMPS |

### 🔷 Rational Approximation (Tabs 51–52)

| Tab | Description |
|-----|-------------|
| **Continued Fractions** | [a₀; a₁, a₂, ...], best approximations, 355/113 |
| **Stern-Brocot** | Binary tree of all positive rationals |

### 🔷 Diophantine Equations (Tabs 53–55)

| Tab | Description |
|-----|-------------|
| **Pythagorean** | a² + b² = c² triples, parametrization (m² − n², 2mn, m² + n²) |
| **Sum of Squares** | r₂(n), Fermat's theorem, Jacobi formula |
| **Quadratic Residues** | Legendre symbol, quadratic reciprocity |

### 🔷 Combinatorial Sequences (Tabs 56–59)

| Tab | Description |
|-----|-------------|
| **Partitions p(n)** | Hardy-Ramanujan asymptotic, Ramanujan congruences |
| **Bernoulli** | B_n, ζ(−n), connection to ζ(2n) = π^{2n} × rational |
| **Fibonacci** | F_n → φ, Binet formula, Zeckendorf representation |
| **Catalan** | C_n = (2n)!/((n+1)!n!), 200+ interpretations |

### 🔷 Divisor Theory (Tabs 60–63)

| Tab | Description |
|-----|-------------|
| **Aliquot** | Iterated σ(n) − n, amicable pairs, sociable cycles |
| **Cyclotomic** | Φ_n(x), primitive roots of unity, deg = φ(n) |
| **Highly Composite** | d(n) record breakers, Ramanujan's analysis |
| **Perfect Numbers** | σ(n) = 2n, Euclid-Euler theorem, odd perfect? |

### 🔷 Famous Numbers (Tabs 64–65)

| Tab | Description |
|-----|-------------|
| **Taxicab** | Ta(2) = 1729 = 1³ + 12³ = 9³ + 10³ (Hardy-Ramanujan) |
| **Elliptic Curves** | y² = x³ + ax + b, group law, BSD conjecture, ECDSA |

### 🔷 Dynamics (Tab 66)

| Tab | Description |
|-----|-------------|
| **Collatz** | 3n+1 conjecture, trajectories, stopping times |

---

## Key Mathematical Theorems Visualized

| Theorem | Year | Visualization |
|---------|------|---------------|
| **Euler Product** ζ(s) = ∏(1−p^{−s})^{−1} | 1737 | Euler ∏ tab |
| **Basel Problem** ζ(2) = π²/6 | 1734 | 2D Lattice, Euler ∏ |
| **Möbius Inversion** | 1832 | Möbius μ(n), Shells |
| **Dirichlet's Theorem** (primes in AP) | 1837 | Dirichlet χ, Prime Races |
| **Prime Number Theorem** π(x) ~ x/ln(x) | 1896 | π(x), Li(x), Chebyshev |
| **Riemann Hypothesis** Re(ρ) = ½ | 1859 | Hardy Z(t), Argand, N(T) |
| **Hardy-Littlewood Conjecture** | 1923 | Twin Primes, k-Tuples |
| **Montgomery Pair Correlation** | 1973 | Montgomery, GUE |

---

## Export Capabilities

### Per-Tab Exports
- **📷 Screenshot** — High-resolution PNG of canvas + dashboard
- **📦 All** — Complete tab export (all canvases + charts + stats)
- **📄 CSV** — Raw data for external analysis

### Export Features
- 4K resolution (2× scale)
- Professional title headers and footers
- Dark/light theme matching
- Timestamped filenames

---

## Technical Details

### Architecture
- **Single HTML file** — No build process, fully self-contained
- **Vanilla JavaScript** — No framework dependencies
- **Plotly.js** — Interactive charts (loaded via CDN)
- **Canvas API** — Custom visualizations
- **CSS Variables** — Theme switching

### Browser Support
- Chrome 80+ ✅
- Firefox 75+ ✅
- Safari 13+ ✅
- Edge 80+ ✅

### Performance
- Debounced slider inputs for smooth interaction
- Efficient canvas rendering with requestAnimationFrame
- Lazy chart initialization on tab switch

---

## Mathematical References

### Primary Sources
- Edwards, H.M. (1974). *Riemann's Zeta Function*. Academic Press.
- Apostol, T.M. (1976). *Introduction to Analytic Number Theory*. Springer.
- Hardy, G.H. & Wright, E.M. (2008). *An Introduction to the Theory of Numbers*. 6th ed. Oxford.
- Titchmarsh, E.C. (1986). *The Theory of the Riemann Zeta Function*. 2nd ed. Oxford.
- Montgomery, H.L. & Vaughan, R.C. (2007). *Multiplicative Number Theory I*. Cambridge.

### Online Resources
- [OEIS](https://oeis.org) — Online Encyclopedia of Integer Sequences
- [LMFDB](https://www.lmfdb.org) — L-functions and Modular Forms Database
- [Prime Pages](https://primes.utm.edu) — Prime number encyclopedia

---

## Credits

### Mathematical Attribution
The platform visualizes theorems and concepts from:
- **Leonhard Euler** — Euler product, Basel problem, totient function
- **Carl Friedrich Gauss** — Gaussian integers, prime counting, circle problem
- **Bernhard Riemann** — Zeta function, Riemann Hypothesis
- **August Ferdinand Möbius** — Möbius function, inversion formula
- **Peter Gustav Lejeune Dirichlet** — L-functions, characters, primes in AP
- **G.H. Hardy & J.E. Littlewood** — Prime constellations, circle method
- **Srinivasa Ramanujan** — Partition asymptotics, tau function, 1729
- **Hugh Montgomery** — Pair correlation conjecture

### Development
Created by **Wessen Getachew** ([@7dview](https://twitter.com/7dview))

---

## License

MIT License — see [LICENSE](LICENSE) for details.

---

## Contributing

Contributions welcome! Please open an issue or pull request for:
- Bug fixes
- New visualization tabs
- Performance improvements
- Documentation updates

---

## Roadmap

### Planned Features
- [ ] Dedekind eta function visualization
- [ ] Modular forms and cusp forms
- [ ] Class number computation
- [ ] Arithmetic geometry visualizations
- [ ] WebGL acceleration for large datasets

---

*"The primes are the atoms of arithmetic."* — Marcus du Sautoy
