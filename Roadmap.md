| expected completion | completion date | description                                                                                  |
|:--------------------|:----------------|:---------------------------------------------------------------------------------------------|
| Mon, 4 June         | Mon, 4 June     | define a reasonable subset of CoffeeScript                                                   |
| Wed, 6 June         | Wed, 6 June     | design the intermediate data representations                                                 |
| Thu, 7 June         | Fri, 8 June     | choose a platform for building the bootstrapping compiler (haskell? jashkenas/coffee-script?)|
| Fri, 8 June         | Fri, 8 June     | implement the AST constructors                                                               |
| Mon, 11 June        | Mon, 11 June    | choose a parsing strategy and library                                                        |
| Wed, 27 June        | Mon, 25 June    | define a parser that can parse my subset of CoffeeScript                                     |
| Thu, 28 June        | on hold         | a simple code generator for CS ASTs, cscodegen                                               |
| Fri, 6 Jul          | Fri, 6 Jul      | start writing the optimising transformations                                                 |
| Wed, 11 Jul         | Mon, 9 Jul      | get the optimiser working                                                                    |
| Fri, 10 Aug         | Fri, 10 Aug     | start writing the transformations from CS ASTs to JS ASTs                                    |
| ...                 | in progress     | start pulling in the test suite from jashkenas/coffee-script                                 |
| Fri, 7 Sep          | Wed, 5 Sep      | use Mozilla’s source map generator to generate source maps                                   |
| Fri, 14 Sep         | in progress     | expand the language and include all the features we initially left out                       |
| N/A                 | in progress     | start using it to compile popular projects; see if they continue to pass their test suites   |
| Fri, 21 Sep         | ...             | pass the current CS compiler's entire test suite                                             |
| Tue, 18 Sep         | Mon, 17 Sep     | self-host                                                                                    |
| Fri, 21 Sep         | ...             | documentation                                                                                |
| ...                 | ...             | finish up cscodegen                                                                          |
| ...                 | ...             | enhance escodegen to accept a grammar for generating CSTs                                    |