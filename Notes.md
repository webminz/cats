Categorical Theory Statements


category theory = algebra of functions 
surprising wide range of applications that can replace SET theory as universal language
1945: Birth in "General theory of natural equivalences"
late 40s, applications in algebraic topology (shapes), homology theory and abstract algebra (equations)
1950: Grothendieck use of CT in algebraic geometry
1960: Lawvere applied CT to logic
1970: CT appears in linguistics, cognitive science, computer science and philosophy
1980: Lambek discovers types and programs as a category, Eugenio Moggi added monads
CT was invented to express Adjunctions, which required natural transformations, Functors, Categories


Limits and Colimits are one object summary of a diagram
duality between tuples and equivalence classes

# D. Spivak

"a graphic has the power to evoke feelings of understanding, without
really meaning much"
"it is possible to use a language such as
English to express ideas that are never made rigorous or clear"
"Science is about agreement"


Hierarchies are partial orders, 
symmetries are group elements, 
data models are categories,
agent actions are monoid actions, 
local-to-global principles are sheaves, 
self-similarity is modeled by operads, 
context can be modeled by monads.


Relativity theory relates to postmodernism: there is no single perspective from which to view the world, no metanarrative to save us (criticism against ontologies)
real power lies in being able to translate between them.

Categorical Logic:
Consider a set I, i.e. an object in the base category, e.g. all possible instances of a metamodel
A predicate X is a subset of I, i.e. an object in the fibre of a respective functor (projection on the second component)
That fibre induces a boolean algebra of predicates: and=intersection, or=union, not=complement, implies=subset, false=emptyset, true=I
forall and exist require and adjunction, i.e. a term in another fibre


What does a diagram (= syntax) mean?
Can we compose them?
Can we reason diagrammatically?
What compositions preserve properties


The subtleties of indexed vs. fibered semantics, i.e. in fibered semantics the default is span(Graph) => default multiplicity is 0..*
What happens to diagrams when we down-type further?
What about attributes?

compact closed means to have loops but still directed
hypergraph category direction does not matter

Ambiguous terms in my work
Models
Diagrams

Collection Functors, i.e. endofunctors SET -> SET
powerset functor (unordered, unique)
multiset functor: assigning a natural number to each element (unordered, nonunique)
kleene closure: lists (ordered, nonunique)


= Bartosz Milewski

Category Theory for Programmers


Programming is about composition
A category is a world where things can be composed
In FP a program is a function
Morphism = Program/Function
Object = Type
Functors = Type constructors
Natural Transformation = Polymorphic function
Universal constructions = algebraic datatypes
CCC = Function and Product Types
Algebras and Coalgebras for Functors = Recursive Datatypes 
Recursive Type Definitions, e.g. List Data X = NonEmpty Data X | Empty, require colimits (fixpoint)
F(unctor)-Algebra is given by an object X (carrier) and a catamorphism cata : F X -> X (eval)
Lambeks theorem: If (F X, a) is initial then a is an isomorphism, i.e. X is a fixpoint for F
And Adameks theorem says every endofunctor has a fixpoint.
Directed Colimits (telescoping unions) are used to create initial algebras: O -> F 0 -> F F 0 -> F F F 0 -> ....
Monads (special functors) = side effects
Powerset monads: X -> P(Y) <=> X -> 2^Z <=> X x Y -> 2, i.e. relations between X and Y
Applicatives are the curried version of lax monoidal functors, have a lift f(a -> b) -> f a -> f b
precomposition is contravariant whereas postcomposition is covariant


cartesian square is another name for a pullback square
cartesian (= eucledian geometry) is all about distances, therefore triangles
triangles are comparisons of distances



# Lawvere Book

Composition is like multiplication
Isomorphisms are like divisions, i.e. finding a multiplicative inverse
Because composition is not commutative, there are left and right inverses
Geometry is about shapes, i.e. constellations of points
In eucledian geomatry transformations (scaling, moving) preserve distances


# Unknown


Concept of span rewriting based on pushouts.
Categorical basis, adhesive cats --> (weak) adhesive HLR cats ---> herediatry pushout cats!
Constants make the initial object isomorphic to the terminal object, which makes forming sums difficult.
Multi-ary ops (requires products) makes sums tricky, both things result in loosing the adhesiveness property

The latter have all important results, existence of pushouts, unqiueness of pushout complements, parrelelization and concurrency theorems
The latter is paramoun for the TGG theory



Multi-Spans are a functor category (modulo some partiality -> monicity conditions) [Comprehensive System Construction]
Diagram Graphs (Sketches) are a functor category [Makkai Construction]
Functor categories can be generalized into Functor -> Span Categories (here are different monads hidden for partial functions, relations, and lists)
Functor -> Span Categories are equivalent to typed graphs

Questions: What universal truth is adhesiveness hiding, i.e. applications of GT rules require it, and amalgamation in fibered semantics (see Harald und Uwes papers)
Questions: Waht is semantic?
Questions: What is the grothendieck construction
Questions: How do we get view frameworks (algebras, universal updateability)


# Computational trinitarianism from ncatlab

in

Paul-André Melliès, Functorial boxes in string diagrams, Procceding of Computer Science Logic 2006 in Szeged, Hungary. 2006
https://dumas.ccsd.cnrs.fr/PPS/hal-00154243


Recall:
Propositions as types
Programs as Proof
Category theory and type theory are really similiar

Proposition = Type = Object
proof = program = generlized element
true = terminal object = unit
false = initial object = empty type
cut rule = pullback of display maps = substitution
cut elimination = counit of hom-tensor adjunctipn = beta reduction
introduction rule = unit of hom-tensor adjunction = eta conversion
conjuction = product = product type
disjunction = coproduct = sum type
implication = exponential = function type
negation = exponential into initial object = function type into the empty type
induction = colimit = inductive type ???
coinduction = limit = coinductive type
modality = monad = monad
linear logic = summetrical monoidal category = linear type theory









