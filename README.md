# Quantitative-Harmonic-Benchmarks-for-the-Three-Dimensional-Quantum-Rotor-Kernel-Zero-Point Energy, Bond Fluctuations, Finite-Size Scaling, and Their Limits within the
FQCU Programme
Quantum Rotor Kernel — Harmonic Benchmarks and Validity Diagnostics 1
Quantitative Harmonic Benchmarks for the
Three-Dimensional Quantum Rotor Kernel
Zero-Point Energy, Bond Fluctuations, Finite-Size Scaling, and Their Limits within the
FQCU Programme
Professor Dr. Md. Faridul Islam Chowdhury
MBBS, MS—Neurosurgery
Tanfarid Vision Research Institute, Bogura, Bangladesh
Revised manuscript — November 15, 2026
Abstract
We formulate harmonic benchmarks for a three-dimensional compact quantum rotor kernel
considered within the Farid Quantum Command Unit (FQCU) programme. Unitary phase operators
define the quantum theory without assuming an unrestricted global angle commutator. The
harmonic construction separates the uniform mode from nonzero oscillators and gives a zero-point
energy per site, local phase variance, and nearest-neighbour bond variance. Direct lattice sums,
tensor Gauss–Legendre quadrature, and independent one-dimensional scaled-Bessel integrals
provide numerical cross-checks. We conservatively quote the thermodynamic constants as I₃ ≈
1.193801121 and W₃ ≈ 0.9106881033, ten significant digits each. Their finite-size differences scale
as L⁻⁴ and L⁻². Gaussian factorization gives a leading quartic-to-quadratic potential ratio of
approximately 0.0995 gQ, where gQ = ħ/√(IJ). This is a perturbative diagnostic, not a rigorous
accuracy bound or an interacting critical-point determination. No physical microscopic scale,
particle identification, or FQCU-specific observable is established. Reproducible calculation files
accompany the manuscript.
Keywords: quantum rotor; harmonic approximation; zero-point energy; bond fluctuations;
Brillouin-zone integrals; finite-size scaling; FQCU; numerical verification.
1. Introduction and programme terminology
A mathematical kernel becomes a useful research instrument when its assumptions, calculable
consequences, approximation errors, and physical interpretation are distinguished. The present
article examines a conventional quantum rotor Hamiltonian as a candidate kernel within the FQCU
programme. It does not claim that solving that kernel identifies a fundamental constituent of nature.
Within this programme, Level 1 denotes specification of the classical rotor kernel, Level 2 denotes
its numerical benchmark programme, and Level 3 denotes the quantum extension examined here.
These are internal organizational labels. They do not imply that all numerical validation
requirements at earlier levels have been completed, nor do they designate experimentally
established layers of matter.
The contribution is a reproducible harmonic reference: consistent compact quantization, energy
normalization, zero-mode treatment, two lattice constants, finite-size checks, and a
tolerance-dependent anharmonic screening measure. Standard quantum many-body and rotor
literature provides the broader context [1,2]. No new physical mechanism is inferred from
agreement with these mathematical results.
2. Classical kernel and energy convention
Consider a periodic cubic lattice with N = L³ sites and spacing ell. Each site has an angle and
conjugate momentum. Every undirected bond is counted once; the conventional six-neighbour lattice
is assumed.
Quantum Rotor Kernel — Harmonic Benchmarks and Validity Diagnostics 2
(1)
(2)
The aligned zero-momentum classical configuration has zero energy in this convention. The
alternative potential −J cos(Δθ) changes the Hamiltonian by −3NJ on the ordinary periodic cubic
lattice. It leaves equations of motion unchanged but changes the quoted ground-state energy.
Throughout this article the shifted, nonnegative interaction convention above is used. Classical XY
rotor dynamics is established background, not a new interaction derived here [3].
3. Compact quantum formulation
Use the periodic Hilbert space given by a tensor product of L²(S¹) spaces, with angular-momentum
operators and unitary phase operators. The conventional integer-momentum representation is
specified explicitly:
(3)
(4)
(5)
The unitary formulation avoids treating the unrestricted angle–momentum commutator as a global
operator identity on a compact coordinate. The dimensionless coupling and bare harmonic speed are
(6)
In the decoupled limit J → 0 at fixed I, the lowest local state has m = 0 and a uniform angular
wavefunction. It is angular-momentum localized and phase delocalized; “localized phases” would
reverse that statement. The interacting thermodynamic phase diagram is not derived below.
4. Harmonic modes and the uniform coordinate
For small neighbouring phase differences, expand 1 − cos(Δφ) = (Δφ)²/2 − (Δφ)⁴/24 + higher orders.
A phase-unwrapped quadratic description about an aligned reference separates the uniform
collective motion from nonzero oscillators:
(7)
(8)
The spectrum is exact for the harmonic lattice equations, not for the interacting compact theory. The
uniform mode is a collective rotor coordinate, not an oscillator of finite frequency. The separation
above belongs to the harmonic reference construction and does not assert an unrestricted global
factorization of the compact many-body Hilbert space.
(9)
Quantum Rotor Kernel — Harmonic Benchmarks and Validity Diagnostics 3
Local variances calculated after removing the uniform mode are relative to an aligned phase
reference. They are not exact compact-angle variances of the finite-system ground state. Symmetry
restoration, compactness, and anharmonicity require separate analysis; no universal exponentially
small tunnelling correction is assumed.
Figure 1. Harmonic axis dispersion in units of √(J/I), compared with its long-wavelength linear approximation. The
difference is a lattice property, not evidence for a physical substrate.
5. Zero-point energy and two lattice sums
(10)
(11)
The indices are nμ = 0,…,L−1, excluding only the uniform mode. In the zero-total-momentum
harmonic sector,
(12)
(13)
(14)
The first expression is energy per site; the second is energy per physical volume. With the unshifted
−J cos interaction, −3J must be added to the per-site energy. Neither convention supplies an
observed cosmological vacuum-energy prediction without a separate physical and gravitational
matching argument.
Quantum Rotor Kernel — Harmonic Benchmarks and Validity Diagnostics 4
6. Numerical evaluation and precision policy
With q a dimensionless Brillouin-zone coordinate, define S(q) = Σμ sin²(qμ/2). The thermodynamic
constants are the zone averages of √S and 1/√S. Near zero, S ≈ |q|²/4. Thus the inverse-frequency
integrand has a 1/|q| singularity, not a logarithmic singularity; its three-dimensional integral is
finite.
(15)
The thermodynamic limit is taken at fixed spacing. It is distinct from a continuum limit in which ell
tends to zero. The reproducibility script evaluates direct finite sums and two forms of numerical
quadrature.
The independent one-dimensional representation uses scaled modified Bessel functions, not an
angular-reduction approximation. Let Iν(z) denote the modified Bessel function and define
(16)
(17)
These follow from a Laplace representation of the powers of S and integration by parts for the
energy integral. Scaled Bessel functions avoid directly multiplying exponentially growing and
decaying factors in floating-point arithmetic.
For the manuscript’s principal results we conservatively quote ten significant digits:
(18)
Points/axis W3: octant GL Difference from Bessel
100 0.91068810975106 6.462e-09
200 0.91068810369691 4.080e-10
400 0.91068810331448 2.562e-11
A conventional positive-octant Gauss–Legendre quadrature with 400 points per axis differs from the
one-dimensional W₃ evaluation by about 2.56 × 10⁻¹¹. Both evaluations round to the main-text value
above. Longer outputs are preserved in numerical_metadata.json and the CSVs as computational
records, not certified digits. Quadrature tolerances and reported error estimates are not rigorous
interval bounds [4]. No fifteen-digit accuracy claim is made.
The direct-sum grid independently tests finite-size convergence. No undocumented Richardson
procedure is claimed to certify the final digits. All scaled differences use the unrounded internal
Bessel reference; using the rounded main-text value would contaminate the small differences,
especially after multiplication by L⁴.
Quantum Rotor Kernel — Harmonic Benchmarks and Validity Diagnostics 5
7. Finite-size convergence
L I3(L) W3(L)
8 1.193592307087 0.896664057602
16 1.193788279156 0.907165291425
32 1.193800321733 0.909806442910
64 1.193801071494 0.910467629592
128 1.193801118309 0.910632981221
256 1.193801121235 0.910674322544
The displayed finite-sum values are rounded floating-point outputs. The next table shows scaled
differences rather than a complete fitted extrapolation model. Its energy coefficient is deliberately
rounded because reference and subtraction errors are amplified by L⁴.
L L⁴[I3 − I3(L)] L²[W3 − W3(L)]
8 0.8553 0.89754
16 0.8416 0.90184
32 0.8385 0.90282
64 0.8378 0.90306
128 0.8376 0.90312
256 0.8376 0.90313
(19)
(20)
The infrared powers are consistent with radial integrals of k³ and k, respectively. This argument
explains the powers, not the numerical coefficients. The coefficients depend on the prescribed
periodic geometry and normalization.
If D = L ell is the physical box length, the corresponding harmonic energy-density difference is
(21)
This is a Casimir-like finite-size property of the harmonic model. It is a mathematical cross-check,
not an experimental Casimir measurement or evidence for gravitational vacuum energy.
Quantum Rotor Kernel — Harmonic Benchmarks and Validity Diagnostics 6
Figure 2. Recomputed harmonic benchmarks: (a) energy-sum convergence; (b) L⁻⁴ energy correction; (c) L⁻²
inverse-frequency correction; (d) zero-mode-removed local and bond RMS values. Panel (d) is a harmonic extrapolation,
not an interacting quantum phase diagram. No critical coupling is shown.
8. Bond fluctuations and anharmonic screening
Since the interaction depends on differences across bonds, the nearest-neighbour variance connects
directly to the cosine expansion. The Fourier form factor and cubic symmetry give
(22)
(23)
At gQ = 1 the local and bond RMS values are approximately 0.477 and 0.631 rad. For this kernel the
bond value is larger and is more directly relevant to expansion of the interaction. It is not a universal
inequality for unrelated models.
Gaussian factorization gives ⟨(Δφ)⁴⟩ = 3⟨(Δφ)²⟩². The magnitude of the leading quartic expectation
relative to the quadratic potential expectation is
(24)
The quartic contribution itself is negative relative to the quadratic term. At gQ = 1 its Gaussian
estimate is about ten percent of the harmonic potential expectation. This is not a ten-percent error
guarantee for the ground state, energy, spectrum, or correlations. It does not establish a critical
point or a universal boundary at gQ = 1.
Quantum Rotor Kernel — Harmonic Benchmarks and Validity Diagnostics 7
(25)
This tolerance-dependent inequality is a screening condition on one leading estimate. Higher orders,
compact configurations, and state changes require direct interacting calculations before an
accuracy claim is made.
9. Limits and next calculations
No interacting critical coupling is determined. A nonperturbative calculation for this Hamiltonian
and normalization is needed. A published Monte Carlo study of a different dimensional model can
guide methods but cannot provide a critical number by direct transfer [2]. No registration of such a
future study is asserted here.
The long-wavelength speed fixes only one parameter combination if calibrated to a measured
constant. The interpretation of ell remains open: it is a prescribed geometric parameter of the lattice
model, not an already measured substrate spacing. The model is not automatically a numerical
regulator of a known continuum theory either; that interpretation requires its own matching
argument.
No photon, electron, quark, or other particle identification is derived. The results follow from a
shared rotor Hamiltonian and do not constitute an FQCU-specific observable. A distinct physical
interpretation must add a justified rule or constraint with measurable consequences that
conventional alternatives cannot reproduce.
The next computational steps are interacting comparisons of bond correlations, ground-state energy
differences, spectra, and stiffness, with size, temperature, and algorithmic convergence where
relevant. Agreement of one quantity does not establish equivalent accuracy for another. Exact code
versions, raw outputs, parameter conventions, and uncertainty procedures should accompany those
studies.
10. Conclusion
The compact rotor kernel admits a defined quantum formulation and a tractable harmonic reference.
Two thermodynamic Brillouin-zone constants have been cross-checked numerically and are quoted
conservatively to ten significant digits. Energy and inverse-frequency sums exhibit different
finite-size powers, while local and bond variances provide complementary fluctuation diagnostics.
The Gaussian quartic ratio is approximately 0.0995 gQ. It is a useful screening quantity but not a
rigorous harmonic bound. The uniform mode and energy baseline require explicit treatment, and
neither the interacting critical point nor a physical microscopic scale follows from this calculation.
The deliverable is a reproducible harmonic benchmark, not a complete interacting quantum theory
and not an experimental discovery. Further progress requires controlled interacting predictions,
physical matching, and a discriminating independent test.
Data and code availability
The accompanying reproducibility package contains verify_rotor_benchmarks.py, the directly
evaluated lattice sums, quadrature comparisons, numerical metadata, execution log, and two
generated figures. The calculations in this package were executed in preparing this revision. No
quantum Monte Carlo or experimental data analysis was performed. Run the script with an
output-directory argument; it requires Python, NumPy, SciPy, pandas, and Matplotlib. No
permanent repository identifier is asserted. The author should archive the exact release and add its
verified identifier before claiming an archival data publication.
Quantum Rotor Kernel — Harmonic Benchmarks and Validity Diagnostics 8
Acknowledgments
The author acknowledges the Tanfarid Vision Research Institute, Bogura, Bangladesh.
References
[1] S. Sachdev, Quantum Phase Transitions, 2nd ed. (Cambridge University Press, 2011).
[2] W. Jiang et al., “Solving quantum rotor model with different Monte Carlo techniques,”
arXiv:1912.08229.
[3] X. Leoncini, A. D. Verga, and S. Ruffo, “Hamiltonian dynamics and the phase transition of the XY
model,” Physical Review E 57, 6377 (1998).
[4] NIST Digital Library of Mathematical Functions, Section 3.1, “Arithmetics and Error Measures,”
numerical error and precision conventions.
