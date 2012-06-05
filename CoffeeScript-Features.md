<table>
<tr><th>feature name</th><th>example</th><th>include?</th><th>AST?</th></tr>
<tr><td>string interpolation</td><td>"a#{b}"</td><td>✓</td></tr>
<tr><td>assignment</td><td>a = b</td><td>✓</td><td>✓</td></tr>
<tr><td>single-line comment</td><td># comment</td><td>✓</td><td>N/A</td></tr>
<tr><td>integer literal</td><td>1</td><td>✓</td></tr>
<tr><td>decimal literal</td><td>1.1</td><td>✓</td></tr>
<tr><td>boolean literal</td><td>true/false</td><td>✓</td><td>✓</td></tr>
<tr><td>parentheses for grouping</td><td>(a or b) and c</td><td>✓</td><td>N/A</td></tr>
<tr><td>logical operators</td><td>and/or/not/&&/||/!</td><td>✓</td><td>✓</td></tr>
<tr><td>comparison operators</td><td></&lt;=/>/>=/==/!=/is/isnt</td><td>✓</td><td>✓</td></tr>
<tr><td>member access</td><td>a.b</td><td>✓</td><td>✓</td></tr>
<tr><td>dynamic member access</td><td>a[b]</td><td>✓</td><td>✓</td></tr>
<tr><td>explicit function application</td><td>a(b, c)</td><td>✓</td></tr>
<tr><td>indentation introduces blocks</td><td>if a &lt;\n> &lt;indent> b</td><td>✓</td></tr>
<tr><td>`then` introduces block</td><td>if a then b</td><td>✓</td></tr>
<tr><td>@-vars</td><td>@a</td><td>✓</td></tr>
<tr><td>unary existential operator</td><td>a?</td><td>✓</td><td>✓</td></tr>
<tr><td>conditional execution</td><td>if a then b</td><td>✓</td></tr>
<tr><td>conditional else clause</td><td>if a then b else c</td><td>✓</td></tr>
<tr><td>negated flow control keywords</td><td>unless/until</td><td>✓</td><td>N/A</td></tr>
<tr><td>in operator</td><td>a in b</td><td>✓</td><td>✓</td></tr>
<tr><td>of operator</td><td>a of b</td><td>✓</td><td>✓</td></tr>
<tr><td>instanceof operator</td><td>a instanceof b</td><td>✓</td><td>✓</td></tr>
<tr><td>negated infix operators</td><td>not in, not of, not instanceof</td><td>✓</td><td>N/A</td></tr>
<tr><td>for-in</td><td>for v, k in a then e</td><td>✓</td></tr>
<tr><td>for-of</td><td>for k, v of o then e</td><td>✓</td></tr>
<tr><td>filtered loops via when</td><td>for a in b when c then d</td><td>✓</td></tr>
<tr><td>own keyword for hasOwnProperty filter</td><td>for own k of o then c</td><td>✓</td></tr>
<tr><td>single-line function literals</td><td>(a, b) -> c</td><td>✓</td></tr>
<tr><td>parameter-less functions</td><td>-> a</td><td>✓</td></tr>
<tr><td>multi-line function literals</td><td>-> &lt;\n> &lt;indent> a</td><td>✓</td></tr>
<tr><td>maths operators</td><td>/, +, -, %, *</td><td>✓</td><td>✓</td></tr>
<tr><td>array literals</td><td>[a, b]</td><td>✓</td></tr>
<tr><td>explicit object literals</td><td>{a: b}</td><td>✓</td></tr>
<tr><td>{pre,post}fix {in,de}crement</td><td>--a, a--, ++a, a++</td><td>✓</td><td>✓</td></tr>
<tr><td>unary +/-</td><td>+a, -a</td><td>✓</td><td>✓</td></tr>
<tr><td>explicit return</td><td>return 0</td><td>✓</td><td>✓</td></tr>
<tr><td>unconditional loop</td><td>loop then a</td><td>✓</td></tr>
<tr><td>break/continue</td><td>loop then break</td><td>✓</td></tr>
<tr><td>classes</td><td>class A</td><td>✓</td></tr>
<tr><td>class-extends</td><td>class A extends B</td><td>✓</td></tr>
<tr><td>class proto-assignments</td><td>class A then m: -></td><td>✓</td></tr>
<tr><td>extends operator</td><td>A extends B</td><td>✓</td></tr>
<tr><td>switch-when-else</td><td>switch a &lt;\n> when b then c</td><td>✓</td></tr>
<tr><td>try-catch</td><td> </td><td>✓</td></tr>
<tr><td>throw</td><td>throw a</td><td>✓</td></tr>
<tr><td>new operator</td><td>new A</td><td>✓</td><td>✓</td></tr>
<tr><td>semicolons as seq operator</td><td>a; b</td><td>✓</td><td>✓</td></tr>
<tr><td>string literals</td><td>"a"</td><td>✓</td></tr>
<tr><td>string hex escapes</td><td>"\x61"</td><td>✓</td></tr>
<tr><td>string character escapes</td><td>"\n"</td><td>✓</td></tr>
<tr><td>string line continuation</td><td>"&lt;\n>a"</td><td>✓</td></tr>
<tr><td>regex literals</td><td>/a/</td><td>✓</td></tr>
<tr><td>do operator</td><td>do a</td><td>✓</td><td>✓</td></tr>
<tr><td>slices</td><td>a[b..c]  a[b...c]</td><td>✓</td></tr>
<tr><td>unbounded slices</td><td>a[b...]  a[..b]</td><td>✓</td></tr>
<tr><td>undefined -> void 0</td><td>undefined</td><td>✓</td><td>✓</td></tr>
<tr><td>null literal</td><td>null</td><td>✓</td><td>✓</td></tr>
<tr><td>compound assignment</td><td>a &lt;binary-op>= b</td><td>✗</td><td>✓</td></tr>
<tr><td>boolean aliases</td><td>yes/no/on/off</td><td>✗</td><td>N/A</td></tr>
<tr><td>exponential notation</td><td>1.2e+4</td><td>✗</td></tr>
<tr><td>bitwise operators</td><td>&/|/^/~/&lt;&lt;/>>/>>></td><td>✗</td><td>✓</td></tr>
<tr><td>soaked member access</td><td>a?.b</td><td>✗</td><td>✓</td></tr>
<tr><td>dynamic soaked member access</td><td>a?[b]</td><td>✗</td><td>✓</td></tr>
<tr><td>binary existential operator</td><td>a ? b</td><td>✗</td><td>✓</td></tr>
<tr><td>implicit function application</td><td>a b, c</td><td>✗</td><td>N/A</td></tr>
<tr><td>proto-member access</td><td>a::b</td><td>✗</td><td>✓</td></tr>
<tr><td>dynamic proto-member access</td><td>a::[b]</td><td>✗</td><td>✓</td></tr>
<tr><td>@ as alias for this</td><td>@</td><td>✗</td></tr>
<tr><td>soaked function application</td><td>a?(b, c)</td><td>✗</td></tr>
<tr><td>while loop</td><td>while a then b</td><td>✗</td></tr>
<tr><td>postfix flow control</td><td>a if b, c until d</td><td>✗</td><td>N/A</td></tr>
<tr><td>inclusive ranges</td><td>[a..b]</td><td>✗</td></tr>
<tr><td>exclusive ranges</td><td>[a...b]</td><td>✗</td></tr>
<tr><td>bound function literals</td><td>=></td><td>✗</td></tr>
<tr><td>object key-omission shorthand</td><td>{a}</td><td>✗</td></tr>
<tr><td>implicit object literals</td><td>a: b</td><td>✗</td></tr>
<tr><td>(splat/rest)-params</td><td>(a...) -></td><td>✗</td></tr>
<tr><td>@-params</td><td>(@a) -></td><td>✗</td></tr>
<tr><td>named destructuring assignment</td><td>{a: b} = c</td><td>✗</td></tr>
<tr><td>positional destructuring assignment</td><td>[a, b] = c</td><td>✗</td></tr>
<tr><td>splat/spread arguments</td><td>fn a...</td><td>✗</td></tr>
<tr><td>chained comparison</td><td>a &lt; b &lt; c</td><td>✗</td></tr>
<tr><td>super</td><td>super</td><td>✗</td></tr>
<tr><td>super with arguments</td><td>super a</td><td>✗</td></tr>
<tr><td>external constructors</td><td>class A then constructor: c</td><td>✗</td></tr>
<tr><td>try-catch-finally</td><td> </td><td>✗</td></tr>
<tr><td>try-finally</td><td> </td><td>✗</td></tr>
<tr><td>try</td><td>try a</td><td>✗</td></tr>
<tr><td>typeof operator</td><td>typeof a</td><td>✗</td><td>✓</td></tr>
<tr><td>continue lines ending in binary operator</td><td>a and &lt;\n> b</td><td>✗</td><td>N/A</td></tr>
<tr><td>backslash continues lines</td><td>a \ &lt;\n> + b</td><td>✗</td><td>N/A</td></tr>
<tr><td>triple-quoted strings</td><td>“””&lt;\n>   a&lt;\n>”””</td><td>✗</td><td>N/A</td></tr>
<tr><td>heregexen</td><td>/// a ///</td><td>✗</td><td>N/A</td></tr>
<tr><td>ACI in multiline array/object literals</td><td>[a&lt;\n>b]</td><td>✗</td><td>N/A</td></tr>
<tr><td>shallow copy of array</td><td>a[..]</td><td>✗</td></tr>
<tr><td>splices</td><td>a[b..c] = d</td><td>✗</td></tr>
<tr><td>unbounded splices</td><td>a[b...] = c</td><td>✗</td></tr>
<tr><td>javascript literals</td><td>`javascript`</td><td>✗</td></tr>
<tr><td>block comments</td><td>### comment ###</td><td>✗</td></tr>
<tr><td>default parameters</td><td>(a = b) -></td><td>✗</td></tr>
</table>