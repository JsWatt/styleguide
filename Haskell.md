[//]: # (http://www.seas.upenn.edu/~cis194/spring13/docs/style.pdf)
## Good Haskell Style

• DO use camelCase for function and variable names.

• DO use descriptive function names, which are as long as they need to
be but no longer than they have to be.

• DON’T use tab characters. Haskell is layout-sensitive and tabs Mess
Everything Up.

• DO try to keep every line under 80 characters.

• DO give every top-level function a type signature. Type signatures
enhance documentation, clarify thinking, and provide nesting sites for
endangered bird species. Top-level type signatures also result in better
error messages. With no type signatures, type errors tend to show up
far from where the real problem is; explicit type signatures help localize
type errors.
Locally defined functions and constants (part of a let expression or
where clause) do not need type signatures, but adding them doesn’t
hurt (in particular, the argument above about localizing type errors
still applies).

• DO precede every top-level function by a comment explaining what it
does.

• DO use -Wall. Either pass -Wall to ghc on the command line, or
(easier) put
{-# OPTIONS_GHC -Wall #-}
at the top of your .hs file. All your submitted programs should compile
with no warnings.

• DO, as much as possible, break up your programs into small functions
that do one thing, and compose them to create more complex functions.

• DO make all your functions total. That is, they should give sensible
results (and not crash) for every input.


## this is a starting point from [CIS 194](http://www.seas.upenn.edu/~cis194/spring13/docs/style.pdf)
