# cirq_hybrid_codes
Hybrid Qudit Surface Codes in [Google Cirq](https://quantumai.google/cirq) are constructed in order to realize surface algebras as a truncated version of the Hilbert-Polya conjecture for low lying zeros of arbitrary Artin L-functions (see for example [Spectral Triples and Zeta-Cycles](https://arxiv.org/abs/2106.01715) for low lying zeros of zeta). We can extend this by taking powers of d and using qudits with dimension a power of d. This is equivalent to modding out by some power of the shift operator mentioned in [Surface Algebras I: Dessins D'enfants, Surface Algebras, and Dessin Orders](https://arxiv.org/abs/1810.06750) where Artin's conjecture was addressed. This of course can be translated into the language of partition functions, and zeros can be used for useful computation of phase-transitions in condensed matter physics. This model may also serve as a useful avenue for constructing features for use in machine learning models for quantum error correction using invariant theory and group equivariant neural networks. A running update to the paper [Surface Algebras I: Dessins D'enfants, Surface Algebras, and Dessin Orders](https://arxiv.org/abs/1810.06750) will be kept here so as not to bombard arXiv. 

Using [circulant matrices](https://arxiv.org/pdf/1506.05149.pdf#page10) we get the local finite Fourier transforms on the qudits. This implies a connection to *prolate spheroidal wave functions* investigated by Slepian and Polloch and mentioned in [Spectral Triples and Zeta-Cycles](https://arxiv.org/abs/2106.01715). Using equivariant neural networks will likely prove useful for error correction and control of these generalized hybrid qudit surface codes (see for example [Gauge Equivariant Mesh CNNs: Anisotropic Convolutions on Geometric Graphs](https://openreview.net/pdf?id=Jnspzp-oIZE), [Surface Networks via General Covers](https://arxiv.org/pdf/1812.10705.pdf), [CNNs on Surfaces using Rotation-Equivariant Features](https://arxiv.org/pdf/2006.01570.pdf), and [equivariant neural networks collection on Github](https://github.com/Chen-Cai-OSU/awesome-equivariant-network). Padding zeros was assumed to be the first obvious way to modify these neural networks, however, upon further inspection *the pullback of the matrix rings provides the correct dimension for these neural networks*. Geometrically one can consider the (Zariski) closed subset inside the direct sum given by the equations on diagonal entries defining the gluing of matrix the rings. We may also need to consider p-adic neural networks if p-adic geometry is being modeled, which is important to p-adic string theory and the p-adic AdS/CFT correspondence. 

Using group equivariant neural networks gives us something like the renormalization group in physics and is likely a good model for human perception and generalizations of human perception to more complex intelligences. We note that the attention mechanism in transformer models such as GPT-3 is a permutation equivariant operation, and as such gives a way of approximating any finite group and therefore any compact group of symmetries in data. 

It is also possible that the spectral compatability constraints described in [Surface Algebras I: Dessins D'enfants, Surface Algebras, and Dessin Orders](https://arxiv.org/abs/1810.06750) given by gluing matrix rings gives a way of reducing the complexity of quantum computation (this is related to geometric phase and the center of the algebra commuting with everything implying it is not observable in the sense of observables in physics and operator algebras). This may also have implications for the way we understand entanglement and [relative and global phases in quantum systems](https://quantum-computing.ibm.com/composer/docs/iqx/guide/introducing-qubit-phase). Perhaps there are implications for quantization? Moreover, it seems possible that semi-invariants might be used as engineered features for improving error correction methods using deep learning. 

We also note that the p-adic geometry mentioned in [Surface Algebras I: Dessins D'enfants, Surface Algebras, and Dessin Orders](https://arxiv.org/abs/1810.06750) can be modeled as well such as in [From p-adic AdS/CFT to prospects in cold atoms](https://www.youtube.com/watch?v=yh4cTozj3z4&t=1485s) and [p-adic AdS/CFT Correspondence](https://ncatlab.org/nlab/show/p-adic+AdS%2FCFT+correspondence). The patterns in information processing in p-adic geometry may be much different from those found in the complex setting. Algorithms using the p-adic geometry should be studied further to understand what applications might arise. The most obvious are phase transitions in quantum systems, cryptography, and control of quantum systems and quantum chaos. 

We also link to the (very sketchy) paper [Surface Algebras and Surface Orders II: Affine Bundles on Curves](https://arxiv.org/abs/1812.00621) as a way of undertsanding the problem geometrically. 

## Questions and Ideas

- Should we forgo the Hilbert space and represent states as operators? This would give a (noncommutative) spatial interpretation of the fiber product, and a relative tensor product intepretation of the noncommutative algebra of functions on that space would be the operators acting on the Hilbert space we converted into operators (so operator algebra acts on itself). Also, **relative tensor product** *same as* fiber product for surface algebras at the level of quivers IIRC (Check the Herschend papers referenced in SAI like [Herschend 4](https://reader.elsevier.com/reader/sd/pii/S0022404907001508?token=FCD1A091C7FDB01F328CC40A2FB71C3D371FB3157A4D8DB7A47F2B7583D688A6CC2E30397D300FEA4A6768FDA16F22EA&originRegion=us-east-1&originCreation=20210930022536) phrased in terms of representations so use direct sum of indecomposable projectives expression of the algebra, which gives us a bimodule structure and is likely related to Bobinski and [Zwara's](https://eudml.org/search/page?q=sc.general*op.AND*l_0*c_0author_0eq%253A1.Grzegorz+Zwara&qt=SEARCH) "Hom-controlled functors" which give geometric results on module varieties of different algebras which are related via a "Hom-controlled functor"; see for example [Schubert varieties and representations of Dynkin quivers](https://eudml.org/doc/284883)). 
- Even though local factors are finite dimensional (restriction imposed by gravity) if we look at noncompact Riemann surfaces with some n-ary tree (think hyperbolic upper half plane or Poincare disk and the AdS/CFT correspondence) then we get an uncountable number of factors which implies uncountable global dimension and the necessity of type III von Neumann algebra factors. Think Cantor filtration of modules over surface algebras. What does the module theory look like in this case? What do projective resolutions look like? Do we get interesting things that converge? What about module varieties? Invariant Theory?
- Center commutes with everything so is independent of any observable and therefore not observable? Also center is spectral and related to geometric phase of system? If center is not observable then should be able to reduce complexity of computation using gluing?
- Truncate series for local interactions like a growing db-scan/persistent homology construction where the ball is expanding (at the speed of light?) How does entanglement propagate? Green’s function gives propagation of influence? Think about Wolfram's explanation of propagating hypermaps (which are essentially just dessins d'enfants); Also maybe Matilde Marcolli's graph grammers and insertion of graphs. What "langauge" is encoded in things like the cosmic microwave background? Related question: what wavelengths of microwaves interact with complex molecules, protiens, and larger organic structures? Could we understand Penrose's idea of encoding information in the cosmic microwave background in this way? 
- Also note there is a decomposition of (global) Hamiltonians 

![image](https://github.com/The-Singularity-Research/cirq_hybrid_codes/blob/master/Screen%20Shot%202021-09-29%20at%209.34.22%20PM.png)

see comment on [Sean Carroll's video](https://youtu.be/3yofwdhQlhI). If we look at this from the perspective of patching things together locally rather than dividing things into subsystems globally, this may give some insight into how the global separation of von Neumann algebras should be separated into factors (of type I, II, and III). Also, we need to tensor over fields/rings other than complex numbers (relative tensor product) like p-adics for example, 

![image](https://github.com/The-Singularity-Research/cirq_hybrid_codes/blob/master/Screen%20Shot%202021-09-29%20at%209.39.21%20PM.png)

and rings of integers or other rings R and S, 

![image](https://github.com/The-Singularity-Research/cirq_hybrid_codes/blob/master/Screen%20Shot%202021-09-29%20at%209.39.33%20PM.png)

How does this relate to Connes Fusion? Is this the same thing?
- Take surface algebra and it’s (Koszul) dual surface algebra together to get 4-D physics? How do they come together? Tensor? Gluing? Super Riemann surfaces? Should relate to mirror symmetry. 
- Differential on the dga structure of surface algebra recovers to topology of Riemann surface. Noncommutative connection defines curvature. Flat is important class of connections for surface algebras. 
- Sean Carroll says "No representation of noncompact group on finite dim Hilbert space."What is he trying to say, because the way this is worded it simply isn't true. Does he need a specific kind of representation? Faithful or some such? Approximate Lorentz invariance/Diffeomorphism invariance/gauge invariance (what about equivariance?) 
- Look at the Fourier transform from l^2(Z) to L^2(T) (and Zwara’s smooth morphisms of module schemes and Hom-controlled functors). This idea can be transferred to surface algebras/orders where we do F^{-1}M_fF: A \to A like at 44:30 in [Vaughn Jones' lecture](https://www.youtube.com/watch?v=AOucTCWylzk&t=3174s) to get convolution. See also Section 8 of [SA2](https://arxiv.org/pdf/1812.00621.pdf).
- Say more about nnitary taking us from an algebra of operators to multiplication, use Fourier transform for example to go to irrational rotation algebra. Talk about realization of measure space $(X, \mu)$ as spectrum of operator. 




 



## Useful papers not referenced or linked on ArXiv

This paper is also very useful [The (cyclic) enhanced nilpotent cone via quiver
representations](https://d-nb.info/1180631099/34) and is not linked via connected papers on arXiv. 





