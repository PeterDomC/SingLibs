<h1>
  SingLibs - A collection of libraries for computing curve sinuglarity invariants and differential algebras
</h1>

SingLibs contains two libraries for the computer algebra system [Singular](https://www.singular.uni-kl.de/).
The library [difform.lib](https://www.singular.uni-kl.de/Manual/4-1-3/sing_2481.htm) contains types and methods that allow for computing over differential algebras in Singular.
The library [curveInv.lib](https://www.singular.uni-kl.de/Manual/4-2-0/sing_1259.htm) contains methods for computing invariants of curve singularities.

Note that the code of both libraries is written in the Singular specific language.

```
Overview of "curveInv.lib".

The library provides functions for computing the following invariants of curve singularities:
    - the delta invariant,
    - the multiplicity of the conductor - namely the colength of 
      the conductor ideal in the normalization,
    - the Deligne number,
    - the colength of derivations along the normalization - namely the colength of derivations 
      relative to derivations on the normalization
```

```
Overview of "difform.lib".

The library provides the new types 'difvar' and 'difform' for representing differential forms over quotient rings.
The former type 'difvar' is used to simulate the basic differential forms dx_1, ..., dx_n
(if the underlying polynomial ring has the variables x_1, ..., x_n).
These basic forms are introduced as new variables dx_i over a non-commutative ring 
that features 'exterior' relations among the dx_i.
For more general differential forms, the type 'difform' can be used.
An object of this type carries a polynomial in the 
differential algebra which represents the differential form.

For computing with general differential forms, most arithmetic operations were implemented.
Additionally, the universal derivation is available as a procedure and can be 
applied to differential forms or polynomials.
The library also supports derivations.
These are linear maps from the first graded part of the differential algebra to the basering.
Derivations are defined via the type 'derivation' and there are procedures for 
arithmetic operations, evaluation, and Lie-derivative.
```

A more detailed documentation can be found in the code and in my master's thesis which is attached to the repository.
