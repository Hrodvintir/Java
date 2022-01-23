# I installed my own Java, and it is later than version 8. Where did rt.jar go?

From the introduction of a ClassLoader capable of reading .,ZIP files until Java 9, the runtime classes were packaged in one or more .ZIP files in the java installation.  They might have been classes.zip, rt.jar, or other, but they were present.

Java 9 introduced a number of controversial changes, and this is one of them.  As per the [Oracle JDK Migration Guide](https://docs.oracle.com/en/java/javase/14/migrate/index.html#JSMIG-GUID-A78CC891-701D-4549-AA4E-B8DD90228B4B), "Class and resource files previously stored in lib/rt.jar, lib/tools.jar, lib/dt.jar and various other internal JAR files are stored in a more efficient format in implementation-specific files in the lib directory."

This leads, as the guide further states, to a number of issues.

This and related changes might be some of the reasons behind the expected longevity of Java 8 in the marketplace.
