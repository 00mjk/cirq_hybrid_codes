# cirq_hybrid_codes
*This is just a long list of ideas to investigate. Nothing here is really very original except maybe the gluing of local things into global things and the implications in terms of entanglement and its connections to number theory.*

- [Ringel Shanghai Lectures](https://www.math.uni-bielefeld.de/~sek/shanghai/text2011.html)

[Hybrid Qudit Surface Codes](https://github.com/The-Singularity-Research/qudit_surface_codes) in [Google Cirq](https://quantumai.google/cirq) are constructed in order to realize surface algebras as a truncated version of the Hilbert-Polya conjecture for low lying zeros of arbitrary Artin L-functions (see for example [Spectral Triples and Zeta-Cycles](https://arxiv.org/abs/2106.01715) for low lying zeros of zeta). However, the details for how this works when working over the 2-adics is unclear, so strictly speaking, we cannot presently say much about zeta. The setup is amenable to arbitrary Artin L-functions though, so this method should provide substantial progress at the very least. Also, the construction works over ramified and unramified primes, as mentioned in [AS1](https://arxiv.org/abs/1810.06750). More generally though, we can extend this by taking powers of d and using qudits with dimension a power of d (d being the number of edges at a vertex of a dessin, which technically speaking should relate to the covering theory). This is equivalent to modding out by some power of the shift operator mentioned in [AS1](https://arxiv.org/abs/1810.06750) where Artin's conjecture on holomorphicity of L-functions was addressed. This of course can be translated into the language of partition functions, and zeros can be used for useful computation of phase-transitions in condensed matter physics. This model may also serve as a useful avenue for constructing features for use in machine learning models for quantum error mitigation using invariant theory and group equivariant neural networks. A running update to the paper [Surface Algebras I: Dessins D'enfants, Surface Algebras, and Dessin Orders](https://arxiv.org/abs/1810.06750) will be kept here so as not to bombard arXiv. See also the other GitHub pages (where some hardware implementations are considered...maybe use QISKit Metal eventually):

- [qudit_surface_codes](https://github.com/The-Singularity-Research/qudit_surface_codes)
- [Surface Codes and Error Correction](https://github.com/The-Singularity-Research/SurfaceCodes)
- [Intro to Surface Codes](https://github.com/The-Singularity-Research/Surface-Codes)
- [Surface Codes Tutorial](https://github.com/The-Singularity-Research/QISKit-Surface-Codes/blob/master/Use%20Case%20Examples/surface_code_tutorial_2.ipynb)

Using [circulant matrices](https://arxiv.org/pdf/1506.05149.pdf#page10) we get the local finite Fourier transforms on the qudits. This implies a connection to *prolate spheroidal wave functions* investigated by Slepian and Pollak and mentioned in [Spectral Triples and Zeta-Cycles](https://arxiv.org/abs/2106.01715). Using equivariant neural networks will likely prove useful for error mitigation of these generalized hybrid qudit surface codes (see for example [Gauge Equivariant Mesh CNNs: Anisotropic Convolutions on Geometric Graphs](https://openreview.net/pdf?id=Jnspzp-oIZE), [Surface Networks via General Covers](https://arxiv.org/pdf/1812.10705.pdf), [CNNs on Surfaces using Rotation-Equivariant Features](https://arxiv.org/pdf/2006.01570.pdf), and [equivariant neural networks collection on Github](https://github.com/Chen-Cai-OSU/awesome-equivariant-network). The following paper is also important for the local picture [Qudit surface codes and gauge theory with finite cyclic groups
](https://arxiv.org/abs/quant-ph/0609070). A more general idea would be to look at permutation equivariance with respect to Galois groups of field extensions, viewing Galois groups as permutation groups (subgroups of symmetric groups for local vertices of a dessin). For example, say we have a field extension of the rationals given by the fifth roots of unity. Then we could look at permutation equivariance with respect to the Galois group of the field extension. Gluing many such field extensions together we could arive at a global group for a dessin. See for example [What is the square root of two? | The Fundamental Theorem of Galois Theory](https://www.youtube.com/watch?v=CwvuZ8aHyH4&t=879s), (see also [Group Representations without Groups](https://eudml.org/doc/139782). Any machine learning models such as transformers would naturally learn the permutation equivariance important for such problems. In general, to build the appropriate neural networks for arbitrary groups equivariance, one needs to construct anisotropic kernels. This can be seen to relate to the papers mentioned below on σ-hole interactions and anisotropic distribution of electrons. Using prolate spheroidal wavefunctions as a basis set may useful for this problem. Padding zeros in the gauge equivariant neural networks for such problems was assumed to be the first obvious way to modify these neural networks, however, upon further inspection *the pullback of the matrix rings provides the correct dimension for these neural networks*. Geometrically one can consider the (Zariski) closed subset inside the *direct sum* given by the equations on diagonal entries defining the gluing of matrix rings associated to vertices of a dessin. We may also need to consider p-adic neural networks if p-adic geometry is being modeled, which is important to p-adic string theory and the p-adic AdS/CFT correspondence. 

- [Toeplitz and Circulant Matrices: A review](https://ee.stanford.edu/~gray/toeplitz.pdf).
- [Prolate Spheroidal Wavefunctions, Fourier Analysis and Uncertainty I](https://mast.queensu.ca/~driegert/papers/pswf_1.pdf)
- [Prolate Spheroidal Wavefunctions, Fourier Analysis and Uncertainty II](https://mast.queensu.ca/~driegert/papers/pswf_2.pdf) (*along with III, IV, V, and VI*)
- [Real-space imaging of anisotropic charge of σ-hole by means of Kelvin probe force microscopy](https://www.science.org/doi/10.1126/science.abk1479)
- [Anisotropy_of_electron_distribution_and_its_dependence_on_basis_set_and_method_used](https://www.researchgate.net/publication/257665958_The_shape_of_the_halogen_atom_-_Anisotropy_of_electron_distribution_and_its_dependence_on_basis_set_and_method_used)
- [Sigma-Hole Interactions in Anion Recognition](https://reader.elsevier.com/reader/sd/pii/S2451929418300834?token=9FF38A41E9C9461EB74B91D483D3E41314781D8E1FE9DCE633D809A464881BD534C2DC4C79EECCAAD6D13E8297F2B41F&originRegion=us-east-1&originCreation=20211112055342)

Using group equivariant neural networks (can be constructed in such a way so that it gives us something like the renormalization group in physics?) and is likely a good model for human perception and generalizations of human perception to more complex intelligences. We note that the attention mechanism in transformer models such as GPT-3 is a permutation equivariant operation, and as such gives a way of approximating any finite group and therefore any compact group of symmetries in data. This could explain the generality in applicability of these models, but there are more efficient ways of capturing specific kinds of symmetries and equivariance of features/data to specific symmetry groups by constructions in "geometric deep learning" using things like anisotropic filters and convolutional layers (and nonlinear/ReLU layers) that respect the symmetries.

It is also possible that the spectral compatability constraints described in [Surface Algebras I: Dessins D'enfants, Surface Algebras, and Dessin Orders](https://arxiv.org/abs/1810.06750) given by gluing matrix rings gives a way of reducing the complexity of quantum computation (this is related to geometric phase and the center of the algebra commuting with everything implying it is not observable in the sense of observables in physics and operator algebras). This may also have implications for the way we understand entanglement and [relative and global phases in quantum systems](https://quantum-computing.ibm.com/composer/docs/iqx/guide/introducing-qubit-phase). Perhaps there are implications for quantization? Moreover, it seems possible that semi-invariants might be used as engineered features for improving error mitigation methods using deep learning. 

We also note that the p-adic geometry mentioned in [Surface Algebras I: Dessins D'enfants, Surface Algebras, and Dessin Orders](https://arxiv.org/abs/1810.06750) can be modeled as well such as in [From p-adic AdS/CFT to prospects in cold atoms](https://www.youtube.com/watch?v=yh4cTozj3z4&t=1485s) and [p-adic AdS/CFT Correspondence](https://ncatlab.org/nlab/show/p-adic+AdS%2FCFT+correspondence). The patterns in information processing in p-adic geometry may be much different from those found in the complex setting. Algorithms using the p-adic geometry should be studied further to understand what applications might arise. The most obvious are phase transitions in quantum systems and quantum chaos. 

We also link to the (very sketchy) paper [Surface Algebras and Surface Orders II: Affine Bundles on Curves](https://arxiv.org/abs/1812.00621) as a way of undertsanding the problem geometrically. 

## Questions and Ideas

- Should we try to interpret the 3-adic quiver universal covering (a Cantor set givent by 4-regular tree as underlying graph) of all surface algebras in terms of 2-adics using the relations of a gentle algebra? Would this give a new way of thinking about zeta? This is where the relation to [Spectral Triples and Zeta-Cycles](https://arxiv.org/abs/2106.01715) for low lying zeros of zeta) becomes unclear. There may be some covering theory involved, perhaps some quotients. I am unsure at this point and this is a problem that will almost certainly (with a probability of *at least* 1-10^{-51}) need to stay distributed due to its complexity. 

- Think of things in terms of density operators and states as being linear functionals (as apposed to states in a Hilbert space). This would give a (noncommutative) spatial interpretation of the fiber product, and a relative tensor product intepretation of the noncommutative algebra of functions on that space. Also, **relative tensor product** related to **fiber product** for surface algebras at the level of quivers (Check the Herschend papers referenced in AS1 like [Herschend1](https://arxiv.org/pdf/0902.2050.pdf) and [Herschend 4](https://reader.elsevier.com/reader/sd/pii/S0022404907001508?token=FCD1A091C7FDB01F328CC40A2FB71C3D371FB3157A4D8DB7A47F2B7583D688A6CC2E30397D300FEA4A6768FDA16F22EA&originRegion=us-east-1&originCreation=20210930022536) phrased in terms of representations/modules so use direct sum of indecomposable projective modules expression of the quiver path algebra, which gives us a bimodule structure and is likely related to Bobinski and [Zwara's](https://eudml.org/search/page?q=sc.general*op.AND*l_0*c_0author_0eq%253A1.Grzegorz+Zwara&qt=SEARCH) "Hom-controlled functors" which give geometric results on module varieties of different algebras which are related via a "Hom-controlled functor"; see for example [Schubert varieties and representations of Dynkin quivers](https://eudml.org/doc/284883)). Also see [Pullback and Pushout Constructions in
C*-Algebra Theory1](https://www.math.ru.nl/~mueger/ped2.pdf).
- Use operator-state correspondence/density matrices and adjoint representation...use geometric phases (roots of unity) to generate more basis vectors...something something Okounkov's infinite wedge and diagonal operators. Hurwitz theory counting coverings of topological structures of operators (think bundles of operators on Riemann surface)...but what is the significance of counting coverings? Some kind of complexity theoretic interpretation in error mitigation of quantum systems?
- Even though local factors could all be finite dimensional (restriction imposed by gravity) if we look at noncompact Riemann surfaces with some n-ary tree (think hyperbolic upper half plane or Poincare disk and the AdS/CFT correspondence) then we get an uncountable number of factors which implies uncountable global dimension and the necessity of type III von Neumann algebra factors. Think Cantor filtration of modules over surface algebras. What does the module theory look like in this case? What do projective resolutions look like? Do we get interesting things that converge? What about module varieties? Invariant Theory?
- Also, if we take tensor products over rings (rather than just the complex numbers), what information do we get from the dimension viewed with respect to various fields or rings? 
- Seems like the central extension given by the center of the surface algebra is very important. See for example Section 9 of [AS1](https://github.com/The-Singularity-Research/cirq_hybrid_codes/blob/master/Surface_Algebras_I%20(3).pdf) and the infinite wedge section of [Bloch-Okounkov](https://arxiv.org/pdf/alg-geom/9712009.pdf) describing the central extension, but instead of taking the quotient by $\mathbb{C} \cdot Id$ take the quotient by $Z(\Lambda)$ the center of the completed surface algebra.
- Center commutes with everything so is independent of any observable and therefore not observable? Also center is spectral and related to geometric phase of quantum system? If center is not observable then should be able to reduce complexity of computation using gluing?
- This gluing gives a description of discrete spacetime and an "explanation" of entanglement. 

### Use k-local Hamiltonian and growing [db-scan](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.DBSCAN.html) to understand Jung's collective mind and certain types of distributed computation. 😻 Beautiful, but how quantum? Ich liebe euch.

*Related question: what wavelengths of microwaves interact with complex molecules, protiens, and larger organic structures? Could we understand Penrose's idea of encoding information in the cosmic microwave background in this way?*

### Note there is a decomposition of (global) Hamiltonians 

![image](https://github.com/The-Singularity-Research/cirq_hybrid_codes/blob/master/Screen%20Shot%202021-09-29%20at%209.34.22%20PM.png)

see comment on [Sean Carroll's video](https://youtu.be/3yofwdhQlhI). If we look at this from the perspective of patching things together locally rather than dividing things into subsystems globally, this may give some insight into how the global separation of von Neumann algebras should be separated into factors (of type I, II, and III). Also, we need to tensor over fields/rings other than complex numbers (relative tensor product) like p-adics for example, 

![image](https://github.com/The-Singularity-Research/cirq_hybrid_codes/blob/master/Screen%20Shot%202021-09-29%20at%209.39.21%20PM.png)

and rings of integers or other rings R and S, (maybe p-adic integers/rationals and q-adic integers/rationals for two matrix algebras and tensor over lcm(p,q)-adics? Relatively prime p and q give interesting things?) 

![image](https://github.com/The-Singularity-Research/cirq_hybrid_codes/blob/master/Screen%20Shot%202021-09-29%20at%209.39.33%20PM.png)

How does this relate to Connes Fusion? Is this the same thing? Maybe import language/theory from vertex operator algebras?
- Take surface algebra and it’s (Koszul) dual surface algebra together to get 4-D physics? How do they come together? Tensor? Gluing? Super Riemann surfaces? Should relate to mirror symmetry? 
- Differential on the dga structure of surface algebra recovers the topology of Riemann surface. Noncommutative connection defines curvature. Flat is important class of connections for surface algebras. 
- [Sean Carroll's video](https://youtu.be/3yofwdhQlhI) says at 1:01:25 "There is no representation of noncompact group on finite dimensional Hilbert space." What is he trying to say, because the way this is worded it simply isn't true. Does he need a specific kind of representation? Unitary or Faithful or some such? This is in regards to (approximate) Lorentz invariance/Diffeomorphism invariance/gauge invariance (what about equivariance?)
- Look at the Fourier transform from l^2(Z) to L^2(T) (and Zwara’s smooth morphisms of module schemes and Hom-controlled functors). This idea can be transferred to surface algebras/orders where we do F^{-1}M_fF: A \to A like at 44:30 in [Vaughn Jones' lecture](https://www.youtube.com/watch?v=AOucTCWylzk&t=3174s) to get convolution. See also Section 8 of [SA2](https://arxiv.org/pdf/1812.00621.pdf).
- Say more about unitary operators taking us from an algebra of operators to multiplication, use Fourier transform for example to go to irrational rotation algebra. Talk about realization of measure space $(X, \mu)$ as spectrum of operator. Maybe look at Lurie's categorification of Fourier transform?
- If Morita equivalence is the appropriate notion of "isomorphism" in noncommutative geometry (as apposed to say, isomorphisms of algebras) then derived equivalent categories should be important. There is a lot of work on this in the case of gentle algebras. The modules realized as paths idea works in the derived categories as well for indecomposable objest. For gentle algebras, this is all very algorithm/computer friendly. What important insights or applications can we gain from this?

- Use the universal localization via projectives of [Aiden Schofield](https://arxiv.org/abs/0708.0246) and [Amnon Neeman, Andrew Ranicki, Aidan Schofield](https://arxiv.org/abs/math/0205034) to get the Leavitt path algebra. This is closely related to the theory of semi-invariants described by maps between projective modules over the surface algebra. Next we should take the analytic completion of the Leavitt path algebras to obtain graph C*-algebras. Some results on pullbacks such as [Leavitt vs. C*-pullbacks](https://arxiv.org/abs/1909.09624) or [A graded pullback structure of Leavitt path algebras of trimmable graphs](https://arxiv.org/abs/1803.10209) may be useful (as it may be easier to study certain aspects of the theory prior to taking pullbacks). Next we should use [The Noncommutative Geometry of Graph C*-Algebras I: The Index Theorem](https://arxiv.org/abs/math/0508025) and other work of [A. Rennie](https://arxiv.org/search/math?searchtype=author&query=Rennie%2C+A) to obtain the theory of spectral triples associated to graph C*-algebras (if they exist) and noncommutative geometry. 

- Understanding how this relates to various kinds of factors of von Neumann algebras is also very important, but I can't say much about this yet. 

- Triangulations and their trivalent (Koszul/equivalently geometric) duals obviously give us (gentle) quivers with (super)potential and links to cluster algebras (see [DWZ1](https://arxiv.org/abs/0704.0649) and [DWZ2](https://arxiv.org/abs/0904.0676), also [IOTW](https://arxiv.org/abs/0708.0798)).

- Develop the appropriate gauge theory (similar to [Qudit surface codes and gauge theory with finite cyclic groups](https://arxiv.org/abs/quant-ph/0609070))

- Develop the theory of non-commutative fundamental groups (see [The fundamental group of a noncommutative space](https://arxiv.org/abs/1910.10127))

- [Geometrization of the local Langlands correspondence](https://arxiv.org/abs/2102.13459) just wow...gotta glue this together in my mind. 

- Represent states as operators in a C*-algebra then allow a (topological structure) of operators inside this C*-algebra to act on these and generate some new structure of operators (could be the whole algebra but more interesting would be some bundle of operators over the Riemann sphere or other Riemann surfaces). Also allow coverings of topological structures of operators to act on the initial topological structure of operators. Think coverings of Riemann surfaces with bundles of operators. The tower of operators goes in both directions. We can think of this as coverings of noncommutative spaces and noncommutative spaces generated by actions of (topological structures of) C*-algebras. Should think of paths on the surface as modules/representations (or indecomposables in the derived category), lifting to sections. Maybe think of a slice of time as a collection of random matrices at each vertex (glued together in "spatial" surface algebra) and each slice of time perturbs the random matrix into something nearby. This would be something like a propogating string which *cut*es ✌️😍 out a pair of pants from a cobordism theory. 
- Via a universal noncommutative localization of a surface (path) algebra, one obtains a Leavitt path algebra. Via the analytic completion of the Leavitt path algebra, one obtains a graph C*-algebra. Thus, there is a Leavitt path algebra, and graph C*-algebra given by localization and completion of a surface algebra. This closely mirrors the procedure of localization and completion of number fields


## Useful papers/ideas not referenced or linked on ArXiv

This paper is also very useful [The (cyclic) enhanced nilpotent cone via quiver
representations](https://d-nb.info/1180631099/34) and is not linked via connected papers on arXiv. 

Work of [Fomin and Zelevinsky](https://arxiv.org/abs/math/9912128) is a good place to begin understanding total positivity in physics and how that relateds to Schubert varieties. This is directly relates to work of [Nima Arkani-Hamed](https://arxiv.org/abs/1703.04541) for example, and likely is implied by von Neumann algebras that with positive spectra in the reals (don't really understand types of factors I/II/III enough to say much yet). Should be some relation of total positivity to Okounkov's infinite wedge construction as well, still working on understanding the details of this. Wedge powers of density operators gives minors of density matrices though, so this is likely pretty straightforward to see how total positivity (of minors of matrices) enters the picture. For example, nth wedge power of a matrix gives the n-by-n minors of that matrix as the entries of the new matrix. This is important in constructions mentioned in Andy Carroll's article [Semi-Invariants for Gentle String Algebras](https://arxiv.org/abs/1106.0774) where minors are used to compute the decomposition of the coordinate ring of the varieties of complexes (which is related to partitions and likely gives the connection to Okounkov's paper [Infinite wedge and random partitions](https://arxiv.org/abs/math/9907127)). Other references to this technique over arbitrary rings (as apposed to algebraically closed fields) include [Universal Complexes and the
Generic Structure of Free Resolutions](https://projecteuclid.org/JournalArticle/PreviewFirstPage?urlid=10.1307%2Fmmj%2F1008719036) and [On the variety of complexes](https://www.sciencedirect.com/science/article/pii/S0001870881800047). This approach is somewhat different from that of Magyar's paper [Affine Schubert Varieties and Circular Complexes](https://arxiv.org/abs/math/0210151) which gives the obvious connection to loop groups and the geometric Langland's program. However, the variety of complexes approach gives the connection to cluster algebras via quivers with potential when the quiver comes from a triangulated surface as apposed to an arbitrary dessin d'enfant. The potential in this case gives the gentle relations on the surface algebra. There are of course other related approaches such as those by Musili and Seshadri, but I am less familiar with these at the moment. 

It may be prudent to look into the work of Pierre-Guy Plamondon, Bernhard Keller, and Claire Amiot on cluster categories and gentle algebras. I have not looked at this in quite some time, so the connection and interpretation in terms of physics is not something I could make off the top of my head. However, the work is beautiful and likely would provide many interesting new ideas considering the geometric interpretation of indecomposable objects in the derived category of gentle algebras as paths on Riemann surfaces (similar to that of the indecomposable modules over gentle algebras). 
- [The category of finite strings](https://arxiv.org/abs/2109.05745)
- [On the Derived Categories of Gentle and Skew Gentle Algebras](https://arxiv.org/pdf/1706.08358.pdf)
- [Derived Categories of Nodal Algebras](https://arxiv.org/abs/math/0307060)
- [Indecomposables in the derived category of certain associative algebras](https://arxiv.org/abs/math/0307062)
- [Non-commutative nodal curves and derived tame algebras](https://arxiv.org/pdf/1805.05174.pdf)
- [Labardini-Frigosa's work](https://arxiv.org/search/math?searchtype=author&query=Labardini-Fragoso%2C+D)
- [Ralf Schiffler's work](https://arxiv.org/search/math?searchtype=author&query=Schiffler%2C+R)
- [Ilke's stuff](https://arxiv.org/search/math?searchtype=author&query=Canakci%2C+I) is just cool. So is she. 
- Some of [Sibylle's work](https://arxiv.org/search/math?searchtype=author&query=Schroll%2C+S) gives a good way of understanding inverse Galois theory and could be transferred to the quantum computing and quantum information language. 

### Latticy Type Things Maybe Useful for Understanding Entanglement and its Connection to Number Theory...good for 🔒

- [Tame matrix problems in Lie theory and commutative algebra](https://github.com/The-Singularity-Research/cirq_hybrid_codes/blob/master/PhD_Thesis_(Gnedin).pdf) (*has a extensive knowledge of lattices over orders, and is where I learned much of it from...an invaluable and powerful mind*).
- [Methods of Representation Theory: with Applications to Finite Groups and Orders vol. 1](https://github.com/The-Singularity-Research/cirq_hybrid_codes/blob/master/methods-of-representation-theory-I.pdf)
- [Methods of Representation Theory: with Applications to Finite Groups and Orders vol. 2](https://github.com/The-Singularity-Research/cirq_hybrid_codes/blob/master/methods-of-representation-theory-II.pdf)
- [Representation Theory of Finite Groups and Associative Algebras](https://github.com/The-Singularity-Research/cirq_hybrid_codes/blob/master/representation-theory-of-finite-groups-and-associative-algebras.pdf)

* Happy to help with 🔒 if needed *

### Infinite Dimensional Error Corresction/Mitigation in Quantum Computing

In [Quantum error correction on infinite-dimensional Hilbert spaces](https://arxiv.org/abs/0811.0421) infinite dimensional error correction is studied (as apposed to finite dimensional qudits). The following papers may be useful in furthering this study. We need both finite and infinite dimensional representations of graph C*-algebras for this. The relationship to the type I, II, and III factors of von Neumann algebras will also need to be understood. We also note that the completions of the local orders at vertices of a dessin can be understood through this lense and this provides the appropriate intepretation in terms of surface algebras and surface orders in SA1 and SA2 and the number theoretic interpretations derived therein. 

- [Indecomposable representations of quivers on infinite-dimensional Hilbert spaces](https://arxiv.org/abs/0707.0966)
- [Locally-scalar representations of graphs in the category of Hilbert spaces](https://arxiv.org/abs/math/0307163)
- [Matrix Problems in Hilbert Spaces](https://arxiv.org/abs/math/0605728)
- [On Regular Locally Scalar Representations of Graph D˜4 in Hilbert Spaces](https://arxiv.org/abs/math/0610931)
- [On the indecomposability in the category of representations of a quiver and in its subcategory of orthoscalar representations](https://arxiv.org/abs/math/0611385)
- [Orthoscalar representations of quivers on the category of Hilberts spaces. II](https://arxiv.org/abs/0901.2296)
- [The minimal representation-infinite algebras which are special biserial](https://arxiv.org/abs/1102.4064)
- [Infinite dimensional representations of canonical algebras](https://arxiv.org/abs/math/0206195)
- [Σ -pure-injective modules for string algebras and linear relations](https://arxiv.org/abs/1705.10145)
- [C*-algebra of the Z^n-tree](http://nyjm.albany.edu/j/2011/17-1p.pdf) could provide connections to lattices over orders and cryptographic phrasing of problems.

### Connection to Hurwitz Theory

There is a project I am aware of connected to Hurwitz theory which should be useful. This may be a place where I could provide some ideas once I've understood Hurwitz theory enough to comment on this paper. Until I have a better grasp of Hurwitz theory though, I do not believe it is my place to say much in this regard. In case it is helpful for *someone else*, you may also want to look at Okounkov's paper on random partitions and the infinite wedge to see if there are connections to the work of Andy Carroll and Calin Chindris on semi-invariants for gentle algebras and the universal complexes of Tchernev mentioned earlier on this page (see also DeConcini and Strickland's description of the variety of complexes and consider *circular complexes*). I truly hope this helps more than I am able to at the moment. Perhaps one day we can learn something from each other. Please be aware, it was told to me that there is a mistake in the DeConcini and Strickland paper involving the simplicial complexes mentioned in their argument (I believe I was told they aren't "spherical" IIRC). However, the Tchernev paper remedies this with a more general approach using Gröbner bases. It should also be checked if there is some connection to Fomin and Zelevinsky's notion of *total positivity*. This would require foregoing the use of any virtual semi-invariants in the context of physical interpretations.

#### Update on Hurwitz Theory...

I've been reading a bit on the Hurwitz theory connection, and it seems like the Maya diagrams for partitions in the infinite wedge construction likely have some connection to modules over the quiver path algebra of a surface algebra. If we think of coverings of surface algebras bu other surface algebras this would correspond to Hurwitz theory. Also, we should think of the matrix algebra at a vertex as corresponding to some local quantum system. I've been thinking of it as a qudit for d = the number of half edges around a vertex, but with d raised to an infinite power to account for the infinite dimension over the complex numbers (assuming we're working in that context and not over p-adics or some other rings as coefficients). This to me seems like an infinite block diagonal subalgebra (blocks of size d) of gl(\infty) at the vertex (and we have a bunch of these glued together to get the surface algebra). Next, we think of walking around the vertex in one direction as generating part of a string module for the quiver path algebra. You can start walking in the opposite direction around a neighboring vertex to continue the string (may also want band modules, not sure yet). Anyway, these give some zig-zag patterns in the Z^2 lattice first described by Gel'fand and Ponomarev and then by Gabriel. These are standard in the quiver literature at this point and all string modules look like this. This might explain or give a new interpetation of the expectation values that give us formulas for Hurwitz numbers. There is a good covering theory developed [Group actions and coverings of Brauer graph algebras](https://arxiv.org/abs/1112.2199) which should work for the surface algebras (see also the Herschend papers cited in [AS1](https://github.com/The-Singularity-Research/cirq_hybrid_codes/blob/master/Surface_Algebras_I%20(3).pdf)). This should also give connections to wall crossing via semi-invariants of quivers. If there is a covering theory of surface algebras in terms of the (gentle) quiver path algebras there should also be a corresponding covering theory of the matrix algebras that are being glued together living over the vertices of the dessin. Perhaps restriction and lifting of representations would also provide some interesting results in this case. In particular, as topological groups, should this not correspond to group coverings for loop groups/loop algebras? Any references? Can't seem to find any. 

Also, is it possible that the factors coming from commutation relations of the operators in the formulas for Hurwitz numbers are related to, or coming from Buchsbaum-Eisenbud multipliers? For example, if we move around the face of a cellularly embedded graph in a Riemann surface (dessin) we are traveling around a cycle of zero relations in the gentle surface algebra. Such cycles are "circular complexes" (of vector spaces or modules) if we fix a representation of the surface algebra with a prescribed dimension vector. Such circular complexes (as described in Magyar's work for example) would naturally give rise to Buchsbaum-Eisenbud multipliers. Such a path on the surface could be interpreted as traveling around the preimage of infinity in a covering of the Riemann sphere. In the path integral defining partition functions in conformal field theories, this might give an interpretation of Hurwitz generating functions and the commutation relations giving rise to determinantal coefficients after commuting operators could possibly be interpreted as Buchsbaum-Eisenbud multipliers (which arise as determinants of minors of matrices). The matrices in question would somehow also be related to the block diagonal Lie subalgebras of the gl(\infty) Lie algebras located over vertices (see Okounkov's random partitions and the infinite wedge construction and wedge powers of operators).  In this formulation, we have a characteristic free way of treating representations of the gentle surface algebra over arbitrary commutative rings via Tchernev's methods with Gröbner bases for varieties of complexes. See also the work of Hochster. This should be very useful for p-adic physics and p-adic string theory and AdS/CFT in particular since it all holds over the integers. 

### Varieties of Complexes and Equivariant Neural Networks

The *Buchsbaum-Eisenbud* varieties of complexes, related to the work of Hochster and Huneke are an approach that can be used for studying surface algebras over arbitrary commutative rings. This will hopefully be useful in constructing [equivariant neural networks](https://colab.research.google.com/github/whitead/dmol-book/blob/master/dl/Equivariant.ipynb) for quantum error mitigation over arbitrary (commutative) coefficient rings. It is a characteristic free approach, and all results hold in full generality over the integers. This may help in developing equivariant [p-adic neural networks](https://github.com/The-Singularity-Research/cirq_hybrid_codes/blob/master/%5BMathematics%20and%20Its%20Applications%20574%5D%20Andrei%20Yu.%20Khrennikov%2C%20Marcus%20Nilson%20-%20P-adic%20Deterministic%20and%20Random%20Dynamics%20(2004%2C%20Springer)%20-%20libgen.lc.pdf) for this project (see also [p-adic Cellular Neural Networks](https://arxiv.org/abs/2107.07980) and [Learning of p-adic neural networks](https://empslocal.ex.ac.uk/people/staff/mrwatkin/zeta/khrennikov-learning.pdf). How nonlinearities/activation functions beyond ReLU in such networks are chosen is unclear to me. Phrasing in terms of cryptography could be useful for understanding. Some references for this topic are:

- [Generic free resolutions and root systems](https://arxiv.org/abs/1609.02083)
- [On the Structure of Free Resolutions of Length 3 ](https://core.ac.uk/download/pdf/82379427.pdf) (IIRC there are some mistakes similar to the mistakes mentioned in the DeConcini and Strickland paper, should be revised and checked)
- [On the minimal free resolution of the universal ring for resolutions of length two](https://arxiv.org/abs/math/0508439)
- [Two results on equations of nilpotent orbits](https://arxiv.org/abs/math/0006232)
- [The Existence of Pure Free Resolutions](https://arxiv.org/abs/0709.1529) (*more related to the Schubert variety perspective*)
- [topics-in-the-homological-theory-of-modules-over-commutative-rings](https://github.com/The-Singularity-Research/cirq_hybrid_codes/blob/master/topics-in-the-homological-theory-of-modules-over-commutative-rings.pdf)
- Buchsbaum, D., Eisenbud, D., What makes a complex exact, J. of Algebra. 25 (1973), 259-268.
- Buchsbaum, D., Eisenbud, D., Some structure theorems for finite free resolutions, Advances in Math. 1 (1974), 84-139.

#### useful for equivariant layers of neural networks
- [Cohomology of Vector Bundles and Syzygies](https://github.com/The-Singularity-Research/cirq_hybrid_codes) (*especially chapter 3 for varieties of complexes,  and 5.4 for equivariant neural network layers*)
- [Semigentle](https://github.com/The-Singularity-Research/cirq_hybrid_codes/blob/master/semigentle.pdf) (*A helpful paper hidden in emails in the depths of an ivory tower*)
- [Local cohomology with support in generic determinantal ideals](https://arxiv.org/abs/1309.0617) 
- [Surface Algebras Book](https://github.com/The-Singularity-Research/cirq_hybrid_codes/blob/master/Surface%20Algebras%20Book.pdf) has some examples and explanations that follow [Cohomology of Vector Bundles and Syzygies](https://github.com/The-Singularity-Research/cirq_hybrid_codes) and straightening algorithms of standard monomials in Chapter 13 of [Lie Groups](https://github.com/The-Singularity-Research/cirq_hybrid_codes/blob/master/Lie-groups.pdf) by Procesi. Also has some constructions involving Auslander-Reiten quivers that are implied by [On the Auslander-Reiten quiver of the representations of an infinite quiver](https://arxiv.org/abs/1201.4833) and [Representation Theory of an Infinite Quiver](https://arxiv.org/abs/1109.3176). This may also be of use later on [A non-existence theorem for almost split sequences](https://arxiv.org/abs/1104.1195).

*Note: this seems to imply that constructing features from semi-invariants may improve the performance of neural networks for error mitigation in quantum computing.*

### More things to investigate

- [Spectral description of non-commutative local systems on surfaces and non-commutative cluster varieties](https://arxiv.org/abs/2108.04168) (saturation of LR-coefficients and triple flag quivers could be useful for understanding this paper, as well as the work of Knutson and Tao on the Honeycomb model of GL(n) and Knutson's paper on Hermitian matrices). 
- [Wick rotation and the positivity of energy in quantum field theory](https://arxiv.org/abs/2105.10161)
- [Multiplication kernels](https://arxiv.org/abs/2105.04238)
- Check out [AQFT](https://ncatlab.org/nlab/show/AQFT) and Haag-Kastler axioms. T.Y. nWab_UwU and fellow catgirls 🐱 ❤️ 
