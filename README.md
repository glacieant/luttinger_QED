# luttinger_QED #

The LaTeX and Wolfram (Mathematica) calculations for the one-loop
renormalization group of non-relativistic electrodynamics in four
space-time dimensions. The key components of these calculations
were published in 2022 [1].

The LaTeX notes carry the calculations done analytically:

	notes/rg        Feynman rules and one-loop fermion and 
                    photon self-energy corrections from the
                    non-relativistic Luttinger QED action 
                    minimally coupled to U(1) gauge fields
	notes/zeeman_coupling	the non-relativistic Pauli-Zeeman 
                            term for any spatial dimension

A Wolfram Mathematica implementation automates the computation steps
using the FeynCalc package [2,3,4] for a subset of the Feynman
diagrams. The following three directories carry Wolfram notebooks that
produce their figures inside their respective "figs" subdirectory:

	aux	notebooks for the band structure, the Landau levels in
		the presence of a finite magnetic field, the spin-3/2
		algebra of the Zeeman coupling, and the time-reversal
		symmetry breaking fluctuation matrix
	rg	notebooks for the Wilsonian and the dimensionally
		regularized one-loop RG counter terms (the Zeeman
		coupling remains yet to be implemented)
	demos	notebooks for large-N diagrams, an alternate
		Pauli-Villars regulator, Feynman parameterization, and
		a comparison with related models [5]

Much of this project base carries material that is at best work in
progress. E.g., each directory carries a copy of the FeynCalc 9.3.1
package in library/ (distributed under the GNU General Public
License), because the notebooks were originally written with that
package and as such they still work most consistently with that
package loaded.

For more details and the associated physics discussions and context,
please refer to Ref. [1]. Further information about the very
capable FeynCalc package can be found in Refs. [2,3,4] and at
https://github.com/FeynCalc/feyncalc.

## References

[1] S. Dey and J. Maciejko, [Quantum-critical electrodynamics of Luttinger fermions](https://doi.org/10.1103/PhysRevB.106.035140), Phys. Rev. B 106, 035140 (2022).

[2] V. Shtabovenko, R. Mertig, and F. Orellana, [FeynCalc 9.3: New features and improvements](https://doi.org/10.1016/j.cpc.2020.107478), Comput. Phys. Commun. 256, 107478 (2020).

[3] V. Shtabovenko, R. Mertig, and F. Orellana, [New Developments in FeynCalc 9.0](https://doi.org/10.1016/j.cpc.2016.06.008), Comput. Phys. Commun. 207, 432 (2016).

[4] R. Mertig, M. Bohm, and A. Denner, [Feyn Calc - Computer-algebraic calculation of Feynman amplitudes](https://doi.org/10.1016/0010-4655%2891%2990130-D), Comput. Phys. Commun. 64, 345 (1991).

[5] E.-G. Moon, C. Xu, Y. B. Kim, and L. Balents, [Non-Fermi-Liquid and Topological States with Strong Spin-Orbit Coupling](https://doi.org/10.1103/PhysRevLett.111.206401), Phys. Rev. Lett. 111, 206401 (2013).
