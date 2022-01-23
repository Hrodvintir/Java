# Java Math Support

Review the Javadocs for [java.lang.Math](https://docs.oracle.com/javase/8/docs/api/java/lang/Math.html).

Note that java.lang.Math is a class, and because it is part of the java.lang package, is implicitly available without importing.  We only use import with java.lang.Math if we are using static imports.

On the other hand, [java.math](https://docs.oracle.com/javase/8/docs/api/java/math/package-summary.html) is a package, and home to the BigDecimal class, which is what we should be using for currency calculations.  IEEE floating point is not an acceptable implementation for monetary calculation.

