---
title: "EuroProofNet Workshop on the development, maintenance, refactoring and search of large libraries of proofs"
layout: single
permalink: /wg4-meeting1-program/
author_profile: true
breadcrumbs: true
---

[Main page](../wg4-meeting1)

**Warning:** Time in Tbilisi (UTC+4)

## Friday 23 September

- 12:30 CLAS lunch time

Session chair: Frédéric Blanqui

- 14:00 [Claudio Sacerdoti](http://www.cs.unibo.it/~sacerdot/) (University of Bologna), The challenges of the EuroProofNet Working Group 4 on proof libraries ([slides](sacerdoti.pdf))

- 14:30 Georges Gonthier (INRIA Saclay) [online], First-class object hierarchies
 ([slides](gonthier.pdf))

As modern algebra is organised in hierarchies of structures, encoding these in the Coq type theory is the foundation of the Mathematical Components library and the proof of the Odd Order Theorem.
As the structures and their hierarchical relations are first class objects in this encoding, it turns out the same techniques can be used to create hierarchies of other mathematical entities, such as functions, sets or relations. These have played a key part in developing a modular library in which a few overloaded lemmas can apply uniformly to a range of entities.

- 15:00 [Enrico Tassi](http://www-sop.inria.fr/members/Enrico.Tassi/) (INRIA Sophia Antipolis), [Hierarchy Builder](https://github.com/math-comp/hierarchy-builder), algebraic hierarchies made easy (in Coq) [online] ([slides](tassi.pdf))

It is nowadays customary to organize libraries of machine checked
proofs around hierarchies of algebraic structures. One influential
example is the Mathematical Components library on top of which the long
and intricate proof of the Odd Order Theorem could be fully formalized.
Still, building algebraic hierarchies in a proof assistant such as Coq
requires a lot of manual labor and often a deep expertise in the
internals of the prover. Moreover, according to our experience, making
a hierarchy evolve without causing breakage in client code is equally
tricky: even a simple refactoring such as splitting a structure into
two simpler ones is hard to get right.
In this talk we describe HB, a high level language to build hierarchies
of algebraic structures and to make these hierarchies evolve without
breaking user code. The key concepts are the ones of factory, builder
and abbreviation that let the hierarchy developer describe an actual
interface for their library. Behind that interface the developer can
provide appropriate code to ensure retro compatibility.
We make a demo the HB language using the hierarchy-builder addon for
the Coq system.

- 15:30 CLAS coffee break

Session chair: Erika Abraham

- 16:00 Roland Coghetto and [Julien Narboux](https://dpt-info.di.unistra.fr/~narboux/) (University of Strasbourg) [online], The GeoCoq library and its porting to Isabelle ([slides](narboux.pdf))

GeoCoq is a formal proof library consisting in a formalization of foundations of geometry. It is based on several different axiom systems by Euclid, Hilbert and Tarski, and includes the arithmetization of geometry, i.e. the link between synthetic and analytic geometry. 
After giving a quick overview of the library, we will discuss how automation and logical foundations are used in each part of the library and the potential impact on porting the library to other proof assistants. Then, we will report on the porting of the library to Isabelle/HOL by Roland Coghetto.

- 16:30 [Marco Maggesi](https://sites.google.com/unifi.it/maggesi/), The HOL Light library of formalized mathematics ([slides](maggesi.pdf))

The HOL Light theorem prover has two seemingly conflicting features.
On the one hand, it is a system with a very thin layer of meta-logical or extra-logical features.
Yet, on the other hand, HOL Light has a library of mathematical results encompassing several advanced mathematical topics, from complex analysis to algebra, including profound results such as the Riemann mapping theorem or Hales’ theorem, to name just two of them.
Because of the simplicity of its architecture, HOL Light has been used as the base for research of various kinds, from exploring variants of the HOL logic, to implementing deep learning models for automated theorem proving.
Thus, HOL Light and its library can be a natural and promising environment for experimenting with the management of formal mathematics libraries.

- 17:00 [Geoff Sutcliffe](https://www.cs.miami.edu/home/geoff/) (University of Miami), Proofs and Models in the TPTP World [online] ([slides](https://www.tptp.org/Seminars/TPTPProofsAndModels/Contents.html))

This talk describes the current (underdeveloped?) representation and use of proofs and models in the TPTPWorld. Topics covered include the SZS ontology; the representation of derivations and finite models; the TSTP solution library; tools for examining and manipulating the derivations; uses of individual solutions, and the TSTP as a whole; projects that have used the TPTP format and tools for proofs and models; the proposed "Tons of Data for Theorem Provers" library; future work and directions to improve the status quo.

- 17:30 [Florian Rabe](https://kwarc.info/people/frabe/) <!--and [Michael Kohlhase](https://kwarc.info/people/mkohlhase/)--> (University of Erlangen), Experiences from Exporting Major Proof Assistant Libraries ([slides](rabe.pdf))

The interoperability of proof assistants and the integration of their libraries is a highly valued but elusive goal in the field of theorem proving.
As a preparatory step, in previous work, we translated the libraries of multiple proof assistants, specifically the ones of Coq, HOL Light, IMPS, Isabelle, Mizar, and
PVS into a universal format: OMDoc/MMT.
Each translation presented great theoretical, technical, and social challenges, some universal and some system-specific, some solvable and some still open.
In this talk, we survey these challenges and compare and evaluate the solutions we chose.
We believe similar library translations will be an essential part of any future system interoperability solution and our experiences will prove valuable to others undertaking such efforts.

- 18:00 discussion session

- 18:30 end

- 19:00 (TBC) dinner at [Apkhazeti](https://www.facebook.com/restaurantApkhazeti), Zviad Gamsakhurdia Named Right Bank, Tbilisi (2.4 km, 30 minutes walk). Shared taxis will be organized. Contact: [Besik Dundua](https://cte.ibsu.edu.ge/en/besik-dundua/)

## Saturday 24 September

- 09:00 CLAS invited speaker slot (TBA)

Session chair: Claudio Sacerdoti

- 10:00 [Reuben Rowe](https://www.cs.rhul.ac.uk/home/rrowe/) (Royal Halloway University of London), Refactoring OCaml ([slides](rowe.pdf))

I will report on our work implementing automatic refactoring techniques
for the OCaml programming language. As a simple case study, we look at
renaming value bindings (e.g. functions). This turns out to be
surprisingly tricky, largely because of OCaml's powerful module system.
Our solution is to define an abstract semantics that captures when
different declarations in an OCaml program denote or refer to the "same"
function, and thus must all be renamed together.

The challenges we describe should be inherited by proof assistants that
adopt similar module systems, like Coq and Agda, and thus our approach
should be applicable there too.

- 10:30 CLAS coffee break

- 11:00 [Fabian Huch](https://www21.in.tum.de/team/huch/) (Technical University of Münich) and [Yiannis Stathopoulos](https://www.cl.cam.ac.uk/~yas23/) (University of Cambridge), Finding facts in large formalization libraries: two Isabelle/AFP attempts ([slides](stathopoulos.pdf))

The Isabelle Archive of Formal proofs is one of the largest
formalization libraries in existence: As of mid-2022, in its 690
entries, a total of 210K lemmas have been proven by 424 different
authors in 3.5M lines of code.
In opened Isabelle theories, finding elements is easily possible, e.g.
by term unification.
However, this approach does not scale to the vast material in the
archives, as loading all formalizations the into the prover is infeasible.
In early 2020, not only one but two new Isabelle search engines emerged
that address the problem in a scalable way.
Both search engines work off-line (i.e., not requiring the proof
assistant), and rely on pre-built indexes. However, approaches and goals
are different:
FindFacts is a pragmatic approach that utilizes Isabelle functionality
for an easy-to-use and fast drill-down search, whereas SErAPIS parses
prover IDE markup to build up a concept-oriented search that abstracts
away from syntax.

- 11:45 [Artur Korniłowicz](http://math.uwb.edu.pl/~arturk/) (University of Bialystok), XML-based representation of Mizar Mathematical Library [online] ([slides](kornilowicz.pdf))

The Mizar Mathematical Library is a collection of mathematical papers written in the Mizar language and fully computer-verified by the Mizar proof checker.
From many years the Mizar Mathematical Library is a subject of translation into other systems for its cross-verification or representing its content in various formats.
To facilitate this task several internal XML-based formats have been designed to be processable by generic tools independent from the Mizar system.
These formats represent various syntactic-semantic information accessible at various stages of proof verification by the Mizar checker.
In this talk we present constructions of the Mizar language and describe how they are represented in the XML formats.
We also present the content of the Mizar Mathematical Library with a focus on its initial articles and discuss the management model of the library.

- 12:30 CLAS lunch time

Session chair: Maribel Fernandez

- 14:00 [Anne Baanen](https://www.cs.vu.nl/~tbn305/) (Vrije Universiteit Amsterdam), Bundling in Dependent Type Theory ([slides](baanen.pdf))

Dependent type theories allow us to bundle proofs and data in the same structure, which can be a great help for automation. On the other hand, unbundled definitions can allow greater flexibility. I discuss my experiences with refactoring between unbundled and bundled definitions in the Lean mathematical library mathlib, especially focusing on the implementation of typeclasses.

- 14:45 [Alexander Best](https://alexjbest.github.io/) (Vrije Universiteit Amsterdam), Metaprogramming for Automation of Library Maintenance ([slides](https://alexjbest.github.io/talks/wg4-kickoff))

Large libraries of formal proofs are becoming increasingly common, and
pose several challenges for the maintenance and upkeep if they are to
be widely useful and remain so.
Specific issues for maintenance include problems such as: ensuring
content is not duplicated, it is organised appropriately, it is
sufficiently general to be useful in other developments, or that a
large library is coherent so different parts can be used together.
Ensuring these properties hold is mostly done by human review, which
while always a useful component can be a limiting factor of
maintenance.
We describe several specific problems that can be addressed with
automated tooling, and give some case studies showing how automation
can help humans review things they may not have the time to look into,
and also help us spot difficult to notice issues.

- 15:30 CLAS coffee break

Session chair: Alexander Best

- 16:00 [Riccardo Brasca](https://webusers.imj-prg.fr/~riccardo.brasca/) (University of Paris Cité), Maintenance of Lean's mathlib and the Liquid tensor experiment ([slides](brasca.pdf))

mathlib is Lean's mathematical library, one of the largest collection of formalized mathematics, with more than 800,000 lines of codes and 130,000 theorems/definitions. I will explain how we maintain such a big library and how new results are added every day. I will also speak about the liquid tensor experiment, a very recent project where we formally verified contemporary mathematics that used mathlib in a crucial way. Rather than focusing on the mathematics, I will explain why a centralized library is necessary for such a project.

- 17:00 [Talia Ringer](https://dependenttyp.es/) (University of Illinois at Urbana-Champaign) [online], Concrete Problems in Proof Automation ([slides](ringer.pdf)) ([AITP video](https://youtu.be/lRczFjl6Ljs))

Machine learning for proof automation has made massive strides in recent years. But are these strides in the right directions? This talk will present challenging and impactful tasks for machine-learning-based proof automation that I believe to be underexplored. It will make a case for the utility of these tasks for users of proof assistants, and the meaning of these tasks for advancing the capabilities of AI systems.

- 17:30 [André Freitas](http://andrefreitas.org/) (University of Manchester), Natural Language & Proofs: A Neuro-symbolic Perspective ([slides](freitas.pdf))

This talk provides an overview of emerging methods and representation paradigms in Natural Language Processing (NLP) to support the interpretation of proofs. We will aim for a synthesis of the increasing dialogue between the neural perspective (e.g. large-scale neural language models) and symbolic inference, looking into specific architectural devices which are used to integrate the properties of both types of representation. We will finalize with an argument of how these methods can support the core aims of EuroProofNet: to improve the interoperability and usability of proof systems.

- 18:10 end

- 19:00 dinner together in some restaurant for those who want (suggestions are welcome)
