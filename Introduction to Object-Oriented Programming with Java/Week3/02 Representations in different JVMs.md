# Representations in different JVMs

The lecture refers to a "Reference Table", and provides a structure for it.  As explained in the video, that structure is merely one, hypothetical, way with which a JVM could be implemented.  [Section 2.7 Representation of Objects](https://docs.oracle.com/javase/specs/jvms/se7/html/jvms-2.html#jvms-2.7) of the Java Virtual Machine Specification says that "the Java Virtual Machine does not mandate any particular internal representation structure for objects."

The Hotspot JVM, originally from Sun and now one of the two choices when installing OpenJDK, has its way of doing it.  Others differ.  IBM's J9 JVM, which was open sourced as OpenJ9 via the Eclipse Foundation, is [well documented](https://eclipse.org/openj9/docs/), including documentation that can help one tune the runtime for real-world production loads.
