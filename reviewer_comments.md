Context and Athenaeum
======================

**The following is a list of comments given by reviewers on a previously unedited version of the paper submitted to a mathematics journal. Most have been addressed in the current version, but for transparencey and accuracy, we leave the comments below in case there is interest or need in a similar fashion to [Open Review](https://openreview.net/). I suggest arxiv adopt a function such as this, and the two be put onto a decentralized platform that can track and incentivize authoring and editing research papers using something like [Fermat's Library](https://fermatslibrary.com/) and a tokenomics/incentive structure similar to [The Graph](https://thegraph.com/), which could also be incorporated into the platform. Perhaps something like Overleaf can also be incorporated as well to improve collaboration in the authoring process. For papers with code, GitHub integration would also be useful. If we have everything in one place on a single platform, it would provide a decentralized and democratic dual to traditional academia, providing us with academic mirror symmetry between the "virtual" and "corporial" worlds. This seems highly prudent considering the events of the last two years.**

**It should also be noted that current systems of editing in academia have many flaws, but also allow for the useful control of information flow. This is obviously a useful property to have, but it could be done much more efficiently. Moreover, a proof-of-useful-work model involving trust scores should also be implemented in a way similar to [COTI](https://coti.io/technology). This would allow for multiple levels of delegator/indexer relationships. Moreover, machine learning agents similar to those constructed in [Fetch.ai](https://fetch.ai/technology/) could be constructed on behalf of users to help refine search parametrs for relevant research articles. The arXiv has included a knowledge graph for research articles via [connected papers](https://www.connectedpapers.com/). An experimental component involving an AI pair programmer or author such as [OpenAI Codex](https://openai.com/blog/openai-codex/) or [GPT-3](https://openai.com/blog/gpt-3-apps/) should be included as well. This may open new avenues of research and idea generation in highly technical fields. Together this would also provide an incredibly novel education system that could scale and open up research on highly technical topics to more people globally who may not have the opportunity to participate in traditional forms of education. Further, GPT-3 or a similar transformer model could be used for translating into languages other than those typically used in academia.**

**Mathematics and science in general is a social activity and we should incentivize prosocial behaviors in research communities. It has become abundantly clear in recent years that misinformation has become an obstacle to the basic functions of society, and academia is not immune. Errors and misconceptions in research, as well as a lack of reliable editing and dissemination of that research are problems that Athenaeum can address effectively.**

Discussion of the paper
=======================

The paper studies interesting objects (surface algebras) and brings possible new links with other subjects in mathematics (such as L-functions).  
However, I think the paper suffers from the following issues.

(a)The action of the absolute Galois group on constellations (and thus on dessins d'enfant) is never recalled in the paper.  
This makes the contents of Theorem 5.4(7) and Theorem 9.1 almost impossible to assess. It also makes it impossible for the reader to check that the two dessins in example 11.1 are indeed in the same orbit. 

(b )Some of the statements lack in precision or clarity, some results are implied and not proved, and some important assumptions that are made 
in the text should be made more prominently.  The following are such cases:

(b1) Abstract: "The surface orders can be constructed in such a way that they are the completion of the path algebra of a quiver with relations which gives the surface algebra of the dessin".  This is implicitly stated several times in the paper, but never explicitly stated as a proposition/theorem and, more importantly, never proved.  Comments (b3) and (b4) below are related to this.

(b2)p.15, proof of theorem 5.4: It is claimed that "[t]he statements concerning the actions of \sigma and \phi [...] will be refined in the 
following sections and proven there".  It would be helpful to point to the precise parts of the paper where this is done.

(b3)p.21, l.-7: "this is exactly the completion of the surface algebra associated to the graph".  The rest of the paper suggests that this is a general fact if all R_i are taken to be isomorphic to k[[x]].  This is an important fact.  It should be stated as a proposition or a theorem, and it should be proved.

(b4)p.25, l.5-6: "For concreteness of examples, we will take the dessin order \Lambda associated to a constellation C=[\sigma, \alpha, \phi] to be the completed path algebra of the surface algebra associated to C."  Two issues here.  Firstly, this sentence is confusing.  Is it claiming that the completed path algebra of the surface algebra of C can always be realized as a dessin order? If so, what are the good choices of R_i and m_i?  I think this sentence should be made more precise, become a proposition or a theorem, and be proved.  Secondly, it seems that from now on in the paper, it is always assumed that the orders are chosen so that the surface orders are the completed surface algebras.  This very important assumption should be made more obvious, as without it some later statements are difficult to understand, and since it reduces the generality in which the later results are proved.

(b5)p.29, Corollary 10.2: The statement is not precise enough.  What does "classifying" mean in this context? Is it claimed that surface algebras (up to isomorphism) are in bijection with constellations?  If so, perhaps some previous results saying that gentle algebras (even infinite-dimensional ones) are in bijection with dissections of surfaces should be cited, such as work of Baur-Coelho, Opper-Plamondon-Schroll and many others.

(c)In the abstract and introduction, it is hard to tell the difference between what will be proven in this paper, what is announced as future work, and what is speculation.  For example:

(c1)Abstract: "are closely related to the fundamental group(oid) of the Riemann surfaces and the associated monodromy group": the fundamental groupoid is never mentioned in the paper, except here and once in the introduction.  What does this sentence mean?

(c2)Sections 2.6 and 2.10 seem to discuss the possibility that the paper is connected with certain topics in mathematics, but their phrasing could lead the reader to believe that such connections will appear later in the paper.  It should be made clearer that these sections contain speculation.

(c3) Section 2.9 announces future results of the author (Theorem 14.3 and Corollary 14.4).  It should be stated clearly within the section that these statements are not proved in the current paper.

(d)Some results on the representation theory of gentle algebras are proved withouth mention of the extensive literature on the subject.  This mostly applies to Theorem 10.1, which is equivalent to computing projective modules and projective resolutions of simple modules over a (possibly infinite-dimensional) gentle algebra, although this is not stated.

(e) The role of sections 12 and 13 should be clarified.  For the moment, they seem to only provide sources of orders. 


Opinion
=======

In view of the above, I do not feel I can recommend the paper to be accepted for publication in [this math journal].


Comments
========

While reading, I have gathered a list of comments which may be of use to the author.

(1) p.2, l.-24: Is it wise to mention the "Benson archive"?

(2)p.3, l.-9: "relations of the form" --> "and relations of the form".

(3)p.3, l.-5: "contruct from" --> "constructed from".

(4)p.3, l.-3: ""cyclic ordering" of the edges": should it not be of the half-edges?

(5)p.4, l.12: "such block are" --> "such blocks are".

(6)p.4, l.23: "and potentially a countably infinite set of other": could this be made more precise?

(7)p.4, l.-14: "dehedral agebras" --> "dihedral algebras".

(8)p.8, l.-6: "surfaceX" --> "surface X".

(9)p.9, l.20: "collection of" --> "product of pairwise disjoint".

(10)p.12, l.1 of section 3.4: "to not" --> "to note".

(11)p.12, section 3.4: It is not clear what the title of this section has to do with its content; for instance, the word "hypermap" does not appear 
at all in the section.

(12)p.12, definition 4.1: One should start by fixing a constellation C.

(13)p.13, l.-5 and l.-3 and l.-1: in all three equations, should it not be the tensor product of d copies of A_1, instead of A?  Also, it should be 
mentioned that the tensor product is taken over A_0.  The same comment applies to Lemma 9.2.

(14)p.14, l.3: the notation "curly A_0" should be defined.

(15)p.14, l.2-3: is it really sufficient that \phi fixes A_0 for \phi to be continuous?

(16)p.14, definition 5.3: it should perhaps be noted that this definition gives a strict subclass of the class of (possibly infinite-dimensional) gentle algebras.

(17)p.14, l.-17: I do not understand the reference to Polya theory.  Could this be clarified?

(18)p.15, point (7) of theorem 5.4: the action of the absolute Galois group on a constellation has not been defined.  It is thus difficult to see 
what point (7) implies.

(19)p.15, proof of theorem 5.4: The proof does not mention the action of the absolute Galois group.  Thus it is hard to see how point (7) is proved.

(20)p.15, Examples 5.5 through 5.8: In the quivers depicted, some arrows are dotted and some are full.  It seems that the convention is that the composition 
of two dotted (or full) arrows is zero.  This should perhaps be explicitly stated.

(21)p.17, definition 6.4: This does not seem to be the usual definition of an order.  What is the reference for it?  Moreover, it seems that it should be 
assumed that k is a subfield of K.  

(22)p.17, definition 6.5: It seems that one should assume that for any i, the quotient R_i/m_i is isomorphic to k.

(23)p.19, l.4: "normalization": could a comment on the choice of terminology be added?

(24)p.19, l.5: "The indecomposable projective \Lambda-modules": please add "up to isomorphism".

(25)p.19, l.4 of section 7: there is a missing "sl" to write "sl_2(C)".

(26)p.19, l.-10: "asked the following question" is followed by a sentence which is not a question.  Could it be replaced by "posed the following problem"?

(27)p.19, l.-10: "Let k, be a" --> "Let k be a".

(28)p.20: Section 8 is titled "Some Examples".  Since section 7 was already an example, perhaps section 8 could be titled "Some Further Examples" instead?

(29)p.24, l.-9: "Notice, the two arms meet back up at "x"": I find this sentence confusing, since it suggests that the two copies of "x" at which the two 
arms meet are identified, but it is not the case.  I suggest reformulating or removing the sentence.

(30)p.25, theorem 9.1: It is hard to understand the statement since the action of the Galois group on constellations has not been defined.

(31)p.25, theorem 9.1: Is Z(\Lambda) the center of \Lambda?

(32)p.25, lemma 9.2(1): it is unclear what multiplying on the left by A_0 means.

(33)p.26, l.-15: "Thus, the ideal" should perhaps be "Thus, the subalgebra"?

(34)p.27, example 9.3: In think the arrows are mis-labelled in the picture.  For example, there is no arrow labelled "c".

(35)p.27, footnote: is this speculation? or is it proved somewhere in the paper?

(36)p.36, l.6: since the field of p-adic number has characteristic 0, it is perhaps better to say that the a_k are integers between 0 and p-1.

(37)p.36, l.-13: "This means O_K are elements" --> "This means O_K is the set of elements".

(38)p.37-38: please provide references for the material in section 13.2.

(39)p.38, l.5: the space "b_- \otimes C[[x_i]]" is not equal to \Lambda_i, as one would perhaps expect seeing the inclusions on line 3 of the same page.  
Is this intentional?

(40)p.38, l.-14: "Iwahara subgroup": what is the reference for this terminology? A Google search provided me with only two results, one from the paper under 
review and one from its sequel.

(41)p.46, theorem 14.3: it is claimed that this result will be proved in a later paper.  However, I could not find it in the paper "Surface algebras and 
surface orders II" of the same author.

(42)p.47, l.17: "potentially suicidal": such colorful turns of phrases are probably best avoided. (This is actually from the Lando-Zvonkin book pg. 115, so I should 
have cited it I suppose. The actual quote is "It would be a suicidal act on our part to start here a careful exposition of
Galois theory: we would never arrived at the next chapter."). 

(43)p.47, references: The following references should be corrected.
  -[ASS] and [ES1] through [ES4]: "Skowronski" --> "Skowroński".
  -[ABCP]: "P-G" --> "P.-G.".
  -[B], [BM], [BS] and [BT]: "Bauer" --> "Baur".
  -[BFZ]: "DUKE MATHEMATICAL JOURNAL" should not be in capital letters.
  -[BR]: "reiten" --> "Reiten".
  -There are two references with label [E].  
  -There are two references with label [ES4].
  -[FH]: Fulton's initial is missing.
  -Between [H3] and [K] is a reference labelled [1].  This is confusing.
  -The two references by A. Schreiber should be labelled [S1] and [S2] instead of [AS2] and [AS3].
  -[AS3] only refers to an author and a title.
  -[SV]: "Berg" --> "Bergh".
  -General comment: Some authors' first names are written in full, and some only have initials.  This should be harmonized.
  -General comment: If one choses to write only initials, then one of the following conventions should be followed, but not both: "A. Schreiber" or "Schreiber, A.".
  -General comment: Some references, such as [E5], are not cited in the text.
