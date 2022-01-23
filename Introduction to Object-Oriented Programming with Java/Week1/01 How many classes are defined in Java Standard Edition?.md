# How many classes are defined in Java Standard Edition?

In the lesson, we discussed that solutions could be made of dozens or hundreds, or even thousands of classes.  A comment was made about the size of Java's own Standard Library.   This list shows the grown of the Standard Library over time:

Here are the counts, the Java versions and links to each version's class documentation.


4569 "https://docs.oracle.com/en/java/javase/14/docs/api/allclasses-index.html" java 14

4545 "https://docs.oracle.com/en/java/javase/13/docs/api/allclasses-index.html" java 13

4433 "https://docs.oracle.com/en/java/javase/12/docs/api/" java 12
 

4411 "https://docs.oracle.com/en/java/javase/11/docs/api/" java 11

6002 "http://docs.oracle.com/javase/10/docs/api/index.html?overview-summary.html" java 10

6005 "http://docs.oracle.com/javase/9/docs/api/index.html?overview-summary.html" java 9

4240 "http://docs.oracle.com/javase/8/docs/api/" java 8

4024 "http://docs.oracle.com/javase/7/docs/api/" java 7

3793 "http://docs.oracle.com/javase/6/docs/api/" java 6

3279 "http://docs.oracle.com/javase/1.5.0/docs/api/" java 5.0

2723 "http://docs.oracle.com/javase/1.4.2/docs/api/" java 1.4.2*

1840 "http://docs.oracle.com/javase/1.3/docs/api/" java 1.3.1*
 
 
 

* Javadocs prior to 5.0 are now offline.

It is not an accident that the class libraries for Java 11+ are smaller than Java 9 and Java 10.  Java 11 removed many classes that were no longer deemed necessary for "standard edition."  Much Java development has standardized on Java 8, and not moved on, even to the next Long Term Support release, Java 11.
