| feature name                              | example                                 | include? | AST? | parse  | compile |  test  |
|:------------------------------------------|:----------------------------------------|:--------:|:----:|:------:|:-------:|:------:|
| string interpolation                      | `"a#{b}"`                               |     ✓    |   ✓  |    ✓   |     ✓   |    ✓   |
| assignment                                | `a = b`                                 |     ✓    |   ✓  |    ✓   |     ✓   |    ✓   |
| single-line comment                       | `# comment`                             |     ✓    | N/A  |    ✓   |   N/A   |        |
| integer literal                           | `1`                                     |     ✓    |   ✓  |    ✓   |     ✓   |        |
| decimal literal                           | `1.1`                                   |     ✓    |   ✓  |    ✓   |     ✓   |        |
| boolean literal                           | `true`/`false`                          |     ✓    |   ✓  |    ✓   |     ✓   |    ✓   |
| parentheses for grouping                  | `(a or b) and c`                        |     ✓    | N/A  |    ✓   |   N/A   |        |
| logical operators                         | `and`/`or`/`not`/`&&`/`!`               |     ✓    |   ✓  |    ✓   |     ✓   |        |
| comparison operators                      | `<`/`<=`/`>`/`>=`/`==`/`!=`/`is`/`isnt` |     ✓    |   ✓  |    ✓   |     ✓   |        |
| member access                             | `a.b`                                   |     ✓    |   ✓  |    ✓   |     ✓   |    ✓   |
| dynamic member access                     | `a[b]`                                  |     ✓    |   ✓  |    ✓   |     ✓   |    ✓   |
| explicit function application             | `a(b, c)`                               |     ✓    |   ✓  |    ✓   |     ✓   |        |
| indentation introduces blocks             | `if a <\n> «indent» b`                  |     ✓    | N/A  |    ✓   |   N/A   |        |
| `then` introduces block                   | `if a then b`                           |     ✓    | N/A  |    ✓   |   N/A   |        |
| `@`-vars                                  | `@a`                                    |     ✓    |   ✓  |    ✓   |     ✓   |        |
| unary existential operator                | `a?`                                    |     ✓    |   ✓  |    ✓   |     ✓   |        |
| conditional execution                     | `if a then b`                           |     ✓    |   ✓  |    ✓   |     ✓   |        |
| conditional else clause                   | `if a then b else c`                    |     ✓    |   ✓  |    ✓   |     ✓   |        |
| negated flow control keywords             | `unless`/`until`                        |     ✓    | N/A  |    ✓   |   N/A   |        |
| in operator                               | `a in b`                                |     ✓    |   ✓  |    ✓   |     ✓   |    ✓   |
| of operator                               | `a of b`                                |     ✓    |   ✓  |    ✓   |     ✓   |    ✓   |
| instanceof operator                       | `a instanceof b`                        |     ✓    |   ✓  |    ✓   |     ✓   |        |
| negated infix operators                   | `not in`, `not of`, `not instanceof`    |     ✓    | N/A  |    ✓   |   N/A   |    ✓   |
| for-in                                    | `for v, k in a then e`                  |     ✓    |   ✓  |    ✓   |     ✓   |        |
| for-of                                    | `for k, v of o then e`                  |     ✓    |   ✓  |    ✓   |     ✓   |        |
| filtered loops via `when`                 | `for a in b when c then d`              |     ✓    |   ✓  |    ✓   |     ✓   |        |
| `own` keyword for `hasOwnProperty` filter | `for own k of o then c`                 |     ✓    |   ✓  |    ✓   |     ✓   |        |
| single-line function literals             | `(a, b) -> c`                           |     ✓    |   ✓  |    ✓   |   N/A   |    ✓   |
| parameter-less functions                  | `-> a`                                  |     ✓    |   ✓  |    ✓   |   N/A   |    ✓   |
| multi-line function literals              | `-> <\n> «indent» a`                  |     ✓    | N/A  |    ✓   |   N/A   |    ✓   |
| maths operators                           | `/, +, -, %, *`                         |     ✓    |   ✓  |    ✓   |     ✓   |        |
| array literals                            | `[a, b]`                                |     ✓    |   ✓  | mostly |     ✓   | mostly |
| explicit object literals                  | `{a: b}`                                |     ✓    |   ✓  | mostly |     ✓   | mostly |
| {pre,post}fix {in,de}crement              | `--a, a--, ++a, a++`                    |     ✓    |   ✓  |    ✓   |     ✓   |        |
| unary `+`/`-`                             | `+a`, `-a`                              |     ✓    |   ✓  |    ✓   |     ✓   |        |
| explicit `return`                         | `return 0`                              |     ✓    |   ✓  |    ✓   |     ✓   |        |
| unconditional loop                        | `loop then a`                           |     ✓    |   ✓  |    ✓   |   N/A   |        |
| `break`/`continue`                        | `loop then break`                       |     ✓    |   ✓  |    ✓   |     ✓   |        |
| classes                                   | `class A`                               |     ✓    |   ✓  |    ✓   |     ✓   |    ✓   |
| class-extends                             | `class A extends B`                     |     ✓    |   ✓  |    ✓   |     ✓   |    ✓   |
| class proto-assignments                   | `class A then m: ->`                    |     ✓    |   ✓  |    ✓   |     ✓   |    ✓   |
| extends operator                          | `A extends B`                           |     ✓    |   ✓  |    ✓   |     ✓   |        |
| `switch`-`when`-`else`                    | `switch a <\n> when b then c`           |     ✓    |   ✓  |    ✓   |     ✓   |        |
| `throw`                                   | `throw a`                               |     ✓    |   ✓  |    ✓   |     ✓   |        |
| `new` operator                            | `new A`                                 |     ✓    |   ✓  |    ✓   |     ✓   |        |
| semicolons as seq operator                | `a; b`                                  |     ✓    |   ✓  |    ✓   |     ✓   |        |
| string literals                           | `"a"`                                   |     ✓    |   ✓  |    ✓   |     ✓   |        |
| string hex escapes                        | `"\x61"`                                |     ✓    | N/A  |    ✓   |     ✓   |        |
| string character escapes                  | `"\n"`                                  |     ✓    | N/A  |    ✓   |     ✓   |        |
| string line continuation                  | `"<\n>a"`                               |     ✓    | N/A  |    ✓   |     ✓   |        |
| regex literals                            | `/a/`                                   |     ✓    |   ✓  |    ✓   |     ✓   |        |
| `do` operator                             | `do a`                                  |     ✓    |   ✓  |    ✓   |     ✓   |        |
| slices                                    | `a[b..c]  a[b...c]`                    |     ✓    |   ✓  |    ✓   |     ✓   |    ✓   |
| unbounded slices                          | `a[b...]  a[..b]`                      |     ✓    |   ✓  |    ✓   |     ✓   |    ✓   |
| `undefined` -> void 0                     | `undefined`                             |     ✓    |   ✓  |    ✓   |     ✓   |        |
| `null` literal                            | `null`                                  |     ✓    |   ✓  |    ✓   |     ✓   |        |
| compound assignment                       | `a «binary-op»= b`                    |    ✗     |   ✓  |    ✓   |     ✓   |        |
| boolean aliases                           | `yes`/`no`/`on`/`off`                   |    ✗     | N/A  |    ✓   |   N/A   |    ✓   |
| exponential notation                      | `1.2e+4`                                |    ✗     | N/A  |    ✓   |   N/A   |        |
| bitwise operators                         | `&`/`&#124;`/`^`/`~`/`<<`/`>>`/`>>>`    |    ✗     |   ✓  |    ✓   |     ✓   |        |
| soaked member access                      | `a?.b`                                  |    ✗     |   ✓  |    ✓   |     ✓   |    ✓   |
| dynamic soaked member access              | `a?[b]`                                 |    ✗     |   ✓  |    ✓   |     ✓   |    ✓   |
| binary existential operator               | `a ? b`                                 |    ✗     |   ✓  |    ✓   |     ✓   |        |
| implicit function application             | `a b, c`                                |    ✗     | N/A  |    ✓   |   N/A   |        |
| proto-member access                       | `a::b`                                  |    ✗     |   ✓  |    ✓   |     ✓   |    ✓   |
| dynamic proto-member access               | `a::[b]`                                |    ✗     |   ✓  |    ✓   |     ✓   |    ✓   |
| `@` as alias for `this`                   | `@`                                     |    ✗     | N/A  |    ✓   |     ✓   |        |
| soaked function application               | `a?(b, c)`                              |    ✗     |   ✓  |        |         |        |
| `while` loop                              | `while a then b`                        |    ✗     |   ✓  |    ✓   |     ✓   |        |
| postfix flow control                      | `a if b, c until d`                     |    ✗     | N/A  |    ✓   |   N/A   |        |
| inclusive ranges                          | `[a..b]`                                |    ✗     |   ✓  |    ✓   |     ✓   |    ✓   |
| exclusive ranges                          | `[a...b]`                               |    ✗     |   ✓  |    ✓   |     ✓   |    ✓   |
| bound function literals                   | `=>`                                    |    ✗     |   ✓  |    ✓   |     ✓   |    ✓   |
| object key-omission shorthand             | `{a}`                                   |    ✗     |   ✓  |    ✓   |   N/A   |        |
| implicit object literals                  | `a: b`                                  |    ✗     | N/A  | mostly |   N/A   |        |
| (splat/rest)-params                       | `(a...) ->`                             |    ✗     |   ✓  |    ✓   |     ✓   |    ✓   |
| `@`-params                                | `(@a) ->`                               |    ✗     |   ✓  |    ✓   |     ✓   |    ✓   |
| named destructuring assignment            | `{a: b} = c`                            |    ✗     |   ✓  |    ✓   |     ✓   |    ✓   |
| positional destructuring assignment       | `[a, b] = c`                            |    ✗     |   ✓  |    ✓   |     ✓   |    ✓   |
| splat/spread arguments                    | `fn a...`                               |    ✗     |   ✓  |    ✓   |     ✓   |    ✓   |
| chained comparison                        | `a < b < c`                             |    ✗     |   ✓  |    ✓   |     ✓   |    ✓   |
| `super`                                   | `super`                                 |    ✗     |   ✓  |        |         |        |
| `super` with arguments                    | `super a`                               |    ✗     |   ✓  |        |         |        |
| external constructors                     | `class A then constructor: c`           |    ✗     | N/A  |    ✓   |     ✓   |    ✓   |
| `try`-`catch`-`finally`                   |                                         |    ✗     |   ✓  |    ✓   |     ✓   |        |
| `try` operator                            | `try a`                                 |    ✗     |   ✓  |    ✓   |     ✓   |        |
| `typeof` operator                         | `typeof a`                              |    ✗     |   ✓  |    ✓   |     ✓   |        |
| continue lines ending in binary operator  | `a and <\n> b`                          |    ✗     | N/A  |    ✓   |   N/A   |        |
| backslash continues lines                 | `a \ <\n> + b`                          |    ✗     | N/A  | mostly |   N/A   |        |
| triple-quoted strings                     | `"""<\n>   a<\n>"""`                   |    ✗     | N/A  |    ✓   |  mostly |        |
| heregexen                                 | `/// a ///`                             |    ✗     |   ✓  |    ✓   |     ✓   |        |
| ACI in multiline array/object literals    | `[a<\n>b]`                              |    ✗     | N/A  | mostly |   N/A   |        |
| shallow copy of array                     | `a[..]`                                 |    ✗     |   ✓  |    ✓   |     ✓   |        |
| splices                                   | `a[b..c] = d`                           |    ✗     |   ✓  |    ✓   |         |        |
| unbounded splices                         | `a[b...] = c`                           |    ✗     |   ✓  |    ✓   |         |        |
| javascript literals                       | `javascript`                            |    ✗     |   ✓  |    ✓   |     ✓   |        |
| block comments                            | `### comment ###`                       |    ✗     |      |    ✓   |         |        |
| default parameters                        | `(a = b) ->`                            |    ✗     |   ✓  |    ✓   |     ✓   |    ✓   |