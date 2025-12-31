

# Möbius Shell Sieve

**An Interactive Number Theory Visualization Platform**

A comprehensive single-file HTML application featuring 68+ interactive tools for exploring prime numbers, the Riemann Hypothesis, modular arithmetic, and foundational number theory concepts.

## Live Demo

**[Launch Möbius Shell Sieve](https://wessengetachew.github.io/2025/)**

## Features

### Unified Explorers

**ℤ² Lattice Explorer** — 3 integrated tools:
- Primitive Lattice Points (6/π² density, Basel problem connection)
- Gaussian Integers ℤ[i] (complex primes, norms, UFD structure)
- Circle Problem (N(R) = πR² + E(R), Hardy conjecture)

**ζ Riemann Hypothesis Hub** — 9 unified tools:
- RH Error Bound (von Koch's conditional estimate)
- Hardy Z(t) Function (real-valued, sign changes = zeros)
- Gram Points (zero organization, Gram's Law)
- Explicit Formula (Riemann's prime counting formula)
- Zero Count N(T) (Riemann-von Mangoldt formula)
- Argand Plot (ζ(½+it) in complex plane)
- Zeta Real Axis (poles, trivial zeros, functional equation)
- Montgomery Pair Correlation (random matrix connection)
- GUE Statistics (Gaussian Unitary Ensemble)

### Original Research Tools

**Wessen Identity** — Novel finite-cutoff framework:
```
R_H(p_max) = A_H × C_H(p_max) × [M_no2(p_max)]^k
```
Connects modular sieve densities to Hardy-Littlewood constants with machine-precision verification.

**Chord CV Analysis** — Geometric approach to prime gap patterns through chord length coefficient of variation.

### Interactive Visualizations (60+ Tools)

**Lattice & Geometry**
- 2D/3D Primitive Points
- Farey Sequences & Ford Circles
- Cayley Transforms
- Smith Chart Projections
- Pythagorean Triples
- Sum of Two Squares

**Prime Distribution**
- Twin Primes & Prime Gaps
- Sophie Germain Primes
- Goldbach Conjecture
- Prime Races (Chebyshev bias)
- Ulam & Sacks Spirals
- Prime Constellations (k-tuples)

**Modular Arithmetic**
- Primitive Roots
- Quadratic Residues
- Dirichlet Characters
- Cyclotomic Polynomials
- Chinese Remainder Theorem

**Arithmetic Functions**
- Möbius Function μ(n)
- Euler's Totient φ(n)
- Divisor Functions σ(n), τ(n)
- Liouville Function λ(n)
- Von Mangoldt Function Λ(n)
- Mertens Function M(n)

**Special Numbers**
- Carmichael Numbers
- Mersenne Primes
- Perfect Numbers
- Highly Composite Numbers
- Taxicab Numbers

**Sequences**
- Fibonacci & Lucas
- Bernoulli Numbers
- Catalan Numbers
- Partition Function p(n)
- Continued Fractions
- Stern-Brocot Tree
- Collatz Conjecture
- Aliquot Sequences

**Advanced Topics**
- L-Functions & Zeros
- Elliptic Curves
- Quantum Number States

## Technical Details

### Single-File Architecture

The entire application is contained in one HTML file (~1.4MB, ~26,000 lines) with:
- Inline CSS with CSS variables for theming
- Vanilla JavaScript (no build tools required)
- Plotly.js for interactive charts
- html2canvas for screenshot exports

### Key Functions

```javascript
// Core enumeration
enum2D(R, shape)        // Enumerate lattice points
gcd(a, b)               // Greatest common divisor
mobius(n)               // Möbius function
euler(n)                // Euler's totient

// Zeta computations
zeta(s)                 // Riemann zeta (real s > 1)
zetaComplex(s, t)       // ζ(s + it) approximation
hardyZ(t)               // Hardy Z-function
thetaRiemann(t)         // Riemann-Siegel theta

// Sieve functions
modularSieve(M, gap)    // Compute sieve statistics
wessenIdentity(M, gap)  // Full identity computation
```

### Export Capabilities

Every tool supports:
- **Screenshot** — Composite image with charts + statistics
- **4K Export** — High-resolution dashboard captures
- **CSV Export** — Raw data for external analysis
- **PNG Export** — Individual chart/canvas images

## Usage

### Local Development

```bash
# Clone the repository
git clone https://github.com/wessengetachew/mobius-shell-sieve.git

# Open directly in browser
open mobius-shell-sieve.html
# or
python -m http.server 8000
```

### Keyboard Shortcuts

- **Enter** in any input field triggers computation
- **Click** on data points, table rows, or canvas elements for detailed analysis modals

### URL Parameters

Direct linking to specific tabs:
```
mobius-shell-sieve.html#t2d      # 2D Lattice
mobius-shell-sieve.html#trh      # RH Hub
mobius-shell-sieve.html#twessen  # Wessen Identity
```

## Mathematical Background

### The Basel Problem Connection

The density of primitive lattice points (coprime pairs) approaches:

```
lim(R→∞) P(R) / πR² = 6/π² = 1/ζ(2) ≈ 0.6079
```

This connects lattice geometry to the Riemann zeta function.

### Möbius Inversion

The shell decomposition uses Möbius inversion:

```
P(R) = Σ_{k=1}^{∞} μ(k) · L(R/k)
```

Where L(r) counts all lattice points in radius r, and μ(k) is the Möbius function.

### Hardy-Littlewood Constants

For prime k-tuples with pattern H = {h₁, ..., h_k}, the conjectured density involves:

```
C_H = ∏_p (1 - ν_H(p)/p) / (1 - 1/p)^k
```

Where ν_H(p) counts distinct residues of H mod p.

## Themes

Four built-in color schemes:
- **Midnight** (default) — Dark blue background
- **Terminal** — Green on black
- **Light** — Clean white background
- **Sepia** — Warm paper tones

## Browser Compatibility

Tested on:
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

Requires JavaScript enabled. WebGL recommended for 3D visualizations.

## Performance Notes

- Most tools handle R ≤ 200 smoothly
- Large computations (R > 500) may cause brief freezes
- 3D visualizations benefit from hardware acceleration

## Contributing

Contributions welcome! Areas of interest:
- Additional number-theoretic visualizations
- Performance optimizations
- Accessibility improvements
- Documentation and tutorials

## License

MIT License — Free for educational and research use.

## Author

**Wessen Getachew**
- GitHub: [@wessengetachew](https://github.com/wessengetachew)
- Twitter: [@7dview](https://twitter.com/7dview)

## Acknowledgments

- Plotly.js for charting
- html2canvas for screenshot generation
- The number theory community for inspiration
- OEIS for reference sequences

---

*"Mathematics is the queen of sciences and number theory is the queen of mathematics."* — Carl Friedrich Gauss

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
