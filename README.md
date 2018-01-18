# JVM Readings

WORK IN PROGRESS

A list of papers and blog posts essential to understanding how the JVM works, and building high performance applications on the JVM. The list is curated and maintained by Reynold Xin ([@rxin](https://twitter.com/rxin)). If you think a paper should be part of this list, please submit a pull request. It might take a while since I need to go over the material.

Also see my other reading list: [Readings in Databases](https://github.com/rxin/db-readings)


JVM Internals

http://blog.jamesdbloom.com/JVMInternals.html

GC

Understanding Garbage Collection
http://www.slideshare.net/dougqh/understanding-garbage-collection


JIT

JVM Mechanics: When Does the JVM JIT & Deoptimize?
http://www.slideshare.net/dougqh/jvm-mechanics-when-does-the


JITWatch

https://github.com/AdoptOpenJDK/jitwatch


JMH

JMH introduction
http://java-performance.info/jmh/

Sample JMH benchmark code (read through all of them)
http://hg.openjdk.java.net/code-tools/jmh/file/tip/jmh-samples/src/main/java/org/openjdk/jmh/samples/


Unsafe

http://mydailyjava.blogspot.com/2013/12/sunmiscunsafe.html


Method Dispatch

This is a good blog post about the cost of polymorphic dispatches. But more importantly, it is a good blog post to understand performance measurement methodology.

http://shipilev.net/blog/2015/black-magic-method-dispatch/


Safepoints

http://chriskirk.blogspot.com/2013/09/what-is-java-safepoint.html


Intrinsics

http://www.slideshare.net/RednaxelaFX/green-teajug-hotspotintrinsics02232013


Java Memory Model

- JMM fundamentals: Access atomicity, word tearing, Sequential Consistency, Synchronization Order, SO-PO/SO consistencies, Synchronizes-With Order, Happens-Before, Sequential Consistency - Data Race Free, "Roach Motel", Out of Thin Air values, Finals semantics, JMM9.
https://shipilev.net/blog/2014/jmm-pragmatics/

- JMM fundamentals follow up. Common misunderstandings, mistakes and misconceptions.
https://shipilev.net/blog/2016/close-encounters-of-jmm-kind/

- JMM in every day life. Combinations of Safe/Unsafe Publications & Safe/Unsafe Initializations. Singletons. Performance and memory costs.
https://shipilev.net/blog/2014/safe-public-construction/

- "The JSR-133 Cookbook for Compiler Writers" by Doug Lea. On Memory Barriers.
http://gee.cs.oswego.edu/dl/jmm/cookbook.html

- "The "Double-Checked Locking is Broken" Declaration" (before JSR133/JavaSE 5).
http://www.cs.umd.edu/~pugh/java/memoryModel/DoubleCheckedLocking.html

- "All Fields Are Final" experimental set up / analysys for final fields perfomance tests. Memory Barriers for final fields.
https://shipilev.net/blog/2014/all-fields-are-final/
