# Operator Precedence

In general, it is best to use parenthesis () to clarify expressions, rather than rely on operator precedence, but here are additional resources on operator precedence:

[Operators, from the official Java Tutorial](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/operators.html)

[The Expressions section from the Java Language Specification](https://docs.oracle.com/javase/specs/jls/se8/html/jls-15.html)

However, rather than rely on operator precedence in a case like:

if (a < b && c > d)

you could clarify it explicitly as:

if ((a < b) && (c > d))

Now it is explicitly clear that the result is the AND of the two comparisons.
