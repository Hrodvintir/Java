# Strings, Buffers and Builders

Strings are one of the most commonly used classes in Java.  But it is important to understand that String instances are immutable.  That means that every method that changes a String, actually returns a new instance.  This can lead to the presence of many String instances that you did not expect, and eventually to considerable garbage collection.

Consider this simple assignment:
```java
msg = "Part 1" + "Part 2" + "Part 3" + "Part 4"
```
In order to produce msg from concatenating all of those String instances, the Java compiler would have had to undertake these steps:
```java
msg = "Part 1Part 2" + "Part 3" + "Part 4"

msg = "Part 1Part 2Part 3" + "Part 4"

msg = "Part 1Part 2Part 3Part 4"
 ```

resulting in a total of 7 String instances:
```java
"Part1"

"Part2"

"Part 1Part 2"

"Part3"

"Part 1Part 2Part 3"

"Part4"

"Part 1Part 2Part 3Part 4"
```
Not very efficient.  And this isn't even taking into account other things that we might want to do, such as substrings, case changes, and so on.

To make it possibly to efficiently manipulate string data, Sun provided the StringBuffer class, which supports editing, thus cutting down on the need for intermediate strings.  And Sun dedicated entire sessions at early JavaOne conferences to pleading with developers to use StringBuffer.

Sun even modified the Java compiler to recognize certain use cases, such as the one shown above, and to automatically replace the code with the use of StringBuffer under the covers.

In fact, many language improvements over the years have been implemented, under the covers, with compiler tricks rather than true run-time changes, such as optimizing string manipulation, autoboxing, generics, inner classes, and lambdas.

However, although a vast improvement on using String to edit, StringBuffer is synchronized, which means that even single threaded use involves a not-insignificant amount of overhead.  So in Java 5, Sun introduced
 StringBuilder, which is exactly the same as StringBuffer, but without the synchronized keyword, and attendant overhead.  StringBuffer and StringBuilder share the bulk of their code by extending AbstractStringBuilder
.  Modern use should always use StringBuilder, unless you know that for some inexplicable reason, it will be shared across threads.

Review the Javadocs for [java.lang.String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html), [java.lang.StringBuffer](https://docs.oracle.com/javase/8/docs/api/java/lang/StringBuffer.html), and [java.lang.StringBuilder](https://docs.oracle.com/javase/8/docs/api/java/lang/StringBuilder.html).  If you are really curious, review the [source code](https://hg.openjdk.java.net/jdk8u/jdk8u/jdk/file/aba0b4743822/src/share/classes/java/lang).

All of these are available without importing them, because they are part of the java.lang package, which is implicitly available without importing.  We would only use import if we wanted to static import something like the format method from the String class.
