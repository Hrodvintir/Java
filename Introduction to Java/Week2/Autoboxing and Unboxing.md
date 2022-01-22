# Autoboxing and Unboxing

n the lesson, we discussed how for each primitive there is a matching Class.  Java 5 introduced autoboxing and unboxing, where the compiler lets us write code almost exclusively using primitives, and takes care of creating moving primitives into and out of objects where necessary.

For more details, read:

Java Tutorial: [Autoboxing and Unboxing](https://docs.oracle.com/javase/tutorial/java/data/autoboxing.html)

Java Documentation: [Autoboxing](https://docs.oracle.com/javase/8/docs/technotes/guides/language/autoboxing.html)

Remember: only Java primitives ultimately contain data in Java.  Objects act as containers for those primitives.  So write your code using primitives.  The few use cases were we need to use the Wrapper classes are when dealing with Collections and when using Generics (the subject of a later less).
