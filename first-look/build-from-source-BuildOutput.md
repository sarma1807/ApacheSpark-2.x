```
[cass@compile spark]$ build/mvn -DskipTests clean package

exec: curl --progress-bar -L https://downloads.typesafe.com/zinc/0.3.9/zinc-0.3.9.tgz
######################################################################## 100.0%
exec: curl --progress-bar -L https://downloads.typesafe.com/scala/2.11.8/scala-2.11.8.tgz
######################################################################## 100.0%
exec: curl --progress-bar -L https://www.apache.org/dyn/closer.lua?action=download&filename=/maven/maven-3/3.3.9/binaries/apache-maven-3.3.9-bin.tar.gz
######################################################################## 100.0%
Using `mvn` from path: /home/cass/spark2/spark/build/apache-maven-3.3.9/bin/mvn
Java HotSpot(TM) 64-Bit Server VM warning: ignoring option MaxPermSize=512M; support was removed in 8.0
[INFO] Scanning for projects...
[INFO] ------------------------------------------------------------------------
[INFO] Reactor Build Order:
[INFO]
[INFO] Spark Project Parent POM
[INFO] Spark Project Tags
[INFO] Spark Project Sketch
[INFO] Spark Project Networking
[INFO] Spark Project Shuffle Streaming Service
[INFO] Spark Project Unsafe
[INFO] Spark Project Launcher
[INFO] Spark Project Core
[INFO] Spark Project GraphX
[INFO] Spark Project Streaming
[INFO] Spark Project Catalyst
[INFO] Spark Project SQL
[INFO] Spark Project ML Local Library
[INFO] Spark Project ML Library
[INFO] Spark Project Tools
[INFO] Spark Project Hive
[INFO] Spark Project HiveContext Compatibility
[INFO] Spark Project REPL
[INFO] Spark Project Assembly
[INFO] Spark Project External Flume Sink
[INFO] Spark Project External Flume
[INFO] Spark Project External Flume Assembly
[INFO] Spark Integration for Kafka 0.8
[INFO] Spark Project Examples
[INFO] Spark Project External Kafka Assembly
[INFO] Spark Project Java 8 Tests
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Spark Project Parent POM 2.0.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.0.0:clean (default-clean) @ spark-parent_2.11 ---
[INFO]
[INFO] --- maven-enforcer-plugin:1.4.1:enforce (enforce-versions) @ spark-parent_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:add-source (eclipse-add-source) @ spark-parent_2.11 ---
[INFO] Add Source directory: /home/cass/spark2/spark/src/main/scala
[INFO] Add Test Source directory: /home/cass/spark2/spark/src/test/scala
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (default-cli) @ spark-parent_2.11 ---
[INFO] Dependencies classpath:
/home/cass/.m2/repository/org/spark-project/spark/unused/1.0.0/unused-1.0.0.jar
[INFO]
[INFO] --- maven-remote-resources-plugin:1.5:process (default) @ spark-parent_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:compile (scala-compile-first) @ spark-parent_2.11 ---
[INFO] No sources to compile
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (create-tmp-dir) @ spark-parent_2.11 ---
[INFO] Executing tasks

main:
    [mkdir] Created dir: /home/cass/spark2/spark/target/tmp
[INFO] Executed tasks
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:testCompile (scala-test-compile-first) @ spark-parent_2.11 ---
[INFO] No sources to compile
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (generate-test-classpath) @ spark-parent_2.11 ---
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (test) @ spark-parent_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- scalatest-maven-plugin:1.0:test (test) @ spark-parent_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (prepare-test-jar) @ spark-parent_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/target/spark-parent_2.11-2.0.0-SNAPSHOT-tests.jar
[INFO]
[INFO] --- maven-site-plugin:3.3:attach-descriptor (attach-descriptor) @ spark-parent_2.11 ---
[INFO]
[INFO] --- maven-shade-plugin:2.4.3:shade (default) @ spark-parent_2.11 ---
[INFO] Including org.spark-project.spark:unused:jar:1.0.0 in the shaded jar.
[INFO] Replacing original artifact with shaded artifact.
[INFO]
[INFO] --- maven-source-plugin:2.4:jar-no-fork (create-source-jar) @ spark-parent_2.11 ---
[INFO]
[INFO] --- maven-source-plugin:2.4:test-jar-no-fork (create-source-jar) @ spark-parent_2.11 ---
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Spark Project Tags 2.0.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.0.0:clean (default-clean) @ spark-tags_2.11 ---
[INFO]
[INFO] --- maven-enforcer-plugin:1.4.1:enforce (enforce-versions) @ spark-tags_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:add-source (eclipse-add-source) @ spark-tags_2.11 ---
[INFO] Add Source directory: /home/cass/spark2/spark/common/tags/src/main/scala
[INFO] Add Test Source directory: /home/cass/spark2/spark/common/tags/src/test/scala
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (default-cli) @ spark-tags_2.11 ---
[INFO] Dependencies classpath:
/home/cass/.m2/repository/org/scala-lang/modules/scala-xml_2.11/1.0.2/scala-xml_2.11-1.0.2.jar:/home/cass/.m2/repository/org/spark-project/spark/unused/1.0.0/unused-1.0.0.jar:/home/cass/.m2/repository/org/scalatest/scalatest_2.11/2.2.6/scalatest_2.11-2.2.6.jar:/home/cass/.m2/repository/org/scala-lang/scala-library/2.11.8/scala-library-2.11.8.jar:/home/cass/.m2/repository/org/scala-lang/scala-reflect/2.11.8/scala-reflect-2.11.8.jar
[INFO]
[INFO] --- maven-remote-resources-plugin:1.5:process (default) @ spark-tags_2.11 ---
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ spark-tags_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/common/tags/src/main/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:compile (scala-compile-first) @ spark-tags_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 2 Scala sources and 8 Java sources to /home/cass/spark2/spark/common/tags/target/scala-2.11/classes...
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] 1 warning
[info] Compile success at May 20, 2016 12:29:08 PM [6.704s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:compile (default-compile) @ spark-tags_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 8 source files to /home/cass/spark2/spark/common/tags/target/scala-2.11/classes
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (create-tmp-dir) @ spark-tags_2.11 ---
[INFO] Executing tasks

main:
    [mkdir] Created dir: /home/cass/spark2/spark/common/tags/target/tmp
[INFO] Executed tasks
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ spark-tags_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/common/tags/src/test/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:testCompile (scala-test-compile-first) @ spark-tags_2.11 ---
[INFO] No sources to compile
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:testCompile (default-testCompile) @ spark-tags_2.11 ---
[INFO] No sources to compile
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (generate-test-classpath) @ spark-tags_2.11 ---
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (default-test) @ spark-tags_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (test) @ spark-tags_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- scalatest-maven-plugin:1.0:test (test) @ spark-tags_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (prepare-test-jar) @ spark-tags_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT-tests.jar
[INFO]
[INFO] --- maven-jar-plugin:2.6:jar (default-jar) @ spark-tags_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-site-plugin:3.3:attach-descriptor (attach-descriptor) @ spark-tags_2.11 ---
[INFO]
[INFO] --- maven-shade-plugin:2.4.3:shade (default) @ spark-tags_2.11 ---
[INFO] Excluding org.scalatest:scalatest_2.11:jar:2.2.6 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-library:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-reflect:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-xml_2.11:jar:1.0.2 from the shaded jar.
[INFO] Including org.spark-project.spark:unused:jar:1.0.0 in the shaded jar.
[INFO] Replacing original artifact with shaded artifact.
[INFO] Replacing /home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT.jar with /home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT-shaded.jar
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/common/tags/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/common/tags/dependency-reduced-pom.xml
[INFO]
[INFO] --- maven-source-plugin:2.4:jar-no-fork (create-source-jar) @ spark-tags_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT-sources.jar
[INFO]
[INFO] --- maven-source-plugin:2.4:test-jar-no-fork (create-source-jar) @ spark-tags_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT-test-sources.jar
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Spark Project Sketch 2.0.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.0.0:clean (default-clean) @ spark-sketch_2.11 ---
[INFO]
[INFO] --- maven-enforcer-plugin:1.4.1:enforce (enforce-versions) @ spark-sketch_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:add-source (eclipse-add-source) @ spark-sketch_2.11 ---
[INFO] Add Source directory: /home/cass/spark2/spark/common/sketch/src/main/scala
[INFO] Add Test Source directory: /home/cass/spark2/spark/common/sketch/src/test/scala
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (default-cli) @ spark-sketch_2.11 ---
[INFO] Dependencies classpath:
/home/cass/.m2/repository/org/spark-project/spark/unused/1.0.0/unused-1.0.0.jar:/home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-remote-resources-plugin:1.5:process (default) @ spark-sketch_2.11 ---
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ spark-sketch_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/common/sketch/src/main/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:compile (scala-compile-first) @ spark-sketch_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 9 Java sources to /home/cass/spark2/spark/common/sketch/target/scala-2.11/classes...
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] 1 warning
[info] Compile success at May 20, 2016 12:29:11 PM [1.025s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:compile (default-compile) @ spark-sketch_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 9 source files to /home/cass/spark2/spark/common/sketch/target/scala-2.11/classes
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (create-tmp-dir) @ spark-sketch_2.11 ---
[INFO] Executing tasks

main:
    [mkdir] Created dir: /home/cass/spark2/spark/common/sketch/target/tmp
[INFO] Executed tasks
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ spark-sketch_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/common/sketch/src/test/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:testCompile (scala-test-compile-first) @ spark-sketch_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 3 Scala sources to /home/cass/spark2/spark/common/sketch/target/scala-2.11/test-classes...
[info] Compile success at May 20, 2016 12:29:15 PM [3.796s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:testCompile (default-testCompile) @ spark-sketch_2.11 ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (generate-test-classpath) @ spark-sketch_2.11 ---
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (default-test) @ spark-sketch_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (test) @ spark-sketch_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- scalatest-maven-plugin:1.0:test (test) @ spark-sketch_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (prepare-test-jar) @ spark-sketch_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/common/sketch/target/spark-sketch_2.11-2.0.0-SNAPSHOT-tests.jar
[INFO]
[INFO] --- maven-jar-plugin:2.6:jar (default-jar) @ spark-sketch_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/common/sketch/target/spark-sketch_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-site-plugin:3.3:attach-descriptor (attach-descriptor) @ spark-sketch_2.11 ---
[INFO]
[INFO] --- maven-shade-plugin:2.4.3:shade (default) @ spark-sketch_2.11 ---
[INFO] Excluding org.apache.spark:spark-tags_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Including org.spark-project.spark:unused:jar:1.0.0 in the shaded jar.
[INFO] Replacing original artifact with shaded artifact.
[INFO] Replacing /home/cass/spark2/spark/common/sketch/target/spark-sketch_2.11-2.0.0-SNAPSHOT.jar with /home/cass/spark2/spark/common/sketch/target/spark-sketch_2.11-2.0.0-SNAPSHOT-shaded.jar
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/common/sketch/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/common/sketch/dependency-reduced-pom.xml
[INFO]
[INFO] --- maven-source-plugin:2.4:jar-no-fork (create-source-jar) @ spark-sketch_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/common/sketch/target/spark-sketch_2.11-2.0.0-SNAPSHOT-sources.jar
[INFO]
[INFO] --- maven-source-plugin:2.4:test-jar-no-fork (create-source-jar) @ spark-sketch_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/common/sketch/target/spark-sketch_2.11-2.0.0-SNAPSHOT-test-sources.jar
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Spark Project Networking 2.0.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.0.0:clean (default-clean) @ spark-network-common_2.11 ---
[INFO]
[INFO] --- maven-enforcer-plugin:1.4.1:enforce (enforce-versions) @ spark-network-common_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:add-source (eclipse-add-source) @ spark-network-common_2.11 ---
[INFO] Add Source directory: /home/cass/spark2/spark/common/network-common/src/main/scala
[INFO] Add Test Source directory: /home/cass/spark2/spark/common/network-common/src/test/scala
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (default-cli) @ spark-network-common_2.11 ---
[INFO] Dependencies classpath:
/home/cass/.m2/repository/org/spark-project/spark/unused/1.0.0/unused-1.0.0.jar:/home/cass/.m2/repository/com/google/code/findbugs/jsr305/1.3.9/jsr305-1.3.9.jar:/home/cass/.m2/repository/org/apache/commons/commons-lang3/3.3.2/commons-lang3-3.3.2.jar:/home/cass/.m2/repository/io/netty/netty-all/4.0.29.Final/netty-all-4.0.29.Final.jar:/home/cass/.m2/repository/com/google/guava/guava/14.0.1/guava-14.0.1.jar:/home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-remote-resources-plugin:1.5:process (default) @ spark-network-common_2.11 ---
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ spark-network-common_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/common/network-common/src/main/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:compile (scala-compile-first) @ spark-network-common_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 64 Java sources to /home/cass/spark2/spark/common/network-common/target/scala-2.11/classes...
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] 1 warning
[info] Compile success at May 20, 2016 12:29:18 PM [2.214s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:compile (default-compile) @ spark-network-common_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 64 source files to /home/cass/spark2/spark/common/network-common/target/scala-2.11/classes
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (create-tmp-dir) @ spark-network-common_2.11 ---
[INFO] Executing tasks

main:
    [mkdir] Created dir: /home/cass/spark2/spark/common/network-common/target/tmp
[INFO] Executed tasks
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ spark-network-common_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 1 resource
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:testCompile (scala-test-compile-first) @ spark-network-common_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 13 Java sources to /home/cass/spark2/spark/common/network-common/target/scala-2.11/test-classes...
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] 1 warning
[info] Compile success at May 20, 2016 12:29:21 PM [1.407s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:testCompile (default-testCompile) @ spark-network-common_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 13 source files to /home/cass/spark2/spark/common/network-common/target/scala-2.11/test-classes
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (generate-test-classpath) @ spark-network-common_2.11 ---
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (test-jar-on-test-compile) @ spark-network-common_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/common/network-common/target/spark-network-common_2.11-2.0.0-SNAPSHOT-tests.jar
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (default-test) @ spark-network-common_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (test) @ spark-network-common_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- scalatest-maven-plugin:1.0:test (test) @ spark-network-common_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (prepare-test-jar) @ spark-network-common_2.11 ---
[INFO]
[INFO] --- maven-jar-plugin:2.6:jar (default-jar) @ spark-network-common_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/common/network-common/target/spark-network-common_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-site-plugin:3.3:attach-descriptor (attach-descriptor) @ spark-network-common_2.11 ---
[INFO]
[INFO] --- maven-shade-plugin:2.4.3:shade (default) @ spark-network-common_2.11 ---
[INFO] Excluding io.netty:netty-all:jar:4.0.29.Final from the shaded jar.
[INFO] Excluding org.apache.commons:commons-lang3:jar:3.3.2 from the shaded jar.
[INFO] Excluding com.google.code.findbugs:jsr305:jar:1.3.9 from the shaded jar.
[INFO] Including com.google.guava:guava:jar:14.0.1 in the shaded jar.
[INFO] Excluding org.apache.spark:spark-tags_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Including org.spark-project.spark:unused:jar:1.0.0 in the shaded jar.
[INFO] Replacing original artifact with shaded artifact.
[INFO] Replacing /home/cass/spark2/spark/common/network-common/target/spark-network-common_2.11-2.0.0-SNAPSHOT.jar with /home/cass/spark2/spark/common/network-common/target/spark-network-common_2.11-2.0.0-SNAPSHOT-shaded.jar
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/common/network-common/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/common/network-common/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/common/network-common/dependency-reduced-pom.xml
[INFO]
[INFO] --- maven-source-plugin:2.4:jar-no-fork (create-source-jar) @ spark-network-common_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/common/network-common/target/spark-network-common_2.11-2.0.0-SNAPSHOT-sources.jar
[INFO]
[INFO] --- maven-source-plugin:2.4:test-jar-no-fork (create-source-jar) @ spark-network-common_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/common/network-common/target/spark-network-common_2.11-2.0.0-SNAPSHOT-test-sources.jar
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Spark Project Shuffle Streaming Service 2.0.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.0.0:clean (default-clean) @ spark-network-shuffle_2.11 ---
[INFO]
[INFO] --- maven-enforcer-plugin:1.4.1:enforce (enforce-versions) @ spark-network-shuffle_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:add-source (eclipse-add-source) @ spark-network-shuffle_2.11 ---
[INFO] Add Source directory: /home/cass/spark2/spark/common/network-shuffle/src/main/scala
[INFO] Add Test Source directory: /home/cass/spark2/spark/common/network-shuffle/src/test/scala
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (default-cli) @ spark-network-shuffle_2.11 ---
[INFO] Dependencies classpath:
/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-core/2.5.3/jackson-core-2.5.3.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-annotations/2.5.3/jackson-annotations-2.5.3.jar:/home/cass/.m2/repository/org/spark-project/spark/unused/1.0.0/unused-1.0.0.jar:/home/cass/.m2/repository/com/google/code/findbugs/jsr305/1.3.9/jsr305-1.3.9.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-databind/2.5.3/jackson-databind-2.5.3.jar:/home/cass/.m2/repository/org/apache/commons/commons-lang3/3.3.2/commons-lang3-3.3.2.jar:/home/cass/.m2/repository/org/fusesource/leveldbjni/leveldbjni-all/1.8/leveldbjni-all-1.8.jar:/home/cass/spark2/spark/common/network-common/target/spark-network-common_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/io/netty/netty-all/4.0.29.Final/netty-all-4.0.29.Final.jar:/home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-remote-resources-plugin:1.5:process (default) @ spark-network-shuffle_2.11 ---
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ spark-network-shuffle_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/common/network-shuffle/src/main/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:compile (scala-compile-first) @ spark-network-shuffle_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 17 Java sources to /home/cass/spark2/spark/common/network-shuffle/target/scala-2.11/classes...
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] 1 warning
[info] Compile success at May 20, 2016 12:29:25 PM [1.396s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:compile (default-compile) @ spark-network-shuffle_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 17 source files to /home/cass/spark2/spark/common/network-shuffle/target/scala-2.11/classes
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (create-tmp-dir) @ spark-network-shuffle_2.11 ---
[INFO] Executing tasks

main:
    [mkdir] Created dir: /home/cass/spark2/spark/common/network-shuffle/target/tmp
[INFO] Executed tasks
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ spark-network-shuffle_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/common/network-shuffle/src/test/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:testCompile (scala-test-compile-first) @ spark-network-shuffle_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 10 Java sources to /home/cass/spark2/spark/common/network-shuffle/target/scala-2.11/test-classes...
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] 1 warning
[info] Compile success at May 20, 2016 12:29:27 PM [1.112s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:testCompile (default-testCompile) @ spark-network-shuffle_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 10 source files to /home/cass/spark2/spark/common/network-shuffle/target/scala-2.11/test-classes
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (generate-test-classpath) @ spark-network-shuffle_2.11 ---
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (default-test) @ spark-network-shuffle_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (test) @ spark-network-shuffle_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- scalatest-maven-plugin:1.0:test (test) @ spark-network-shuffle_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (prepare-test-jar) @ spark-network-shuffle_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/common/network-shuffle/target/spark-network-shuffle_2.11-2.0.0-SNAPSHOT-tests.jar
[INFO]
[INFO] --- maven-jar-plugin:2.6:jar (default-jar) @ spark-network-shuffle_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/common/network-shuffle/target/spark-network-shuffle_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-site-plugin:3.3:attach-descriptor (attach-descriptor) @ spark-network-shuffle_2.11 ---
[INFO]
[INFO] --- maven-shade-plugin:2.4.3:shade (default) @ spark-network-shuffle_2.11 ---
[INFO] Excluding org.apache.spark:spark-network-common_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding io.netty:netty-all:jar:4.0.29.Final from the shaded jar.
[INFO] Excluding org.apache.commons:commons-lang3:jar:3.3.2 from the shaded jar.
[INFO] Excluding com.google.code.findbugs:jsr305:jar:1.3.9 from the shaded jar.
[INFO] Excluding org.fusesource.leveldbjni:leveldbjni-all:jar:1.8 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-databind:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-core:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-annotations:jar:2.5.3 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-tags_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Including org.spark-project.spark:unused:jar:1.0.0 in the shaded jar.
[INFO] Replacing original artifact with shaded artifact.
[INFO] Replacing /home/cass/spark2/spark/common/network-shuffle/target/spark-network-shuffle_2.11-2.0.0-SNAPSHOT.jar with /home/cass/spark2/spark/common/network-shuffle/target/spark-network-shuffle_2.11-2.0.0-SNAPSHOT-shaded.jar
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/common/network-shuffle/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/common/network-shuffle/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/common/network-shuffle/dependency-reduced-pom.xml
[INFO]
[INFO] --- maven-source-plugin:2.4:jar-no-fork (create-source-jar) @ spark-network-shuffle_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/common/network-shuffle/target/spark-network-shuffle_2.11-2.0.0-SNAPSHOT-sources.jar
[INFO]
[INFO] --- maven-source-plugin:2.4:test-jar-no-fork (create-source-jar) @ spark-network-shuffle_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/common/network-shuffle/target/spark-network-shuffle_2.11-2.0.0-SNAPSHOT-test-sources.jar
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Spark Project Unsafe 2.0.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.0.0:clean (default-clean) @ spark-unsafe_2.11 ---
[INFO]
[INFO] --- maven-enforcer-plugin:1.4.1:enforce (enforce-versions) @ spark-unsafe_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:add-source (eclipse-add-source) @ spark-unsafe_2.11 ---
[INFO] Add Source directory: /home/cass/spark2/spark/common/unsafe/src/main/scala
[INFO] Add Test Source directory: /home/cass/spark2/spark/common/unsafe/src/test/scala
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (default-cli) @ spark-unsafe_2.11 ---
[INFO] Dependencies classpath:
/home/cass/.m2/repository/com/twitter/chill-java/0.8.0/chill-java-0.8.0.jar:/home/cass/.m2/repository/com/esotericsoftware/minlog/1.3.0/minlog-1.3.0.jar:/home/cass/.m2/repository/org/spark-project/spark/unused/1.0.0/unused-1.0.0.jar:/home/cass/.m2/repository/com/google/code/findbugs/jsr305/1.3.9/jsr305-1.3.9.jar:/home/cass/.m2/repository/org/scala-lang/scala-library/2.11.8/scala-library-2.11.8.jar:/home/cass/.m2/repository/com/esotericsoftware/kryo-shaded/3.0.3/kryo-shaded-3.0.3.jar:/home/cass/.m2/repository/com/twitter/chill_2.11/0.8.0/chill_2.11-0.8.0.jar:/home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/objenesis/objenesis/2.1/objenesis-2.1.jar
[INFO]
[INFO] --- maven-remote-resources-plugin:1.5:process (default) @ spark-unsafe_2.11 ---
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ spark-unsafe_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/common/unsafe/src/main/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:compile (scala-compile-first) @ spark-unsafe_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 14 Java sources to /home/cass/spark2/spark/common/unsafe/target/scala-2.11/classes...
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] /home/cass/spark2/spark/common/unsafe/src/main/java/org/apache/spark/unsafe/Platform.java:158: warning: [rawtypes] found raw type: Class
[warn]       Class cls = Class.forName("java.nio.DirectByteBuffer");
[warn]       ^
[warn]   missing type arguments for generic class Class<T>
[warn]   where T is a type-variable:
[warn]     T extends Object declared in class Class
[warn] /home/cass/spark2/spark/common/unsafe/src/main/java/org/apache/spark/unsafe/Platform.java:159: warning: [rawtypes] found raw type: Constructor
[warn]       Constructor constructor = cls.getDeclaredConstructor(Long.TYPE, Integer.TYPE);
[warn]       ^
[warn]   missing type arguments for generic class Constructor<T>
[warn]   where T is a type-variable:
[warn]     T extends Object declared in class Constructor
[warn] 3 warnings
[info] Compile success at May 20, 2016 12:29:30 PM [1.198s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:compile (default-compile) @ spark-unsafe_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 14 source files to /home/cass/spark2/spark/common/unsafe/target/scala-2.11/classes
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (create-tmp-dir) @ spark-unsafe_2.11 ---
[INFO] Executing tasks

main:
    [mkdir] Created dir: /home/cass/spark2/spark/common/unsafe/target/tmp
[INFO] Executed tasks
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ spark-unsafe_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/common/unsafe/src/test/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:testCompile (scala-test-compile-first) @ spark-unsafe_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 1 Scala source and 5 Java sources to /home/cass/spark2/spark/common/unsafe/target/scala-2.11/test-classes...
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] 1 warning
[info] Compile success at May 20, 2016 12:29:35 PM [4.087s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:testCompile (default-testCompile) @ spark-unsafe_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 5 source files to /home/cass/spark2/spark/common/unsafe/target/scala-2.11/test-classes
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (generate-test-classpath) @ spark-unsafe_2.11 ---
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (default-test) @ spark-unsafe_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (test) @ spark-unsafe_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- scalatest-maven-plugin:1.0:test (test) @ spark-unsafe_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (prepare-test-jar) @ spark-unsafe_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/common/unsafe/target/spark-unsafe_2.11-2.0.0-SNAPSHOT-tests.jar
[INFO]
[INFO] --- maven-jar-plugin:2.6:jar (default-jar) @ spark-unsafe_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/common/unsafe/target/spark-unsafe_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-site-plugin:3.3:attach-descriptor (attach-descriptor) @ spark-unsafe_2.11 ---
[INFO]
[INFO] --- maven-shade-plugin:2.4.3:shade (default) @ spark-unsafe_2.11 ---
[INFO] Excluding org.apache.spark:spark-tags_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding com.twitter:chill_2.11:jar:0.8.0 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-library:jar:2.11.8 from the shaded jar.
[INFO] Excluding com.twitter:chill-java:jar:0.8.0 from the shaded jar.
[INFO] Excluding com.esotericsoftware:kryo-shaded:jar:3.0.3 from the shaded jar.
[INFO] Excluding com.esotericsoftware:minlog:jar:1.3.0 from the shaded jar.
[INFO] Excluding com.google.code.findbugs:jsr305:jar:1.3.9 from the shaded jar.
[INFO] Excluding org.objenesis:objenesis:jar:2.1 from the shaded jar.
[INFO] Including org.spark-project.spark:unused:jar:1.0.0 in the shaded jar.
[INFO] Replacing original artifact with shaded artifact.
[INFO] Replacing /home/cass/spark2/spark/common/unsafe/target/spark-unsafe_2.11-2.0.0-SNAPSHOT.jar with /home/cass/spark2/spark/common/unsafe/target/spark-unsafe_2.11-2.0.0-SNAPSHOT-shaded.jar
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/common/unsafe/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/common/unsafe/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/common/unsafe/dependency-reduced-pom.xml
[INFO]
[INFO] --- maven-source-plugin:2.4:jar-no-fork (create-source-jar) @ spark-unsafe_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/common/unsafe/target/spark-unsafe_2.11-2.0.0-SNAPSHOT-sources.jar
[INFO]
[INFO] --- maven-source-plugin:2.4:test-jar-no-fork (create-source-jar) @ spark-unsafe_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/common/unsafe/target/spark-unsafe_2.11-2.0.0-SNAPSHOT-test-sources.jar
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Spark Project Launcher 2.0.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.0.0:clean (default-clean) @ spark-launcher_2.11 ---
[INFO]
[INFO] --- maven-enforcer-plugin:1.4.1:enforce (enforce-versions) @ spark-launcher_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:add-source (eclipse-add-source) @ spark-launcher_2.11 ---
[INFO] Add Source directory: /home/cass/spark2/spark/launcher/src/main/scala
[INFO] Add Test Source directory: /home/cass/spark2/spark/launcher/src/test/scala
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (default-cli) @ spark-launcher_2.11 ---
[INFO] Dependencies classpath:
/home/cass/.m2/repository/javax/inject/javax.inject/1/javax.inject-1.jar:/home/cass/.m2/repository/org/spark-project/spark/unused/1.0.0/unused-1.0.0.jar:/home/cass/.m2/repository/com/google/inject/guice/3.0/guice-3.0.jar:/home/cass/.m2/repository/commons-io/commons-io/2.4/commons-io-2.4.jar:/home/cass/.m2/repository/com/google/protobuf/protobuf-java/2.5.0/protobuf-java-2.5.0.jar:/home/cass/.m2/repository/aopalliance/aopalliance/1.0/aopalliance-1.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-api/2.2.0/hadoop-yarn-api-2.2.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-common/2.2.0/hadoop-yarn-common-2.2.0.jar:/home/cass/.m2/repository/org/apache/avro/avro/1.7.7/avro-1.7.7.jar:/home/cass/.m2/repository/org/xerial/snappy/snappy-java/1.1.2.4/snappy-java-1.1.2.4.jar:/home/cass/.m2/repository/org/apache/commons/commons-compress/1.4.1/commons-compress-1.4.1.jar:/home/cass/.m2/repository/org/apache/zookeeper/zookeeper/3.4.5/zookeeper-3.4.5.jar:/home/cass/.m2/repository/com/thoughtworks/paranamer/paranamer/2.3/paranamer-2.3.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-core-asl/1.9.13/jackson-core-asl-1.9.13.jar:/home/cass/.m2/repository/org/tukaani/xz/1.0/xz-1.0.jar:/home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-client/2.2.0/hadoop-yarn-client-2.2.0.jar
[INFO]
[INFO] --- maven-remote-resources-plugin:1.5:process (default) @ spark-launcher_2.11 ---
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ spark-launcher_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/launcher/src/main/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:compile (scala-compile-first) @ spark-launcher_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 15 Java sources to /home/cass/spark2/spark/launcher/target/scala-2.11/classes...
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] 1 warning
[info] Compile success at May 20, 2016 12:29:39 PM [1.307s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:compile (default-compile) @ spark-launcher_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 15 source files to /home/cass/spark2/spark/launcher/target/scala-2.11/classes
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (create-tmp-dir) @ spark-launcher_2.11 ---
[INFO] Executing tasks

main:
    [mkdir] Created dir: /home/cass/spark2/spark/launcher/target/tmp
[INFO] Executed tasks
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ spark-launcher_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 2 resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:testCompile (scala-test-compile-first) @ spark-launcher_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 5 Java sources to /home/cass/spark2/spark/launcher/target/scala-2.11/test-classes...
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] 1 warning
[info] Compile success at May 20, 2016 12:29:42 PM [1.174s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:testCompile (default-testCompile) @ spark-launcher_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 5 source files to /home/cass/spark2/spark/launcher/target/scala-2.11/test-classes
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (generate-test-classpath) @ spark-launcher_2.11 ---
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (default-test) @ spark-launcher_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (test) @ spark-launcher_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- scalatest-maven-plugin:1.0:test (test) @ spark-launcher_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (prepare-test-jar) @ spark-launcher_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/launcher/target/spark-launcher_2.11-2.0.0-SNAPSHOT-tests.jar
[INFO]
[INFO] --- maven-jar-plugin:2.6:jar (default-jar) @ spark-launcher_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/launcher/target/spark-launcher_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-site-plugin:3.3:attach-descriptor (attach-descriptor) @ spark-launcher_2.11 ---
[INFO]
[INFO] --- maven-shade-plugin:2.4.3:shade (default) @ spark-launcher_2.11 ---
[INFO] Excluding org.apache.spark:spark-tags_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding commons-io:commons-io:jar:2.4 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-core-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding org.apache.avro:avro:jar:1.7.7 from the shaded jar.
[INFO] Excluding com.thoughtworks.paranamer:paranamer:jar:2.3 from the shaded jar.
[INFO] Excluding org.xerial.snappy:snappy-java:jar:1.1.2.4 from the shaded jar.
[INFO] Excluding com.google.protobuf:protobuf-java:jar:2.5.0 from the shaded jar.
[INFO] Excluding org.apache.zookeeper:zookeeper:jar:3.4.5 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-compress:jar:1.4.1 from the shaded jar.
[INFO] Excluding org.tukaani:xz:jar:1.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding com.google.inject:guice:jar:3.0 from the shaded jar.
[INFO] Excluding javax.inject:javax.inject:jar:1 from the shaded jar.
[INFO] Excluding aopalliance:aopalliance:jar:1.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-api:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-common:jar:2.2.0 from the shaded jar.
[INFO] Including org.spark-project.spark:unused:jar:1.0.0 in the shaded jar.
[INFO] Replacing original artifact with shaded artifact.
[INFO] Replacing /home/cass/spark2/spark/launcher/target/spark-launcher_2.11-2.0.0-SNAPSHOT.jar with /home/cass/spark2/spark/launcher/target/spark-launcher_2.11-2.0.0-SNAPSHOT-shaded.jar
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/launcher/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/launcher/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/launcher/dependency-reduced-pom.xml
[INFO]
[INFO] --- maven-source-plugin:2.4:jar-no-fork (create-source-jar) @ spark-launcher_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/launcher/target/spark-launcher_2.11-2.0.0-SNAPSHOT-sources.jar
[INFO]
[INFO] --- maven-source-plugin:2.4:test-jar-no-fork (create-source-jar) @ spark-launcher_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/launcher/target/spark-launcher_2.11-2.0.0-SNAPSHOT-test-sources.jar
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Spark Project Core 2.0.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.0.0:clean (default-clean) @ spark-core_2.11 ---
[INFO]
[INFO] --- maven-enforcer-plugin:1.4.1:enforce (enforce-versions) @ spark-core_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:add-source (eclipse-add-source) @ spark-core_2.11 ---
[INFO] Add Source directory: /home/cass/spark2/spark/core/src/main/scala
[INFO] Add Test Source directory: /home/cass/spark2/spark/core/src/test/scala
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (default-cli) @ spark-core_2.11 ---
[INFO] Dependencies classpath:
/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-jobclient/2.2.0/hadoop-mapreduce-client-jobclient-2.2.0.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-core/3.1.2/metrics-core-3.1.2.jar:/home/cass/.m2/repository/com/google/protobuf/protobuf-java/2.5.0/protobuf-java-2.5.0.jar:/home/cass/.m2/repository/aopalliance/aopalliance/1.0/aopalliance-1.0.jar:/home/cass/.m2/repository/net/razorvine/pyrolite/4.9/pyrolite-4.9.jar:/home/cass/.m2/repository/org/eclipse/jetty/jetty-servlet/9.2.16.v20160414/jetty-servlet-9.2.16.v20160414.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-jvm/3.1.2/metrics-jvm-3.1.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-client/2.2.0/hadoop-client-2.2.0.jar:/home/cass/.m2/repository/org/fusesource/leveldbjni/leveldbjni-all/1.8/leveldbjni-all-1.8.jar:/home/cass/.m2/repository/org/apache/commons/commons-math/2.2/commons-math-2.2.jar:/home/cass/.m2/repository/org/glassfish/jersey/bundles/repackaged/jersey-guava/2.22.2/jersey-guava-2.22.2.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-json/3.1.2/metrics-json-3.1.2.jar:/home/cass/.m2/repository/net/java/dev/jets3t/jets3t/0.7.1/jets3t-0.7.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-common/2.2.0/hadoop-common-2.2.0.jar:/home/cass/.m2/repository/com/google/inject/guice/3.0/guice-3.0.jar:/home/cass/.m2/repository/commons-io/commons-io/2.4/commons-io-2.4.jar:/home/cass/.m2/repository/org/scala-lang/scala-reflect/2.11.8/scala-reflect-2.11.8.jar:/home/cass/.m2/repository/org/xerial/snappy/snappy-java/1.1.2.4/snappy-java-1.1.2.4.jar:/home/cass/.m2/repository/org/json4s/json4s-jackson_2.11/3.2.11/json4s-jackson_2.11-3.2.11.jar:/home/cass/.m2/repository/com/esotericsoftware/minlog/1.3.0/minlog-1.3.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-auth/2.2.0/hadoop-auth-2.2.0.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-core-asl/1.9.13/jackson-core-asl-1.9.13.jar:/home/cass/.m2/repository/javax/validation/validation-api/1.1.0.Final/validation-api-1.1.0.Final.jar:/home/cass/.m2/repository/org/eclipse/jetty/jetty-security/9.2.16.v20160414/jetty-security-9.2.16.v20160414.jar:/home/cass/.m2/repository/net/jpountz/lz4/lz4/1.3.0/lz4-1.3.0.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-common/2.22.2/jersey-common-2.22.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-client/2.2.0/hadoop-yarn-client-2.2.0.jar:/home/cass/.m2/repository/org/eclipse/jetty/jetty-xml/9.2.16.v20160414/jetty-xml-9.2.16.v20160414.jar:/home/cass/.m2/repository/io/netty/netty/3.8.0.Final/netty-3.8.0.Final.jar:/home/cass/.m2/repository/org/eclipse/jetty/jetty-io/9.2.16.v20160414/jetty-io-9.2.16.v20160414.jar:/home/cass/.m2/repository/org/apache/mesos/mesos/0.21.1/mesos-0.21.1-shaded-protobuf.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-annotations/2.5.3/jackson-annotations-2.5.3.jar:/home/cass/.m2/repository/com/google/code/findbugs/jsr305/1.3.9/jsr305-1.3.9.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-api/2.4.0-b34/hk2-api-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-server/2.22.2/jersey-server-2.22.2.jar:/home/cass/.m2/repository/net/sf/py4j/py4j/0.10.1/py4j-0.10.1.jar:/home/cass/.m2/repository/com/twitter/chill-java/0.8.0/chill-java-0.8.0.jar:/home/cass/.m2/repository/commons-lang/commons-lang/2.6/commons-lang-2.6.jar:/home/cass/.m2/repository/org/tukaani/xz/1.0/xz-1.0.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-databind/2.5.3/jackson-databind-2.5.3.jar:/home/cass/.m2/repository/commons-codec/commons-codec/1.10/commons-codec-1.10.jar:/home/cass/.m2/repository/org/apache/curator/curator-recipes/2.4.0/curator-recipes-2.4.0.jar:/home/cass/.m2/repository/org/eclipse/jetty/jetty-util/9.2.16.v20160414/jetty-util-9.2.16.v20160414.jar:/home/cass/.m2/repository/org/apache/ivy/ivy/2.4.0/ivy-2.4.0.jar:/home/cass/.m2/repository/javax/inject/javax.inject/1/javax.inject-1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-core/2.2.0/hadoop-mapreduce-client-core-2.2.0.jar:/home/cass/.m2/repository/com/fasterxml/jackson/module/jackson-module-scala_2.11/2.5.3/jackson-module-scala_2.11-2.5.3.jar:/home/cass/.m2/repository/org/javassist/javassist/3.15.0-GA/javassist-3.15.0-GA.jar:/home/cass/.m2/repository/commons-beanutils/commons-beanutils-core/1.8.0/commons-beanutils-core-1.8.0.jar:/home/cass/.m2/repository/javax/servlet/javax.servlet-api/3.1.0/javax.servlet-api-3.1.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/osgi-resource-locator/1.0.1/osgi-resource-locator-1.0.1.jar:/home/cass/.m2/repository/org/apache/commons/commons-math3/3.4.1/commons-math3-3.4.1.jar:/home/cass/spark2/spark/common/network-common/target/spark-network-common_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/avro/avro/1.7.7/avro-1.7.7.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-common/2.2.0/hadoop-mapreduce-client-common-2.2.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-utils/2.4.0-b34/hk2-utils-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/hk2/external/aopalliance-repackaged/2.4.0-b34/aopalliance-repackaged-2.4.0-b34.jar:/home/cass/.m2/repository/org/eclipse/jetty/jetty-server/9.2.16.v20160414/jetty-server-9.2.16.v20160414.jar:/home/cass/.m2/repository/org/glassfish/hk2/external/javax.inject/2.4.0-b34/javax.inject-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/jersey/containers/jersey-container-servlet-core/2.22.2/jersey-container-servlet-core-2.22.2.jar:/home/cass/.m2/repository/org/eclipse/jetty/jetty-continuation/9.2.16.v20160414/jetty-continuation-9.2.16.v20160414.jar:/home/cass/.m2/repository/oro/oro/2.0.8/oro-2.0.8.jar:/home/cass/.m2/repository/org/scala-lang/scala-compiler/2.11.8/scala-compiler-2.11.8.jar:/home/cass/.m2/repository/org/roaringbitmap/RoaringBitmap/0.5.11/RoaringBitmap-0.5.11.jar:/home/cass/.m2/repository/log4j/log4j/1.2.17/log4j-1.2.17.jar:/home/cass/.m2/repository/org/scala-lang/scala-library/2.11.8/scala-library-2.11.8.jar:/home/cass/.m2/repository/org/apache/curator/curator-client/2.4.0/curator-client-2.4.0.jar:/home/cass/.m2/repository/org/eclipse/jetty/jetty-jndi/9.2.16.v20160414/jetty-jndi-9.2.16.v20160414.jar:/home/cass/.m2/repository/org/apache/commons/commons-compress/1.4.1/commons-compress-1.4.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-app/2.2.0/hadoop-mapreduce-client-app-2.2.0.jar:/home/cass/.m2/repository/org/slf4j/slf4j-api/1.7.16/slf4j-api-1.7.16.jar:/home/cass/.m2/repository/org/apache/xbean/xbean-asm5-shaded/4.4/xbean-asm5-shaded-4.4.jar:/home/cass/.m2/repository/org/eclipse/jetty/jetty-webapp/9.2.16.v20160414/jetty-webapp-9.2.16.v20160414.jar:/home/cass/.m2/repository/org/json4s/json4s-core_2.11/3.2.11/json4s-core_2.11-3.2.11.jar:/home/cass/.m2/repository/org/mortbay/jetty/jetty-util/6.1.26/jetty-util-6.1.26.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-server-common/2.2.0/hadoop-yarn-server-common-2.2.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-hdfs/2.2.0/hadoop-hdfs-2.2.0.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-mapper-asl/1.9.13/jackson-mapper-asl-1.9.13.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-api/2.2.0/hadoop-yarn-api-2.2.0.jar:/home/cass/.m2/repository/com/esotericsoftware/kryo-shaded/3.0.3/kryo-shaded-3.0.3.jar:/home/cass/.m2/repository/javax/ws/rs/javax.ws.rs-api/2.0.1/javax.ws.rs-api-2.0.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-common/2.2.0/hadoop-yarn-common-2.2.0.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-client/2.22.2/jersey-client-2.22.2.jar:/home/cass/spark2/spark/common/unsafe/target/spark-unsafe_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/avro/avro-mapred/1.7.7/avro-mapred-1.7.7-hadoop2.jar:/home/cass/.m2/repository/xmlenc/xmlenc/0.52/xmlenc-0.52.jar:/home/cass/.m2/repository/com/ning/compress-lzf/1.0.3/compress-lzf-1.0.3.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-shuffle/2.2.0/hadoop-mapreduce-client-shuffle-2.2.0.jar:/home/cass/.m2/repository/org/apache/zookeeper/zookeeper/3.4.5/zookeeper-3.4.5.jar:/home/cass/.m2/repository/org/apache/curator/curator-framework/2.4.0/curator-framework-2.4.0.jar:/home/cass/.m2/repository/commons-net/commons-net/2.2/commons-net-2.2.jar:/home/cass/.m2/repository/org/apache/commons/commons-lang3/3.3.2/commons-lang3-3.3.2.jar:/home/cass/.m2/repository/org/json4s/json4s-ast_2.11/3.2.11/json4s-ast_2.11-3.2.11.jar:/home/cass/spark2/spark/launcher/target/spark-launcher_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/scala-lang/scalap/2.11.8/scalap-2.11.8.jar:/home/cass/.m2/repository/com/clearspring/analytics/stream/2.7.0/stream-2.7.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-annotations/2.2.0/hadoop-annotations-2.2.0.jar:/home/cass/.m2/repository/com/thoughtworks/paranamer/paranamer/2.6/paranamer-2.6.jar:/home/cass/.m2/repository/commons-configuration/commons-configuration/1.6/commons-configuration-1.6.jar:/home/cass/.m2/repository/org/glassfish/jersey/containers/jersey-container-servlet/2.22.2/jersey-container-servlet-2.22.2.jar:/home/cass/.m2/repository/commons-digester/commons-digester/1.8/commons-digester-1.8.jar:/home/cass/.m2/repository/org/slf4j/jul-to-slf4j/1.7.16/jul-to-slf4j-1.7.16.jar:/home/cass/.m2/repository/commons-beanutils/commons-beanutils/1.7.0/commons-beanutils-1.7.0.jar:/home/cass/spark2/spark/common/network-shuffle/target/spark-network-shuffle_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-xml_2.11/1.0.2/scala-xml_2.11-1.0.2.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-parser-combinators_2.11/1.0.4/scala-parser-combinators_2.11-1.0.4.jar:/home/cass/.m2/repository/commons-cli/commons-cli/1.2/commons-cli-1.2.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-graphite/3.1.2/metrics-graphite-3.1.2.jar:/home/cass/.m2/repository/javax/annotation/javax.annotation-api/1.2/javax.annotation-api-1.2.jar:/home/cass/.m2/repository/org/objenesis/objenesis/2.1/objenesis-2.1.jar:/home/cass/.m2/repository/org/slf4j/slf4j-log4j12/1.7.16/slf4j-log4j12-1.7.16.jar:/home/cass/.m2/repository/org/eclipse/jetty/jetty-plus/9.2.16.v20160414/jetty-plus-9.2.16.v20160414.jar:/home/cass/.m2/repository/org/eclipse/jetty/jetty-servlets/9.2.16.v20160414/jetty-servlets-9.2.16.v20160414.jar:/home/cass/.m2/repository/org/glassfish/jersey/media/jersey-media-jaxb/2.22.2/jersey-media-jaxb-2.22.2.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-core/2.5.3/jackson-core-2.5.3.jar:/home/cass/.m2/repository/org/spark-project/spark/unused/1.0.0/unused-1.0.0.jar:/home/cass/.m2/repository/org/apache/avro/avro-ipc/1.7.7/avro-ipc-1.7.7.jar:/home/cass/.m2/repository/commons-collections/commons-collections/3.2.2/commons-collections-3.2.2.jar:/home/cass/.m2/repository/com/twitter/chill_2.11/0.8.0/chill_2.11-0.8.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-locator/2.4.0-b34/hk2-locator-2.4.0-b34.jar:/home/cass/.m2/repository/org/eclipse/jetty/jetty-http/9.2.16.v20160414/jetty-http-9.2.16.v20160414.jar:/home/cass/.m2/repository/org/slf4j/jcl-over-slf4j/1.7.16/jcl-over-slf4j-1.7.16.jar:/home/cass/.m2/repository/commons-httpclient/commons-httpclient/3.1/commons-httpclient-3.1.jar:/home/cass/.m2/repository/io/netty/netty-all/4.0.29.Final/netty-all-4.0.29.Final.jar:/home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-remote-resources-plugin:1.5:process (default) @ spark-core_2.11 ---
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ spark-core_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 33 resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:compile (scala-compile-first) @ spark-core_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 479 Scala sources and 74 Java sources to /home/cass/spark2/spark/core/target/scala-2.11/classes...
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:533: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn]   def intAccumulator(initialValue: Int): Accumulator[java.lang.Integer] =
[warn]                                          ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:534: method accumulator in class SparkContext is deprecated: use AccumulatorV2
[warn]     sc.accumulator(initialValue)(IntAccumulatorParam).asInstanceOf[Accumulator[java.lang.Integer]]
[warn]        ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:534: object IntAccumulatorParam in object AccumulatorParam is deprecated: use AccumulatorV2
[warn]     sc.accumulator(initialValue)(IntAccumulatorParam).asInstanceOf[Accumulator[java.lang.Integer]]
[warn]                                  ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:534: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn]     sc.accumulator(initialValue)(IntAccumulatorParam).asInstanceOf[Accumulator[java.lang.Integer]]
[warn]                                                                    ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:542: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn]   def intAccumulator(initialValue: Int, name: String): Accumulator[java.lang.Integer] =
[warn]                                                        ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:543: method accumulator in class SparkContext is deprecated: use AccumulatorV2
[warn]     sc.accumulator(initialValue, name)(IntAccumulatorParam)
[warn]        ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:543: object IntAccumulatorParam in object AccumulatorParam is deprecated: use AccumulatorV2
[warn]     sc.accumulator(initialValue, name)(IntAccumulatorParam)
[warn]                                        ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:544: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn]       .asInstanceOf[Accumulator[java.lang.Integer]]
[warn]                     ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:550: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn]   def doubleAccumulator(initialValue: Double): Accumulator[java.lang.Double] =
[warn]                                                ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:551: method accumulator in class SparkContext is deprecated: use AccumulatorV2
[warn]     sc.accumulator(initialValue)(DoubleAccumulatorParam).asInstanceOf[Accumulator[java.lang.Double]]
[warn]        ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:551: object DoubleAccumulatorParam in object AccumulatorParam is deprecated: use AccumulatorV2
[warn]     sc.accumulator(initialValue)(DoubleAccumulatorParam).asInstanceOf[Accumulator[java.lang.Double]]
[warn]                                  ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:551: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn]     sc.accumulator(initialValue)(DoubleAccumulatorParam).asInstanceOf[Accumulator[java.lang.Double]]
[warn]                                                                       ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:559: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn]   def doubleAccumulator(initialValue: Double, name: String): Accumulator[java.lang.Double] =
[warn]                                                              ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:560: method accumulator in class SparkContext is deprecated: use AccumulatorV2
[warn]     sc.accumulator(initialValue, name)(DoubleAccumulatorParam)
[warn]        ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:560: object DoubleAccumulatorParam in object AccumulatorParam is deprecated: use AccumulatorV2
[warn]     sc.accumulator(initialValue, name)(DoubleAccumulatorParam)
[warn]                                        ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:561: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn]       .asInstanceOf[Accumulator[java.lang.Double]]
[warn]                     ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:567: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn]   def accumulator(initialValue: Int): Accumulator[java.lang.Integer] = intAccumulator(initialValue)
[warn]                                       ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:575: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn]   def accumulator(initialValue: Int, name: String): Accumulator[java.lang.Integer] =
[warn]                                                     ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:582: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn]   def accumulator(initialValue: Double): Accumulator[java.lang.Double] =
[warn]                                          ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:592: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn]   def accumulator(initialValue: Double, name: String): Accumulator[java.lang.Double] =
[warn]                                                        ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:599: trait AccumulatorParam in package spark is deprecated: use AccumulatorV2
[warn]   def accumulator[T](initialValue: T, accumulatorParam: AccumulatorParam[T]): Accumulator[T] =
[warn]                                                         ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:599: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn]   def accumulator[T](initialValue: T, accumulatorParam: AccumulatorParam[T]): Accumulator[T] =
[warn]                                                                               ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:600: method accumulator in class SparkContext is deprecated: use AccumulatorV2
[warn]     sc.accumulator(initialValue)(accumulatorParam)
[warn]        ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:608: trait AccumulatorParam in package spark is deprecated: use AccumulatorV2
[warn]   def accumulator[T](initialValue: T, name: String, accumulatorParam: AccumulatorParam[T])
[warn]                                                                       ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:609: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn]       : Accumulator[T] =
[warn]         ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:610: method accumulator in class SparkContext is deprecated: use AccumulatorV2
[warn]     sc.accumulator(initialValue, name)(accumulatorParam)
[warn]        ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:616: trait AccumulableParam in package spark is deprecated: use AccumulatorV2
[warn]   def accumulable[T, R](initialValue: T, param: AccumulableParam[T, R]): Accumulable[T, R] =
[warn]                                                 ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:616: class Accumulable in package spark is deprecated: use AccumulatorV2
[warn]   def accumulable[T, R](initialValue: T, param: AccumulableParam[T, R]): Accumulable[T, R] =
[warn]                                                                          ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:617: method accumulable in class SparkContext is deprecated: use AccumulatorV2
[warn]     sc.accumulable(initialValue)(param)
[warn]        ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:625: trait AccumulableParam in package spark is deprecated: use AccumulatorV2
[warn]   def accumulable[T, R](initialValue: T, name: String, param: AccumulableParam[T, R])
[warn]                                                               ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:626: class Accumulable in package spark is deprecated: use AccumulatorV2
[warn]       : Accumulable[T, R] =
[warn]         ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/java/JavaSparkContext.scala:627: method accumulable in class SparkContext is deprecated: use AccumulatorV2
[warn]     sc.accumulable(initialValue, name)(param)
[warn]        ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/python/PythonRDD.scala:78: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn]     accumulator: Accumulator[JList[Array[Byte]]])
[warn]                  ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/python/PythonRDD.scala:71: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn] private[spark] case class PythonFunction(
[warn]                           ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/api/python/PythonRDD.scala:873: trait AccumulatorParam in package spark is deprecated: use AccumulatorV2
[warn]   extends AccumulatorParam[JList[Array[Byte]]] {
[warn]           ^
[warn] /home/cass/spark2/spark/core/src/main/scala/org/apache/spark/util/AccumulatorV2.scala:451: trait AccumulableParam in package spark is deprecated: use AccumulatorV2
[warn]     param: org.apache.spark.AccumulableParam[R, T]) extends AccumulatorV2[T, R] {
[warn]                             ^
[warn] 36 warnings found
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] 1 warning
[info] Compile success at May 20, 2016 12:30:46 PM [1:00.341s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:compile (default-compile) @ spark-core_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 74 source files to /home/cass/spark2/spark/core/target/scala-2.11/classes
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (create-tmp-dir) @ spark-core_2.11 ---
[INFO] Executing tasks

main:
    [mkdir] Created dir: /home/cass/spark2/spark/core/target/tmp
[INFO] Executed tasks
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ spark-core_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 50 resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:testCompile (scala-test-compile-first) @ spark-core_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 207 Scala sources and 20 Java sources to /home/cass/spark2/spark/core/target/scala-2.11/test-classes...
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/AccumulatorSuite.scala:48: trait AccumulableParam in package spark is deprecated: use AccumulatorV2
[warn]   implicit def setAccum[A]: AccumulableParam[mutable.Set[A], A] =
[warn]                             ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/AccumulatorSuite.scala:49: trait AccumulableParam in package spark is deprecated: use AccumulatorV2
[warn]     new AccumulableParam[mutable.Set[A], A] {
[warn]         ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/AccumulatorSuite.scala:86: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn]     val acc: Accumulator[Int] = sc.accumulator(0)
[warn]              ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/AccumulatorSuite.scala:86: method accumulator in class SparkContext is deprecated: use AccumulatorV2
[warn]     val acc: Accumulator[Int] = sc.accumulator(0)
[warn]                                    ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/AccumulatorSuite.scala:86: object IntAccumulatorParam in object AccumulatorParam is deprecated: use AccumulatorV2
[warn]     val acc: Accumulator[Int] = sc.accumulator(0)
[warn]                                               ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/AccumulatorSuite.scala:92: method accumulator in class SparkContext is deprecated: use AccumulatorV2
[warn]     val longAcc = sc.accumulator(0L)
[warn]                      ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/AccumulatorSuite.scala:92: object LongAccumulatorParam in object AccumulatorParam is deprecated: use AccumulatorV2
[warn]     val longAcc = sc.accumulator(0L)
[warn]                                 ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/AccumulatorSuite.scala:100: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn]     val acc: Accumulator[Int] = sc.accumulator(0)
[warn]              ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/AccumulatorSuite.scala:100: method accumulator in class SparkContext is deprecated: use AccumulatorV2
[warn]     val acc: Accumulator[Int] = sc.accumulator(0)
[warn]                                    ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/AccumulatorSuite.scala:100: object IntAccumulatorParam in object AccumulatorParam is deprecated: use AccumulatorV2
[warn]     val acc: Accumulator[Int] = sc.accumulator(0)
[warn]                                               ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/AccumulatorSuite.scala:110: class Accumulable in package spark is deprecated: use AccumulatorV2
[warn]       val acc: Accumulable[mutable.Set[Any], Any] = sc.accumulable(new mutable.HashSet[Any]())
[warn]                ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/AccumulatorSuite.scala:110: method accumulable in class SparkContext is deprecated: use AccumulatorV2
[warn]       val acc: Accumulable[mutable.Set[Any], Any] = sc.accumulable(new mutable.HashSet[Any]())
[warn]                                                        ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/AccumulatorSuite.scala:127: class Accumulable in package spark is deprecated: use AccumulatorV2
[warn]       val acc: Accumulable[mutable.Set[Any], Any] = sc.accumulable(new mutable.HashSet[Any]())
[warn]                ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/AccumulatorSuite.scala:127: method accumulable in class SparkContext is deprecated: use AccumulatorV2
[warn]       val acc: Accumulable[mutable.Set[Any], Any] = sc.accumulable(new mutable.HashSet[Any]())
[warn]                                                        ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/AccumulatorSuite.scala:143: method accumulableCollection in class SparkContext is deprecated: use AccumulatorV2
[warn]       val setAcc = sc.accumulableCollection(mutable.HashSet[Int]())
[warn]                       ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/AccumulatorSuite.scala:144: method accumulableCollection in class SparkContext is deprecated: use AccumulatorV2
[warn]       val bufferAcc = sc.accumulableCollection(mutable.ArrayBuffer[Int]())
[warn]                          ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/AccumulatorSuite.scala:145: method accumulableCollection in class SparkContext is deprecated: use AccumulatorV2
[warn]       val mapAcc = sc.accumulableCollection(mutable.HashMap[Int, String]())
[warn]                       ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/AccumulatorSuite.scala:168: class Accumulable in package spark is deprecated: use AccumulatorV2
[warn]       val acc: Accumulable[mutable.Set[Any], Any] = sc.accumulable(new mutable.HashSet[Any]())
[warn]                ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/AccumulatorSuite.scala:168: method accumulable in class SparkContext is deprecated: use AccumulatorV2
[warn]       val acc: Accumulable[mutable.Set[Any], Any] = sc.accumulable(new mutable.HashSet[Any]())
[warn]                                                        ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/AccumulatorSuite.scala:182: class Accumulable in package spark is deprecated: use AccumulatorV2
[warn]     var acc: Accumulable[mutable.Set[Any], Any] = sc.accumulable(new mutable.HashSet[Any]())
[warn]              ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/AccumulatorSuite.scala:182: method accumulable in class SparkContext is deprecated: use AccumulatorV2
[warn]     var acc: Accumulable[mutable.Set[Any], Any] = sc.accumulable(new mutable.HashSet[Any]())
[warn]                                                      ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/AccumulatorSuite.scala:225: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn]     val acc = new Accumulator("", StringAccumulatorParam, Some("darkness"))
[warn]                   ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/AccumulatorSuite.scala:225: object StringAccumulatorParam in object AccumulatorParam is deprecated: use AccumulatorV2
[warn]     val acc = new Accumulator("", StringAccumulatorParam, Some("darkness"))
[warn]                                   ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/DistributedSuite.scala:95: method accumulator in class SparkContext is deprecated: use AccumulatorV2
[warn]     val accum = sc.accumulator(0)
[warn]                    ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/DistributedSuite.scala:95: object IntAccumulatorParam in object AccumulatorParam is deprecated: use AccumulatorV2
[warn]     val accum = sc.accumulator(0)
[warn]                               ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/DistributedSuite.scala:112: method accumulator in class SparkContext is deprecated: use AccumulatorV2
[warn]     val accum = sc.accumulator(0)
[warn]                    ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/DistributedSuite.scala:112: object IntAccumulatorParam in object AccumulatorParam is deprecated: use AccumulatorV2
[warn]     val accum = sc.accumulator(0)
[warn]                               ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/scheduler/DAGSchedulerSuite.scala:1596: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn]     val acc = new Accumulator[Int](0, new AccumulatorParam[Int] {
[warn]                   ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/scheduler/DAGSchedulerSuite.scala:1596: trait AccumulatorParam in package spark is deprecated: use AccumulatorV2
[warn]     val acc = new Accumulator[Int](0, new AccumulatorParam[Int] {
[warn]                                           ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/scheduler/TaskContextSuite.scala:149: object LongAccumulatorParam in object AccumulatorParam is deprecated: use AccumulatorV2
[warn]     val param = AccumulatorParam.LongAccumulatorParam
[warn]                                  ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/scheduler/TaskContextSuite.scala:149: object AccumulatorParam in package spark is deprecated: use AccumulatorV2
[warn]     val param = AccumulatorParam.LongAccumulatorParam
[warn]                 ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/scheduler/TaskContextSuite.scala:151: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn]     val acc1 = new Accumulator(0L, param, Some("x"), countFailedValues = true)
[warn]                    ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/scheduler/TaskContextSuite.scala:152: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn]     val acc2 = new Accumulator(0L, param, Some("y"), countFailedValues = false)
[warn]                    ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/util/AccumulatorV2Suite.scala:131: object StringAccumulatorParam in object AccumulatorParam is deprecated: use AccumulatorV2
[warn]     val acc = new LegacyAccumulatorWrapper("default", AccumulatorParam.StringAccumulatorParam)
[warn]                                                                        ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/spark/util/AccumulatorV2Suite.scala:131: object AccumulatorParam in package spark is deprecated: use AccumulatorV2
[warn]     val acc = new LegacyAccumulatorWrapper("default", AccumulatorParam.StringAccumulatorParam)
[warn]                                                       ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/sparktest/ImplicitSuite.scala:79: method accumulator in class SparkContext is deprecated: use AccumulatorV2
[warn]     sc.accumulator(123.4)
[warn]        ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/sparktest/ImplicitSuite.scala:79: object DoubleAccumulatorParam in object AccumulatorParam is deprecated: use AccumulatorV2
[warn]     sc.accumulator(123.4)
[warn]                   ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/sparktest/ImplicitSuite.scala:84: method accumulator in class SparkContext is deprecated: use AccumulatorV2
[warn]     sc.accumulator(123)
[warn]        ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/sparktest/ImplicitSuite.scala:84: object IntAccumulatorParam in object AccumulatorParam is deprecated: use AccumulatorV2
[warn]     sc.accumulator(123)
[warn]                   ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/sparktest/ImplicitSuite.scala:89: method accumulator in class SparkContext is deprecated: use AccumulatorV2
[warn]     sc.accumulator(123L)
[warn]        ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/sparktest/ImplicitSuite.scala:89: object LongAccumulatorParam in object AccumulatorParam is deprecated: use AccumulatorV2
[warn]     sc.accumulator(123L)
[warn]                   ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/sparktest/ImplicitSuite.scala:94: method accumulator in class SparkContext is deprecated: use AccumulatorV2
[warn]     sc.accumulator(123F)
[warn]        ^
[warn] /home/cass/spark2/spark/core/src/test/scala/org/apache/sparktest/ImplicitSuite.scala:94: object FloatAccumulatorParam in object AccumulatorParam is deprecated: use AccumulatorV2
[warn]     sc.accumulator(123F)
[warn]                   ^
[warn] 43 warnings found
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] /home/cass/spark2/spark/core/src/test/java/org/apache/spark/JavaAPISuite.java:290: warning: [deprecation] Accumulator in org.apache.spark has been deprecated
[warn]     final Accumulator<Integer> accum = sc.accumulator(0);
[warn]           ^
[warn] /home/cass/spark2/spark/core/src/test/java/org/apache/spark/JavaAPISuite.java:303: warning: [deprecation] Accumulator in org.apache.spark has been deprecated
[warn]     final Accumulator<Integer> accum = sc.accumulator(0);
[warn]           ^
[warn] /home/cass/spark2/spark/core/src/test/java/org/apache/spark/JavaAPISuite.java:1384: warning: [deprecation] Accumulator in org.apache.spark has been deprecated
[warn]     final Accumulator<Integer> intAccum = sc.intAccumulator(10);
[warn]           ^
[warn] /home/cass/spark2/spark/core/src/test/java/org/apache/spark/JavaAPISuite.java:1393: warning: [deprecation] Accumulator in org.apache.spark has been deprecated
[warn]     final Accumulator<Double> doubleAccum = sc.doubleAccumulator(10.0);
[warn]           ^
[warn] /home/cass/spark2/spark/core/src/test/java/org/apache/spark/JavaAPISuite.java:1403: warning: [deprecation] AccumulatorParam in org.apache.spark has been deprecated
[warn]     AccumulatorParam<Float> floatAccumulatorParam = new AccumulatorParam<Float>() {
[warn]     ^
[warn] /home/cass/spark2/spark/core/src/test/java/org/apache/spark/JavaAPISuite.java:1403: warning: [deprecation] AccumulatorParam in org.apache.spark has been deprecated
[warn]     AccumulatorParam<Float> floatAccumulatorParam = new AccumulatorParam<Float>() {
[warn]                                                         ^
[warn] /home/cass/spark2/spark/core/src/test/java/org/apache/spark/JavaAPISuite.java:1420: warning: [deprecation] Accumulator in org.apache.spark has been deprecated
[warn]     final Accumulator<Float> floatAccum = sc.accumulator(10.0f, floatAccumulatorParam);
[warn]           ^
[warn] 8 warnings
[info] Compile success at May 20, 2016 12:31:36 PM [47.343s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:testCompile (default-testCompile) @ spark-core_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 20 source files to /home/cass/spark2/spark/core/target/scala-2.11/test-classes
[WARNING] /home/cass/spark2/spark/core/src/test/java/org/apache/spark/JavaAPISuite.java:[290,10] [deprecation] Accumulator in org.apache.spark has been deprecated
[WARNING] /home/cass/spark2/spark/core/src/test/java/org/apache/spark/JavaAPISuite.java:[303,10] [deprecation] Accumulator in org.apache.spark has been deprecated
[WARNING] /home/cass/spark2/spark/core/src/test/java/org/apache/spark/JavaAPISuite.java:[1384,10] [deprecation] Accumulator in org.apache.spark has been deprecated
[WARNING] /home/cass/spark2/spark/core/src/test/java/org/apache/spark/JavaAPISuite.java:[1393,10] [deprecation] Accumulator in org.apache.spark has been deprecated
[WARNING] /home/cass/spark2/spark/core/src/test/java/org/apache/spark/JavaAPISuite.java:[1403,4] [deprecation] AccumulatorParam in org.apache.spark has been deprecated
[WARNING] /home/cass/spark2/spark/core/src/test/java/org/apache/spark/JavaAPISuite.java:[1403,56] [deprecation] AccumulatorParam in org.apache.spark has been deprecated
[WARNING] /home/cass/spark2/spark/core/src/test/java/org/apache/spark/JavaAPISuite.java:[1420,10] [deprecation] Accumulator in org.apache.spark has been deprecated
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (generate-test-classpath) @ spark-core_2.11 ---
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (default-test) @ spark-core_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (test) @ spark-core_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- scalatest-maven-plugin:1.0:test (test) @ spark-core_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (prepare-test-jar) @ spark-core_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/core/target/spark-core_2.11-2.0.0-SNAPSHOT-tests.jar
[INFO]
[INFO] --- maven-jar-plugin:2.6:jar (default-jar) @ spark-core_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/core/target/spark-core_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-site-plugin:3.3:attach-descriptor (attach-descriptor) @ spark-core_2.11 ---
[INFO]
[INFO] --- maven-dependency-plugin:2.10:copy-dependencies (copy-dependencies) @ spark-core_2.11 ---
[INFO]
[INFO] --- maven-shade-plugin:2.4.3:shade (default) @ spark-core_2.11 ---
[INFO] Excluding org.apache.avro:avro-mapred:jar:hadoop2:1.7.7 from the shaded jar.
[INFO] Excluding org.apache.avro:avro-ipc:jar:1.7.7 from the shaded jar.
[INFO] Excluding org.apache.avro:avro:jar:1.7.7 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-core-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-mapper-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding com.twitter:chill_2.11:jar:0.8.0 from the shaded jar.
[INFO] Excluding com.esotericsoftware:kryo-shaded:jar:3.0.3 from the shaded jar.
[INFO] Excluding com.esotericsoftware:minlog:jar:1.3.0 from the shaded jar.
[INFO] Excluding com.twitter:chill-java:jar:0.8.0 from the shaded jar.
[INFO] Excluding org.apache.xbean:xbean-asm5-shaded:jar:4.4 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding commons-cli:commons-cli:jar:1.2 from the shaded jar.
[INFO] Excluding xmlenc:xmlenc:jar:0.52 from the shaded jar.
[INFO] Excluding commons-io:commons-io:jar:2.4 from the shaded jar.
[INFO] Excluding commons-lang:commons-lang:jar:2.6 from the shaded jar.
[INFO] Excluding commons-configuration:commons-configuration:jar:1.6 from the shaded jar.
[INFO] Excluding commons-digester:commons-digester:jar:1.8 from the shaded jar.
[INFO] Excluding commons-beanutils:commons-beanutils:jar:1.7.0 from the shaded jar.
[INFO] Excluding commons-beanutils:commons-beanutils-core:jar:1.8.0 from the shaded jar.
[INFO] Excluding com.google.protobuf:protobuf-java:jar:2.5.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-auth:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-compress:jar:1.4.1 from the shaded jar.
[INFO] Excluding org.tukaani:xz:jar:1.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-hdfs:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.mortbay.jetty:jetty-util:jar:6.1.26 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-app:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding com.google.inject:guice:jar:3.0 from the shaded jar.
[INFO] Excluding javax.inject:javax.inject:jar:1 from the shaded jar.
[INFO] Excluding aopalliance:aopalliance:jar:1.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-server-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-shuffle:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-api:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-core:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-jobclient:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-annotations:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-launcher_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-network-common_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-network-shuffle_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.fusesource.leveldbjni:leveldbjni-all:jar:1.8 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-annotations:jar:2.5.3 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-unsafe_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding net.java.dev.jets3t:jets3t:jar:0.7.1 from the shaded jar.
[INFO] Excluding commons-codec:commons-codec:jar:1.10 from the shaded jar.
[INFO] Excluding commons-httpclient:commons-httpclient:jar:3.1 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-recipes:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-framework:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-client:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.zookeeper:zookeeper:jar:3.4.5 from the shaded jar.
[INFO] Including org.eclipse.jetty:jetty-plus:jar:9.2.16.v20160414 in the shaded jar.
[INFO] Excluding org.eclipse.jetty:jetty-webapp:jar:9.2.16.v20160414 from the shaded jar.
[INFO] Excluding org.eclipse.jetty:jetty-xml:jar:9.2.16.v20160414 from the shaded jar.
[INFO] Excluding org.eclipse.jetty:jetty-jndi:jar:9.2.16.v20160414 from the shaded jar.
[INFO] Including org.eclipse.jetty:jetty-security:jar:9.2.16.v20160414 in the shaded jar.
[INFO] Including org.eclipse.jetty:jetty-util:jar:9.2.16.v20160414 in the shaded jar.
[INFO] Including org.eclipse.jetty:jetty-server:jar:9.2.16.v20160414 in the shaded jar.
[INFO] Including org.eclipse.jetty:jetty-io:jar:9.2.16.v20160414 in the shaded jar.
[INFO] Including org.eclipse.jetty:jetty-http:jar:9.2.16.v20160414 in the shaded jar.
[INFO] Including org.eclipse.jetty:jetty-continuation:jar:9.2.16.v20160414 in the shaded jar.
[INFO] Including org.eclipse.jetty:jetty-servlet:jar:9.2.16.v20160414 in the shaded jar.
[INFO] Including org.eclipse.jetty:jetty-servlets:jar:9.2.16.v20160414 in the shaded jar.
[INFO] Excluding javax.servlet:javax.servlet-api:jar:3.1.0 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-lang3:jar:3.3.2 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-math3:jar:3.4.1 from the shaded jar.
[INFO] Excluding com.google.code.findbugs:jsr305:jar:1.3.9 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-api:jar:1.7.16 from the shaded jar.
[INFO] Excluding org.slf4j:jul-to-slf4j:jar:1.7.16 from the shaded jar.
[INFO] Excluding org.slf4j:jcl-over-slf4j:jar:1.7.16 from the shaded jar.
[INFO] Excluding log4j:log4j:jar:1.2.17 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-log4j12:jar:1.7.16 from the shaded jar.
[INFO] Excluding com.ning:compress-lzf:jar:1.0.3 from the shaded jar.
[INFO] Excluding org.xerial.snappy:snappy-java:jar:1.1.2.4 from the shaded jar.
[INFO] Excluding net.jpountz.lz4:lz4:jar:1.3.0 from the shaded jar.
[INFO] Excluding org.roaringbitmap:RoaringBitmap:jar:0.5.11 from the shaded jar.
[INFO] Excluding commons-net:commons-net:jar:2.2 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-library:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.json4s:json4s-jackson_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.json4s:json4s-core_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.json4s:json4s-ast_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.scala-lang:scalap:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-compiler:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-parser-combinators_2.11:jar:1.0.4 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-client:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.ws.rs:javax.ws.rs-api:jar:2.0.1 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-api:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-utils:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2.external:aopalliance-repackaged:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2.external:javax.inject:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-locator:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-common:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.annotation:javax.annotation-api:jar:1.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.bundles.repackaged:jersey-guava:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:osgi-resource-locator:jar:1.0.1 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-server:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.media:jersey-media-jaxb:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.validation:validation-api:jar:1.1.0.Final from the shaded jar.
[INFO] Excluding org.glassfish.jersey.containers:jersey-container-servlet:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.containers:jersey-container-servlet-core:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.apache.mesos:mesos:jar:shaded-protobuf:0.21.1 from the shaded jar.
[INFO] Excluding io.netty:netty-all:jar:4.0.29.Final from the shaded jar.
[INFO] Excluding io.netty:netty:jar:3.8.0.Final from the shaded jar.
[INFO] Excluding com.clearspring.analytics:stream:jar:2.7.0 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-core:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-jvm:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-json:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-graphite:jar:3.1.2 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-databind:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-core:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.module:jackson-module-scala_2.11:jar:2.5.3 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-reflect:jar:2.11.8 from the shaded jar.
[INFO] Excluding com.thoughtworks.paranamer:paranamer:jar:2.6 from the shaded jar.
[INFO] Excluding org.apache.ivy:ivy:jar:2.4.0 from the shaded jar.
[INFO] Excluding oro:oro:jar:2.0.8 from the shaded jar.
[INFO] Excluding commons-collections:commons-collections:jar:3.2.2 from the shaded jar.
[INFO] Excluding org.objenesis:objenesis:jar:2.1 from the shaded jar.
[INFO] Excluding org.javassist:javassist:jar:3.15.0-GA from the shaded jar.
[INFO] Excluding org.apache.commons:commons-math:jar:2.2 from the shaded jar.
[INFO] Excluding net.razorvine:pyrolite:jar:4.9 from the shaded jar.
[INFO] Excluding net.sf.py4j:py4j:jar:0.10.1 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-tags_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Including org.spark-project.spark:unused:jar:1.0.0 in the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-xml_2.11:jar:1.0.2 from the shaded jar.
[INFO] Replacing original artifact with shaded artifact.
[INFO] Replacing /home/cass/spark2/spark/core/target/spark-core_2.11-2.0.0-SNAPSHOT.jar with /home/cass/spark2/spark/core/target/spark-core_2.11-2.0.0-SNAPSHOT-shaded.jar
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/core/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/core/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/core/dependency-reduced-pom.xml
[INFO]
[INFO] --- maven-source-plugin:2.4:jar-no-fork (create-source-jar) @ spark-core_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/core/target/spark-core_2.11-2.0.0-SNAPSHOT-sources.jar
[INFO]
[INFO] --- maven-source-plugin:2.4:test-jar-no-fork (create-source-jar) @ spark-core_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/core/target/spark-core_2.11-2.0.0-SNAPSHOT-test-sources.jar
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Spark Project GraphX 2.0.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.0.0:clean (default-clean) @ spark-graphx_2.11 ---
[INFO]
[INFO] --- maven-enforcer-plugin:1.4.1:enforce (enforce-versions) @ spark-graphx_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:add-source (eclipse-add-source) @ spark-graphx_2.11 ---
[INFO] Add Source directory: /home/cass/spark2/spark/graphx/src/main/scala
[INFO] Add Test Source directory: /home/cass/spark2/spark/graphx/src/test/scala
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (default-cli) @ spark-graphx_2.11 ---
[INFO] Dependencies classpath:
/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-jobclient/2.2.0/hadoop-mapreduce-client-jobclient-2.2.0.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-core/3.1.2/metrics-core-3.1.2.jar:/home/cass/.m2/repository/com/google/protobuf/protobuf-java/2.5.0/protobuf-java-2.5.0.jar:/home/cass/.m2/repository/aopalliance/aopalliance/1.0/aopalliance-1.0.jar:/home/cass/.m2/repository/net/razorvine/pyrolite/4.9/pyrolite-4.9.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-jvm/3.1.2/metrics-jvm-3.1.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-client/2.2.0/hadoop-client-2.2.0.jar:/home/cass/.m2/repository/org/fusesource/leveldbjni/leveldbjni-all/1.8/leveldbjni-all-1.8.jar:/home/cass/.m2/repository/org/glassfish/jersey/bundles/repackaged/jersey-guava/2.22.2/jersey-guava-2.22.2.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-json/3.1.2/metrics-json-3.1.2.jar:/home/cass/.m2/repository/net/java/dev/jets3t/jets3t/0.7.1/jets3t-0.7.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-common/2.2.0/hadoop-common-2.2.0.jar:/home/cass/.m2/repository/com/google/inject/guice/3.0/guice-3.0.jar:/home/cass/.m2/repository/commons-io/commons-io/2.4/commons-io-2.4.jar:/home/cass/.m2/repository/net/sourceforge/f2j/arpack_combined_all/0.1/arpack_combined_all-0.1.jar:/home/cass/.m2/repository/org/scala-lang/scala-reflect/2.11.8/scala-reflect-2.11.8.jar:/home/cass/.m2/repository/org/xerial/snappy/snappy-java/1.1.2.4/snappy-java-1.1.2.4.jar:/home/cass/.m2/repository/org/json4s/json4s-jackson_2.11/3.2.11/json4s-jackson_2.11-3.2.11.jar:/home/cass/.m2/repository/com/esotericsoftware/minlog/1.3.0/minlog-1.3.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-auth/2.2.0/hadoop-auth-2.2.0.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-core-asl/1.9.13/jackson-core-asl-1.9.13.jar:/home/cass/.m2/repository/javax/validation/validation-api/1.1.0.Final/validation-api-1.1.0.Final.jar:/home/cass/.m2/repository/net/jpountz/lz4/lz4/1.3.0/lz4-1.3.0.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-common/2.22.2/jersey-common-2.22.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-client/2.2.0/hadoop-yarn-client-2.2.0.jar:/home/cass/.m2/repository/io/netty/netty/3.8.0.Final/netty-3.8.0.Final.jar:/home/cass/.m2/repository/org/apache/mesos/mesos/0.21.1/mesos-0.21.1-shaded-protobuf.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-annotations/2.5.3/jackson-annotations-2.5.3.jar:/home/cass/.m2/repository/com/google/code/findbugs/jsr305/1.3.9/jsr305-1.3.9.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-api/2.4.0-b34/hk2-api-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-server/2.22.2/jersey-server-2.22.2.jar:/home/cass/.m2/repository/net/sf/py4j/py4j/0.10.1/py4j-0.10.1.jar:/home/cass/.m2/repository/com/twitter/chill-java/0.8.0/chill-java-0.8.0.jar:/home/cass/.m2/repository/commons-lang/commons-lang/2.6/commons-lang-2.6.jar:/home/cass/.m2/repository/org/tukaani/xz/1.0/xz-1.0.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-databind/2.5.3/jackson-databind-2.5.3.jar:/home/cass/.m2/repository/commons-codec/commons-codec/1.10/commons-codec-1.10.jar:/home/cass/.m2/repository/org/apache/curator/curator-recipes/2.4.0/curator-recipes-2.4.0.jar:/home/cass/.m2/repository/org/javassist/javassist/3.18.1-GA/javassist-3.18.1-GA.jar:/home/cass/.m2/repository/org/apache/ivy/ivy/2.4.0/ivy-2.4.0.jar:/home/cass/.m2/repository/javax/inject/javax.inject/1/javax.inject-1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-core/2.2.0/hadoop-mapreduce-client-core-2.2.0.jar:/home/cass/.m2/repository/com/fasterxml/jackson/module/jackson-module-scala_2.11/2.5.3/jackson-module-scala_2.11-2.5.3.jar:/home/cass/.m2/repository/commons-beanutils/commons-beanutils-core/1.8.0/commons-beanutils-core-1.8.0.jar:/home/cass/.m2/repository/javax/servlet/javax.servlet-api/3.1.0/javax.servlet-api-3.1.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/osgi-resource-locator/1.0.1/osgi-resource-locator-1.0.1.jar:/home/cass/.m2/repository/org/apache/commons/commons-math3/3.4.1/commons-math3-3.4.1.jar:/home/cass/spark2/spark/common/network-common/target/spark-network-common_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/avro/avro/1.7.7/avro-1.7.7.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-common/2.2.0/hadoop-mapreduce-client-common-2.2.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-utils/2.4.0-b34/hk2-utils-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/hk2/external/aopalliance-repackaged/2.4.0-b34/aopalliance-repackaged-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/hk2/external/javax.inject/2.4.0-b34/javax.inject-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/jersey/containers/jersey-container-servlet-core/2.22.2/jersey-container-servlet-core-2.22.2.jar:/home/cass/.m2/repository/oro/oro/2.0.8/oro-2.0.8.jar:/home/cass/.m2/repository/org/scala-lang/scala-compiler/2.11.8/scala-compiler-2.11.8.jar:/home/cass/.m2/repository/org/roaringbitmap/RoaringBitmap/0.5.11/RoaringBitmap-0.5.11.jar:/home/cass/.m2/repository/log4j/log4j/1.2.17/log4j-1.2.17.jar:/home/cass/.m2/repository/org/scala-lang/scala-library/2.11.8/scala-library-2.11.8.jar:/home/cass/.m2/repository/org/apache/curator/curator-client/2.4.0/curator-client-2.4.0.jar:/home/cass/.m2/repository/org/apache/commons/commons-compress/1.4.1/commons-compress-1.4.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-app/2.2.0/hadoop-mapreduce-client-app-2.2.0.jar:/home/cass/.m2/repository/org/slf4j/slf4j-api/1.7.16/slf4j-api-1.7.16.jar:/home/cass/.m2/repository/org/apache/xbean/xbean-asm5-shaded/4.4/xbean-asm5-shaded-4.4.jar:/home/cass/.m2/repository/org/json4s/json4s-core_2.11/3.2.11/json4s-core_2.11-3.2.11.jar:/home/cass/.m2/repository/com/github/fommil/netlib/core/1.1.2/core-1.1.2.jar:/home/cass/.m2/repository/org/mortbay/jetty/jetty-util/6.1.26/jetty-util-6.1.26.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-server-common/2.2.0/hadoop-yarn-server-common-2.2.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-hdfs/2.2.0/hadoop-hdfs-2.2.0.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-mapper-asl/1.9.13/jackson-mapper-asl-1.9.13.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-api/2.2.0/hadoop-yarn-api-2.2.0.jar:/home/cass/.m2/repository/com/esotericsoftware/kryo-shaded/3.0.3/kryo-shaded-3.0.3.jar:/home/cass/.m2/repository/javax/ws/rs/javax.ws.rs-api/2.0.1/javax.ws.rs-api-2.0.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-common/2.2.0/hadoop-yarn-common-2.2.0.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-client/2.22.2/jersey-client-2.22.2.jar:/home/cass/spark2/spark/common/unsafe/target/spark-unsafe_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/avro/avro-mapred/1.7.7/avro-mapred-1.7.7-hadoop2.jar:/home/cass/.m2/repository/xmlenc/xmlenc/0.52/xmlenc-0.52.jar:/home/cass/.m2/repository/com/ning/compress-lzf/1.0.3/compress-lzf-1.0.3.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-shuffle/2.2.0/hadoop-mapreduce-client-shuffle-2.2.0.jar:/home/cass/.m2/repository/org/apache/zookeeper/zookeeper/3.4.5/zookeeper-3.4.5.jar:/home/cass/.m2/repository/org/apache/curator/curator-framework/2.4.0/curator-framework-2.4.0.jar:/home/cass/.m2/repository/commons-net/commons-net/2.2/commons-net-2.2.jar:/home/cass/.m2/repository/org/apache/commons/commons-lang3/3.3.2/commons-lang3-3.3.2.jar:/home/cass/.m2/repository/org/json4s/json4s-ast_2.11/3.2.11/json4s-ast_2.11-3.2.11.jar:/home/cass/spark2/spark/launcher/target/spark-launcher_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/scala-lang/scalap/2.11.8/scalap-2.11.8.jar:/home/cass/.m2/repository/com/clearspring/analytics/stream/2.7.0/stream-2.7.0.jar:/home/cass/.m2/repository/org/apache/commons/commons-math/2.1/commons-math-2.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-annotations/2.2.0/hadoop-annotations-2.2.0.jar:/home/cass/.m2/repository/com/thoughtworks/paranamer/paranamer/2.6/paranamer-2.6.jar:/home/cass/.m2/repository/commons-configuration/commons-configuration/1.6/commons-configuration-1.6.jar:/home/cass/.m2/repository/org/glassfish/jersey/containers/jersey-container-servlet/2.22.2/jersey-container-servlet-2.22.2.jar:/home/cass/.m2/repository/commons-digester/commons-digester/1.8/commons-digester-1.8.jar:/home/cass/.m2/repository/org/slf4j/jul-to-slf4j/1.7.16/jul-to-slf4j-1.7.16.jar:/home/cass/.m2/repository/commons-beanutils/commons-beanutils/1.7.0/commons-beanutils-1.7.0.jar:/home/cass/spark2/spark/common/network-shuffle/target/spark-network-shuffle_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-xml_2.11/1.0.2/scala-xml_2.11-1.0.2.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-parser-combinators_2.11/1.0.4/scala-parser-combinators_2.11-1.0.4.jar:/home/cass/.m2/repository/commons-cli/commons-cli/1.2/commons-cli-1.2.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-graphite/3.1.2/metrics-graphite-3.1.2.jar:/home/cass/.m2/repository/org/objenesis/objenesis/2.1/objenesis-2.1.jar:/home/cass/.m2/repository/javax/annotation/javax.annotation-api/1.2/javax.annotation-api-1.2.jar:/home/cass/.m2/repository/org/slf4j/slf4j-log4j12/1.7.16/slf4j-log4j12-1.7.16.jar:/home/cass/spark2/spark/core/target/spark-core_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/glassfish/jersey/media/jersey-media-jaxb/2.22.2/jersey-media-jaxb-2.22.2.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-core/2.5.3/jackson-core-2.5.3.jar:/home/cass/.m2/repository/org/spark-project/spark/unused/1.0.0/unused-1.0.0.jar:/home/cass/.m2/repository/org/apache/avro/avro-ipc/1.7.7/avro-ipc-1.7.7.jar:/home/cass/.m2/repository/commons-collections/commons-collections/3.2.2/commons-collections-3.2.2.jar:/home/cass/.m2/repository/com/twitter/chill_2.11/0.8.0/chill_2.11-0.8.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-locator/2.4.0-b34/hk2-locator-2.4.0-b34.jar:/home/cass/.m2/repository/org/slf4j/jcl-over-slf4j/1.7.16/jcl-over-slf4j-1.7.16.jar:/home/cass/.m2/repository/commons-httpclient/commons-httpclient/3.1/commons-httpclient-3.1.jar:/home/cass/.m2/repository/io/netty/netty-all/4.0.29.Final/netty-all-4.0.29.Final.jar:/home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-remote-resources-plugin:1.5:process (default) @ spark-graphx_2.11 ---
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ spark-graphx_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/graphx/src/main/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:compile (scala-compile-first) @ spark-graphx_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 37 Scala sources and 5 Java sources to /home/cass/spark2/spark/graphx/target/scala-2.11/classes...
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] 1 warning
[info] Compile success at May 20, 2016 12:31:50 PM [5.443s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:compile (default-compile) @ spark-graphx_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 5 source files to /home/cass/spark2/spark/graphx/target/scala-2.11/classes
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (create-tmp-dir) @ spark-graphx_2.11 ---
[INFO] Executing tasks

main:
    [mkdir] Created dir: /home/cass/spark2/spark/graphx/target/tmp
[INFO] Executed tasks
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ spark-graphx_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 2 resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:testCompile (scala-test-compile-first) @ spark-graphx_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 19 Scala sources to /home/cass/spark2/spark/graphx/target/scala-2.11/test-classes...
[info] Compile success at May 20, 2016 12:31:54 PM [4.220s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:testCompile (default-testCompile) @ spark-graphx_2.11 ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (generate-test-classpath) @ spark-graphx_2.11 ---
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (default-test) @ spark-graphx_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (test) @ spark-graphx_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- scalatest-maven-plugin:1.0:test (test) @ spark-graphx_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (prepare-test-jar) @ spark-graphx_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/graphx/target/spark-graphx_2.11-2.0.0-SNAPSHOT-tests.jar
[INFO]
[INFO] --- maven-jar-plugin:2.6:jar (default-jar) @ spark-graphx_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/graphx/target/spark-graphx_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-site-plugin:3.3:attach-descriptor (attach-descriptor) @ spark-graphx_2.11 ---
[INFO]
[INFO] --- maven-shade-plugin:2.4.3:shade (default) @ spark-graphx_2.11 ---
[INFO] Excluding org.apache.spark:spark-core_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.avro:avro-mapred:jar:hadoop2:1.7.7 from the shaded jar.
[INFO] Excluding org.apache.avro:avro-ipc:jar:1.7.7 from the shaded jar.
[INFO] Excluding org.apache.avro:avro:jar:1.7.7 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-core-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-mapper-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding com.twitter:chill_2.11:jar:0.8.0 from the shaded jar.
[INFO] Excluding com.esotericsoftware:kryo-shaded:jar:3.0.3 from the shaded jar.
[INFO] Excluding com.esotericsoftware:minlog:jar:1.3.0 from the shaded jar.
[INFO] Excluding org.objenesis:objenesis:jar:2.1 from the shaded jar.
[INFO] Excluding com.twitter:chill-java:jar:0.8.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding commons-cli:commons-cli:jar:1.2 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-math:jar:2.1 from the shaded jar.
[INFO] Excluding xmlenc:xmlenc:jar:0.52 from the shaded jar.
[INFO] Excluding commons-io:commons-io:jar:2.4 from the shaded jar.
[INFO] Excluding commons-lang:commons-lang:jar:2.6 from the shaded jar.
[INFO] Excluding commons-configuration:commons-configuration:jar:1.6 from the shaded jar.
[INFO] Excluding commons-collections:commons-collections:jar:3.2.2 from the shaded jar.
[INFO] Excluding commons-digester:commons-digester:jar:1.8 from the shaded jar.
[INFO] Excluding commons-beanutils:commons-beanutils:jar:1.7.0 from the shaded jar.
[INFO] Excluding commons-beanutils:commons-beanutils-core:jar:1.8.0 from the shaded jar.
[INFO] Excluding com.google.protobuf:protobuf-java:jar:2.5.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-auth:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-compress:jar:1.4.1 from the shaded jar.
[INFO] Excluding org.tukaani:xz:jar:1.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-hdfs:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.mortbay.jetty:jetty-util:jar:6.1.26 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-app:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding com.google.inject:guice:jar:3.0 from the shaded jar.
[INFO] Excluding javax.inject:javax.inject:jar:1 from the shaded jar.
[INFO] Excluding aopalliance:aopalliance:jar:1.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-server-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-shuffle:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-api:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-core:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-jobclient:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-annotations:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-launcher_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-network-common_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-network-shuffle_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.fusesource.leveldbjni:leveldbjni-all:jar:1.8 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-annotations:jar:2.5.3 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-unsafe_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding net.java.dev.jets3t:jets3t:jar:0.7.1 from the shaded jar.
[INFO] Excluding commons-codec:commons-codec:jar:1.10 from the shaded jar.
[INFO] Excluding commons-httpclient:commons-httpclient:jar:3.1 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-recipes:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-framework:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-client:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.zookeeper:zookeeper:jar:3.4.5 from the shaded jar.
[INFO] Excluding javax.servlet:javax.servlet-api:jar:3.1.0 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-lang3:jar:3.3.2 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-math3:jar:3.4.1 from the shaded jar.
[INFO] Excluding com.google.code.findbugs:jsr305:jar:1.3.9 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-api:jar:1.7.16 from the shaded jar.
[INFO] Excluding org.slf4j:jul-to-slf4j:jar:1.7.16 from the shaded jar.
[INFO] Excluding org.slf4j:jcl-over-slf4j:jar:1.7.16 from the shaded jar.
[INFO] Excluding log4j:log4j:jar:1.2.17 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-log4j12:jar:1.7.16 from the shaded jar.
[INFO] Excluding com.ning:compress-lzf:jar:1.0.3 from the shaded jar.
[INFO] Excluding org.xerial.snappy:snappy-java:jar:1.1.2.4 from the shaded jar.
[INFO] Excluding net.jpountz.lz4:lz4:jar:1.3.0 from the shaded jar.
[INFO] Excluding org.roaringbitmap:RoaringBitmap:jar:0.5.11 from the shaded jar.
[INFO] Excluding commons-net:commons-net:jar:2.2 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-library:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.json4s:json4s-jackson_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.json4s:json4s-core_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.json4s:json4s-ast_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.scala-lang:scalap:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-compiler:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-parser-combinators_2.11:jar:1.0.4 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-client:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.ws.rs:javax.ws.rs-api:jar:2.0.1 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-api:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-utils:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2.external:aopalliance-repackaged:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2.external:javax.inject:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-locator:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.javassist:javassist:jar:3.18.1-GA from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-common:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.annotation:javax.annotation-api:jar:1.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.bundles.repackaged:jersey-guava:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:osgi-resource-locator:jar:1.0.1 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-server:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.media:jersey-media-jaxb:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.validation:validation-api:jar:1.1.0.Final from the shaded jar.
[INFO] Excluding org.glassfish.jersey.containers:jersey-container-servlet:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.containers:jersey-container-servlet-core:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.apache.mesos:mesos:jar:shaded-protobuf:0.21.1 from the shaded jar.
[INFO] Excluding io.netty:netty-all:jar:4.0.29.Final from the shaded jar.
[INFO] Excluding io.netty:netty:jar:3.8.0.Final from the shaded jar.
[INFO] Excluding com.clearspring.analytics:stream:jar:2.7.0 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-core:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-jvm:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-json:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-graphite:jar:3.1.2 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-databind:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-core:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.module:jackson-module-scala_2.11:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.thoughtworks.paranamer:paranamer:jar:2.6 from the shaded jar.
[INFO] Excluding org.apache.ivy:ivy:jar:2.4.0 from the shaded jar.
[INFO] Excluding oro:oro:jar:2.0.8 from the shaded jar.
[INFO] Excluding net.razorvine:pyrolite:jar:4.9 from the shaded jar.
[INFO] Excluding net.sf.py4j:py4j:jar:0.10.1 from the shaded jar.
[INFO] Excluding org.apache.xbean:xbean-asm5-shaded:jar:4.4 from the shaded jar.
[INFO] Excluding com.github.fommil.netlib:core:jar:1.1.2 from the shaded jar.
[INFO] Excluding net.sourceforge.f2j:arpack_combined_all:jar:0.1 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-tags_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Including org.spark-project.spark:unused:jar:1.0.0 in the shaded jar.
[INFO] Excluding org.scala-lang:scala-reflect:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-xml_2.11:jar:1.0.2 from the shaded jar.
[INFO] Replacing original artifact with shaded artifact.
[INFO] Replacing /home/cass/spark2/spark/graphx/target/spark-graphx_2.11-2.0.0-SNAPSHOT.jar with /home/cass/spark2/spark/graphx/target/spark-graphx_2.11-2.0.0-SNAPSHOT-shaded.jar
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/graphx/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/graphx/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/graphx/dependency-reduced-pom.xml
[INFO]
[INFO] --- maven-source-plugin:2.4:jar-no-fork (create-source-jar) @ spark-graphx_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/graphx/target/spark-graphx_2.11-2.0.0-SNAPSHOT-sources.jar
[INFO]
[INFO] --- maven-source-plugin:2.4:test-jar-no-fork (create-source-jar) @ spark-graphx_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/graphx/target/spark-graphx_2.11-2.0.0-SNAPSHOT-test-sources.jar
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Spark Project Streaming 2.0.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.0.0:clean (default-clean) @ spark-streaming_2.11 ---
[INFO]
[INFO] --- maven-enforcer-plugin:1.4.1:enforce (enforce-versions) @ spark-streaming_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:add-source (eclipse-add-source) @ spark-streaming_2.11 ---
[INFO] Add Source directory: /home/cass/spark2/spark/streaming/src/main/scala
[INFO] Add Test Source directory: /home/cass/spark2/spark/streaming/src/test/scala
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (default-cli) @ spark-streaming_2.11 ---
[INFO] Dependencies classpath:
/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-jobclient/2.2.0/hadoop-mapreduce-client-jobclient-2.2.0.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-core/3.1.2/metrics-core-3.1.2.jar:/home/cass/.m2/repository/com/google/protobuf/protobuf-java/2.5.0/protobuf-java-2.5.0.jar:/home/cass/.m2/repository/aopalliance/aopalliance/1.0/aopalliance-1.0.jar:/home/cass/.m2/repository/net/razorvine/pyrolite/4.9/pyrolite-4.9.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-jvm/3.1.2/metrics-jvm-3.1.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-client/2.2.0/hadoop-client-2.2.0.jar:/home/cass/.m2/repository/org/fusesource/leveldbjni/leveldbjni-all/1.8/leveldbjni-all-1.8.jar:/home/cass/.m2/repository/org/glassfish/jersey/bundles/repackaged/jersey-guava/2.22.2/jersey-guava-2.22.2.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-json/3.1.2/metrics-json-3.1.2.jar:/home/cass/.m2/repository/net/java/dev/jets3t/jets3t/0.7.1/jets3t-0.7.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-common/2.2.0/hadoop-common-2.2.0.jar:/home/cass/.m2/repository/com/google/inject/guice/3.0/guice-3.0.jar:/home/cass/.m2/repository/commons-io/commons-io/2.4/commons-io-2.4.jar:/home/cass/.m2/repository/org/scala-lang/scala-reflect/2.11.8/scala-reflect-2.11.8.jar:/home/cass/.m2/repository/org/xerial/snappy/snappy-java/1.1.2.4/snappy-java-1.1.2.4.jar:/home/cass/.m2/repository/org/json4s/json4s-jackson_2.11/3.2.11/json4s-jackson_2.11-3.2.11.jar:/home/cass/.m2/repository/com/esotericsoftware/minlog/1.3.0/minlog-1.3.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-auth/2.2.0/hadoop-auth-2.2.0.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-core-asl/1.9.13/jackson-core-asl-1.9.13.jar:/home/cass/.m2/repository/javax/validation/validation-api/1.1.0.Final/validation-api-1.1.0.Final.jar:/home/cass/.m2/repository/net/jpountz/lz4/lz4/1.3.0/lz4-1.3.0.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-common/2.22.2/jersey-common-2.22.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-client/2.2.0/hadoop-yarn-client-2.2.0.jar:/home/cass/.m2/repository/io/netty/netty/3.8.0.Final/netty-3.8.0.Final.jar:/home/cass/.m2/repository/org/apache/mesos/mesos/0.21.1/mesos-0.21.1-shaded-protobuf.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-annotations/2.5.3/jackson-annotations-2.5.3.jar:/home/cass/.m2/repository/com/google/code/findbugs/jsr305/1.3.9/jsr305-1.3.9.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-api/2.4.0-b34/hk2-api-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-server/2.22.2/jersey-server-2.22.2.jar:/home/cass/.m2/repository/net/sf/py4j/py4j/0.10.1/py4j-0.10.1.jar:/home/cass/.m2/repository/com/twitter/chill-java/0.8.0/chill-java-0.8.0.jar:/home/cass/.m2/repository/commons-lang/commons-lang/2.6/commons-lang-2.6.jar:/home/cass/.m2/repository/org/tukaani/xz/1.0/xz-1.0.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-databind/2.5.3/jackson-databind-2.5.3.jar:/home/cass/.m2/repository/commons-codec/commons-codec/1.10/commons-codec-1.10.jar:/home/cass/.m2/repository/org/apache/curator/curator-recipes/2.4.0/curator-recipes-2.4.0.jar:/home/cass/.m2/repository/org/javassist/javassist/3.18.1-GA/javassist-3.18.1-GA.jar:/home/cass/.m2/repository/org/apache/ivy/ivy/2.4.0/ivy-2.4.0.jar:/home/cass/.m2/repository/javax/inject/javax.inject/1/javax.inject-1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-core/2.2.0/hadoop-mapreduce-client-core-2.2.0.jar:/home/cass/.m2/repository/com/fasterxml/jackson/module/jackson-module-scala_2.11/2.5.3/jackson-module-scala_2.11-2.5.3.jar:/home/cass/.m2/repository/commons-beanutils/commons-beanutils-core/1.8.0/commons-beanutils-core-1.8.0.jar:/home/cass/.m2/repository/javax/servlet/javax.servlet-api/3.1.0/javax.servlet-api-3.1.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/osgi-resource-locator/1.0.1/osgi-resource-locator-1.0.1.jar:/home/cass/.m2/repository/org/apache/commons/commons-math3/3.4.1/commons-math3-3.4.1.jar:/home/cass/spark2/spark/common/network-common/target/spark-network-common_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/avro/avro/1.7.7/avro-1.7.7.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-common/2.2.0/hadoop-mapreduce-client-common-2.2.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-utils/2.4.0-b34/hk2-utils-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/hk2/external/aopalliance-repackaged/2.4.0-b34/aopalliance-repackaged-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/hk2/external/javax.inject/2.4.0-b34/javax.inject-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/jersey/containers/jersey-container-servlet-core/2.22.2/jersey-container-servlet-core-2.22.2.jar:/home/cass/.m2/repository/oro/oro/2.0.8/oro-2.0.8.jar:/home/cass/.m2/repository/org/scala-lang/scala-compiler/2.11.8/scala-compiler-2.11.8.jar:/home/cass/.m2/repository/org/roaringbitmap/RoaringBitmap/0.5.11/RoaringBitmap-0.5.11.jar:/home/cass/.m2/repository/log4j/log4j/1.2.17/log4j-1.2.17.jar:/home/cass/.m2/repository/org/scala-lang/scala-library/2.11.8/scala-library-2.11.8.jar:/home/cass/.m2/repository/org/apache/curator/curator-client/2.4.0/curator-client-2.4.0.jar:/home/cass/.m2/repository/org/apache/commons/commons-compress/1.4.1/commons-compress-1.4.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-app/2.2.0/hadoop-mapreduce-client-app-2.2.0.jar:/home/cass/.m2/repository/org/slf4j/slf4j-api/1.7.16/slf4j-api-1.7.16.jar:/home/cass/.m2/repository/org/apache/xbean/xbean-asm5-shaded/4.4/xbean-asm5-shaded-4.4.jar:/home/cass/.m2/repository/org/json4s/json4s-core_2.11/3.2.11/json4s-core_2.11-3.2.11.jar:/home/cass/.m2/repository/org/mortbay/jetty/jetty-util/6.1.26/jetty-util-6.1.26.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-server-common/2.2.0/hadoop-yarn-server-common-2.2.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-hdfs/2.2.0/hadoop-hdfs-2.2.0.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-mapper-asl/1.9.13/jackson-mapper-asl-1.9.13.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-api/2.2.0/hadoop-yarn-api-2.2.0.jar:/home/cass/.m2/repository/com/esotericsoftware/kryo-shaded/3.0.3/kryo-shaded-3.0.3.jar:/home/cass/.m2/repository/javax/ws/rs/javax.ws.rs-api/2.0.1/javax.ws.rs-api-2.0.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-common/2.2.0/hadoop-yarn-common-2.2.0.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-client/2.22.2/jersey-client-2.22.2.jar:/home/cass/spark2/spark/common/unsafe/target/spark-unsafe_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/avro/avro-mapred/1.7.7/avro-mapred-1.7.7-hadoop2.jar:/home/cass/.m2/repository/xmlenc/xmlenc/0.52/xmlenc-0.52.jar:/home/cass/.m2/repository/com/ning/compress-lzf/1.0.3/compress-lzf-1.0.3.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-shuffle/2.2.0/hadoop-mapreduce-client-shuffle-2.2.0.jar:/home/cass/.m2/repository/org/apache/zookeeper/zookeeper/3.4.5/zookeeper-3.4.5.jar:/home/cass/.m2/repository/org/apache/curator/curator-framework/2.4.0/curator-framework-2.4.0.jar:/home/cass/.m2/repository/commons-net/commons-net/2.2/commons-net-2.2.jar:/home/cass/.m2/repository/org/apache/commons/commons-lang3/3.3.2/commons-lang3-3.3.2.jar:/home/cass/.m2/repository/org/json4s/json4s-ast_2.11/3.2.11/json4s-ast_2.11-3.2.11.jar:/home/cass/spark2/spark/launcher/target/spark-launcher_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/scala-lang/scalap/2.11.8/scalap-2.11.8.jar:/home/cass/.m2/repository/com/clearspring/analytics/stream/2.7.0/stream-2.7.0.jar:/home/cass/.m2/repository/org/apache/commons/commons-math/2.1/commons-math-2.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-annotations/2.2.0/hadoop-annotations-2.2.0.jar:/home/cass/.m2/repository/com/thoughtworks/paranamer/paranamer/2.6/paranamer-2.6.jar:/home/cass/.m2/repository/commons-configuration/commons-configuration/1.6/commons-configuration-1.6.jar:/home/cass/.m2/repository/org/glassfish/jersey/containers/jersey-container-servlet/2.22.2/jersey-container-servlet-2.22.2.jar:/home/cass/.m2/repository/commons-digester/commons-digester/1.8/commons-digester-1.8.jar:/home/cass/.m2/repository/org/slf4j/jul-to-slf4j/1.7.16/jul-to-slf4j-1.7.16.jar:/home/cass/.m2/repository/commons-beanutils/commons-beanutils/1.7.0/commons-beanutils-1.7.0.jar:/home/cass/spark2/spark/common/network-shuffle/target/spark-network-shuffle_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-xml_2.11/1.0.2/scala-xml_2.11-1.0.2.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-parser-combinators_2.11/1.0.4/scala-parser-combinators_2.11-1.0.4.jar:/home/cass/.m2/repository/commons-cli/commons-cli/1.2/commons-cli-1.2.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-graphite/3.1.2/metrics-graphite-3.1.2.jar:/home/cass/.m2/repository/javax/annotation/javax.annotation-api/1.2/javax.annotation-api-1.2.jar:/home/cass/.m2/repository/org/objenesis/objenesis/2.1/objenesis-2.1.jar:/home/cass/.m2/repository/org/slf4j/slf4j-log4j12/1.7.16/slf4j-log4j12-1.7.16.jar:/home/cass/spark2/spark/core/target/spark-core_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/glassfish/jersey/media/jersey-media-jaxb/2.22.2/jersey-media-jaxb-2.22.2.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-core/2.5.3/jackson-core-2.5.3.jar:/home/cass/.m2/repository/org/spark-project/spark/unused/1.0.0/unused-1.0.0.jar:/home/cass/.m2/repository/org/apache/avro/avro-ipc/1.7.7/avro-ipc-1.7.7.jar:/home/cass/.m2/repository/commons-collections/commons-collections/3.2.2/commons-collections-3.2.2.jar:/home/cass/.m2/repository/com/twitter/chill_2.11/0.8.0/chill_2.11-0.8.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-locator/2.4.0-b34/hk2-locator-2.4.0-b34.jar:/home/cass/.m2/repository/org/slf4j/jcl-over-slf4j/1.7.16/jcl-over-slf4j-1.7.16.jar:/home/cass/.m2/repository/commons-httpclient/commons-httpclient/3.1/commons-httpclient-3.1.jar:/home/cass/.m2/repository/io/netty/netty-all/4.0.29.Final/netty-all-4.0.29.Final.jar:/home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-remote-resources-plugin:1.5:process (default) @ spark-streaming_2.11 ---
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ spark-streaming_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 2 resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:compile (scala-compile-first) @ spark-streaming_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 100 Scala sources and 5 Java sources to /home/cass/spark2/spark/streaming/target/scala-2.11/classes...
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] 1 warning
[info] Compile success at May 20, 2016 12:32:05 PM [9.657s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:compile (default-compile) @ spark-streaming_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 5 source files to /home/cass/spark2/spark/streaming/target/scala-2.11/classes
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (create-tmp-dir) @ spark-streaming_2.11 ---
[INFO] Executing tasks

main:
    [mkdir] Created dir: /home/cass/spark2/spark/streaming/target/tmp
[INFO] Executed tasks
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ spark-streaming_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 1 resource
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:testCompile (scala-test-compile-first) @ spark-streaming_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 40 Scala sources and 8 Java sources to /home/cass/spark2/spark/streaming/target/scala-2.11/test-classes...
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] /home/cass/spark2/spark/streaming/src/test/java/org/apache/spark/streaming/JavaAPISuite.java:39: warning: [deprecation] Accumulator in org.apache.spark has been deprecated
[warn] import org.apache.spark.Accumulator;
[warn]                        ^
[warn] /home/cass/spark2/spark/streaming/src/test/java/org/apache/spark/streaming/JavaAPISuite.java:797: warning: [deprecation] Accumulator in org.apache.spark has been deprecated
[warn]     final Accumulator<Integer> accumRdd = ssc.sparkContext().accumulator(0);
[warn]           ^
[warn] /home/cass/spark2/spark/streaming/src/test/java/org/apache/spark/streaming/JavaAPISuite.java:798: warning: [deprecation] Accumulator in org.apache.spark has been deprecated
[warn]     final Accumulator<Integer> accumEle = ssc.sparkContext().accumulator(0);
[warn]           ^
[warn] 4 warnings
[info] Compile success at May 20, 2016 12:32:19 PM [12.903s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:testCompile (default-testCompile) @ spark-streaming_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 8 source files to /home/cass/spark2/spark/streaming/target/scala-2.11/test-classes
[WARNING] /home/cass/spark2/spark/streaming/src/test/java/org/apache/spark/streaming/JavaAPISuite.java:[39,23] [deprecation] Accumulator in org.apache.spark has been deprecated
[WARNING] /home/cass/spark2/spark/streaming/src/test/java/org/apache/spark/streaming/JavaAPISuite.java:[797,10] [deprecation] Accumulator in org.apache.spark has been deprecated
[WARNING] /home/cass/spark2/spark/streaming/src/test/java/org/apache/spark/streaming/JavaAPISuite.java:[798,10] [deprecation] Accumulator in org.apache.spark has been deprecated
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (generate-test-classpath) @ spark-streaming_2.11 ---
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (default-test) @ spark-streaming_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (test) @ spark-streaming_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- scalatest-maven-plugin:1.0:test (test) @ spark-streaming_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (prepare-test-jar) @ spark-streaming_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/streaming/target/spark-streaming_2.11-2.0.0-SNAPSHOT-tests.jar
[INFO]
[INFO] --- maven-jar-plugin:2.6:jar (default-jar) @ spark-streaming_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/streaming/target/spark-streaming_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-site-plugin:3.3:attach-descriptor (attach-descriptor) @ spark-streaming_2.11 ---
[INFO]
[INFO] --- maven-shade-plugin:2.4.3:shade (default) @ spark-streaming_2.11 ---
[INFO] Excluding org.apache.spark:spark-core_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.avro:avro-mapred:jar:hadoop2:1.7.7 from the shaded jar.
[INFO] Excluding org.apache.avro:avro-ipc:jar:1.7.7 from the shaded jar.
[INFO] Excluding org.apache.avro:avro:jar:1.7.7 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-core-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-mapper-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding com.twitter:chill_2.11:jar:0.8.0 from the shaded jar.
[INFO] Excluding com.esotericsoftware:kryo-shaded:jar:3.0.3 from the shaded jar.
[INFO] Excluding com.esotericsoftware:minlog:jar:1.3.0 from the shaded jar.
[INFO] Excluding com.twitter:chill-java:jar:0.8.0 from the shaded jar.
[INFO] Excluding org.apache.xbean:xbean-asm5-shaded:jar:4.4 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding commons-cli:commons-cli:jar:1.2 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-math:jar:2.1 from the shaded jar.
[INFO] Excluding xmlenc:xmlenc:jar:0.52 from the shaded jar.
[INFO] Excluding commons-lang:commons-lang:jar:2.6 from the shaded jar.
[INFO] Excluding commons-configuration:commons-configuration:jar:1.6 from the shaded jar.
[INFO] Excluding commons-digester:commons-digester:jar:1.8 from the shaded jar.
[INFO] Excluding commons-beanutils:commons-beanutils:jar:1.7.0 from the shaded jar.
[INFO] Excluding commons-beanutils:commons-beanutils-core:jar:1.8.0 from the shaded jar.
[INFO] Excluding com.google.protobuf:protobuf-java:jar:2.5.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-auth:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-compress:jar:1.4.1 from the shaded jar.
[INFO] Excluding org.tukaani:xz:jar:1.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-hdfs:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.mortbay.jetty:jetty-util:jar:6.1.26 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-app:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding com.google.inject:guice:jar:3.0 from the shaded jar.
[INFO] Excluding javax.inject:javax.inject:jar:1 from the shaded jar.
[INFO] Excluding aopalliance:aopalliance:jar:1.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-server-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-shuffle:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-api:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-core:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-jobclient:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-annotations:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-launcher_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-network-common_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-network-shuffle_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.fusesource.leveldbjni:leveldbjni-all:jar:1.8 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-annotations:jar:2.5.3 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-unsafe_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding net.java.dev.jets3t:jets3t:jar:0.7.1 from the shaded jar.
[INFO] Excluding commons-codec:commons-codec:jar:1.10 from the shaded jar.
[INFO] Excluding commons-httpclient:commons-httpclient:jar:3.1 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-recipes:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-framework:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-client:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.zookeeper:zookeeper:jar:3.4.5 from the shaded jar.
[INFO] Excluding javax.servlet:javax.servlet-api:jar:3.1.0 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-lang3:jar:3.3.2 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-math3:jar:3.4.1 from the shaded jar.
[INFO] Excluding com.google.code.findbugs:jsr305:jar:1.3.9 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-api:jar:1.7.16 from the shaded jar.
[INFO] Excluding org.slf4j:jul-to-slf4j:jar:1.7.16 from the shaded jar.
[INFO] Excluding org.slf4j:jcl-over-slf4j:jar:1.7.16 from the shaded jar.
[INFO] Excluding log4j:log4j:jar:1.2.17 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-log4j12:jar:1.7.16 from the shaded jar.
[INFO] Excluding com.ning:compress-lzf:jar:1.0.3 from the shaded jar.
[INFO] Excluding org.xerial.snappy:snappy-java:jar:1.1.2.4 from the shaded jar.
[INFO] Excluding net.jpountz.lz4:lz4:jar:1.3.0 from the shaded jar.
[INFO] Excluding org.roaringbitmap:RoaringBitmap:jar:0.5.11 from the shaded jar.
[INFO] Excluding commons-net:commons-net:jar:2.2 from the shaded jar.
[INFO] Excluding org.json4s:json4s-jackson_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.json4s:json4s-core_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.json4s:json4s-ast_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.scala-lang:scalap:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-compiler:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-parser-combinators_2.11:jar:1.0.4 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-client:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.ws.rs:javax.ws.rs-api:jar:2.0.1 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-api:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-utils:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2.external:aopalliance-repackaged:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2.external:javax.inject:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-locator:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.javassist:javassist:jar:3.18.1-GA from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-common:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.annotation:javax.annotation-api:jar:1.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.bundles.repackaged:jersey-guava:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:osgi-resource-locator:jar:1.0.1 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-server:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.media:jersey-media-jaxb:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.validation:validation-api:jar:1.1.0.Final from the shaded jar.
[INFO] Excluding org.glassfish.jersey.containers:jersey-container-servlet:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.containers:jersey-container-servlet-core:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.apache.mesos:mesos:jar:shaded-protobuf:0.21.1 from the shaded jar.
[INFO] Excluding io.netty:netty-all:jar:4.0.29.Final from the shaded jar.
[INFO] Excluding io.netty:netty:jar:3.8.0.Final from the shaded jar.
[INFO] Excluding com.clearspring.analytics:stream:jar:2.7.0 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-core:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-jvm:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-json:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-graphite:jar:3.1.2 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-databind:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-core:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.module:jackson-module-scala_2.11:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.thoughtworks.paranamer:paranamer:jar:2.6 from the shaded jar.
[INFO] Excluding org.apache.ivy:ivy:jar:2.4.0 from the shaded jar.
[INFO] Excluding oro:oro:jar:2.0.8 from the shaded jar.
[INFO] Excluding net.razorvine:pyrolite:jar:4.9 from the shaded jar.
[INFO] Excluding net.sf.py4j:py4j:jar:0.10.1 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-tags_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.scala-lang:scala-library:jar:2.11.8 from the shaded jar.
[INFO] Excluding commons-io:commons-io:jar:2.4 from the shaded jar.
[INFO] Excluding commons-collections:commons-collections:jar:3.2.2 from the shaded jar.
[INFO] Excluding org.objenesis:objenesis:jar:2.1 from the shaded jar.
[INFO] Including org.spark-project.spark:unused:jar:1.0.0 in the shaded jar.
[INFO] Excluding org.scala-lang:scala-reflect:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-xml_2.11:jar:1.0.2 from the shaded jar.
[INFO] Replacing original artifact with shaded artifact.
[INFO] Replacing /home/cass/spark2/spark/streaming/target/spark-streaming_2.11-2.0.0-SNAPSHOT.jar with /home/cass/spark2/spark/streaming/target/spark-streaming_2.11-2.0.0-SNAPSHOT-shaded.jar
[INFO] Replacing original test artifact with shaded test artifact.
[INFO] Replacing /home/cass/spark2/spark/streaming/target/spark-streaming_2.11-2.0.0-SNAPSHOT-tests.jar with /home/cass/spark2/spark/streaming/target/spark-streaming_2.11-2.0.0-SNAPSHOT-shaded-tests.jar
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/streaming/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/streaming/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/streaming/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/streaming/dependency-reduced-pom.xml
[INFO]
[INFO] --- maven-source-plugin:2.4:jar-no-fork (create-source-jar) @ spark-streaming_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/streaming/target/spark-streaming_2.11-2.0.0-SNAPSHOT-sources.jar
[INFO]
[INFO] --- maven-source-plugin:2.4:test-jar-no-fork (create-source-jar) @ spark-streaming_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/streaming/target/spark-streaming_2.11-2.0.0-SNAPSHOT-test-sources.jar
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Spark Project Catalyst 2.0.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.0.0:clean (default-clean) @ spark-catalyst_2.11 ---
[INFO]
[INFO] --- maven-enforcer-plugin:1.4.1:enforce (enforce-versions) @ spark-catalyst_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:add-source (eclipse-add-source) @ spark-catalyst_2.11 ---
[INFO] Add Source directory: /home/cass/spark2/spark/sql/catalyst/src/main/scala
[INFO] Add Test Source directory: /home/cass/spark2/spark/sql/catalyst/src/test/scala
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (default-cli) @ spark-catalyst_2.11 ---
[INFO] Dependencies classpath:
/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-jobclient/2.2.0/hadoop-mapreduce-client-jobclient-2.2.0.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-core/3.1.2/metrics-core-3.1.2.jar:/home/cass/.m2/repository/com/google/protobuf/protobuf-java/2.5.0/protobuf-java-2.5.0.jar:/home/cass/.m2/repository/aopalliance/aopalliance/1.0/aopalliance-1.0.jar:/home/cass/.m2/repository/net/razorvine/pyrolite/4.9/pyrolite-4.9.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-jvm/3.1.2/metrics-jvm-3.1.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-client/2.2.0/hadoop-client-2.2.0.jar:/home/cass/.m2/repository/org/fusesource/leveldbjni/leveldbjni-all/1.8/leveldbjni-all-1.8.jar:/home/cass/.m2/repository/org/glassfish/jersey/bundles/repackaged/jersey-guava/2.22.2/jersey-guava-2.22.2.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-json/3.1.2/metrics-json-3.1.2.jar:/home/cass/.m2/repository/net/java/dev/jets3t/jets3t/0.7.1/jets3t-0.7.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-common/2.2.0/hadoop-common-2.2.0.jar:/home/cass/.m2/repository/com/google/inject/guice/3.0/guice-3.0.jar:/home/cass/.m2/repository/commons-io/commons-io/2.4/commons-io-2.4.jar:/home/cass/.m2/repository/org/scala-lang/scala-reflect/2.11.8/scala-reflect-2.11.8.jar:/home/cass/.m2/repository/org/xerial/snappy/snappy-java/1.1.2.4/snappy-java-1.1.2.4.jar:/home/cass/.m2/repository/org/json4s/json4s-jackson_2.11/3.2.11/json4s-jackson_2.11-3.2.11.jar:/home/cass/.m2/repository/com/esotericsoftware/minlog/1.3.0/minlog-1.3.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-auth/2.2.0/hadoop-auth-2.2.0.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-core-asl/1.9.13/jackson-core-asl-1.9.13.jar:/home/cass/.m2/repository/javax/validation/validation-api/1.1.0.Final/validation-api-1.1.0.Final.jar:/home/cass/.m2/repository/net/jpountz/lz4/lz4/1.3.0/lz4-1.3.0.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-common/2.22.2/jersey-common-2.22.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-client/2.2.0/hadoop-yarn-client-2.2.0.jar:/home/cass/.m2/repository/io/netty/netty/3.8.0.Final/netty-3.8.0.Final.jar:/home/cass/.m2/repository/org/apache/mesos/mesos/0.21.1/mesos-0.21.1-shaded-protobuf.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-annotations/2.5.3/jackson-annotations-2.5.3.jar:/home/cass/.m2/repository/com/google/code/findbugs/jsr305/1.3.9/jsr305-1.3.9.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-api/2.4.0-b34/hk2-api-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-server/2.22.2/jersey-server-2.22.2.jar:/home/cass/.m2/repository/net/sf/py4j/py4j/0.10.1/py4j-0.10.1.jar:/home/cass/.m2/repository/com/twitter/chill-java/0.8.0/chill-java-0.8.0.jar:/home/cass/.m2/repository/commons-lang/commons-lang/2.6/commons-lang-2.6.jar:/home/cass/.m2/repository/org/tukaani/xz/1.0/xz-1.0.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-databind/2.5.3/jackson-databind-2.5.3.jar:/home/cass/.m2/repository/org/codehaus/janino/janino/2.7.8/janino-2.7.8.jar:/home/cass/.m2/repository/org/apache/curator/curator-recipes/2.4.0/curator-recipes-2.4.0.jar:/home/cass/.m2/repository/commons-codec/commons-codec/1.10/commons-codec-1.10.jar:/home/cass/.m2/repository/org/javassist/javassist/3.18.1-GA/javassist-3.18.1-GA.jar:/home/cass/.m2/repository/org/apache/ivy/ivy/2.4.0/ivy-2.4.0.jar:/home/cass/.m2/repository/javax/inject/javax.inject/1/javax.inject-1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-core/2.2.0/hadoop-mapreduce-client-core-2.2.0.jar:/home/cass/.m2/repository/com/fasterxml/jackson/module/jackson-module-scala_2.11/2.5.3/jackson-module-scala_2.11-2.5.3.jar:/home/cass/.m2/repository/commons-beanutils/commons-beanutils-core/1.8.0/commons-beanutils-core-1.8.0.jar:/home/cass/.m2/repository/javax/servlet/javax.servlet-api/3.1.0/javax.servlet-api-3.1.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/osgi-resource-locator/1.0.1/osgi-resource-locator-1.0.1.jar:/home/cass/.m2/repository/org/apache/commons/commons-math3/3.4.1/commons-math3-3.4.1.jar:/home/cass/spark2/spark/common/network-common/target/spark-network-common_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/avro/avro/1.7.7/avro-1.7.7.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-common/2.2.0/hadoop-mapreduce-client-common-2.2.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-utils/2.4.0-b34/hk2-utils-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/hk2/external/aopalliance-repackaged/2.4.0-b34/aopalliance-repackaged-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/hk2/external/javax.inject/2.4.0-b34/javax.inject-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/jersey/containers/jersey-container-servlet-core/2.22.2/jersey-container-servlet-core-2.22.2.jar:/home/cass/.m2/repository/oro/oro/2.0.8/oro-2.0.8.jar:/home/cass/.m2/repository/org/scala-lang/scala-compiler/2.11.8/scala-compiler-2.11.8.jar:/home/cass/.m2/repository/org/roaringbitmap/RoaringBitmap/0.5.11/RoaringBitmap-0.5.11.jar:/home/cass/.m2/repository/log4j/log4j/1.2.17/log4j-1.2.17.jar:/home/cass/.m2/repository/org/scala-lang/scala-library/2.11.8/scala-library-2.11.8.jar:/home/cass/.m2/repository/org/codehaus/janino/commons-compiler/2.7.8/commons-compiler-2.7.8.jar:/home/cass/.m2/repository/org/apache/curator/curator-client/2.4.0/curator-client-2.4.0.jar:/home/cass/.m2/repository/org/apache/commons/commons-compress/1.4.1/commons-compress-1.4.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-app/2.2.0/hadoop-mapreduce-client-app-2.2.0.jar:/home/cass/.m2/repository/org/slf4j/slf4j-api/1.7.16/slf4j-api-1.7.16.jar:/home/cass/.m2/repository/org/apache/xbean/xbean-asm5-shaded/4.4/xbean-asm5-shaded-4.4.jar:/home/cass/.m2/repository/org/json4s/json4s-core_2.11/3.2.11/json4s-core_2.11-3.2.11.jar:/home/cass/.m2/repository/org/mortbay/jetty/jetty-util/6.1.26/jetty-util-6.1.26.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-server-common/2.2.0/hadoop-yarn-server-common-2.2.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-hdfs/2.2.0/hadoop-hdfs-2.2.0.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-mapper-asl/1.9.13/jackson-mapper-asl-1.9.13.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-api/2.2.0/hadoop-yarn-api-2.2.0.jar:/home/cass/.m2/repository/com/esotericsoftware/kryo-shaded/3.0.3/kryo-shaded-3.0.3.jar:/home/cass/.m2/repository/javax/ws/rs/javax.ws.rs-api/2.0.1/javax.ws.rs-api-2.0.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-common/2.2.0/hadoop-yarn-common-2.2.0.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-client/2.22.2/jersey-client-2.22.2.jar:/home/cass/spark2/spark/common/unsafe/target/spark-unsafe_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/avro/avro-mapred/1.7.7/avro-mapred-1.7.7-hadoop2.jar:/home/cass/.m2/repository/xmlenc/xmlenc/0.52/xmlenc-0.52.jar:/home/cass/.m2/repository/com/ning/compress-lzf/1.0.3/compress-lzf-1.0.3.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-shuffle/2.2.0/hadoop-mapreduce-client-shuffle-2.2.0.jar:/home/cass/.m2/repository/org/apache/zookeeper/zookeeper/3.4.5/zookeeper-3.4.5.jar:/home/cass/.m2/repository/org/apache/curator/curator-framework/2.4.0/curator-framework-2.4.0.jar:/home/cass/.m2/repository/commons-net/commons-net/2.2/commons-net-2.2.jar:/home/cass/.m2/repository/org/apache/commons/commons-lang3/3.3.2/commons-lang3-3.3.2.jar:/home/cass/.m2/repository/org/json4s/json4s-ast_2.11/3.2.11/json4s-ast_2.11-3.2.11.jar:/home/cass/spark2/spark/launcher/target/spark-launcher_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/scala-lang/scalap/2.11.8/scalap-2.11.8.jar:/home/cass/.m2/repository/com/clearspring/analytics/stream/2.7.0/stream-2.7.0.jar:/home/cass/.m2/repository/org/apache/commons/commons-math/2.1/commons-math-2.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-annotations/2.2.0/hadoop-annotations-2.2.0.jar:/home/cass/.m2/repository/com/thoughtworks/paranamer/paranamer/2.6/paranamer-2.6.jar:/home/cass/.m2/repository/commons-configuration/commons-configuration/1.6/commons-configuration-1.6.jar:/home/cass/.m2/repository/org/glassfish/jersey/containers/jersey-container-servlet/2.22.2/jersey-container-servlet-2.22.2.jar:/home/cass/.m2/repository/commons-digester/commons-digester/1.8/commons-digester-1.8.jar:/home/cass/.m2/repository/org/slf4j/jul-to-slf4j/1.7.16/jul-to-slf4j-1.7.16.jar:/home/cass/.m2/repository/commons-beanutils/commons-beanutils/1.7.0/commons-beanutils-1.7.0.jar:/home/cass/.m2/repository/org/antlr/antlr4-runtime/4.5.2-1/antlr4-runtime-4.5.2-1.jar:/home/cass/spark2/spark/common/network-shuffle/target/spark-network-shuffle_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-xml_2.11/1.0.2/scala-xml_2.11-1.0.2.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-parser-combinators_2.11/1.0.4/scala-parser-combinators_2.11-1.0.4.jar:/home/cass/.m2/repository/commons-cli/commons-cli/1.2/commons-cli-1.2.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-graphite/3.1.2/metrics-graphite-3.1.2.jar:/home/cass/.m2/repository/org/objenesis/objenesis/2.1/objenesis-2.1.jar:/home/cass/.m2/repository/javax/annotation/javax.annotation-api/1.2/javax.annotation-api-1.2.jar:/home/cass/.m2/repository/org/slf4j/slf4j-log4j12/1.7.16/slf4j-log4j12-1.7.16.jar:/home/cass/spark2/spark/core/target/spark-core_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/glassfish/jersey/media/jersey-media-jaxb/2.22.2/jersey-media-jaxb-2.22.2.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-core/2.5.3/jackson-core-2.5.3.jar:/home/cass/.m2/repository/org/spark-project/spark/unused/1.0.0/unused-1.0.0.jar:/home/cass/.m2/repository/org/apache/avro/avro-ipc/1.7.7/avro-ipc-1.7.7.jar:/home/cass/.m2/repository/commons-collections/commons-collections/3.2.2/commons-collections-3.2.2.jar:/home/cass/.m2/repository/com/twitter/chill_2.11/0.8.0/chill_2.11-0.8.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-locator/2.4.0-b34/hk2-locator-2.4.0-b34.jar:/home/cass/.m2/repository/org/slf4j/jcl-over-slf4j/1.7.16/jcl-over-slf4j-1.7.16.jar:/home/cass/.m2/repository/commons-httpclient/commons-httpclient/3.1/commons-httpclient-3.1.jar:/home/cass/.m2/repository/io/netty/netty-all/4.0.29.Final/netty-all-4.0.29.Final.jar:/home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- antlr4-maven-plugin:4.5.2-1:antlr4 (default) @ spark-catalyst_2.11 ---
[INFO] ANTLR 4: Processing source directory /home/cass/spark2/spark/sql/catalyst/src/main/antlr4
[INFO] Processing grammar: org/apache/spark/sql/catalyst/parser/SqlBase.g4
[INFO]
[INFO] --- maven-remote-resources-plugin:1.5:process (default) @ spark-catalyst_2.11 ---
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ spark-catalyst_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/sql/catalyst/src/main/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:compile (scala-compile-first) @ spark-catalyst_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 169 Scala sources and 21 Java sources to /home/cass/spark2/spark/sql/catalyst/target/scala-2.11/classes...
[warn] /home/cass/spark2/spark/sql/catalyst/src/main/scala/org/apache/spark/sql/catalyst/ScalaReflection.scala:392: method tpe in trait AnnotationApi is deprecated: Use `tree.tpe` instead
[warn]       case t if t.typeSymbol.annotations.exists(_.tpe =:= typeOf[SQLUserDefinedType]) =>
[warn]                                                   ^
[warn] /home/cass/spark2/spark/sql/catalyst/src/main/scala/org/apache/spark/sql/catalyst/ScalaReflection.scala:630: method tpe in trait AnnotationApi is deprecated: Use `tree.tpe` instead
[warn]         case t if t.typeSymbol.annotations.exists(_.tpe =:= typeOf[SQLUserDefinedType]) =>
[warn]                                                     ^
[warn] /home/cass/spark2/spark/sql/catalyst/src/main/scala/org/apache/spark/sql/catalyst/ScalaReflection.scala:722: method tpe in trait AnnotationApi is deprecated: Use `tree.tpe` instead
[warn]       case t if t.typeSymbol.annotations.exists(_.tpe =:= typeOf[SQLUserDefinedType]) =>
[warn]                                                   ^
[warn] /home/cass/spark2/spark/sql/catalyst/src/main/scala/org/apache/spark/sql/catalyst/ScalaReflection.scala:822: method normalize in class TypeApi is deprecated: Use `dealias` or `etaExpand` instead
[warn]     tag.in(mirror).tpe.normalize
[warn]                        ^
[warn] /home/cass/spark2/spark/sql/catalyst/src/main/scala/org/apache/spark/sql/catalyst/ScalaReflection.scala:863: value nme in trait StandardNames is deprecated: Use `termNames` instead
[warn]     val constructorSymbol = tpe.member(nme.CONSTRUCTOR)
[warn]                                        ^
[warn] /home/cass/spark2/spark/sql/catalyst/src/main/scala/org/apache/spark/sql/catalyst/ScalaReflection.scala:865: method paramss in trait MethodSymbolApi is deprecated: Use `paramLists` instead
[warn]       constructorSymbol.asMethod.paramss
[warn]                                  ^
[warn] /home/cass/spark2/spark/sql/catalyst/src/main/scala/org/apache/spark/sql/catalyst/ScalaReflection.scala:873: method paramss in trait MethodSymbolApi is deprecated: Use `paramLists` instead
[warn]         primaryConstructorSymbol.get.asMethod.paramss
[warn]                                               ^
[warn] /home/cass/spark2/spark/sql/catalyst/src/main/scala/org/apache/spark/sql/catalyst/expressions/codegen/package.scala:54: class AbstractFileClassLoader in package interpreter is deprecated: Use `scala.tools.nsc.util.AbstractFileClassLoader`
[warn]           .asInstanceOf[scala.tools.nsc.interpreter.AbstractFileClassLoader]
[warn]                                                     ^
[warn] 8 warnings found
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] 1 warning
[info] Compile success at May 20, 2016 12:32:55 PM [30.392s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:compile (default-compile) @ spark-catalyst_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 21 source files to /home/cass/spark2/spark/sql/catalyst/target/scala-2.11/classes
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (create-tmp-dir) @ spark-catalyst_2.11 ---
[INFO] Executing tasks

main:
    [mkdir] Created dir: /home/cass/spark2/spark/sql/catalyst/target/tmp
[INFO] Executed tasks
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ spark-catalyst_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 1 resource
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:testCompile (scala-test-compile-first) @ spark-catalyst_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 110 Scala sources and 1 Java source to /home/cass/spark2/spark/sql/catalyst/target/scala-2.11/test-classes...
[warn] /home/cass/spark2/spark/sql/catalyst/src/test/scala/org/apache/spark/sql/catalyst/ScalaReflectionSuite.scala:291: non-variable type argument org.apache.spark.sql.catalyst.util.GenericArrayData in type Class[org.apache.spark.sql.catalyst.util.GenericArrayData] (the underlying of Class[org.apache.spark.sql.catalyst.util.GenericArrayData]) is unchecked since it is eliminated by erasure
[warn]       .cls.isInstanceOf[Class[org.apache.spark.sql.catalyst.util.GenericArrayData]])
[warn]                        ^
[warn] /home/cass/spark2/spark/sql/catalyst/src/test/scala/org/apache/spark/sql/catalyst/ScalaReflectionSuite.scala:290: non-variable type argument org.apache.spark.sql.catalyst.util.GenericArrayData in type Class[org.apache.spark.sql.catalyst.util.GenericArrayData] (the underlying of Class[org.apache.spark.sql.catalyst.util.GenericArrayData]) is unchecked since it is eliminated by erasure
[warn]     assert(serializer.children.last.asInstanceOf[NewInstance]
[warn]           ^
[warn] /home/cass/spark2/spark/sql/catalyst/src/test/scala/org/apache/spark/sql/catalyst/encoders/ExpressionEncoderSuite.scala:342: non-variable type argument Any in type pattern Comparable[Any] is unchecked since it is eliminated by erasure
[warn]         case (left: Comparable[Any], right: Comparable[Any]) => left.compareTo(right) == 0
[warn]                     ^
[warn] /home/cass/spark2/spark/sql/catalyst/src/test/scala/org/apache/spark/sql/catalyst/encoders/ExpressionEncoderSuite.scala:342: non-variable type argument Any in type pattern Comparable[Any] is unchecked since it is eliminated by erasure
[warn]         case (left: Comparable[Any], right: Comparable[Any]) => left.compareTo(right) == 0
[warn]                                             ^
[warn] four warnings found
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] 1 warning
[info] Compile success at May 20, 2016 12:33:18 PM [20.412s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:testCompile (default-testCompile) @ spark-catalyst_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 1 source file to /home/cass/spark2/spark/sql/catalyst/target/scala-2.11/test-classes
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (generate-test-classpath) @ spark-catalyst_2.11 ---
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (test-jar-on-test-compile) @ spark-catalyst_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/sql/catalyst/target/spark-catalyst_2.11-2.0.0-SNAPSHOT-tests.jar
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (default-test) @ spark-catalyst_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (test) @ spark-catalyst_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- scalatest-maven-plugin:1.0:test (test) @ spark-catalyst_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (prepare-test-jar) @ spark-catalyst_2.11 ---
[INFO]
[INFO] --- maven-jar-plugin:2.6:jar (default-jar) @ spark-catalyst_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/sql/catalyst/target/spark-catalyst_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-site-plugin:3.3:attach-descriptor (attach-descriptor) @ spark-catalyst_2.11 ---
[INFO]
[INFO] --- maven-shade-plugin:2.4.3:shade (default) @ spark-catalyst_2.11 ---
[INFO] Excluding org.scala-lang:scala-reflect:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-library:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-core_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.avro:avro-mapred:jar:hadoop2:1.7.7 from the shaded jar.
[INFO] Excluding org.apache.avro:avro-ipc:jar:1.7.7 from the shaded jar.
[INFO] Excluding org.apache.avro:avro:jar:1.7.7 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-core-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-mapper-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding com.twitter:chill_2.11:jar:0.8.0 from the shaded jar.
[INFO] Excluding com.esotericsoftware:kryo-shaded:jar:3.0.3 from the shaded jar.
[INFO] Excluding com.esotericsoftware:minlog:jar:1.3.0 from the shaded jar.
[INFO] Excluding org.objenesis:objenesis:jar:2.1 from the shaded jar.
[INFO] Excluding com.twitter:chill-java:jar:0.8.0 from the shaded jar.
[INFO] Excluding org.apache.xbean:xbean-asm5-shaded:jar:4.4 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding commons-cli:commons-cli:jar:1.2 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-math:jar:2.1 from the shaded jar.
[INFO] Excluding xmlenc:xmlenc:jar:0.52 from the shaded jar.
[INFO] Excluding commons-io:commons-io:jar:2.4 from the shaded jar.
[INFO] Excluding commons-lang:commons-lang:jar:2.6 from the shaded jar.
[INFO] Excluding commons-configuration:commons-configuration:jar:1.6 from the shaded jar.
[INFO] Excluding commons-collections:commons-collections:jar:3.2.2 from the shaded jar.
[INFO] Excluding commons-digester:commons-digester:jar:1.8 from the shaded jar.
[INFO] Excluding commons-beanutils:commons-beanutils:jar:1.7.0 from the shaded jar.
[INFO] Excluding commons-beanutils:commons-beanutils-core:jar:1.8.0 from the shaded jar.
[INFO] Excluding com.google.protobuf:protobuf-java:jar:2.5.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-auth:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-compress:jar:1.4.1 from the shaded jar.
[INFO] Excluding org.tukaani:xz:jar:1.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-hdfs:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.mortbay.jetty:jetty-util:jar:6.1.26 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-app:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding com.google.inject:guice:jar:3.0 from the shaded jar.
[INFO] Excluding javax.inject:javax.inject:jar:1 from the shaded jar.
[INFO] Excluding aopalliance:aopalliance:jar:1.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-server-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-shuffle:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-api:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-core:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-jobclient:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-annotations:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-launcher_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-network-common_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-network-shuffle_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.fusesource.leveldbjni:leveldbjni-all:jar:1.8 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-annotations:jar:2.5.3 from the shaded jar.
[INFO] Excluding net.java.dev.jets3t:jets3t:jar:0.7.1 from the shaded jar.
[INFO] Excluding commons-httpclient:commons-httpclient:jar:3.1 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-recipes:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-framework:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-client:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.zookeeper:zookeeper:jar:3.4.5 from the shaded jar.
[INFO] Excluding javax.servlet:javax.servlet-api:jar:3.1.0 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-lang3:jar:3.3.2 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-math3:jar:3.4.1 from the shaded jar.
[INFO] Excluding com.google.code.findbugs:jsr305:jar:1.3.9 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-api:jar:1.7.16 from the shaded jar.
[INFO] Excluding org.slf4j:jul-to-slf4j:jar:1.7.16 from the shaded jar.
[INFO] Excluding org.slf4j:jcl-over-slf4j:jar:1.7.16 from the shaded jar.
[INFO] Excluding log4j:log4j:jar:1.2.17 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-log4j12:jar:1.7.16 from the shaded jar.
[INFO] Excluding com.ning:compress-lzf:jar:1.0.3 from the shaded jar.
[INFO] Excluding org.xerial.snappy:snappy-java:jar:1.1.2.4 from the shaded jar.
[INFO] Excluding net.jpountz.lz4:lz4:jar:1.3.0 from the shaded jar.
[INFO] Excluding org.roaringbitmap:RoaringBitmap:jar:0.5.11 from the shaded jar.
[INFO] Excluding commons-net:commons-net:jar:2.2 from the shaded jar.
[INFO] Excluding org.json4s:json4s-jackson_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.json4s:json4s-core_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.json4s:json4s-ast_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.scala-lang:scalap:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-compiler:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-parser-combinators_2.11:jar:1.0.4 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-client:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.ws.rs:javax.ws.rs-api:jar:2.0.1 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-api:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-utils:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2.external:aopalliance-repackaged:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2.external:javax.inject:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-locator:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.javassist:javassist:jar:3.18.1-GA from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-common:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.annotation:javax.annotation-api:jar:1.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.bundles.repackaged:jersey-guava:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:osgi-resource-locator:jar:1.0.1 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-server:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.media:jersey-media-jaxb:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.validation:validation-api:jar:1.1.0.Final from the shaded jar.
[INFO] Excluding org.glassfish.jersey.containers:jersey-container-servlet:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.containers:jersey-container-servlet-core:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.apache.mesos:mesos:jar:shaded-protobuf:0.21.1 from the shaded jar.
[INFO] Excluding io.netty:netty-all:jar:4.0.29.Final from the shaded jar.
[INFO] Excluding io.netty:netty:jar:3.8.0.Final from the shaded jar.
[INFO] Excluding com.clearspring.analytics:stream:jar:2.7.0 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-core:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-jvm:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-json:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-graphite:jar:3.1.2 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-databind:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-core:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.module:jackson-module-scala_2.11:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.thoughtworks.paranamer:paranamer:jar:2.6 from the shaded jar.
[INFO] Excluding org.apache.ivy:ivy:jar:2.4.0 from the shaded jar.
[INFO] Excluding oro:oro:jar:2.0.8 from the shaded jar.
[INFO] Excluding net.razorvine:pyrolite:jar:4.9 from the shaded jar.
[INFO] Excluding net.sf.py4j:py4j:jar:0.10.1 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-tags_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-unsafe_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.codehaus.janino:janino:jar:2.7.8 from the shaded jar.
[INFO] Excluding org.codehaus.janino:commons-compiler:jar:2.7.8 from the shaded jar.
[INFO] Excluding org.antlr:antlr4-runtime:jar:4.5.2-1 from the shaded jar.
[INFO] Excluding commons-codec:commons-codec:jar:1.10 from the shaded jar.
[INFO] Including org.spark-project.spark:unused:jar:1.0.0 in the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-xml_2.11:jar:1.0.2 from the shaded jar.
[INFO] Replacing original artifact with shaded artifact.
[INFO] Replacing /home/cass/spark2/spark/sql/catalyst/target/spark-catalyst_2.11-2.0.0-SNAPSHOT.jar with /home/cass/spark2/spark/sql/catalyst/target/spark-catalyst_2.11-2.0.0-SNAPSHOT-shaded.jar
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/sql/catalyst/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/sql/catalyst/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/sql/catalyst/dependency-reduced-pom.xml
[INFO]
[INFO] --- maven-source-plugin:2.4:jar-no-fork (create-source-jar) @ spark-catalyst_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/sql/catalyst/target/spark-catalyst_2.11-2.0.0-SNAPSHOT-sources.jar
[INFO]
[INFO] --- maven-source-plugin:2.4:test-jar-no-fork (create-source-jar) @ spark-catalyst_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/sql/catalyst/target/spark-catalyst_2.11-2.0.0-SNAPSHOT-test-sources.jar
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (default) @ spark-catalyst_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/sql/catalyst/target/spark-catalyst_2.11-2.0.0-SNAPSHOT-tests.jar
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Spark Project SQL 2.0.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.0.0:clean (default-clean) @ spark-sql_2.11 ---
[INFO]
[INFO] --- maven-enforcer-plugin:1.4.1:enforce (enforce-versions) @ spark-sql_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:add-source (eclipse-add-source) @ spark-sql_2.11 ---
[INFO] Add Source directory: /home/cass/spark2/spark/sql/core/src/main/scala
[INFO] Add Test Source directory: /home/cass/spark2/spark/sql/core/src/test/scala
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (default-cli) @ spark-sql_2.11 ---
[INFO] Dependencies classpath:
/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-jobclient/2.2.0/hadoop-mapreduce-client-jobclient-2.2.0.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-jackson/1.7.0/parquet-jackson-1.7.0.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-core/3.1.2/metrics-core-3.1.2.jar:/home/cass/.m2/repository/com/google/protobuf/protobuf-java/2.5.0/protobuf-java-2.5.0.jar:/home/cass/.m2/repository/aopalliance/aopalliance/1.0/aopalliance-1.0.jar:/home/cass/.m2/repository/net/razorvine/pyrolite/4.9/pyrolite-4.9.jar:/home/cass/.m2/repository/com/univocity/univocity-parsers/2.1.0/univocity-parsers-2.1.0.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-jvm/3.1.2/metrics-jvm-3.1.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-client/2.2.0/hadoop-client-2.2.0.jar:/home/cass/.m2/repository/org/fusesource/leveldbjni/leveldbjni-all/1.8/leveldbjni-all-1.8.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-format/2.3.0-incubating/parquet-format-2.3.0-incubating.jar:/home/cass/.m2/repository/org/glassfish/jersey/bundles/repackaged/jersey-guava/2.22.2/jersey-guava-2.22.2.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-json/3.1.2/metrics-json-3.1.2.jar:/home/cass/.m2/repository/net/java/dev/jets3t/jets3t/0.7.1/jets3t-0.7.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-common/2.2.0/hadoop-common-2.2.0.jar:/home/cass/.m2/repository/com/google/inject/guice/3.0/guice-3.0.jar:/home/cass/.m2/repository/commons-io/commons-io/2.4/commons-io-2.4.jar:/home/cass/.m2/repository/org/scala-lang/scala-reflect/2.11.8/scala-reflect-2.11.8.jar:/home/cass/.m2/repository/org/xerial/snappy/snappy-java/1.1.2.4/snappy-java-1.1.2.4.jar:/home/cass/.m2/repository/org/json4s/json4s-jackson_2.11/3.2.11/json4s-jackson_2.11-3.2.11.jar:/home/cass/.m2/repository/com/esotericsoftware/minlog/1.3.0/minlog-1.3.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-auth/2.2.0/hadoop-auth-2.2.0.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-core-asl/1.9.13/jackson-core-asl-1.9.13.jar:/home/cass/.m2/repository/javax/validation/validation-api/1.1.0.Final/validation-api-1.1.0.Final.jar:/home/cass/.m2/repository/net/jpountz/lz4/lz4/1.3.0/lz4-1.3.0.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-common/2.22.2/jersey-common-2.22.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-client/2.2.0/hadoop-yarn-client-2.2.0.jar:/home/cass/.m2/repository/io/netty/netty/3.8.0.Final/netty-3.8.0.Final.jar:/home/cass/.m2/repository/org/apache/mesos/mesos/0.21.1/mesos-0.21.1-shaded-protobuf.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-annotations/2.5.3/jackson-annotations-2.5.3.jar:/home/cass/.m2/repository/com/google/code/findbugs/jsr305/1.3.9/jsr305-1.3.9.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-api/2.4.0-b34/hk2-api-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-server/2.22.2/jersey-server-2.22.2.jar:/home/cass/.m2/repository/net/sf/py4j/py4j/0.10.1/py4j-0.10.1.jar:/home/cass/.m2/repository/com/twitter/chill-java/0.8.0/chill-java-0.8.0.jar:/home/cass/.m2/repository/commons-lang/commons-lang/2.6/commons-lang-2.6.jar:/home/cass/.m2/repository/org/tukaani/xz/1.0/xz-1.0.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-databind/2.5.3/jackson-databind-2.5.3.jar:/home/cass/.m2/repository/org/codehaus/janino/janino/2.7.8/janino-2.7.8.jar:/home/cass/.m2/repository/org/apache/curator/curator-recipes/2.4.0/curator-recipes-2.4.0.jar:/home/cass/.m2/repository/commons-codec/commons-codec/1.10/commons-codec-1.10.jar:/home/cass/.m2/repository/org/javassist/javassist/3.18.1-GA/javassist-3.18.1-GA.jar:/home/cass/.m2/repository/org/apache/ivy/ivy/2.4.0/ivy-2.4.0.jar:/home/cass/.m2/repository/javax/inject/javax.inject/1/javax.inject-1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-core/2.2.0/hadoop-mapreduce-client-core-2.2.0.jar:/home/cass/.m2/repository/com/fasterxml/jackson/module/jackson-module-scala_2.11/2.5.3/jackson-module-scala_2.11-2.5.3.jar:/home/cass/.m2/repository/commons-beanutils/commons-beanutils-core/1.8.0/commons-beanutils-core-1.8.0.jar:/home/cass/.m2/repository/javax/servlet/javax.servlet-api/3.1.0/javax.servlet-api-3.1.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/osgi-resource-locator/1.0.1/osgi-resource-locator-1.0.1.jar:/home/cass/.m2/repository/org/apache/commons/commons-math3/3.4.1/commons-math3-3.4.1.jar:/home/cass/spark2/spark/common/network-common/target/spark-network-common_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/avro/avro/1.7.7/avro-1.7.7.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-common/2.2.0/hadoop-mapreduce-client-common-2.2.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-utils/2.4.0-b34/hk2-utils-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/hk2/external/aopalliance-repackaged/2.4.0-b34/aopalliance-repackaged-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/hk2/external/javax.inject/2.4.0-b34/javax.inject-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/jersey/containers/jersey-container-servlet-core/2.22.2/jersey-container-servlet-core-2.22.2.jar:/home/cass/.m2/repository/oro/oro/2.0.8/oro-2.0.8.jar:/home/cass/.m2/repository/org/scala-lang/scala-compiler/2.11.8/scala-compiler-2.11.8.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-encoding/1.7.0/parquet-encoding-1.7.0.jar:/home/cass/.m2/repository/org/roaringbitmap/RoaringBitmap/0.5.11/RoaringBitmap-0.5.11.jar:/home/cass/.m2/repository/log4j/log4j/1.2.17/log4j-1.2.17.jar:/home/cass/.m2/repository/org/scala-lang/scala-library/2.11.8/scala-library-2.11.8.jar:/home/cass/.m2/repository/org/codehaus/janino/commons-compiler/2.7.8/commons-compiler-2.7.8.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-hadoop/1.7.0/parquet-hadoop-1.7.0.jar:/home/cass/.m2/repository/org/apache/curator/curator-client/2.4.0/curator-client-2.4.0.jar:/home/cass/.m2/repository/org/apache/commons/commons-compress/1.4.1/commons-compress-1.4.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-app/2.2.0/hadoop-mapreduce-client-app-2.2.0.jar:/home/cass/.m2/repository/org/slf4j/slf4j-api/1.7.16/slf4j-api-1.7.16.jar:/home/cass/.m2/repository/org/json4s/json4s-core_2.11/3.2.11/json4s-core_2.11-3.2.11.jar:/home/cass/.m2/repository/org/mortbay/jetty/jetty-util/6.1.26/jetty-util-6.1.26.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-server-common/2.2.0/hadoop-yarn-server-common-2.2.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-hdfs/2.2.0/hadoop-hdfs-2.2.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-api/2.2.0/hadoop-yarn-api-2.2.0.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-mapper-asl/1.9.13/jackson-mapper-asl-1.9.13.jar:/home/cass/.m2/repository/com/esotericsoftware/kryo-shaded/3.0.3/kryo-shaded-3.0.3.jar:/home/cass/.m2/repository/javax/ws/rs/javax.ws.rs-api/2.0.1/javax.ws.rs-api-2.0.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-common/2.2.0/hadoop-yarn-common-2.2.0.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-client/2.22.2/jersey-client-2.22.2.jar:/home/cass/spark2/spark/common/unsafe/target/spark-unsafe_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/avro/avro-mapred/1.7.7/avro-mapred-1.7.7-hadoop2.jar:/home/cass/spark2/spark/sql/catalyst/target/spark-catalyst_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-column/1.7.0/parquet-column-1.7.0.jar:/home/cass/.m2/repository/xmlenc/xmlenc/0.52/xmlenc-0.52.jar:/home/cass/.m2/repository/com/ning/compress-lzf/1.0.3/compress-lzf-1.0.3.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-shuffle/2.2.0/hadoop-mapreduce-client-shuffle-2.2.0.jar:/home/cass/.m2/repository/org/apache/zookeeper/zookeeper/3.4.5/zookeeper-3.4.5.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-common/1.7.0/parquet-common-1.7.0.jar:/home/cass/.m2/repository/org/apache/curator/curator-framework/2.4.0/curator-framework-2.4.0.jar:/home/cass/.m2/repository/commons-net/commons-net/2.2/commons-net-2.2.jar:/home/cass/.m2/repository/org/apache/commons/commons-lang3/3.3.2/commons-lang3-3.3.2.jar:/home/cass/.m2/repository/org/json4s/json4s-ast_2.11/3.2.11/json4s-ast_2.11-3.2.11.jar:/home/cass/spark2/spark/launcher/target/spark-launcher_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/scala-lang/scalap/2.11.8/scalap-2.11.8.jar:/home/cass/.m2/repository/com/clearspring/analytics/stream/2.7.0/stream-2.7.0.jar:/home/cass/.m2/repository/org/apache/commons/commons-math/2.1/commons-math-2.1.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-generator/1.7.0/parquet-generator-1.7.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-annotations/2.2.0/hadoop-annotations-2.2.0.jar:/home/cass/.m2/repository/com/thoughtworks/paranamer/paranamer/2.6/paranamer-2.6.jar:/home/cass/.m2/repository/commons-configuration/commons-configuration/1.6/commons-configuration-1.6.jar:/home/cass/.m2/repository/org/glassfish/jersey/containers/jersey-container-servlet/2.22.2/jersey-container-servlet-2.22.2.jar:/home/cass/.m2/repository/commons-digester/commons-digester/1.8/commons-digester-1.8.jar:/home/cass/.m2/repository/org/slf4j/jul-to-slf4j/1.7.16/jul-to-slf4j-1.7.16.jar:/home/cass/.m2/repository/commons-beanutils/commons-beanutils/1.7.0/commons-beanutils-1.7.0.jar:/home/cass/.m2/repository/org/antlr/antlr4-runtime/4.5.2-1/antlr4-runtime-4.5.2-1.jar:/home/cass/spark2/spark/common/network-shuffle/target/spark-network-shuffle_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-xml_2.11/1.0.2/scala-xml_2.11-1.0.2.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-parser-combinators_2.11/1.0.4/scala-parser-combinators_2.11-1.0.4.jar:/home/cass/.m2/repository/commons-cli/commons-cli/1.2/commons-cli-1.2.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-graphite/3.1.2/metrics-graphite-3.1.2.jar:/home/cass/.m2/repository/javax/annotation/javax.annotation-api/1.2/javax.annotation-api-1.2.jar:/home/cass/.m2/repository/org/objenesis/objenesis/2.1/objenesis-2.1.jar:/home/cass/.m2/repository/org/slf4j/slf4j-log4j12/1.7.16/slf4j-log4j12-1.7.16.jar:/home/cass/spark2/spark/common/sketch/target/spark-sketch_2.11-2.0.0-SNAPSHOT.jar:/home/cass/spark2/spark/core/target/spark-core_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/glassfish/jersey/media/jersey-media-jaxb/2.22.2/jersey-media-jaxb-2.22.2.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-core/2.5.3/jackson-core-2.5.3.jar:/home/cass/.m2/repository/org/spark-project/spark/unused/1.0.0/unused-1.0.0.jar:/home/cass/.m2/repository/org/apache/avro/avro-ipc/1.7.7/avro-ipc-1.7.7.jar:/home/cass/.m2/repository/commons-collections/commons-collections/3.2.2/commons-collections-3.2.2.jar:/home/cass/.m2/repository/com/twitter/chill_2.11/0.8.0/chill_2.11-0.8.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-locator/2.4.0-b34/hk2-locator-2.4.0-b34.jar:/home/cass/.m2/repository/org/slf4j/jcl-over-slf4j/1.7.16/jcl-over-slf4j-1.7.16.jar:/home/cass/.m2/repository/commons-httpclient/commons-httpclient/3.1/commons-httpclient-3.1.jar:/home/cass/.m2/repository/io/netty/netty-all/4.0.29.Final/netty-all-4.0.29.Final.jar:/home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-remote-resources-plugin:1.5:process (default) @ spark-sql_2.11 ---
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ spark-sql_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 4 resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:compile (scala-compile-first) @ spark-sql_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 218 Scala sources and 41 Java sources to /home/cass/spark2/spark/sql/core/target/scala-2.11/classes...
[warn] /home/cass/spark2/spark/sql/core/src/main/scala/org/apache/spark/sql/api/r/SQLUtils.scala:37: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]     SQLContext.getOrCreate(jsc.sc)
[warn]                ^
[warn] /home/cass/spark2/spark/sql/core/src/main/scala/org/apache/spark/sql/execution/columnar/InMemoryTableScanExec.scala:292: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn]   lazy val readPartitions: Accumulator[Int] = sparkContext.accumulator(0)
[warn]                            ^
[warn] /home/cass/spark2/spark/sql/core/src/main/scala/org/apache/spark/sql/execution/columnar/InMemoryTableScanExec.scala:292: method accumulator in class SparkContext is deprecated: use AccumulatorV2
[warn]   lazy val readPartitions: Accumulator[Int] = sparkContext.accumulator(0)
[warn]                                                            ^
[warn] /home/cass/spark2/spark/sql/core/src/main/scala/org/apache/spark/sql/execution/columnar/InMemoryTableScanExec.scala:292: object IntAccumulatorParam in object AccumulatorParam is deprecated: use AccumulatorV2
[warn]   lazy val readPartitions: Accumulator[Int] = sparkContext.accumulator(0)
[warn]                                                                       ^
[warn] /home/cass/spark2/spark/sql/core/src/main/scala/org/apache/spark/sql/execution/columnar/InMemoryTableScanExec.scala:293: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn]   lazy val readBatches: Accumulator[Int] = sparkContext.accumulator(0)
[warn]                         ^
[warn] /home/cass/spark2/spark/sql/core/src/main/scala/org/apache/spark/sql/execution/columnar/InMemoryTableScanExec.scala:293: method accumulator in class SparkContext is deprecated: use AccumulatorV2
[warn]   lazy val readBatches: Accumulator[Int] = sparkContext.accumulator(0)
[warn]                                                         ^
[warn] /home/cass/spark2/spark/sql/core/src/main/scala/org/apache/spark/sql/execution/columnar/InMemoryTableScanExec.scala:293: object IntAccumulatorParam in object AccumulatorParam is deprecated: use AccumulatorV2
[warn]   lazy val readBatches: Accumulator[Int] = sparkContext.accumulator(0)
[warn]                                                                    ^
[warn] /home/cass/spark2/spark/sql/core/src/main/scala/org/apache/spark/sql/execution/debug/package.scala:110: trait AccumulatorParam in package spark is deprecated: use AccumulatorV2
[warn]     implicit object SetAccumulatorParam extends AccumulatorParam[HashSet[String]] {
[warn]                                                 ^
[warn] /home/cass/spark2/spark/sql/core/src/main/scala/org/apache/spark/sql/execution/debug/package.scala:129: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn]       elementTypes: Accumulator[HashSet[String]] = sparkContext.accumulator(HashSet.empty))
[warn]                     ^
[warn] /home/cass/spark2/spark/sql/core/src/main/scala/org/apache/spark/sql/execution/debug/package.scala:129: method accumulator in class SparkContext is deprecated: use AccumulatorV2
[warn]       elementTypes: Accumulator[HashSet[String]] = sparkContext.accumulator(HashSet.empty))
[warn]                                                                 ^
[warn] /home/cass/spark2/spark/sql/core/src/main/scala/org/apache/spark/sql/execution/debug/package.scala:128: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn]     case class ColumnMetrics(
[warn]                ^
[warn] /home/cass/spark2/spark/sql/core/src/main/scala/org/apache/spark/sql/execution/debug/package.scala:131: class Accumulator in package spark is deprecated: use AccumulatorV2
[warn]     val tupleCount: Accumulator[Int] = sparkContext.accumulator[Int](0)
[warn]                     ^
[warn] /home/cass/spark2/spark/sql/core/src/main/scala/org/apache/spark/sql/execution/debug/package.scala:131: method accumulator in class SparkContext is deprecated: use AccumulatorV2
[warn]     val tupleCount: Accumulator[Int] = sparkContext.accumulator[Int](0)
[warn]                                                     ^
[warn] /home/cass/spark2/spark/sql/core/src/main/scala/org/apache/spark/sql/execution/debug/package.scala:131: object IntAccumulatorParam in object AccumulatorParam is deprecated: use AccumulatorV2
[warn]     val tupleCount: Accumulator[Int] = sparkContext.accumulator[Int](0)
[warn]                                                                     ^
[warn] 14 warnings found
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] 1 warning
[info] Compile success at May 20, 2016 12:33:50 PM [26.483s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:compile (default-compile) @ spark-sql_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 41 source files to /home/cass/spark2/spark/sql/core/target/scala-2.11/classes
[INFO]
[INFO] --- build-helper-maven-plugin:1.10:add-test-source (add-scala-test-sources) @ spark-sql_2.11 ---
[INFO] Test Source directory: /home/cass/spark2/spark/sql/core/src/test/gen-java added.
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (create-tmp-dir) @ spark-sql_2.11 ---
[INFO] Executing tasks

main:
    [mkdir] Created dir: /home/cass/spark2/spark/sql/core/target/tmp
[INFO] Executed tasks
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ spark-sql_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 35 resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:testCompile (scala-test-compile-first) @ spark-sql_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 156 Scala sources and 18 Java sources to /home/cass/spark2/spark/sql/core/target/scala-2.11/test-classes...
[warn] /home/cass/spark2/spark/sql/core/src/test/scala/org/apache/spark/sql/JoinSuite.scala:45: inferred existential type (String, Class[_$1]) forSome { type _$1 }, which cannot be expressed by wildcards,  should be enabled
[warn] by making the implicit value scala.language.existentials visible.
[warn] This can be achieved by adding the import clause 'import scala.language.existentials'
[warn] or by setting the compiler option -language:existentials.
[warn] See the Scaladoc for value scala.language.existentials for a discussion
[warn] why the feature should be explicitly enabled.
[warn]     val (sqlString, c) = pair
[warn]         ^
[warn] /home/cass/spark2/spark/sql/core/src/test/scala/org/apache/spark/sql/execution/datasources/FileCatalogSuite.scala:39: reflective access of structural type member method leafFilePaths should be enabled
[warn] by making the implicit value scala.language.reflectiveCalls visible.
[warn] This can be achieved by adding the import clause 'import scala.language.reflectiveCalls'
[warn] or by setting the compiler option -language:reflectiveCalls.
[warn] See the Scaladoc for value scala.language.reflectiveCalls for a discussion
[warn] why the feature should be explicitly enabled.
[warn]       assert(catalog.leafFilePaths.forall(p => p.toString.startsWith("file:/")))
[warn]                      ^
[warn] /home/cass/spark2/spark/sql/core/src/test/scala/org/apache/spark/sql/execution/datasources/FileCatalogSuite.scala:40: reflective access of structural type member method leafDirPaths should be enabled
[warn] by making the implicit value scala.language.reflectiveCalls visible.
[warn]       assert(catalog.leafDirPaths.forall(p => p.toString.startsWith("file:/")))
[warn]                      ^
[warn] /home/cass/spark2/spark/sql/core/src/test/scala/org/apache/spark/sql/SQLContextSuite.scala:32: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]     val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                 ^
[warn] /home/cass/spark2/spark/sql/core/src/test/scala/org/apache/spark/sql/SQLContextSuite.scala:34: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]     assert(SQLContext.getOrCreate(sc).eq(sqlContext),
[warn]                       ^
[warn] /home/cass/spark2/spark/sql/core/src/test/scala/org/apache/spark/sql/SQLContextSuite.scala:39: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]     val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                 ^
[warn] /home/cass/spark2/spark/sql/core/src/test/scala/org/apache/spark/sql/SQLContextSuite.scala:41: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]     assert(SQLContext.getOrCreate(sc).eq(sqlContext),
[warn]                       ^
[warn] /home/cass/spark2/spark/sql/core/src/test/scala/org/apache/spark/sql/SQLContextSuite.scala:44: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]     assert(SQLContext.getOrCreate(sc).eq(newSession),
[warn]                       ^
[warn] /home/cass/spark2/spark/sql/core/src/test/scala/org/apache/spark/sql/SQLContextSuite.scala:49: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]     val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                 ^
[warn] /home/cass/spark2/spark/sql/core/src/test/scala/org/apache/spark/sql/SQLContextSuite.scala:77: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]     val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                 ^
[warn] /home/cass/spark2/spark/sql/core/src/test/scala/org/apache/spark/sql/SQLQuerySuite.scala:2064: method accumulator in class SparkContext is deprecated: use AccumulatorV2
[warn]       val countAcc = sparkContext.accumulator(0, "CallCount")
[warn]                                   ^
[warn] /home/cass/spark2/spark/sql/core/src/test/scala/org/apache/spark/sql/SQLQuerySuite.scala:2064: object IntAccumulatorParam in object AccumulatorParam is deprecated: use AccumulatorV2
[warn]       val countAcc = sparkContext.accumulator(0, "CallCount")
[warn]                                              ^
[warn] /home/cass/spark2/spark/sql/core/src/test/scala/org/apache/spark/sql/execution/metric/SQLMetricsSuite.scala:53: method accumulator in class SparkContext is deprecated: use AccumulatorV2
[warn]     val l = sparkContext.accumulator(0L)
[warn]                          ^
[warn] /home/cass/spark2/spark/sql/core/src/test/scala/org/apache/spark/sql/execution/metric/SQLMetricsSuite.scala:53: object LongAccumulatorParam in object AccumulatorParam is deprecated: use AccumulatorV2
[warn]     val l = sparkContext.accumulator(0L)
[warn]                                     ^
[warn] /home/cass/spark2/spark/sql/core/src/test/scala/org/apache/spark/sql/execution/ui/SQLListenerSuite.scala:368: method accumulator in class SparkContext is deprecated: use AccumulatorV2
[warn]     val nonSqlMetric = sparkContext.accumulator[Int](0, "baseball")
[warn]                                     ^
[warn] /home/cass/spark2/spark/sql/core/src/test/scala/org/apache/spark/sql/execution/ui/SQLListenerSuite.scala:368: object IntAccumulatorParam in object AccumulatorParam is deprecated: use AccumulatorV2
[warn]     val nonSqlMetric = sparkContext.accumulator[Int](0, "baseball")
[warn]                                                     ^
[warn] /home/cass/spark2/spark/sql/core/src/test/scala/org/apache/spark/sql/internal/SQLConfSuite.scala:30: constructor SQLContext in class SQLContext is deprecated: Use SparkSession.builder instead
[warn]     val newContext = new SQLContext(sparkContext)
[warn]                      ^
[warn] /home/cass/spark2/spark/sql/core/src/test/scala/org/apache/spark/sql/sources/DataSourceTest.scala:27: constructor SQLContext in class SQLContext is deprecated: Use SparkSession.builder instead
[warn]     val ctx = new SQLContext(spark.sparkContext)
[warn]               ^
[warn] 18 warnings found
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] /home/cass/spark2/spark/sql/core/src/test/java/test/org/apache/spark/sql/JavaDatasetSuite.java:35: warning: [deprecation] Accumulator in org.apache.spark has been deprecated
[warn] import org.apache.spark.Accumulator;
[warn]                        ^
[warn] /home/cass/spark2/spark/sql/core/src/test/java/test/org/apache/spark/sql/JavaDatasetSuite.java:147: warning: [deprecation] Accumulator in org.apache.spark has been deprecated
[warn]     final Accumulator<Integer> accum = jsc.accumulator(0);
[warn]           ^
[warn] 3 warnings
[info] Compile success at May 20, 2016 12:34:34 PM [42.639s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:testCompile (default-testCompile) @ spark-sql_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 18 source files to /home/cass/spark2/spark/sql/core/target/scala-2.11/test-classes
[WARNING] /home/cass/spark2/spark/sql/core/src/test/java/test/org/apache/spark/sql/JavaDatasetSuite.java:[35,23] [deprecation] Accumulator in org.apache.spark has been deprecated
[WARNING] /home/cass/spark2/spark/sql/core/src/test/java/test/org/apache/spark/sql/JavaDatasetSuite.java:[147,10] [deprecation] Accumulator in org.apache.spark has been deprecated
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (generate-test-classpath) @ spark-sql_2.11 ---
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (default-test) @ spark-sql_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (test) @ spark-sql_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- scalatest-maven-plugin:1.0:test (test) @ spark-sql_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (prepare-test-jar) @ spark-sql_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/sql/core/target/spark-sql_2.11-2.0.0-SNAPSHOT-tests.jar
[INFO]
[INFO] --- maven-jar-plugin:2.6:jar (default-jar) @ spark-sql_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/sql/core/target/spark-sql_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-site-plugin:3.3:attach-descriptor (attach-descriptor) @ spark-sql_2.11 ---
[INFO]
[INFO] --- maven-shade-plugin:2.4.3:shade (default) @ spark-sql_2.11 ---
[INFO] Excluding com.univocity:univocity-parsers:jar:2.1.0 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-sketch_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-core_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.avro:avro-mapred:jar:hadoop2:1.7.7 from the shaded jar.
[INFO] Excluding org.apache.avro:avro-ipc:jar:1.7.7 from the shaded jar.
[INFO] Excluding com.twitter:chill_2.11:jar:0.8.0 from the shaded jar.
[INFO] Excluding com.esotericsoftware:kryo-shaded:jar:3.0.3 from the shaded jar.
[INFO] Excluding com.esotericsoftware:minlog:jar:1.3.0 from the shaded jar.
[INFO] Excluding com.twitter:chill-java:jar:0.8.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding commons-cli:commons-cli:jar:1.2 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-math:jar:2.1 from the shaded jar.
[INFO] Excluding xmlenc:xmlenc:jar:0.52 from the shaded jar.
[INFO] Excluding commons-io:commons-io:jar:2.4 from the shaded jar.
[INFO] Excluding commons-lang:commons-lang:jar:2.6 from the shaded jar.
[INFO] Excluding commons-configuration:commons-configuration:jar:1.6 from the shaded jar.
[INFO] Excluding commons-collections:commons-collections:jar:3.2.2 from the shaded jar.
[INFO] Excluding commons-digester:commons-digester:jar:1.8 from the shaded jar.
[INFO] Excluding commons-beanutils:commons-beanutils:jar:1.7.0 from the shaded jar.
[INFO] Excluding commons-beanutils:commons-beanutils-core:jar:1.8.0 from the shaded jar.
[INFO] Excluding com.google.protobuf:protobuf-java:jar:2.5.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-auth:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-hdfs:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.mortbay.jetty:jetty-util:jar:6.1.26 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-app:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding com.google.inject:guice:jar:3.0 from the shaded jar.
[INFO] Excluding javax.inject:javax.inject:jar:1 from the shaded jar.
[INFO] Excluding aopalliance:aopalliance:jar:1.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-server-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-shuffle:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-api:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-core:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-jobclient:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-annotations:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-launcher_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-network-common_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-network-shuffle_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.fusesource.leveldbjni:leveldbjni-all:jar:1.8 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-unsafe_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding net.java.dev.jets3t:jets3t:jar:0.7.1 from the shaded jar.
[INFO] Excluding commons-httpclient:commons-httpclient:jar:3.1 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-recipes:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-framework:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-client:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.zookeeper:zookeeper:jar:3.4.5 from the shaded jar.
[INFO] Excluding javax.servlet:javax.servlet-api:jar:3.1.0 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-lang3:jar:3.3.2 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-math3:jar:3.4.1 from the shaded jar.
[INFO] Excluding com.google.code.findbugs:jsr305:jar:1.3.9 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-api:jar:1.7.16 from the shaded jar.
[INFO] Excluding org.slf4j:jul-to-slf4j:jar:1.7.16 from the shaded jar.
[INFO] Excluding org.slf4j:jcl-over-slf4j:jar:1.7.16 from the shaded jar.
[INFO] Excluding log4j:log4j:jar:1.2.17 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-log4j12:jar:1.7.16 from the shaded jar.
[INFO] Excluding com.ning:compress-lzf:jar:1.0.3 from the shaded jar.
[INFO] Excluding org.xerial.snappy:snappy-java:jar:1.1.2.4 from the shaded jar.
[INFO] Excluding net.jpountz.lz4:lz4:jar:1.3.0 from the shaded jar.
[INFO] Excluding org.roaringbitmap:RoaringBitmap:jar:0.5.11 from the shaded jar.
[INFO] Excluding commons-net:commons-net:jar:2.2 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-library:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.json4s:json4s-jackson_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.json4s:json4s-core_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.json4s:json4s-ast_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.scala-lang:scalap:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-compiler:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-parser-combinators_2.11:jar:1.0.4 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-client:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.ws.rs:javax.ws.rs-api:jar:2.0.1 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-api:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-utils:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2.external:aopalliance-repackaged:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2.external:javax.inject:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-locator:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.javassist:javassist:jar:3.18.1-GA from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-common:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.annotation:javax.annotation-api:jar:1.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.bundles.repackaged:jersey-guava:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:osgi-resource-locator:jar:1.0.1 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-server:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.media:jersey-media-jaxb:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.validation:validation-api:jar:1.1.0.Final from the shaded jar.
[INFO] Excluding org.glassfish.jersey.containers:jersey-container-servlet:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.containers:jersey-container-servlet-core:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.apache.mesos:mesos:jar:shaded-protobuf:0.21.1 from the shaded jar.
[INFO] Excluding io.netty:netty-all:jar:4.0.29.Final from the shaded jar.
[INFO] Excluding io.netty:netty:jar:3.8.0.Final from the shaded jar.
[INFO] Excluding com.clearspring.analytics:stream:jar:2.7.0 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-core:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-jvm:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-json:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-graphite:jar:3.1.2 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.module:jackson-module-scala_2.11:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.thoughtworks.paranamer:paranamer:jar:2.6 from the shaded jar.
[INFO] Excluding org.apache.ivy:ivy:jar:2.4.0 from the shaded jar.
[INFO] Excluding oro:oro:jar:2.0.8 from the shaded jar.
[INFO] Excluding net.razorvine:pyrolite:jar:4.9 from the shaded jar.
[INFO] Excluding net.sf.py4j:py4j:jar:0.10.1 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-catalyst_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.scala-lang:scala-reflect:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.codehaus.janino:janino:jar:2.7.8 from the shaded jar.
[INFO] Excluding org.codehaus.janino:commons-compiler:jar:2.7.8 from the shaded jar.
[INFO] Excluding org.antlr:antlr4-runtime:jar:4.5.2-1 from the shaded jar.
[INFO] Excluding commons-codec:commons-codec:jar:1.10 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-tags_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-column:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-common:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-encoding:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-generator:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-hadoop:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-format:jar:2.3.0-incubating from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-jackson:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-mapper-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-core-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-databind:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-annotations:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-core:jar:2.5.3 from the shaded jar.
[INFO] Excluding org.apache.avro:avro:jar:1.7.7 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-compress:jar:1.4.1 from the shaded jar.
[INFO] Excluding org.tukaani:xz:jar:1.0 from the shaded jar.
[INFO] Excluding org.objenesis:objenesis:jar:2.1 from the shaded jar.
[INFO] Including org.spark-project.spark:unused:jar:1.0.0 in the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-xml_2.11:jar:1.0.2 from the shaded jar.
[INFO] Replacing original artifact with shaded artifact.
[INFO] Replacing /home/cass/spark2/spark/sql/core/target/spark-sql_2.11-2.0.0-SNAPSHOT.jar with /home/cass/spark2/spark/sql/core/target/spark-sql_2.11-2.0.0-SNAPSHOT-shaded.jar
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/sql/core/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/sql/core/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/sql/core/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/sql/core/dependency-reduced-pom.xml
[INFO]
[INFO] --- maven-source-plugin:2.4:jar-no-fork (create-source-jar) @ spark-sql_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/sql/core/target/spark-sql_2.11-2.0.0-SNAPSHOT-sources.jar
[INFO]
[INFO] --- maven-source-plugin:2.4:test-jar-no-fork (create-source-jar) @ spark-sql_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/sql/core/target/spark-sql_2.11-2.0.0-SNAPSHOT-test-sources.jar
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Spark Project ML Local Library 2.0.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.0.0:clean (default-clean) @ spark-mllib-local_2.11 ---
[INFO]
[INFO] --- maven-enforcer-plugin:1.4.1:enforce (enforce-versions) @ spark-mllib-local_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:add-source (eclipse-add-source) @ spark-mllib-local_2.11 ---
[INFO] Add Source directory: /home/cass/spark2/spark/mllib-local/src/main/scala
[INFO] Add Test Source directory: /home/cass/spark2/spark/mllib-local/src/test/scala
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (default-cli) @ spark-mllib-local_2.11 ---
[INFO] Dependencies classpath:
/home/cass/.m2/repository/org/scalanlp/breeze-macros_2.11/0.11.2/breeze-macros_2.11-0.11.2.jar:/home/cass/.m2/repository/org/spark-project/spark/unused/1.0.0/unused-1.0.0.jar:/home/cass/.m2/repository/org/scala-lang/scala-library/2.11.8/scala-library-2.11.8.jar:/home/cass/.m2/repository/org/spire-math/spire-macros_2.11/0.7.4/spire-macros_2.11-0.7.4.jar:/home/cass/.m2/repository/org/apache/commons/commons-math3/3.4.1/commons-math3-3.4.1.jar:/home/cass/.m2/repository/net/sourceforge/f2j/arpack_combined_all/0.1/arpack_combined_all-0.1.jar:/home/cass/.m2/repository/net/sf/opencsv/opencsv/2.3/opencsv-2.3.jar:/home/cass/.m2/repository/org/scala-lang/scala-reflect/2.11.8/scala-reflect-2.11.8.jar:/home/cass/.m2/repository/org/slf4j/slf4j-api/1.7.16/slf4j-api-1.7.16.jar:/home/cass/.m2/repository/com/github/rwl/jtransforms/2.4.0/jtransforms-2.4.0.jar:/home/cass/.m2/repository/org/scalanlp/breeze_2.11/0.11.2/breeze_2.11-0.11.2.jar:/home/cass/.m2/repository/org/spire-math/spire_2.11/0.7.4/spire_2.11-0.7.4.jar:/home/cass/.m2/repository/com/github/fommil/netlib/core/1.1.2/core-1.1.2.jar:/home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-remote-resources-plugin:1.5:process (default) @ spark-mllib-local_2.11 ---
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ spark-mllib-local_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/mllib-local/src/main/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:compile (scala-compile-first) @ spark-mllib-local_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 5 Scala sources to /home/cass/spark2/spark/mllib-local/target/scala-2.11/classes...
[info] Compile success at May 20, 2016 12:34:43 PM [2.554s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:compile (default-compile) @ spark-mllib-local_2.11 ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (create-tmp-dir) @ spark-mllib-local_2.11 ---
[INFO] Executing tasks

main:
    [mkdir] Created dir: /home/cass/spark2/spark/mllib-local/target/tmp
[INFO] Executed tasks
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ spark-mllib-local_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/mllib-local/src/test/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:testCompile (scala-test-compile-first) @ spark-mllib-local_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 10 Scala sources to /home/cass/spark2/spark/mllib-local/target/scala-2.11/test-classes...
[info] Compile success at May 20, 2016 12:34:46 PM [2.787s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:testCompile (default-testCompile) @ spark-mllib-local_2.11 ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (generate-test-classpath) @ spark-mllib-local_2.11 ---
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (default-test) @ spark-mllib-local_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (test) @ spark-mllib-local_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- scalatest-maven-plugin:1.0:test (test) @ spark-mllib-local_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (prepare-test-jar) @ spark-mllib-local_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/mllib-local/target/spark-mllib-local_2.11-2.0.0-SNAPSHOT-tests.jar
[INFO]
[INFO] --- maven-jar-plugin:2.6:jar (default-jar) @ spark-mllib-local_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/mllib-local/target/spark-mllib-local_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-site-plugin:3.3:attach-descriptor (attach-descriptor) @ spark-mllib-local_2.11 ---
[INFO]
[INFO] --- maven-shade-plugin:2.4.3:shade (default) @ spark-mllib-local_2.11 ---
[INFO] Excluding org.scalanlp:breeze_2.11:jar:0.11.2 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-library:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scalanlp:breeze-macros_2.11:jar:0.11.2 from the shaded jar.
[INFO] Excluding com.github.fommil.netlib:core:jar:1.1.2 from the shaded jar.
[INFO] Excluding net.sourceforge.f2j:arpack_combined_all:jar:0.1 from the shaded jar.
[INFO] Excluding net.sf.opencsv:opencsv:jar:2.3 from the shaded jar.
[INFO] Excluding com.github.rwl:jtransforms:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.spire-math:spire_2.11:jar:0.7.4 from the shaded jar.
[INFO] Excluding org.spire-math:spire-macros_2.11:jar:0.7.4 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-api:jar:1.7.16 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-math3:jar:3.4.1 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-tags_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Including org.spark-project.spark:unused:jar:1.0.0 in the shaded jar.
[INFO] Excluding org.scala-lang:scala-reflect:jar:2.11.8 from the shaded jar.
[INFO] Replacing original artifact with shaded artifact.
[INFO] Replacing /home/cass/spark2/spark/mllib-local/target/spark-mllib-local_2.11-2.0.0-SNAPSHOT.jar with /home/cass/spark2/spark/mllib-local/target/spark-mllib-local_2.11-2.0.0-SNAPSHOT-shaded.jar
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/mllib-local/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/mllib-local/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/mllib-local/dependency-reduced-pom.xml
[INFO]
[INFO] --- maven-source-plugin:2.4:jar-no-fork (create-source-jar) @ spark-mllib-local_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/mllib-local/target/spark-mllib-local_2.11-2.0.0-SNAPSHOT-sources.jar
[INFO]
[INFO] --- maven-source-plugin:2.4:test-jar-no-fork (create-source-jar) @ spark-mllib-local_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/mllib-local/target/spark-mllib-local_2.11-2.0.0-SNAPSHOT-test-sources.jar
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Spark Project ML Library 2.0.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.0.0:clean (default-clean) @ spark-mllib_2.11 ---
[INFO]
[INFO] --- maven-enforcer-plugin:1.4.1:enforce (enforce-versions) @ spark-mllib_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:add-source (eclipse-add-source) @ spark-mllib_2.11 ---
[INFO] Add Source directory: /home/cass/spark2/spark/mllib/src/main/scala
[INFO] Add Test Source directory: /home/cass/spark2/spark/mllib/src/test/scala
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (default-cli) @ spark-mllib_2.11 ---
[INFO] Dependencies classpath:
/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-jobclient/2.2.0/hadoop-mapreduce-client-jobclient-2.2.0.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-jackson/1.7.0/parquet-jackson-1.7.0.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-core/3.1.2/metrics-core-3.1.2.jar:/home/cass/.m2/repository/com/google/protobuf/protobuf-java/2.5.0/protobuf-java-2.5.0.jar:/home/cass/.m2/repository/aopalliance/aopalliance/1.0/aopalliance-1.0.jar:/home/cass/.m2/repository/org/spire-math/spire-macros_2.11/0.7.4/spire-macros_2.11-0.7.4.jar:/home/cass/.m2/repository/net/razorvine/pyrolite/4.9/pyrolite-4.9.jar:/home/cass/.m2/repository/com/univocity/univocity-parsers/2.1.0/univocity-parsers-2.1.0.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-jvm/3.1.2/metrics-jvm-3.1.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-client/2.2.0/hadoop-client-2.2.0.jar:/home/cass/.m2/repository/org/fusesource/leveldbjni/leveldbjni-all/1.8/leveldbjni-all-1.8.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-format/2.3.0-incubating/parquet-format-2.3.0-incubating.jar:/home/cass/.m2/repository/org/glassfish/jersey/bundles/repackaged/jersey-guava/2.22.2/jersey-guava-2.22.2.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-json/3.1.2/metrics-json-3.1.2.jar:/home/cass/.m2/repository/org/spire-math/spire_2.11/0.7.4/spire_2.11-0.7.4.jar:/home/cass/.m2/repository/net/java/dev/jets3t/jets3t/0.7.1/jets3t-0.7.1.jar:/home/cass/spark2/spark/graphx/target/spark-graphx_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-common/2.2.0/hadoop-common-2.2.0.jar:/home/cass/.m2/repository/org/jpmml/pmml-schema/1.2.7/pmml-schema-1.2.7.jar:/home/cass/.m2/repository/com/google/inject/guice/3.0/guice-3.0.jar:/home/cass/.m2/repository/commons-io/commons-io/2.4/commons-io-2.4.jar:/home/cass/spark2/spark/sql/core/target/spark-sql_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/net/sourceforge/f2j/arpack_combined_all/0.1/arpack_combined_all-0.1.jar:/home/cass/.m2/repository/org/scala-lang/scala-reflect/2.11.8/scala-reflect-2.11.8.jar:/home/cass/.m2/repository/org/xerial/snappy/snappy-java/1.1.2.4/snappy-java-1.1.2.4.jar:/home/cass/.m2/repository/org/json4s/json4s-jackson_2.11/3.2.11/json4s-jackson_2.11-3.2.11.jar:/home/cass/.m2/repository/org/jpmml/pmml-agent/1.2.7/pmml-agent-1.2.7.jar:/home/cass/.m2/repository/com/esotericsoftware/minlog/1.3.0/minlog-1.3.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-auth/2.2.0/hadoop-auth-2.2.0.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-core-asl/1.9.13/jackson-core-asl-1.9.13.jar:/home/cass/.m2/repository/javax/validation/validation-api/1.1.0.Final/validation-api-1.1.0.Final.jar:/home/cass/.m2/repository/net/jpountz/lz4/lz4/1.3.0/lz4-1.3.0.jar:/home/cass/.m2/repository/com/github/rwl/jtransforms/2.4.0/jtransforms-2.4.0.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-common/2.22.2/jersey-common-2.22.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-client/2.2.0/hadoop-yarn-client-2.2.0.jar:/home/cass/.m2/repository/io/netty/netty/3.8.0.Final/netty-3.8.0.Final.jar:/home/cass/.m2/repository/org/apache/mesos/mesos/0.21.1/mesos-0.21.1-shaded-protobuf.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-annotations/2.5.3/jackson-annotations-2.5.3.jar:/home/cass/.m2/repository/com/google/code/findbugs/jsr305/1.3.9/jsr305-1.3.9.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-api/2.4.0-b34/hk2-api-2.4.0-b34.jar:/home/cass/.m2/repository/net/sf/opencsv/opencsv/2.3/opencsv-2.3.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-server/2.22.2/jersey-server-2.22.2.jar:/home/cass/.m2/repository/net/sf/py4j/py4j/0.10.1/py4j-0.10.1.jar:/home/cass/.m2/repository/com/twitter/chill-java/0.8.0/chill-java-0.8.0.jar:/home/cass/.m2/repository/commons-lang/commons-lang/2.6/commons-lang-2.6.jar:/home/cass/.m2/repository/org/tukaani/xz/1.0/xz-1.0.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-databind/2.5.3/jackson-databind-2.5.3.jar:/home/cass/.m2/repository/org/codehaus/janino/janino/2.7.8/janino-2.7.8.jar:/home/cass/.m2/repository/commons-codec/commons-codec/1.10/commons-codec-1.10.jar:/home/cass/.m2/repository/org/apache/curator/curator-recipes/2.4.0/curator-recipes-2.4.0.jar:/home/cass/.m2/repository/org/javassist/javassist/3.18.1-GA/javassist-3.18.1-GA.jar:/home/cass/.m2/repository/org/apache/ivy/ivy/2.4.0/ivy-2.4.0.jar:/home/cass/.m2/repository/javax/inject/javax.inject/1/javax.inject-1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-core/2.2.0/hadoop-mapreduce-client-core-2.2.0.jar:/home/cass/.m2/repository/com/fasterxml/jackson/module/jackson-module-scala_2.11/2.5.3/jackson-module-scala_2.11-2.5.3.jar:/home/cass/.m2/repository/commons-beanutils/commons-beanutils-core/1.8.0/commons-beanutils-core-1.8.0.jar:/home/cass/.m2/repository/javax/servlet/javax.servlet-api/3.1.0/javax.servlet-api-3.1.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/osgi-resource-locator/1.0.1/osgi-resource-locator-1.0.1.jar:/home/cass/.m2/repository/org/apache/commons/commons-math3/3.4.1/commons-math3-3.4.1.jar:/home/cass/spark2/spark/common/network-common/target/spark-network-common_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/avro/avro/1.7.7/avro-1.7.7.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-common/2.2.0/hadoop-mapreduce-client-common-2.2.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-utils/2.4.0-b34/hk2-utils-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/hk2/external/aopalliance-repackaged/2.4.0-b34/aopalliance-repackaged-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/hk2/external/javax.inject/2.4.0-b34/javax.inject-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/jersey/containers/jersey-container-servlet-core/2.22.2/jersey-container-servlet-core-2.22.2.jar:/home/cass/.m2/repository/oro/oro/2.0.8/oro-2.0.8.jar:/home/cass/.m2/repository/org/scala-lang/scala-compiler/2.11.8/scala-compiler-2.11.8.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-encoding/1.7.0/parquet-encoding-1.7.0.jar:/home/cass/.m2/repository/org/roaringbitmap/RoaringBitmap/0.5.11/RoaringBitmap-0.5.11.jar:/home/cass/.m2/repository/log4j/log4j/1.2.17/log4j-1.2.17.jar:/home/cass/.m2/repository/org/scala-lang/scala-library/2.11.8/scala-library-2.11.8.jar:/home/cass/.m2/repository/org/codehaus/janino/commons-compiler/2.7.8/commons-compiler-2.7.8.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-hadoop/1.7.0/parquet-hadoop-1.7.0.jar:/home/cass/.m2/repository/org/apache/curator/curator-client/2.4.0/curator-client-2.4.0.jar:/home/cass/.m2/repository/org/jpmml/pmml-model/1.2.7/pmml-model-1.2.7.jar:/home/cass/.m2/repository/org/apache/commons/commons-compress/1.4.1/commons-compress-1.4.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-app/2.2.0/hadoop-mapreduce-client-app-2.2.0.jar:/home/cass/.m2/repository/org/slf4j/slf4j-api/1.7.16/slf4j-api-1.7.16.jar:/home/cass/.m2/repository/org/apache/xbean/xbean-asm5-shaded/4.4/xbean-asm5-shaded-4.4.jar:/home/cass/.m2/repository/org/json4s/json4s-core_2.11/3.2.11/json4s-core_2.11-3.2.11.jar:/home/cass/.m2/repository/com/github/fommil/netlib/core/1.1.2/core-1.1.2.jar:/home/cass/.m2/repository/org/mortbay/jetty/jetty-util/6.1.26/jetty-util-6.1.26.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-server-common/2.2.0/hadoop-yarn-server-common-2.2.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-hdfs/2.2.0/hadoop-hdfs-2.2.0.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-mapper-asl/1.9.13/jackson-mapper-asl-1.9.13.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-api/2.2.0/hadoop-yarn-api-2.2.0.jar:/home/cass/.m2/repository/com/esotericsoftware/kryo-shaded/3.0.3/kryo-shaded-3.0.3.jar:/home/cass/.m2/repository/javax/ws/rs/javax.ws.rs-api/2.0.1/javax.ws.rs-api-2.0.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-common/2.2.0/hadoop-yarn-common-2.2.0.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-client/2.22.2/jersey-client-2.22.2.jar:/home/cass/spark2/spark/common/unsafe/target/spark-unsafe_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/avro/avro-mapred/1.7.7/avro-mapred-1.7.7-hadoop2.jar:/home/cass/spark2/spark/sql/catalyst/target/spark-catalyst_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-column/1.7.0/parquet-column-1.7.0.jar:/home/cass/.m2/repository/xmlenc/xmlenc/0.52/xmlenc-0.52.jar:/home/cass/.m2/repository/com/ning/compress-lzf/1.0.3/compress-lzf-1.0.3.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-shuffle/2.2.0/hadoop-mapreduce-client-shuffle-2.2.0.jar:/home/cass/.m2/repository/org/apache/zookeeper/zookeeper/3.4.5/zookeeper-3.4.5.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-common/1.7.0/parquet-common-1.7.0.jar:/home/cass/.m2/repository/org/apache/curator/curator-framework/2.4.0/curator-framework-2.4.0.jar:/home/cass/.m2/repository/commons-net/commons-net/2.2/commons-net-2.2.jar:/home/cass/.m2/repository/org/apache/commons/commons-lang3/3.3.2/commons-lang3-3.3.2.jar:/home/cass/.m2/repository/org/json4s/json4s-ast_2.11/3.2.11/json4s-ast_2.11-3.2.11.jar:/home/cass/spark2/spark/launcher/target/spark-launcher_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/scala-lang/scalap/2.11.8/scalap-2.11.8.jar:/home/cass/.m2/repository/com/clearspring/analytics/stream/2.7.0/stream-2.7.0.jar:/home/cass/.m2/repository/org/apache/commons/commons-math/2.1/commons-math-2.1.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-generator/1.7.0/parquet-generator-1.7.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-annotations/2.2.0/hadoop-annotations-2.2.0.jar:/home/cass/.m2/repository/com/thoughtworks/paranamer/paranamer/2.6/paranamer-2.6.jar:/home/cass/.m2/repository/commons-configuration/commons-configuration/1.6/commons-configuration-1.6.jar:/home/cass/.m2/repository/org/glassfish/jersey/containers/jersey-container-servlet/2.22.2/jersey-container-servlet-2.22.2.jar:/home/cass/.m2/repository/commons-digester/commons-digester/1.8/commons-digester-1.8.jar:/home/cass/.m2/repository/org/slf4j/jul-to-slf4j/1.7.16/jul-to-slf4j-1.7.16.jar:/home/cass/.m2/repository/commons-beanutils/commons-beanutils/1.7.0/commons-beanutils-1.7.0.jar:/home/cass/.m2/repository/org/antlr/antlr4-runtime/4.5.2-1/antlr4-runtime-4.5.2-1.jar:/home/cass/spark2/spark/common/network-shuffle/target/spark-network-shuffle_2.11-2.0.0-SNAPSHOT.jar:/home/cass/spark2/spark/mllib-local/target/spark-mllib-local_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-xml_2.11/1.0.2/scala-xml_2.11-1.0.2.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-parser-combinators_2.11/1.0.4/scala-parser-combinators_2.11-1.0.4.jar:/home/cass/.m2/repository/commons-cli/commons-cli/1.2/commons-cli-1.2.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-graphite/3.1.2/metrics-graphite-3.1.2.jar:/home/cass/.m2/repository/org/scalanlp/breeze_2.11/0.11.2/breeze_2.11-0.11.2.jar:/home/cass/.m2/repository/javax/annotation/javax.annotation-api/1.2/javax.annotation-api-1.2.jar:/home/cass/.m2/repository/org/objenesis/objenesis/2.1/objenesis-2.1.jar:/home/cass/.m2/repository/org/slf4j/slf4j-log4j12/1.7.16/slf4j-log4j12-1.7.16.jar:/home/cass/spark2/spark/common/sketch/target/spark-sketch_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/scalanlp/breeze-macros_2.11/0.11.2/breeze-macros_2.11-0.11.2.jar:/home/cass/spark2/spark/core/target/spark-core_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/glassfish/jersey/media/jersey-media-jaxb/2.22.2/jersey-media-jaxb-2.22.2.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-core/2.5.3/jackson-core-2.5.3.jar:/home/cass/spark2/spark/streaming/target/spark-streaming_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/spark-project/spark/unused/1.0.0/unused-1.0.0.jar:/home/cass/.m2/repository/org/apache/avro/avro-ipc/1.7.7/avro-ipc-1.7.7.jar:/home/cass/.m2/repository/commons-collections/commons-collections/3.2.2/commons-collections-3.2.2.jar:/home/cass/.m2/repository/com/twitter/chill_2.11/0.8.0/chill_2.11-0.8.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-locator/2.4.0-b34/hk2-locator-2.4.0-b34.jar:/home/cass/.m2/repository/org/slf4j/jcl-over-slf4j/1.7.16/jcl-over-slf4j-1.7.16.jar:/home/cass/.m2/repository/commons-httpclient/commons-httpclient/3.1/commons-httpclient-3.1.jar:/home/cass/.m2/repository/io/netty/netty-all/4.0.29.Final/netty-all-4.0.29.Final.jar:/home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-remote-resources-plugin:1.5:process (default) @ spark-mllib_2.11 ---
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ spark-mllib_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 16 resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:compile (scala-compile-first) @ spark-mllib_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 251 Scala sources and 4 Java sources to /home/cass/spark2/spark/mllib/target/scala-2.11/classes...
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/clustering/GaussianMixture.scala:138: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]     val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                 ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/evaluation/MulticlassClassificationEvaluator.scala:85: value precision in class MulticlassMetrics is deprecated: Use accuracy.
[warn]       case "precision" => metrics.precision
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/evaluation/MulticlassClassificationEvaluator.scala:86: value recall in class MulticlassMetrics is deprecated: Use accuracy.
[warn]       case "recall" => metrics.recall
[warn]                                ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/feature/SQLTransformer.scala:78: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]     val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                 ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/feature/Word2Vec.scala:187: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]     val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                 ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/feature/Word2Vec.scala:209: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]     val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                 ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/regression/LinearRegression.scala:570: value model in class LinearRegressionSummary is deprecated: The model field is deprecated and will be removed in 2.1.0.
[warn]     !model.getFitIntercept)
[warn]      ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/regression/LinearRegression.scala:634: value model in class LinearRegressionSummary is deprecated: The model field is deprecated and will be removed in 2.1.0.
[warn]   private val degreesOfFreedom: Long = if (model.getFitIntercept) {
[warn]                                            ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/regression/LinearRegression.scala:635: value model in class LinearRegressionSummary is deprecated: The model field is deprecated and will be removed in 2.1.0.
[warn]     numInstances - model.coefficients.size - 1
[warn]                    ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/regression/LinearRegression.scala:637: value model in class LinearRegressionSummary is deprecated: The model field is deprecated and will be removed in 2.1.0.
[warn]     numInstances - model.coefficients.size
[warn]                    ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/regression/LinearRegression.scala:645: value model in class LinearRegressionSummary is deprecated: The model field is deprecated and will be removed in 2.1.0.
[warn]     val weighted = if (!model.isDefined(model.weightCol) || model.getWeightCol.isEmpty) {
[warn]                         ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/regression/LinearRegression.scala:645: value model in class LinearRegressionSummary is deprecated: The model field is deprecated and will be removed in 2.1.0.
[warn]     val weighted = if (!model.isDefined(model.weightCol) || model.getWeightCol.isEmpty) {
[warn]                                         ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/regression/LinearRegression.scala:645: value model in class LinearRegressionSummary is deprecated: The model field is deprecated and will be removed in 2.1.0.
[warn]     val weighted = if (!model.isDefined(model.weightCol) || model.getWeightCol.isEmpty) {
[warn]                                                             ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/regression/LinearRegression.scala:648: value model in class LinearRegressionSummary is deprecated: The model field is deprecated and will be removed in 2.1.0.
[warn]       sqrt(col(model.getWeightCol))
[warn]                ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/regression/LinearRegression.scala:650: value model in class LinearRegressionSummary is deprecated: The model field is deprecated and will be removed in 2.1.0.
[warn]     val dr = predictions.select(col(model.getLabelCol).minus(col(model.getPredictionCol))
[warn]                                     ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/regression/LinearRegression.scala:650: value model in class LinearRegressionSummary is deprecated: The model field is deprecated and will be removed in 2.1.0.
[warn]     val dr = predictions.select(col(model.getLabelCol).minus(col(model.getPredictionCol))
[warn]                                                                  ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/regression/LinearRegression.scala:671: value model in class LinearRegressionSummary is deprecated: The model field is deprecated and will be removed in 2.1.0.
[warn]       val rss = if (!model.isDefined(model.weightCol) || model.getWeightCol.isEmpty) {
[warn]                      ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/regression/LinearRegression.scala:671: value model in class LinearRegressionSummary is deprecated: The model field is deprecated and will be removed in 2.1.0.
[warn]       val rss = if (!model.isDefined(model.weightCol) || model.getWeightCol.isEmpty) {
[warn]                                      ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/regression/LinearRegression.scala:671: value model in class LinearRegressionSummary is deprecated: The model field is deprecated and will be removed in 2.1.0.
[warn]       val rss = if (!model.isDefined(model.weightCol) || model.getWeightCol.isEmpty) {
[warn]                                                          ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/regression/LinearRegression.scala:676: value model in class LinearRegressionSummary is deprecated: The model field is deprecated and will be removed in 2.1.0.
[warn]         predictions.select(t(col(model.getPredictionCol), col(model.getLabelCol),
[warn]                                  ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/regression/LinearRegression.scala:676: value model in class LinearRegressionSummary is deprecated: The model field is deprecated and will be removed in 2.1.0.
[warn]         predictions.select(t(col(model.getPredictionCol), col(model.getLabelCol),
[warn]                                                               ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/regression/LinearRegression.scala:677: value model in class LinearRegressionSummary is deprecated: The model field is deprecated and will be removed in 2.1.0.
[warn]           col(model.getWeightCol)).as("wse")).agg(sum(col("wse"))).first().getDouble(0)
[warn]               ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/regression/LinearRegression.scala:698: value model in class LinearRegressionSummary is deprecated: The model field is deprecated and will be removed in 2.1.0.
[warn]       val estimate = if (model.getFitIntercept) {
[warn]                          ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/regression/LinearRegression.scala:699: value model in class LinearRegressionSummary is deprecated: The model field is deprecated and will be removed in 2.1.0.
[warn]         Array.concat(model.coefficients.toArray, Array(model.intercept))
[warn]                      ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/regression/LinearRegression.scala:699: value model in class LinearRegressionSummary is deprecated: The model field is deprecated and will be removed in 2.1.0.
[warn]         Array.concat(model.coefficients.toArray, Array(model.intercept))
[warn]                                                        ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/regression/LinearRegression.scala:701: value model in class LinearRegressionSummary is deprecated: The model field is deprecated and will be removed in 2.1.0.
[warn]         model.coefficients.toArray
[warn]         ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/ml/util/ReadWrite.scala:59: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       optionSQLContext = Some(SQLContext.getOrCreate(SparkContext.getOrCreate()))
[warn]                                          ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/api/python/PythonMLLibAPI.scala:155: class LinearRegressionWithSGD in package regression is deprecated: Use ml.regression.LinearRegression or LBFGS
[warn]     val lrAlg = new LinearRegressionWithSGD()
[warn]                     ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/api/python/PythonMLLibAPI.scala:184: class LassoWithSGD in package regression is deprecated: Use ml.regression.LinearRegression with elasticNetParam = 1.0. Note the default regParam is 0.01 for LassoWithSGD, but is 0.0 for LinearRegression.
[warn]     val lassoAlg = new LassoWithSGD()
[warn]                        ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/api/python/PythonMLLibAPI.scala:212: class RidgeRegressionWithSGD in package regression is deprecated: Use ml.regression.LinearRegression with elasticNetParam = 0.0. Note the default regParam is 0.01 for RidgeRegressionWithSGD, but is 0.0 for LinearRegression.
[warn]     val ridgeAlg = new RidgeRegressionWithSGD()
[warn]                        ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/api/python/PythonMLLibAPI.scala:271: class LogisticRegressionWithSGD in package classification is deprecated: Use ml.classification.LogisticRegression or LogisticRegressionWithLBFGS
[warn]     val LogRegAlg = new LogisticRegressionWithSGD()
[warn]                         ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/api/python/PythonMLLibAPI.scala:1181: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]     val sqlContext = SQLContext.getOrCreate(indexedRowMatrix.rows.sparkContext)
[warn]                                 ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/api/python/PythonMLLibAPI.scala:1191: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]     val sqlContext = SQLContext.getOrCreate(coordinateMatrix.entries.sparkContext)
[warn]                                 ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/api/python/PythonMLLibAPI.scala:1201: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]     val sqlContext = SQLContext.getOrCreate(blockMatrix.blocks.sparkContext)
[warn]                                 ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/classification/LogisticRegression.scala:440: constructor SQLContext in class SQLContext is deprecated: Use SparkSession.builder instead
[warn]         val sqlContext = new SQLContext(input.context)
[warn]                          ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/classification/NaiveBayes.scala:196: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/classification/NaiveBayes.scala:212: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/classification/NaiveBayes.scala:243: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/classification/NaiveBayes.scala:258: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/classification/StreamingLogisticRegressionWithSGD.scala:51: class LogisticRegressionWithSGD in package classification is deprecated: Use ml.classification.LogisticRegression or LogisticRegressionWithLBFGS
[warn]   extends StreamingLinearAlgorithm[LogisticRegressionModel, LogisticRegressionWithSGD]
[warn]           ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/classification/StreamingLogisticRegressionWithSGD.scala:63: class LogisticRegressionWithSGD in package classification is deprecated: Use ml.classification.LogisticRegression or LogisticRegressionWithLBFGS
[warn]   protected val algorithm = new LogisticRegressionWithSGD(
[warn]                                 ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/classification/impl/GLMClassificationModel.scala:54: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/classification/impl/GLMClassificationModel.scala:77: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/clustering/BisectingKMeansModel.scala:147: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/clustering/BisectingKMeansModel.scala:170: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/clustering/GaussianMixtureModel.scala:147: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/clustering/GaussianMixtureModel.scala:164: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/clustering/KMeansModel.scala:126: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/clustering/KMeansModel.scala:139: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/clustering/LDAModel.scala:449: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/clustering/LDAModel.scala:475: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/clustering/LDAModel.scala:856: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/clustering/LDAModel.scala:894: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/clustering/PowerIterationClustering.scala:73: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/clustering/PowerIterationClustering.scala:87: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/feature/ChiSqSelector.scala:137: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/feature/ChiSqSelector.scala:153: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/feature/Word2Vec.scala:613: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/feature/Word2Vec.scala:625: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/fpm/FPGrowth.scala:102: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/fpm/FPGrowth.scala:126: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/fpm/PrefixSpan.scala:619: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/fpm/PrefixSpan.scala:643: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/recommendation/MatrixFactorizationModel.scala:357: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/recommendation/MatrixFactorizationModel.scala:368: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/regression/IsotonicRegression.scala:188: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/regression/IsotonicRegression.scala:201: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/regression/StreamingLinearRegressionWithSGD.scala:48: class LinearRegressionWithSGD in package regression is deprecated: Use ml.regression.LinearRegression or LBFGS
[warn]   extends StreamingLinearAlgorithm[LinearRegressionModel, LinearRegressionWithSGD]
[warn]           ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/regression/StreamingLinearRegressionWithSGD.scala:61: class LinearRegressionWithSGD in package regression is deprecated: Use ml.regression.LinearRegression or LBFGS
[warn]   val algorithm = new LinearRegressionWithSGD(stepSize, numIterations, regParam, miniBatchFraction)
[warn]                       ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/regression/impl/GLMRegressionModel.scala:50: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/regression/impl/GLMRegressionModel.scala:71: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/tree/model/DecisionTreeModel.scala:205: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/tree/model/DecisionTreeModel.scala:246: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/tree/model/treeEnsembleModels.scala:416: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/main/scala/org/apache/spark/mllib/tree/model/treeEnsembleModels.scala:476: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]       val sqlContext = SQLContext.getOrCreate(sc)
[warn]                                   ^
[warn] 75 warnings found
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] 1 warning
[info] Compile success at May 20, 2016 12:35:18 PM [30.698s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:compile (default-compile) @ spark-mllib_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 4 source files to /home/cass/spark2/spark/mllib/target/scala-2.11/classes
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (create-tmp-dir) @ spark-mllib_2.11 ---
[INFO] Executing tasks

main:
    [mkdir] Created dir: /home/cass/spark2/spark/mllib/target/tmp
[INFO] Executed tasks
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ spark-mllib_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 1 resource
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:testCompile (scala-test-compile-first) @ spark-mllib_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 155 Scala sources and 61 Java sources to /home/cass/spark2/spark/mllib/target/scala-2.11/test-classes...
[warn] /home/cass/spark2/spark/mllib/src/test/scala/org/apache/spark/mllib/fpm/PrefixSpanSuite.scala:384: inferred existential type scala.collection.immutable.Set[(Seq[scala.collection.immutable.Set[_$2]], Long)] forSome { type _$2 }, which cannot be expressed by wildcards,  should be enabled
[warn] by making the implicit value scala.language.existentials visible.
[warn] This can be achieved by adding the import clause 'import scala.language.existentials'
[warn] or by setting the compiler option -language:existentials.
[warn] See the Scaladoc for value scala.language.existentials for a discussion
[warn] why the feature should be explicitly enabled.
[warn]       }.toSet
[warn]         ^
[warn] /home/cass/spark2/spark/mllib/src/test/scala/org/apache/spark/ml/feature/QuantileDiscretizerSuite.scala:30: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]     val sqlCtx = SQLContext.getOrCreate(sc)
[warn]                             ^
[warn] /home/cass/spark2/spark/mllib/src/test/scala/org/apache/spark/ml/feature/QuantileDiscretizerSuite.scala:56: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]     val sqlCtx = SQLContext.getOrCreate(sc)
[warn]                             ^
[warn] /home/cass/spark2/spark/mllib/src/test/scala/org/apache/spark/ml/feature/QuantileDiscretizerSuite.scala:85: method getOrCreate in object SQLContext is deprecated: Use SparkSession.builder instead
[warn]     val sqlCtx = SQLContext.getOrCreate(sc)
[warn]                             ^
[warn] /home/cass/spark2/spark/mllib/src/test/scala/org/apache/spark/mllib/classification/LogisticRegressionSuite.scala:227: class LogisticRegressionWithSGD in package classification is deprecated: Use ml.classification.LogisticRegression or LogisticRegressionWithLBFGS
[warn]     val lr = new LogisticRegressionWithSGD().setIntercept(true)
[warn]                  ^
[warn] /home/cass/spark2/spark/mllib/src/test/scala/org/apache/spark/mllib/classification/LogisticRegressionSuite.scala:303: class LogisticRegressionWithSGD in package classification is deprecated: Use ml.classification.LogisticRegression or LogisticRegressionWithLBFGS
[warn]     val lr = new LogisticRegressionWithSGD().setIntercept(true)
[warn]                  ^
[warn] /home/cass/spark2/spark/mllib/src/test/scala/org/apache/spark/mllib/classification/LogisticRegressionSuite.scala:338: class LogisticRegressionWithSGD in package classification is deprecated: Use ml.classification.LogisticRegression or LogisticRegressionWithLBFGS
[warn]     val lr = new LogisticRegressionWithSGD().setIntercept(true)
[warn]                  ^
[warn] /home/cass/spark2/spark/mllib/src/test/scala/org/apache/spark/mllib/classification/LogisticRegressionSuite.scala:919: object LogisticRegressionWithSGD in package classification is deprecated: Use ml.classification.LogisticRegression or LogisticRegressionWithLBFGS
[warn]     val model = LogisticRegressionWithSGD.train(points, 2)
[warn]                 ^
[warn] /home/cass/spark2/spark/mllib/src/test/scala/org/apache/spark/mllib/evaluation/MulticlassMetricsSuite.scala:74: value precision in class MulticlassMetrics is deprecated: Use accuracy.
[warn]     assert(math.abs(metrics.accuracy - metrics.precision) < delta)
[warn]                                                ^
[warn] /home/cass/spark2/spark/mllib/src/test/scala/org/apache/spark/mllib/evaluation/MulticlassMetricsSuite.scala:75: value recall in class MulticlassMetrics is deprecated: Use accuracy.
[warn]     assert(math.abs(metrics.accuracy - metrics.recall) < delta)
[warn]                                                ^
[warn] /home/cass/spark2/spark/mllib/src/test/scala/org/apache/spark/mllib/evaluation/MulticlassMetricsSuite.scala:76: value fMeasure in class MulticlassMetrics is deprecated: Use accuracy.
[warn]     assert(math.abs(metrics.accuracy - metrics.fMeasure) < delta)
[warn]                                                ^
[warn] /home/cass/spark2/spark/mllib/src/test/scala/org/apache/spark/mllib/regression/LassoSuite.scala:58: class LassoWithSGD in package regression is deprecated: Use ml.regression.LinearRegression with elasticNetParam = 1.0. Note the default regParam is 0.01 for LassoWithSGD, but is 0.0 for LinearRegression.
[warn]     val ls = new LassoWithSGD()
[warn]                  ^
[warn] /home/cass/spark2/spark/mllib/src/test/scala/org/apache/spark/mllib/regression/LassoSuite.scala:102: class LassoWithSGD in package regression is deprecated: Use ml.regression.LinearRegression with elasticNetParam = 1.0. Note the default regParam is 0.01 for LassoWithSGD, but is 0.0 for LinearRegression.
[warn]     val ls = new LassoWithSGD()
[warn]                  ^
[warn] /home/cass/spark2/spark/mllib/src/test/scala/org/apache/spark/mllib/regression/LassoSuite.scala:156: object LassoWithSGD in package regression is deprecated: Use ml.regression.LinearRegression with elasticNetParam = 1.0. Note the default regParam is 0.01 for LassoWithSGD, but is 0.0 for LinearRegression.
[warn]     val model = LassoWithSGD.train(points, 2)
[warn]                 ^
[warn] /home/cass/spark2/spark/mllib/src/test/scala/org/apache/spark/mllib/regression/LinearRegressionSuite.scala:49: class LinearRegressionWithSGD in package regression is deprecated: Use ml.regression.LinearRegression or LBFGS
[warn]     val linReg = new LinearRegressionWithSGD().setIntercept(true)
[warn]                      ^
[warn] /home/cass/spark2/spark/mllib/src/test/scala/org/apache/spark/mllib/regression/LinearRegressionSuite.scala:75: class LinearRegressionWithSGD in package regression is deprecated: Use ml.regression.LinearRegression or LBFGS
[warn]     val linReg = new LinearRegressionWithSGD().setIntercept(false)
[warn]                      ^
[warn] /home/cass/spark2/spark/mllib/src/test/scala/org/apache/spark/mllib/regression/LinearRegressionSuite.scala:106: class LinearRegressionWithSGD in package regression is deprecated: Use ml.regression.LinearRegression or LBFGS
[warn]     val linReg = new LinearRegressionWithSGD().setIntercept(false)
[warn]                      ^
[warn] /home/cass/spark2/spark/mllib/src/test/scala/org/apache/spark/mllib/regression/LinearRegressionSuite.scala:163: object LinearRegressionWithSGD in package regression is deprecated: Use ml.regression.LinearRegression or LBFGS
[warn]     val model = LinearRegressionWithSGD.train(points, 2)
[warn]                 ^
[warn] /home/cass/spark2/spark/mllib/src/test/scala/org/apache/spark/mllib/regression/RidgeRegressionSuite.scala:63: class LinearRegressionWithSGD in package regression is deprecated: Use ml.regression.LinearRegression or LBFGS
[warn]     val linearReg = new LinearRegressionWithSGD()
[warn]                         ^
[warn] /home/cass/spark2/spark/mllib/src/test/scala/org/apache/spark/mllib/regression/RidgeRegressionSuite.scala:71: class RidgeRegressionWithSGD in package regression is deprecated: Use ml.regression.LinearRegression with elasticNetParam = 0.0. Note the default regParam is 0.01 for RidgeRegressionWithSGD, but is 0.0 for LinearRegression.
[warn]     val ridgeReg = new RidgeRegressionWithSGD()
[warn]                        ^
[warn] /home/cass/spark2/spark/mllib/src/test/scala/org/apache/spark/mllib/regression/RidgeRegressionSuite.scala:113: object RidgeRegressionWithSGD in package regression is deprecated: Use ml.regression.LinearRegression with elasticNetParam = 0.0. Note the default regParam is 0.01 for RidgeRegressionWithSGD, but is 0.0 for LinearRegression.
[warn]     val model = RidgeRegressionWithSGD.train(points, 2)
[warn]                 ^
[warn] /home/cass/spark2/spark/mllib/src/test/scala/org/apache/spark/mllib/util/MLlibTestSparkContext.scala:49: method clearActive in object SQLContext is deprecated: Use SparkSession.clearActiveSession instead
[warn]       SQLContext.clearActive()
[warn]                  ^
[warn] 22 warnings found
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/classification/JavaLogisticRegressionSuite.java:53: warning: [deprecation] LogisticRegressionWithSGD in org.apache.spark.mllib.classification has been deprecated
[warn]     LogisticRegressionWithSGD lrImpl = new LogisticRegressionWithSGD();
[warn]     ^
[warn] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/classification/JavaLogisticRegressionSuite.java:53: warning: [deprecation] LogisticRegressionWithSGD in org.apache.spark.mllib.classification has been deprecated
[warn]     LogisticRegressionWithSGD lrImpl = new LogisticRegressionWithSGD();
[warn]                                            ^
[warn] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/classification/JavaLogisticRegressionSuite.java:75: warning: [deprecation] LogisticRegressionWithSGD in org.apache.spark.mllib.classification has been deprecated
[warn]     LogisticRegressionModel model = LogisticRegressionWithSGD.train(
[warn]                                     ^
[warn] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/fpm/JavaPrefixSpanSuite.java:75: warning: [rawtypes] found raw type: PrefixSpanModel
[warn]       PrefixSpanModel newModel = PrefixSpanModel.load(spark.sparkContext(), outputPath);
[warn]       ^
[warn]   missing type arguments for generic class PrefixSpanModel<Item>
[warn]   where Item is a type-variable:
[warn]     Item extends Object declared in class PrefixSpanModel
[warn] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/fpm/JavaPrefixSpanSuite.java:76: warning: [unchecked] unchecked conversion
[warn]       JavaRDD<FreqSequence<Integer>> freqSeqs = newModel.freqSequences().toJavaRDD();
[warn]                                                                                   ^
[warn]   required: JavaRDD<FreqSequence<Integer>>
[warn]   found:    JavaRDD
[warn] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/regression/JavaLassoSuite.java:54: warning: [deprecation] LassoWithSGD in org.apache.spark.mllib.regression has been deprecated
[warn]     LassoWithSGD lassoSGDImpl = new LassoWithSGD();
[warn]     ^
[warn] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/regression/JavaLassoSuite.java:54: warning: [deprecation] LassoWithSGD in org.apache.spark.mllib.regression has been deprecated
[warn]     LassoWithSGD lassoSGDImpl = new LassoWithSGD();
[warn]                                     ^
[warn] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/regression/JavaLassoSuite.java:75: warning: [deprecation] LassoWithSGD in org.apache.spark.mllib.regression has been deprecated
[warn]     LassoModel model = LassoWithSGD.train(testRDD.rdd(), 100, 1.0, 0.01, 1.0);
[warn]                        ^
[warn] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/regression/JavaLinearRegressionSuite.java:56: warning: [deprecation] LinearRegressionWithSGD in org.apache.spark.mllib.regression has been deprecated
[warn]     LinearRegressionWithSGD linSGDImpl = new LinearRegressionWithSGD();
[warn]     ^
[warn] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/regression/JavaLinearRegressionSuite.java:56: warning: [deprecation] LinearRegressionWithSGD in org.apache.spark.mllib.regression has been deprecated
[warn]     LinearRegressionWithSGD linSGDImpl = new LinearRegressionWithSGD();
[warn]                                              ^
[warn] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/regression/JavaLinearRegressionSuite.java:75: warning: [deprecation] LinearRegressionWithSGD in org.apache.spark.mllib.regression has been deprecated
[warn]     LinearRegressionModel model = LinearRegressionWithSGD.train(testRDD.rdd(), 100);
[warn]                                   ^
[warn] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/regression/JavaLinearRegressionSuite.java:88: warning: [deprecation] LinearRegressionWithSGD in org.apache.spark.mllib.regression has been deprecated
[warn]     LinearRegressionWithSGD linSGDImpl = new LinearRegressionWithSGD();
[warn]     ^
[warn] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/regression/JavaLinearRegressionSuite.java:88: warning: [deprecation] LinearRegressionWithSGD in org.apache.spark.mllib.regression has been deprecated
[warn]     LinearRegressionWithSGD linSGDImpl = new LinearRegressionWithSGD();
[warn]                                              ^
[warn] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/regression/JavaRidgeRegressionSuite.java:61: warning: [deprecation] RidgeRegressionWithSGD in org.apache.spark.mllib.regression has been deprecated
[warn]     RidgeRegressionWithSGD ridgeSGDImpl = new RidgeRegressionWithSGD();
[warn]     ^
[warn] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/regression/JavaRidgeRegressionSuite.java:61: warning: [deprecation] RidgeRegressionWithSGD in org.apache.spark.mllib.regression has been deprecated
[warn]     RidgeRegressionWithSGD ridgeSGDImpl = new RidgeRegressionWithSGD();
[warn]                                               ^
[warn] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/regression/JavaRidgeRegressionSuite.java:85: warning: [deprecation] RidgeRegressionWithSGD in org.apache.spark.mllib.regression has been deprecated
[warn]     RidgeRegressionModel model = RidgeRegressionWithSGD.train(testRDD.rdd(), 200, 1.0, 0.0);
[warn]                                  ^
[warn] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/regression/JavaRidgeRegressionSuite.java:88: warning: [deprecation] RidgeRegressionWithSGD in org.apache.spark.mllib.regression has been deprecated
[warn]     model = RidgeRegressionWithSGD.train(testRDD.rdd(), 200, 1.0, 0.1);
[warn]             ^
[warn] 18 warnings
[info] Compile success at May 20, 2016 12:35:52 PM [32.538s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:testCompile (default-testCompile) @ spark-mllib_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 61 source files to /home/cass/spark2/spark/mllib/target/scala-2.11/test-classes
[WARNING] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/classification/JavaLogisticRegressionSuite.java:[53,4] [deprecation] LogisticRegressionWithSGD in org.apache.spark.mllib.classification has been deprecated
[WARNING] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/classification/JavaLogisticRegressionSuite.java:[53,43] [deprecation] LogisticRegressionWithSGD in org.apache.spark.mllib.classification has been deprecated
[WARNING] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/classification/JavaLogisticRegressionSuite.java:[75,36] [deprecation] LogisticRegressionWithSGD in org.apache.spark.mllib.classification has been deprecated
[WARNING] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/regression/JavaLassoSuite.java:[54,4] [deprecation] LassoWithSGD in org.apache.spark.mllib.regression has been deprecated
[WARNING] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/regression/JavaLassoSuite.java:[54,36] [deprecation] LassoWithSGD in org.apache.spark.mllib.regression has been deprecated
[WARNING] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/regression/JavaLassoSuite.java:[75,23] [deprecation] LassoWithSGD in org.apache.spark.mllib.regression has been deprecated
[WARNING] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/regression/JavaRidgeRegressionSuite.java:[61,4] [deprecation] RidgeRegressionWithSGD in org.apache.spark.mllib.regression has been deprecated
[WARNING] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/regression/JavaRidgeRegressionSuite.java:[61,46] [deprecation] RidgeRegressionWithSGD in org.apache.spark.mllib.regression has been deprecated
[WARNING] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/regression/JavaRidgeRegressionSuite.java:[85,33] [deprecation] RidgeRegressionWithSGD in org.apache.spark.mllib.regression has been deprecated
[WARNING] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/regression/JavaRidgeRegressionSuite.java:[88,12] [deprecation] RidgeRegressionWithSGD in org.apache.spark.mllib.regression has been deprecated
[WARNING] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/regression/JavaLinearRegressionSuite.java:[56,4] [deprecation] LinearRegressionWithSGD in org.apache.spark.mllib.regression has been deprecated
[WARNING] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/regression/JavaLinearRegressionSuite.java:[56,45] [deprecation] LinearRegressionWithSGD in org.apache.spark.mllib.regression has been deprecated
[WARNING] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/regression/JavaLinearRegressionSuite.java:[75,34] [deprecation] LinearRegressionWithSGD in org.apache.spark.mllib.regression has been deprecated
[WARNING] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/regression/JavaLinearRegressionSuite.java:[88,4] [deprecation] LinearRegressionWithSGD in org.apache.spark.mllib.regression has been deprecated
[WARNING] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/regression/JavaLinearRegressionSuite.java:[88,45] [deprecation] LinearRegressionWithSGD in org.apache.spark.mllib.regression has been deprecated
[WARNING] /home/cass/spark2/spark/mllib/src/test/java/org/apache/spark/mllib/fpm/JavaPrefixSpanSuite.java:[76,82] [unchecked] unchecked conversion
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (generate-test-classpath) @ spark-mllib_2.11 ---
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (default-test) @ spark-mllib_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (test) @ spark-mllib_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- scalatest-maven-plugin:1.0:test (test) @ spark-mllib_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (prepare-test-jar) @ spark-mllib_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/mllib/target/spark-mllib_2.11-2.0.0-SNAPSHOT-tests.jar
[INFO]
[INFO] --- maven-jar-plugin:2.6:jar (default-jar) @ spark-mllib_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/mllib/target/spark-mllib_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-site-plugin:3.3:attach-descriptor (attach-descriptor) @ spark-mllib_2.11 ---
[INFO]
[INFO] --- maven-shade-plugin:2.4.3:shade (default) @ spark-mllib_2.11 ---
[INFO] Excluding org.apache.spark:spark-core_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.avro:avro-mapred:jar:hadoop2:1.7.7 from the shaded jar.
[INFO] Excluding org.apache.avro:avro-ipc:jar:1.7.7 from the shaded jar.
[INFO] Excluding org.apache.avro:avro:jar:1.7.7 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-core-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-mapper-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding com.twitter:chill_2.11:jar:0.8.0 from the shaded jar.
[INFO] Excluding com.esotericsoftware:kryo-shaded:jar:3.0.3 from the shaded jar.
[INFO] Excluding com.esotericsoftware:minlog:jar:1.3.0 from the shaded jar.
[INFO] Excluding com.twitter:chill-java:jar:0.8.0 from the shaded jar.
[INFO] Excluding org.apache.xbean:xbean-asm5-shaded:jar:4.4 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding commons-cli:commons-cli:jar:1.2 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-math:jar:2.1 from the shaded jar.
[INFO] Excluding xmlenc:xmlenc:jar:0.52 from the shaded jar.
[INFO] Excluding commons-io:commons-io:jar:2.4 from the shaded jar.
[INFO] Excluding commons-lang:commons-lang:jar:2.6 from the shaded jar.
[INFO] Excluding commons-configuration:commons-configuration:jar:1.6 from the shaded jar.
[INFO] Excluding commons-collections:commons-collections:jar:3.2.2 from the shaded jar.
[INFO] Excluding commons-digester:commons-digester:jar:1.8 from the shaded jar.
[INFO] Excluding commons-beanutils:commons-beanutils:jar:1.7.0 from the shaded jar.
[INFO] Excluding commons-beanutils:commons-beanutils-core:jar:1.8.0 from the shaded jar.
[INFO] Excluding com.google.protobuf:protobuf-java:jar:2.5.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-auth:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-compress:jar:1.4.1 from the shaded jar.
[INFO] Excluding org.tukaani:xz:jar:1.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-hdfs:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.mortbay.jetty:jetty-util:jar:6.1.26 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-app:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding com.google.inject:guice:jar:3.0 from the shaded jar.
[INFO] Excluding javax.inject:javax.inject:jar:1 from the shaded jar.
[INFO] Excluding aopalliance:aopalliance:jar:1.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-server-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-shuffle:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-api:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-core:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-jobclient:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-annotations:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-launcher_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-network-common_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-network-shuffle_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.fusesource.leveldbjni:leveldbjni-all:jar:1.8 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-annotations:jar:2.5.3 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-unsafe_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding net.java.dev.jets3t:jets3t:jar:0.7.1 from the shaded jar.
[INFO] Excluding commons-codec:commons-codec:jar:1.10 from the shaded jar.
[INFO] Excluding commons-httpclient:commons-httpclient:jar:3.1 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-recipes:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-framework:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-client:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.zookeeper:zookeeper:jar:3.4.5 from the shaded jar.
[INFO] Excluding javax.servlet:javax.servlet-api:jar:3.1.0 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-lang3:jar:3.3.2 from the shaded jar.
[INFO] Excluding com.google.code.findbugs:jsr305:jar:1.3.9 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-api:jar:1.7.16 from the shaded jar.
[INFO] Excluding org.slf4j:jul-to-slf4j:jar:1.7.16 from the shaded jar.
[INFO] Excluding org.slf4j:jcl-over-slf4j:jar:1.7.16 from the shaded jar.
[INFO] Excluding log4j:log4j:jar:1.2.17 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-log4j12:jar:1.7.16 from the shaded jar.
[INFO] Excluding com.ning:compress-lzf:jar:1.0.3 from the shaded jar.
[INFO] Excluding org.xerial.snappy:snappy-java:jar:1.1.2.4 from the shaded jar.
[INFO] Excluding net.jpountz.lz4:lz4:jar:1.3.0 from the shaded jar.
[INFO] Excluding org.roaringbitmap:RoaringBitmap:jar:0.5.11 from the shaded jar.
[INFO] Excluding commons-net:commons-net:jar:2.2 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-library:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.json4s:json4s-jackson_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.json4s:json4s-core_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.json4s:json4s-ast_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.scala-lang:scalap:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-compiler:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-parser-combinators_2.11:jar:1.0.4 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-client:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.ws.rs:javax.ws.rs-api:jar:2.0.1 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-api:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-utils:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2.external:aopalliance-repackaged:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2.external:javax.inject:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-locator:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.javassist:javassist:jar:3.18.1-GA from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-common:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.annotation:javax.annotation-api:jar:1.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.bundles.repackaged:jersey-guava:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:osgi-resource-locator:jar:1.0.1 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-server:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.media:jersey-media-jaxb:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.validation:validation-api:jar:1.1.0.Final from the shaded jar.
[INFO] Excluding org.glassfish.jersey.containers:jersey-container-servlet:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.containers:jersey-container-servlet-core:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.apache.mesos:mesos:jar:shaded-protobuf:0.21.1 from the shaded jar.
[INFO] Excluding io.netty:netty-all:jar:4.0.29.Final from the shaded jar.
[INFO] Excluding io.netty:netty:jar:3.8.0.Final from the shaded jar.
[INFO] Excluding com.clearspring.analytics:stream:jar:2.7.0 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-core:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-jvm:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-json:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-graphite:jar:3.1.2 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-databind:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-core:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.module:jackson-module-scala_2.11:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.thoughtworks.paranamer:paranamer:jar:2.6 from the shaded jar.
[INFO] Excluding org.apache.ivy:ivy:jar:2.4.0 from the shaded jar.
[INFO] Excluding oro:oro:jar:2.0.8 from the shaded jar.
[INFO] Excluding net.razorvine:pyrolite:jar:4.9 from the shaded jar.
[INFO] Excluding net.sf.py4j:py4j:jar:0.10.1 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-streaming_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-sql_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding com.univocity:univocity-parsers:jar:2.1.0 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-sketch_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-catalyst_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.codehaus.janino:janino:jar:2.7.8 from the shaded jar.
[INFO] Excluding org.codehaus.janino:commons-compiler:jar:2.7.8 from the shaded jar.
[INFO] Excluding org.antlr:antlr4-runtime:jar:4.5.2-1 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-column:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-common:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-encoding:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-generator:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-hadoop:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-format:jar:2.3.0-incubating from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-jackson:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-graphx_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding com.github.fommil.netlib:core:jar:1.1.2 from the shaded jar.
[INFO] Excluding net.sourceforge.f2j:arpack_combined_all:jar:0.1 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-mllib-local_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.scalanlp:breeze_2.11:jar:0.11.2 from the shaded jar.
[INFO] Excluding org.scalanlp:breeze-macros_2.11:jar:0.11.2 from the shaded jar.
[INFO] Excluding net.sf.opencsv:opencsv:jar:2.3 from the shaded jar.
[INFO] Excluding com.github.rwl:jtransforms:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.spire-math:spire_2.11:jar:0.7.4 from the shaded jar.
[INFO] Excluding org.spire-math:spire-macros_2.11:jar:0.7.4 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-math3:jar:3.4.1 from the shaded jar.
[INFO] Excluding org.objenesis:objenesis:jar:2.1 from the shaded jar.
[INFO] Excluding org.jpmml:pmml-model:jar:1.2.7 from the shaded jar.
[INFO] Excluding org.jpmml:pmml-agent:jar:1.2.7 from the shaded jar.
[INFO] Excluding org.jpmml:pmml-schema:jar:1.2.7 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-tags_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Including org.spark-project.spark:unused:jar:1.0.0 in the shaded jar.
[INFO] Excluding org.scala-lang:scala-reflect:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-xml_2.11:jar:1.0.2 from the shaded jar.
[INFO] Replacing original artifact with shaded artifact.
[INFO] Replacing /home/cass/spark2/spark/mllib/target/spark-mllib_2.11-2.0.0-SNAPSHOT.jar with /home/cass/spark2/spark/mllib/target/spark-mllib_2.11-2.0.0-SNAPSHOT-shaded.jar
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/mllib/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/mllib/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/mllib/dependency-reduced-pom.xml
[INFO]
[INFO] --- maven-source-plugin:2.4:jar-no-fork (create-source-jar) @ spark-mllib_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/mllib/target/spark-mllib_2.11-2.0.0-SNAPSHOT-sources.jar
[INFO]
[INFO] --- maven-source-plugin:2.4:test-jar-no-fork (create-source-jar) @ spark-mllib_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/mllib/target/spark-mllib_2.11-2.0.0-SNAPSHOT-test-sources.jar
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Spark Project Tools 2.0.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.0.0:clean (default-clean) @ spark-tools_2.11 ---
[INFO]
[INFO] --- maven-enforcer-plugin:1.4.1:enforce (enforce-versions) @ spark-tools_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:add-source (eclipse-add-source) @ spark-tools_2.11 ---
[INFO] Add Source directory: /home/cass/spark2/spark/tools/src/main/scala
[INFO] Add Test Source directory: /home/cass/spark2/spark/tools/src/test/scala
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (default-cli) @ spark-tools_2.11 ---
[INFO] Dependencies classpath:
/home/cass/.m2/repository/org/clapper/classutil_2.11/1.0.6/classutil_2.11-1.0.6.jar:/home/cass/.m2/repository/org/spark-project/spark/unused/1.0.0/unused-1.0.0.jar:/home/cass/.m2/repository/org/clapper/grizzled-slf4j_2.11/1.0.2/grizzled-slf4j_2.11-1.0.2.jar:/home/cass/.m2/repository/org/scala-lang/scala-library/2.11.8/scala-library-2.11.8.jar:/home/cass/.m2/repository/jline/jline/2.6/jline-2.6.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-async_2.11/0.9.1/scala-async_2.11-0.9.1.jar:/home/cass/.m2/repository/org/scala-lang/scala-reflect/2.11.8/scala-reflect-2.11.8.jar:/home/cass/.m2/repository/org/clapper/grizzled-scala_2.11/1.4.0/grizzled-scala_2.11-1.4.0.jar:/home/cass/.m2/repository/org/ow2/asm/asm-commons/5.0.2/asm-commons-5.0.2.jar:/home/cass/.m2/repository/org/ow2/asm/asm-tree/5.0.2/asm-tree-5.0.2.jar:/home/cass/.m2/repository/org/ow2/asm/asm-util/5.0.2/asm-util-5.0.2.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-parser-combinators_2.11/1.0.4/scala-parser-combinators_2.11-1.0.4.jar:/home/cass/.m2/repository/org/slf4j/slf4j-api/1.7.16/slf4j-api-1.7.16.jar:/home/cass/.m2/repository/org/scala-lang/scala-compiler/2.11.8/scala-compiler-2.11.8.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-xml_2.11/1.0.4/scala-xml_2.11-1.0.4.jar:/home/cass/.m2/repository/org/ow2/asm/asm/5.0.2/asm-5.0.2.jar
[INFO]
[INFO] --- maven-remote-resources-plugin:1.5:process (default) @ spark-tools_2.11 ---
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ spark-tools_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/tools/src/main/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:compile (scala-compile-first) @ spark-tools_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 1 Scala source to /home/cass/spark2/spark/tools/target/scala-2.11/classes...
[info] Compile success at May 20, 2016 12:35:58 PM [0.773s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:compile (default-compile) @ spark-tools_2.11 ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (create-tmp-dir) @ spark-tools_2.11 ---
[INFO] Executing tasks

main:
    [mkdir] Created dir: /home/cass/spark2/spark/tools/target/tmp
[INFO] Executed tasks
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ spark-tools_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/tools/src/test/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:testCompile (scala-test-compile-first) @ spark-tools_2.11 ---
[INFO] No sources to compile
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:testCompile (default-testCompile) @ spark-tools_2.11 ---
[INFO] No sources to compile
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (generate-test-classpath) @ spark-tools_2.11 ---
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (default-test) @ spark-tools_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (test) @ spark-tools_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- scalatest-maven-plugin:1.0:test (test) @ spark-tools_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (prepare-test-jar) @ spark-tools_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/tools/target/spark-tools_2.11-2.0.0-SNAPSHOT-tests.jar
[INFO]
[INFO] --- maven-jar-plugin:2.6:jar (default-jar) @ spark-tools_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/tools/target/spark-tools_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-site-plugin:3.3:attach-descriptor (attach-descriptor) @ spark-tools_2.11 ---
[INFO]
[INFO] --- maven-shade-plugin:2.4.3:shade (default) @ spark-tools_2.11 ---
[INFO] Excluding org.scala-lang:scala-reflect:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-library:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-compiler:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-xml_2.11:jar:1.0.4 from the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-parser-combinators_2.11:jar:1.0.4 from the shaded jar.
[INFO] Excluding org.clapper:classutil_2.11:jar:1.0.6 from the shaded jar.
[INFO] Excluding org.ow2.asm:asm:jar:5.0.2 from the shaded jar.
[INFO] Excluding org.ow2.asm:asm-commons:jar:5.0.2 from the shaded jar.
[INFO] Excluding org.ow2.asm:asm-tree:jar:5.0.2 from the shaded jar.
[INFO] Excluding org.ow2.asm:asm-util:jar:5.0.2 from the shaded jar.
[INFO] Excluding org.clapper:grizzled-scala_2.11:jar:1.4.0 from the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-async_2.11:jar:0.9.1 from the shaded jar.
[INFO] Excluding jline:jline:jar:2.6 from the shaded jar.
[INFO] Excluding org.clapper:grizzled-slf4j_2.11:jar:1.0.2 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-api:jar:1.7.16 from the shaded jar.
[INFO] Including org.spark-project.spark:unused:jar:1.0.0 in the shaded jar.
[INFO] Replacing original artifact with shaded artifact.
[INFO] Replacing /home/cass/spark2/spark/tools/target/spark-tools_2.11-2.0.0-SNAPSHOT.jar with /home/cass/spark2/spark/tools/target/spark-tools_2.11-2.0.0-SNAPSHOT-shaded.jar
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/tools/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/tools/dependency-reduced-pom.xml
[INFO]
[INFO] --- maven-source-plugin:2.4:jar-no-fork (create-source-jar) @ spark-tools_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/tools/target/spark-tools_2.11-2.0.0-SNAPSHOT-sources.jar
[INFO]
[INFO] --- maven-source-plugin:2.4:test-jar-no-fork (create-source-jar) @ spark-tools_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/tools/target/spark-tools_2.11-2.0.0-SNAPSHOT-test-sources.jar
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Spark Project Hive 2.0.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.0.0:clean (default-clean) @ spark-hive_2.11 ---
[INFO]
[INFO] --- maven-enforcer-plugin:1.4.1:enforce (enforce-versions) @ spark-hive_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:add-source (eclipse-add-source) @ spark-hive_2.11 ---
[INFO] Add Source directory: /home/cass/spark2/spark/sql/hive/src/main/scala
[INFO] Add Test Source directory: /home/cass/spark2/spark/sql/hive/src/test/scala
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (default-cli) @ spark-hive_2.11 ---
[INFO] Dependencies classpath:
/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-jobclient/2.2.0/hadoop-mapreduce-client-jobclient-2.2.0.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-jackson/1.7.0/parquet-jackson-1.7.0.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-core/3.1.2/metrics-core-3.1.2.jar:/home/cass/.m2/repository/com/google/protobuf/protobuf-java/2.5.0/protobuf-java-2.5.0.jar:/home/cass/.m2/repository/aopalliance/aopalliance/1.0/aopalliance-1.0.jar:/home/cass/.m2/repository/net/razorvine/pyrolite/4.9/pyrolite-4.9.jar:/home/cass/.m2/repository/org/apache/derby/derby/10.11.1.1/derby-10.11.1.1.jar:/home/cass/.m2/repository/com/univocity/univocity-parsers/2.1.0/univocity-parsers-2.1.0.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-jvm/3.1.2/metrics-jvm-3.1.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-client/2.2.0/hadoop-client-2.2.0.jar:/home/cass/.m2/repository/com/googlecode/javaewah/JavaEWAH/0.3.2/JavaEWAH-0.3.2.jar:/home/cass/.m2/repository/org/fusesource/leveldbjni/leveldbjni-all/1.8/leveldbjni-all-1.8.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-format/2.3.0-incubating/parquet-format-2.3.0-incubating.jar:/home/cass/.m2/repository/org/antlr/stringtemplate/3.2.1/stringtemplate-3.2.1.jar:/home/cass/.m2/repository/org/glassfish/jersey/bundles/repackaged/jersey-guava/2.22.2/jersey-guava-2.22.2.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-json/3.1.2/metrics-json-3.1.2.jar:/home/cass/.m2/repository/net/java/dev/jets3t/jets3t/0.7.1/jets3t-0.7.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-common/2.2.0/hadoop-common-2.2.0.jar:/home/cass/.m2/repository/com/google/inject/guice/3.0/guice-3.0.jar:/home/cass/.m2/repository/commons-io/commons-io/2.4/commons-io-2.4.jar:/home/cass/spark2/spark/sql/core/target/spark-sql_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/commons-dbcp/commons-dbcp/1.4/commons-dbcp-1.4.jar:/home/cass/.m2/repository/org/scala-lang/scala-reflect/2.11.8/scala-reflect-2.11.8.jar:/home/cass/.m2/repository/org/xerial/snappy/snappy-java/1.1.2.4/snappy-java-1.1.2.4.jar:/home/cass/.m2/repository/org/json4s/json4s-jackson_2.11/3.2.11/json4s-jackson_2.11-3.2.11.jar:/home/cass/.m2/repository/com/esotericsoftware/minlog/1.3.0/minlog-1.3.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-auth/2.2.0/hadoop-auth-2.2.0.jar:/home/cass/.m2/repository/org/antlr/ST4/4.0.4/ST4-4.0.4.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-core-asl/1.9.13/jackson-core-asl-1.9.13.jar:/home/cass/.m2/repository/javax/validation/validation-api/1.1.0.Final/validation-api-1.1.0.Final.jar:/home/cass/.m2/repository/net/jpountz/lz4/lz4/1.3.0/lz4-1.3.0.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-common/2.22.2/jersey-common-2.22.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-client/2.2.0/hadoop-yarn-client-2.2.0.jar:/home/cass/.m2/repository/joda-time/joda-time/2.9.3/joda-time-2.9.3.jar:/home/cass/.m2/repository/io/netty/netty/3.8.0.Final/netty-3.8.0.Final.jar:/home/cass/.m2/repository/org/apache/mesos/mesos/0.21.1/mesos-0.21.1-shaded-protobuf.jar:/home/cass/.m2/repository/org/iq80/snappy/snappy/0.2/snappy-0.2.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-annotations/2.5.3/jackson-annotations-2.5.3.jar:/home/cass/.m2/repository/com/google/code/findbugs/jsr305/1.3.9/jsr305-1.3.9.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-api/2.4.0-b34/hk2-api-2.4.0-b34.jar:/home/cass/.m2/repository/net/sf/opencsv/opencsv/2.3/opencsv-2.3.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-server/2.22.2/jersey-server-2.22.2.jar:/home/cass/.m2/repository/net/sf/py4j/py4j/0.10.1/py4j-0.10.1.jar:/home/cass/.m2/repository/com/twitter/chill-java/0.8.0/chill-java-0.8.0.jar:/home/cass/.m2/repository/commons-lang/commons-lang/2.6/commons-lang-2.6.jar:/home/cass/.m2/repository/org/spark-project/hive/hive-exec/1.2.1.spark2/hive-exec-1.2.1.spark2.jar:/home/cass/.m2/repository/org/tukaani/xz/1.0/xz-1.0.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-databind/2.5.3/jackson-databind-2.5.3.jar:/home/cass/.m2/repository/javolution/javolution/5.5.1/javolution-5.5.1.jar:/home/cass/.m2/repository/com/jolbox/bonecp/0.8.0.RELEASE/bonecp-0.8.0.RELEASE.jar:/home/cass/.m2/repository/org/codehaus/janino/janino/2.7.8/janino-2.7.8.jar:/home/cass/.m2/repository/org/apache/curator/curator-recipes/2.4.0/curator-recipes-2.4.0.jar:/home/cass/.m2/repository/org/codehaus/janino/commons-compiler/2.7.6/commons-compiler-2.7.6.jar:/home/cass/.m2/repository/commons-codec/commons-codec/1.10/commons-codec-1.10.jar:/home/cass/.m2/repository/org/javassist/javassist/3.18.1-GA/javassist-3.18.1-GA.jar:/home/cass/.m2/repository/org/apache/ivy/ivy/2.4.0/ivy-2.4.0.jar:/home/cass/.m2/repository/javax/inject/javax.inject/1/javax.inject-1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-core/2.2.0/hadoop-mapreduce-client-core-2.2.0.jar:/home/cass/.m2/repository/com/fasterxml/jackson/module/jackson-module-scala_2.11/2.5.3/jackson-module-scala_2.11-2.5.3.jar:/home/cass/.m2/repository/commons-beanutils/commons-beanutils-core/1.8.0/commons-beanutils-core-1.8.0.jar:/home/cass/.m2/repository/javax/servlet/javax.servlet-api/3.1.0/javax.servlet-api-3.1.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/osgi-resource-locator/1.0.1/osgi-resource-locator-1.0.1.jar:/home/cass/.m2/repository/org/apache/commons/commons-math3/3.4.1/commons-math3-3.4.1.jar:/home/cass/spark2/spark/common/network-common/target/spark-network-common_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/javax/transaction/jta/1.1/jta-1.1.jar:/home/cass/.m2/repository/org/apache/avro/avro/1.7.7/avro-1.7.7.jar:/home/cass/.m2/repository/org/apache/thrift/libthrift/0.9.2/libthrift-0.9.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-common/2.2.0/hadoop-mapreduce-client-common-2.2.0.jar:/home/cass/.m2/repository/log4j/apache-log4j-extras/1.2.17/apache-log4j-extras-1.2.17.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-utils/2.4.0-b34/hk2-utils-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/hk2/external/aopalliance-repackaged/2.4.0-b34/aopalliance-repackaged-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/hk2/external/javax.inject/2.4.0-b34/javax.inject-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/jersey/containers/jersey-container-servlet-core/2.22.2/jersey-container-servlet-core-2.22.2.jar:/home/cass/.m2/repository/org/apache/calcite/calcite-core/1.2.0-incubating/calcite-core-1.2.0-incubating.jar:/home/cass/.m2/repository/oro/oro/2.0.8/oro-2.0.8.jar:/home/cass/.m2/repository/javax/jdo/jdo-api/3.0.1/jdo-api-3.0.1.jar:/home/cass/.m2/repository/org/scala-lang/scala-compiler/2.11.8/scala-compiler-2.11.8.jar:/home/cass/.m2/repository/org/antlr/antlr-runtime/3.4/antlr-runtime-3.4.jar:/home/cass/.m2/repository/stax/stax-api/1.0.1/stax-api-1.0.1.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-encoding/1.7.0/parquet-encoding-1.7.0.jar:/home/cass/.m2/repository/org/apache/calcite/calcite-avatica/1.2.0-incubating/calcite-avatica-1.2.0-incubating.jar:/home/cass/.m2/repository/org/roaringbitmap/RoaringBitmap/0.5.11/RoaringBitmap-0.5.11.jar:/home/cass/.m2/repository/log4j/log4j/1.2.17/log4j-1.2.17.jar:/home/cass/.m2/repository/com/twitter/parquet-hadoop-bundle/1.6.0/parquet-hadoop-bundle-1.6.0.jar:/home/cass/.m2/repository/org/scala-lang/scala-library/2.11.8/scala-library-2.11.8.jar:/home/cass/.m2/repository/org/datanucleus/datanucleus-core/3.2.10/datanucleus-core-3.2.10.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-hadoop/1.7.0/parquet-hadoop-1.7.0.jar:/home/cass/.m2/repository/jline/jline/2.12/jline-2.12.jar:/home/cass/.m2/repository/org/apache/curator/curator-client/2.4.0/curator-client-2.4.0.jar:/home/cass/.m2/repository/org/apache/commons/commons-compress/1.4.1/commons-compress-1.4.1.jar:/home/cass/.m2/repository/org/apache/calcite/calcite-linq4j/1.2.0-incubating/calcite-linq4j-1.2.0-incubating.jar:/home/cass/.m2/repository/antlr/antlr/2.7.7/antlr-2.7.7.jar:/home/cass/.m2/repository/commons-pool/commons-pool/1.5.4/commons-pool-1.5.4.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-app/2.2.0/hadoop-mapreduce-client-app-2.2.0.jar:/home/cass/.m2/repository/org/slf4j/slf4j-api/1.7.16/slf4j-api-1.7.16.jar:/home/cass/.m2/repository/org/apache/xbean/xbean-asm5-shaded/4.4/xbean-asm5-shaded-4.4.jar:/home/cass/.m2/repository/org/json4s/json4s-core_2.11/3.2.11/json4s-core_2.11-3.2.11.jar:/home/cass/.m2/repository/org/apache/httpcomponents/httpclient/4.5.2/httpclient-4.5.2.jar:/home/cass/.m2/repository/org/mortbay/jetty/jetty-util/6.1.26/jetty-util-6.1.26.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-server-common/2.2.0/hadoop-yarn-server-common-2.2.0.jar:/home/cass/.m2/repository/org/jodd/jodd-core/3.5.2/jodd-core-3.5.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-hdfs/2.2.0/hadoop-hdfs-2.2.0.jar:/home/cass/.m2/repository/org/apache/thrift/libfb303/0.9.2/libfb303-0.9.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-api/2.2.0/hadoop-yarn-api-2.2.0.jar:/home/cass/.m2/repository/net/hydromatic/eigenbase-properties/1.1.5/eigenbase-properties-1.1.5.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-mapper-asl/1.9.13/jackson-mapper-asl-1.9.13.jar:/home/cass/.m2/repository/com/esotericsoftware/kryo-shaded/3.0.3/kryo-shaded-3.0.3.jar:/home/cass/.m2/repository/javax/ws/rs/javax.ws.rs-api/2.0.1/javax.ws.rs-api-2.0.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-common/2.2.0/hadoop-yarn-common-2.2.0.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-client/2.22.2/jersey-client-2.22.2.jar:/home/cass/spark2/spark/common/unsafe/target/spark-unsafe_2.11-2.0.0-SNAPSHOT.jar:/home/cass/spark2/spark/sql/catalyst/target/spark-catalyst_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-column/1.7.0/parquet-column-1.7.0.jar:/home/cass/.m2/repository/org/apache/avro/avro-mapred/1.7.7/avro-mapred-1.7.7-hadoop2.jar:/home/cass/.m2/repository/xmlenc/xmlenc/0.52/xmlenc-0.52.jar:/home/cass/.m2/repository/com/ning/compress-lzf/1.0.3/compress-lzf-1.0.3.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-shuffle/2.2.0/hadoop-mapreduce-client-shuffle-2.2.0.jar:/home/cass/.m2/repository/org/apache/zookeeper/zookeeper/3.4.5/zookeeper-3.4.5.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-common/1.7.0/parquet-common-1.7.0.jar:/home/cass/.m2/repository/org/spark-project/hive/hive-metastore/1.2.1.spark2/hive-metastore-1.2.1.spark2.jar:/home/cass/.m2/repository/com/thoughtworks/paranamer/paranamer/2.3/paranamer-2.3.jar:/home/cass/.m2/repository/org/apache/curator/curator-framework/2.4.0/curator-framework-2.4.0.jar:/home/cass/.m2/repository/commons-net/commons-net/2.2/commons-net-2.2.jar:/home/cass/.m2/repository/org/apache/commons/commons-lang3/3.3.2/commons-lang3-3.3.2.jar:/home/cass/.m2/repository/org/json4s/json4s-ast_2.11/3.2.11/json4s-ast_2.11-3.2.11.jar:/home/cass/spark2/spark/launcher/target/spark-launcher_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/scala-lang/scalap/2.11.8/scalap-2.11.8.jar:/home/cass/.m2/repository/com/clearspring/analytics/stream/2.7.0/stream-2.7.0.jar:/home/cass/.m2/repository/org/apache/commons/commons-math/2.1/commons-math-2.1.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-generator/1.7.0/parquet-generator-1.7.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-annotations/2.2.0/hadoop-annotations-2.2.0.jar:/home/cass/.m2/repository/commons-configuration/commons-configuration/1.6/commons-configuration-1.6.jar:/home/cass/.m2/repository/org/glassfish/jersey/containers/jersey-container-servlet/2.22.2/jersey-container-servlet-2.22.2.jar:/home/cass/.m2/repository/commons-digester/commons-digester/1.8/commons-digester-1.8.jar:/home/cass/.m2/repository/org/slf4j/jul-to-slf4j/1.7.16/jul-to-slf4j-1.7.16.jar:/home/cass/.m2/repository/commons-beanutils/commons-beanutils/1.7.0/commons-beanutils-1.7.0.jar:/home/cass/.m2/repository/org/antlr/antlr4-runtime/4.5.2-1/antlr4-runtime-4.5.2-1.jar:/home/cass/spark2/spark/common/network-shuffle/target/spark-network-shuffle_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-xml_2.11/1.0.2/scala-xml_2.11-1.0.2.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-parser-combinators_2.11/1.0.4/scala-parser-combinators_2.11-1.0.4.jar:/home/cass/.m2/repository/commons-cli/commons-cli/1.2/commons-cli-1.2.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-graphite/3.1.2/metrics-graphite-3.1.2.jar:/home/cass/.m2/repository/org/objenesis/objenesis/2.1/objenesis-2.1.jar:/home/cass/.m2/repository/javax/annotation/javax.annotation-api/1.2/javax.annotation-api-1.2.jar:/home/cass/.m2/repository/org/slf4j/slf4j-log4j12/1.7.16/slf4j-log4j12-1.7.16.jar:/home/cass/spark2/spark/common/sketch/target/spark-sketch_2.11-2.0.0-SNAPSHOT.jar:/home/cass/spark2/spark/core/target/spark-core_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/glassfish/jersey/media/jersey-media-jaxb/2.22.2/jersey-media-jaxb-2.22.2.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-core/2.5.3/jackson-core-2.5.3.jar:/home/cass/.m2/repository/org/spark-project/spark/unused/1.0.0/unused-1.0.0.jar:/home/cass/.m2/repository/org/apache/avro/avro-ipc/1.7.7/avro-ipc-1.7.7.jar:/home/cass/.m2/repository/commons-collections/commons-collections/3.2.2/commons-collections-3.2.2.jar:/home/cass/.m2/repository/org/datanucleus/datanucleus-rdbms/3.2.9/datanucleus-rdbms-3.2.9.jar:/home/cass/.m2/repository/com/twitter/chill_2.11/0.8.0/chill_2.11-0.8.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-locator/2.4.0-b34/hk2-locator-2.4.0-b34.jar:/home/cass/.m2/repository/commons-logging/commons-logging/1.1.3/commons-logging-1.1.3.jar:/home/cass/.m2/repository/org/datanucleus/datanucleus-api-jdo/3.2.6/datanucleus-api-jdo-3.2.6.jar:/home/cass/.m2/repository/org/slf4j/jcl-over-slf4j/1.7.16/jcl-over-slf4j-1.7.16.jar:/home/cass/.m2/repository/org/json/json/20090211/json-20090211.jar:/home/cass/.m2/repository/io/netty/netty-all/4.0.29.Final/netty-all-4.0.29.Final.jar:/home/cass/.m2/repository/commons-httpclient/commons-httpclient/3.1/commons-httpclient-3.1.jar:/home/cass/.m2/repository/org/apache/httpcomponents/httpcore/4.4.4/httpcore-4.4.4.jar:/home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-remote-resources-plugin:1.5:process (default) @ spark-hive_2.11 ---
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ spark-hive_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 1 resource
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:compile (scala-compile-first) @ spark-hive_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 28 Scala sources and 2 Java sources to /home/cass/spark2/spark/sql/hive/target/scala-2.11/classes...
[warn] /home/cass/spark2/spark/sql/hive/src/main/scala/org/apache/spark/sql/hive/TableReader.scala:85: trait Deserializer in package serde2 is deprecated: see corresponding Javadoc for more information.
[warn]       Utils.classForName(relation.tableDesc.getSerdeClassName).asInstanceOf[Class[Deserializer]],
[warn]                                                                             ^
[warn] /home/cass/spark2/spark/sql/hive/src/main/scala/org/apache/spark/sql/hive/TableReader.scala:99: trait Deserializer in package serde2 is deprecated: see corresponding Javadoc for more information.
[warn]       deserializerClass: Class[_ <: Deserializer],
[warn]                          ^
[warn] /home/cass/spark2/spark/sql/hive/src/main/scala/org/apache/spark/sql/hive/TableReader.scala:133: trait Deserializer in package serde2 is deprecated: see corresponding Javadoc for more information.
[warn]       (part, part.getDeserializer.getClass.asInstanceOf[Class[Deserializer]])).toMap
[warn]                                                         ^
[warn] /home/cass/spark2/spark/sql/hive/src/main/scala/org/apache/spark/sql/hive/TableReader.scala:148: trait Deserializer in package serde2 is deprecated: see corresponding Javadoc for more information.
[warn]       partitionToDeserializer: Map[HivePartition,
[warn]                                ^
[warn] /home/cass/spark2/spark/sql/hive/src/main/scala/org/apache/spark/sql/hive/TableReader.scala:154: trait Deserializer in package serde2 is deprecated: see corresponding Javadoc for more information.
[warn]         partitionToDeserializer: Map[HivePartition, Class[_ <: Deserializer]]):
[warn]                                  ^
[warn] /home/cass/spark2/spark/sql/hive/src/main/scala/org/apache/spark/sql/hive/TableReader.scala:155: trait Deserializer in package serde2 is deprecated: see corresponding Javadoc for more information.
[warn]         Map[HivePartition, Class[_ <: Deserializer]] = {
[warn]         ^
[warn] /home/cass/spark2/spark/sql/hive/src/main/scala/org/apache/spark/sql/hive/TableReader.scala:346: trait Deserializer in package serde2 is deprecated: see corresponding Javadoc for more information.
[warn]       rawDeser: Deserializer,
[warn]                 ^
[warn] /home/cass/spark2/spark/sql/hive/src/main/scala/org/apache/spark/sql/hive/TableReader.scala:349: trait Deserializer in package serde2 is deprecated: see corresponding Javadoc for more information.
[warn]       tableDeser: Deserializer): Iterator[InternalRow] = {
[warn]                   ^
[warn] /home/cass/spark2/spark/sql/hive/src/main/scala/org/apache/spark/sql/hive/execution/ScriptTransformation.scala:396: method initialize in class AbstractSerDe is deprecated: see corresponding Javadoc for more information.
[warn]     serde.initialize(null, properties)
[warn]           ^
[warn] /home/cass/spark2/spark/sql/hive/src/main/scala/org/apache/spark/sql/hive/hiveUDFs.scala:197: method initialize in class GenericUDTF is deprecated: see corresponding Javadoc for more information.
[warn]   protected lazy val outputInspector = function.initialize(inputInspectors.toArray)
[warn]                                                 ^
[warn] /home/cass/spark2/spark/sql/hive/src/main/scala/org/apache/spark/sql/hive/hiveUDFs.scala:274: class UDAF in package exec is deprecated: see corresponding Javadoc for more information.
[warn]       new GenericUDAFBridge(funcWrapper.createFunction[UDAF]())
[warn]                                                        ^
[warn] /home/cass/spark2/spark/sql/hive/src/main/scala/org/apache/spark/sql/hive/hiveUDFs.scala:296: trait AggregationBuffer in object GenericUDAFEvaluator is deprecated: see corresponding Javadoc for more information.
[warn]   private[this] var buffer: GenericUDAFEvaluator.AggregationBuffer = _
[warn]                                                  ^
[warn] /home/cass/spark2/spark/sql/hive/src/main/scala/org/apache/spark/sql/hive/hiveWriterContainers.scala:158: trait Serializer in package serde2 is deprecated: see corresponding Javadoc for more information.
[warn]   def newSerializer(tableDesc: TableDesc): Serializer = {
[warn]                                            ^
[warn] /home/cass/spark2/spark/sql/hive/src/main/scala/org/apache/spark/sql/hive/hiveWriterContainers.scala:159: trait Serializer in package serde2 is deprecated: see corresponding Javadoc for more information.
[warn]     val serializer = tableDesc.getDeserializerClass.newInstance().asInstanceOf[Serializer]
[warn]                                                                                ^
[warn] /home/cass/spark2/spark/sql/hive/src/main/scala/org/apache/spark/sql/hive/hiveWriterContainers.scala:182: trait Serializer in package serde2 is deprecated: see corresponding Javadoc for more information.
[warn]       val (serializer, standardOI, fieldOIs, dataTypes, wrappers, outputData) = prepareForWrite()
[warn]                                                                                                ^
[warn] /home/cass/spark2/spark/sql/hive/src/main/scala/org/apache/spark/sql/hive/hiveWriterContainers.scala:254: trait Serializer in package serde2 is deprecated: see corresponding Javadoc for more information.
[warn]     val (serializer, standardOI, fieldOIs, dataTypes, wrappers, outputData) = prepareForWrite()
[warn]                                                                                              ^
[warn] 16 warnings found
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] 1 warning
[info] Compile success at May 20, 2016 12:36:06 PM [7.117s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:compile (default-compile) @ spark-hive_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 2 source files to /home/cass/spark2/spark/sql/hive/target/scala-2.11/classes
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (create-tmp-dir) @ spark-hive_2.11 ---
[INFO] Executing tasks

main:
    [mkdir] Created dir: /home/cass/spark2/spark/sql/hive/target/tmp
[INFO] Executed tasks
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ spark-hive_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 9263 resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:testCompile (scala-test-compile-first) @ spark-hive_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 66 Scala sources and 14 Java sources to /home/cass/spark2/spark/sql/hive/target/scala-2.11/test-classes...
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] /home/cass/spark2/spark/sql/hive/src/test/java/org/apache/spark/sql/hive/test/Complex.java:53: warning: [rawtypes] found raw type: IScheme
[warn]   private static final Map<Class<? extends IScheme>, SchemeFactory> schemes = new HashMap<>();
[warn]                                            ^
[warn]   missing type arguments for generic class IScheme<T>
[warn]   where T is a type-variable:
[warn]     T extends TBase declared in interface IScheme
[warn] /home/cass/spark2/spark/sql/hive/src/test/java/org/apache/spark/sql/hive/test/Complex.java:464: warning: [unchecked] unchecked cast
[warn]         setLint((List<Integer>)value);
[warn]                                ^
[warn]   required: List<Integer>
[warn]   found:    Object
[warn] /home/cass/spark2/spark/sql/hive/src/test/java/org/apache/spark/sql/hive/test/Complex.java:472: warning: [unchecked] unchecked cast
[warn]         setLString((List<String>)value);
[warn]                                  ^
[warn]   required: List<String>
[warn]   found:    Object
[warn] /home/cass/spark2/spark/sql/hive/src/test/java/org/apache/spark/sql/hive/test/Complex.java:480: warning: [unchecked] unchecked cast
[warn]         setLintString((List<IntString>)value);
[warn]                                        ^
[warn]   required: List<IntString>
[warn]   found:    Object
[warn] /home/cass/spark2/spark/sql/hive/src/test/java/org/apache/spark/sql/hive/test/Complex.java:488: warning: [unchecked] unchecked cast
[warn]         setMStringString((Map<String,String>)value);
[warn]                                              ^
[warn]   required: Map<String,String>
[warn]   found:    Object
[warn] /home/cass/spark2/spark/sql/hive/src/test/java/org/apache/spark/sql/hive/test/Complex.java:679: warning: [cast] redundant cast to Complex
[warn]     Complex typedOther = (Complex)other;
[warn]                          ^
[warn] /home/cass/spark2/spark/sql/hive/src/test/java/org/apache/spark/sql/hive/test/Complex.java:749: warning: [unchecked] unchecked call to read(TProtocol,T) as a member of the raw type IScheme
[warn]     schemes.get(iprot.getScheme()).getScheme().read(iprot, this);
[warn]                                                    ^
[warn]   where T is a type-variable:
[warn]     T extends TBase declared in interface IScheme
[warn] /home/cass/spark2/spark/sql/hive/src/test/java/org/apache/spark/sql/hive/test/Complex.java:753: warning: [unchecked] unchecked call to write(TProtocol,T) as a member of the raw type IScheme
[warn]     schemes.get(oprot.getScheme()).getScheme().write(oprot, this);
[warn]                                                     ^
[warn]   where T is a type-variable:
[warn]     T extends TBase declared in interface IScheme
[warn] /home/cass/spark2/spark/sql/hive/src/test/java/org/apache/spark/sql/hive/test/Complex.java:842: warning: [unchecked] getScheme() in ComplexStandardSchemeFactory implements <S>getScheme() in SchemeFactory
[warn]     public ComplexStandardScheme getScheme() {
[warn]                                  ^
[warn]   return type requires unchecked conversion from ComplexStandardScheme to S
[warn]   where S is a type-variable:
[warn]     S extends IScheme declared in method <S>getScheme()
[warn] /home/cass/spark2/spark/sql/hive/src/test/java/org/apache/spark/sql/hive/test/Complex.java:1027: warning: [unchecked] getScheme() in ComplexTupleSchemeFactory implements <S>getScheme() in SchemeFactory
[warn]     public ComplexTupleScheme getScheme() {
[warn]                               ^
[warn]   return type requires unchecked conversion from ComplexTupleScheme to S
[warn]   where S is a type-variable:
[warn]     S extends IScheme declared in method <S>getScheme()
[warn] 11 warnings
[info] Compile success at May 20, 2016 12:36:27 PM [18.662s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:testCompile (default-testCompile) @ spark-hive_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 14 source files to /home/cass/spark2/spark/sql/hive/target/scala-2.11/test-classes
[WARNING] /home/cass/spark2/spark/sql/hive/src/test/java/org/apache/spark/sql/hive/test/Complex.java:[464,31] [unchecked] unchecked cast
[WARNING]   required: List<Integer>
  found:    Object
/home/cass/spark2/spark/sql/hive/src/test/java/org/apache/spark/sql/hive/test/Complex.java:[472,33] [unchecked] unchecked cast
[WARNING]   required: List<String>
  found:    Object
/home/cass/spark2/spark/sql/hive/src/test/java/org/apache/spark/sql/hive/test/Complex.java:[480,39] [unchecked] unchecked cast
[WARNING]   required: List<IntString>
  found:    Object
/home/cass/spark2/spark/sql/hive/src/test/java/org/apache/spark/sql/hive/test/Complex.java:[488,45] [unchecked] unchecked cast
[WARNING]   required: Map<String,String>
  found:    Object
/home/cass/spark2/spark/sql/hive/src/test/java/org/apache/spark/sql/hive/test/Complex.java:[749,51] [unchecked] unchecked call to read(TProtocol,T) as a member of the raw type IScheme
[WARNING]   where T is a type-variable:
    T extends TBase declared in interface IScheme
/home/cass/spark2/spark/sql/hive/src/test/java/org/apache/spark/sql/hive/test/Complex.java:[753,52] [unchecked] unchecked call to write(TProtocol,T) as a member of the raw type IScheme
[WARNING]   where T is a type-variable:
    T extends TBase declared in interface IScheme
/home/cass/spark2/spark/sql/hive/src/test/java/org/apache/spark/sql/hive/test/Complex.java:[842,33] [unchecked] getScheme() in ComplexStandardSchemeFactory implements <S>getScheme() in SchemeFactory
[WARNING]   return type requires unchecked conversion from ComplexStandardScheme to S
  where S is a type-variable:
    S extends IScheme declared in method <S>getScheme()
/home/cass/spark2/spark/sql/hive/src/test/java/org/apache/spark/sql/hive/test/Complex.java:[1027,30] [unchecked] getScheme() in ComplexTupleSchemeFactory implements <S>getScheme() in SchemeFactory
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (generate-test-classpath) @ spark-hive_2.11 ---
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (default-test) @ spark-hive_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (test) @ spark-hive_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- scalatest-maven-plugin:1.0:test (test) @ spark-hive_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (prepare-test-jar) @ spark-hive_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/sql/hive/target/spark-hive_2.11-2.0.0-SNAPSHOT-tests.jar
[INFO]
[INFO] --- maven-jar-plugin:2.6:jar (default-jar) @ spark-hive_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/sql/hive/target/spark-hive_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-site-plugin:3.3:attach-descriptor (attach-descriptor) @ spark-hive_2.11 ---
[INFO]
[INFO] --- maven-shade-plugin:2.4.3:shade (default) @ spark-hive_2.11 ---
[INFO] Excluding com.twitter:parquet-hadoop-bundle:jar:1.6.0 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-core_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding com.twitter:chill_2.11:jar:0.8.0 from the shaded jar.
[INFO] Excluding com.esotericsoftware:kryo-shaded:jar:3.0.3 from the shaded jar.
[INFO] Excluding com.esotericsoftware:minlog:jar:1.3.0 from the shaded jar.
[INFO] Excluding org.objenesis:objenesis:jar:2.1 from the shaded jar.
[INFO] Excluding com.twitter:chill-java:jar:0.8.0 from the shaded jar.
[INFO] Excluding org.apache.xbean:xbean-asm5-shaded:jar:4.4 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-math:jar:2.1 from the shaded jar.
[INFO] Excluding xmlenc:xmlenc:jar:0.52 from the shaded jar.
[INFO] Excluding commons-configuration:commons-configuration:jar:1.6 from the shaded jar.
[INFO] Excluding commons-collections:commons-collections:jar:3.2.2 from the shaded jar.
[INFO] Excluding commons-digester:commons-digester:jar:1.8 from the shaded jar.
[INFO] Excluding commons-beanutils:commons-beanutils:jar:1.7.0 from the shaded jar.
[INFO] Excluding commons-beanutils:commons-beanutils-core:jar:1.8.0 from the shaded jar.
[INFO] Excluding com.google.protobuf:protobuf-java:jar:2.5.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-auth:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-hdfs:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.mortbay.jetty:jetty-util:jar:6.1.26 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-app:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding com.google.inject:guice:jar:3.0 from the shaded jar.
[INFO] Excluding javax.inject:javax.inject:jar:1 from the shaded jar.
[INFO] Excluding aopalliance:aopalliance:jar:1.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-server-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-shuffle:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-api:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-core:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-jobclient:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-annotations:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-launcher_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-network-common_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-network-shuffle_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.fusesource.leveldbjni:leveldbjni-all:jar:1.8 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-annotations:jar:2.5.3 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-unsafe_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding net.java.dev.jets3t:jets3t:jar:0.7.1 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-recipes:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-framework:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-client:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.zookeeper:zookeeper:jar:3.4.5 from the shaded jar.
[INFO] Excluding javax.servlet:javax.servlet-api:jar:3.1.0 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-lang3:jar:3.3.2 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-math3:jar:3.4.1 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-api:jar:1.7.16 from the shaded jar.
[INFO] Excluding org.slf4j:jul-to-slf4j:jar:1.7.16 from the shaded jar.
[INFO] Excluding org.slf4j:jcl-over-slf4j:jar:1.7.16 from the shaded jar.
[INFO] Excluding log4j:log4j:jar:1.2.17 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-log4j12:jar:1.7.16 from the shaded jar.
[INFO] Excluding com.ning:compress-lzf:jar:1.0.3 from the shaded jar.
[INFO] Excluding org.xerial.snappy:snappy-java:jar:1.1.2.4 from the shaded jar.
[INFO] Excluding net.jpountz.lz4:lz4:jar:1.3.0 from the shaded jar.
[INFO] Excluding org.roaringbitmap:RoaringBitmap:jar:0.5.11 from the shaded jar.
[INFO] Excluding commons-net:commons-net:jar:2.2 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-library:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.json4s:json4s-jackson_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.json4s:json4s-core_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.json4s:json4s-ast_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.scala-lang:scalap:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-compiler:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-parser-combinators_2.11:jar:1.0.4 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-client:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.ws.rs:javax.ws.rs-api:jar:2.0.1 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-api:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-utils:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2.external:aopalliance-repackaged:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2.external:javax.inject:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-locator:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.javassist:javassist:jar:3.18.1-GA from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-common:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.annotation:javax.annotation-api:jar:1.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.bundles.repackaged:jersey-guava:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:osgi-resource-locator:jar:1.0.1 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-server:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.media:jersey-media-jaxb:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.validation:validation-api:jar:1.1.0.Final from the shaded jar.
[INFO] Excluding org.glassfish.jersey.containers:jersey-container-servlet:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.containers:jersey-container-servlet-core:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.apache.mesos:mesos:jar:shaded-protobuf:0.21.1 from the shaded jar.
[INFO] Excluding io.netty:netty-all:jar:4.0.29.Final from the shaded jar.
[INFO] Excluding io.netty:netty:jar:3.8.0.Final from the shaded jar.
[INFO] Excluding com.clearspring.analytics:stream:jar:2.7.0 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-core:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-jvm:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-json:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-graphite:jar:3.1.2 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-databind:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-core:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.module:jackson-module-scala_2.11:jar:2.5.3 from the shaded jar.
[INFO] Excluding org.apache.ivy:ivy:jar:2.4.0 from the shaded jar.
[INFO] Excluding oro:oro:jar:2.0.8 from the shaded jar.
[INFO] Excluding net.razorvine:pyrolite:jar:4.9 from the shaded jar.
[INFO] Excluding net.sf.py4j:py4j:jar:0.10.1 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-sql_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding com.univocity:univocity-parsers:jar:2.1.0 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-sketch_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-catalyst_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-column:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-common:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-encoding:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-generator:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-hadoop:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-format:jar:2.3.0-incubating from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-jackson:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-tags_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.spark-project.hive:hive-exec:jar:1.2.1.spark2 from the shaded jar.
[INFO] Excluding commons-io:commons-io:jar:2.4 from the shaded jar.
[INFO] Excluding commons-lang:commons-lang:jar:2.6 from the shaded jar.
[INFO] Excluding javolution:javolution:jar:5.5.1 from the shaded jar.
[INFO] Excluding log4j:apache-log4j-extras:jar:1.2.17 from the shaded jar.
[INFO] Excluding org.antlr:antlr-runtime:jar:3.4 from the shaded jar.
[INFO] Excluding org.antlr:stringtemplate:jar:3.2.1 from the shaded jar.
[INFO] Excluding antlr:antlr:jar:2.7.7 from the shaded jar.
[INFO] Excluding org.antlr:ST4:jar:4.0.4 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-compress:jar:1.4.1 from the shaded jar.
[INFO] Excluding org.tukaani:xz:jar:1.0 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-core-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding com.googlecode.javaewah:JavaEWAH:jar:0.3.2 from the shaded jar.
[INFO] Excluding org.iq80.snappy:snappy:jar:0.2 from the shaded jar.
[INFO] Excluding org.json:json:jar:20090211 from the shaded jar.
[INFO] Excluding stax:stax-api:jar:1.0.1 from the shaded jar.
[INFO] Excluding net.sf.opencsv:opencsv:jar:2.3 from the shaded jar.
[INFO] Excluding jline:jline:jar:2.12 from the shaded jar.
[INFO] Excluding org.spark-project.hive:hive-metastore:jar:1.2.1.spark2 from the shaded jar.
[INFO] Excluding com.jolbox:bonecp:jar:0.8.0.RELEASE from the shaded jar.
[INFO] Excluding commons-cli:commons-cli:jar:1.2 from the shaded jar.
[INFO] Excluding commons-logging:commons-logging:jar:1.1.3 from the shaded jar.
[INFO] Excluding org.apache.derby:derby:jar:10.11.1.1 from the shaded jar.
[INFO] Excluding org.datanucleus:datanucleus-api-jdo:jar:3.2.6 from the shaded jar.
[INFO] Excluding org.datanucleus:datanucleus-rdbms:jar:3.2.9 from the shaded jar.
[INFO] Excluding commons-pool:commons-pool:jar:1.5.4 from the shaded jar.
[INFO] Excluding commons-dbcp:commons-dbcp:jar:1.4 from the shaded jar.
[INFO] Excluding javax.jdo:jdo-api:jar:3.0.1 from the shaded jar.
[INFO] Excluding javax.transaction:jta:jar:1.1 from the shaded jar.
[INFO] Excluding org.apache.avro:avro:jar:1.7.7 from the shaded jar.
[INFO] Excluding com.thoughtworks.paranamer:paranamer:jar:2.3 from the shaded jar.
[INFO] Excluding org.apache.avro:avro-mapred:jar:hadoop2:1.7.7 from the shaded jar.
[INFO] Excluding org.apache.avro:avro-ipc:jar:1.7.7 from the shaded jar.
[INFO] Excluding commons-httpclient:commons-httpclient:jar:3.1 from the shaded jar.
[INFO] Excluding org.apache.calcite:calcite-avatica:jar:1.2.0-incubating from the shaded jar.
[INFO] Excluding org.apache.calcite:calcite-core:jar:1.2.0-incubating from the shaded jar.
[INFO] Excluding org.apache.calcite:calcite-linq4j:jar:1.2.0-incubating from the shaded jar.
[INFO] Excluding net.hydromatic:eigenbase-properties:jar:1.1.5 from the shaded jar.
[INFO] Excluding org.codehaus.janino:commons-compiler:jar:2.7.6 from the shaded jar.
[INFO] Excluding org.apache.httpcomponents:httpclient:jar:4.5.2 from the shaded jar.
[INFO] Excluding org.apache.httpcomponents:httpcore:jar:4.4.4 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-mapper-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding commons-codec:commons-codec:jar:1.10 from the shaded jar.
[INFO] Excluding joda-time:joda-time:jar:2.9.3 from the shaded jar.
[INFO] Excluding org.jodd:jodd-core:jar:3.5.2 from the shaded jar.
[INFO] Excluding com.google.code.findbugs:jsr305:jar:1.3.9 from the shaded jar.
[INFO] Excluding org.datanucleus:datanucleus-core:jar:3.2.10 from the shaded jar.
[INFO] Excluding org.apache.thrift:libthrift:jar:0.9.2 from the shaded jar.
[INFO] Excluding org.apache.thrift:libfb303:jar:0.9.2 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-reflect:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.codehaus.janino:janino:jar:2.7.8 from the shaded jar.
[INFO] Excluding org.antlr:antlr4-runtime:jar:4.5.2-1 from the shaded jar.
[INFO] Including org.spark-project.spark:unused:jar:1.0.0 in the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-xml_2.11:jar:1.0.2 from the shaded jar.
[INFO] Replacing original artifact with shaded artifact.
[INFO] Replacing /home/cass/spark2/spark/sql/hive/target/spark-hive_2.11-2.0.0-SNAPSHOT.jar with /home/cass/spark2/spark/sql/hive/target/spark-hive_2.11-2.0.0-SNAPSHOT-shaded.jar
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/sql/hive/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/sql/hive/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/sql/hive/dependency-reduced-pom.xml
[INFO]
[INFO] --- maven-source-plugin:2.4:jar-no-fork (create-source-jar) @ spark-hive_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/sql/hive/target/spark-hive_2.11-2.0.0-SNAPSHOT-sources.jar
[INFO]
[INFO] --- maven-source-plugin:2.4:test-jar-no-fork (create-source-jar) @ spark-hive_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/sql/hive/target/spark-hive_2.11-2.0.0-SNAPSHOT-test-sources.jar
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Spark Project HiveContext Compatibility 2.0.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.0.0:clean (default-clean) @ spark-hivecontext-compatibility_2.11 ---
[INFO]
[INFO] --- maven-enforcer-plugin:1.4.1:enforce (enforce-versions) @ spark-hivecontext-compatibility_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:add-source (eclipse-add-source) @ spark-hivecontext-compatibility_2.11 ---
[INFO] Add Source directory: /home/cass/spark2/spark/sql/hivecontext-compatibility/src/main/scala
[INFO] Add Test Source directory: /home/cass/spark2/spark/sql/hivecontext-compatibility/src/test/scala
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (default-cli) @ spark-hivecontext-compatibility_2.11 ---
[INFO] Dependencies classpath:
/home/cass/.m2/repository/org/apache/parquet/parquet-jackson/1.7.0/parquet-jackson-1.7.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-jobclient/2.2.0/hadoop-mapreduce-client-jobclient-2.2.0.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-core/3.1.2/metrics-core-3.1.2.jar:/home/cass/.m2/repository/com/google/protobuf/protobuf-java/2.5.0/protobuf-java-2.5.0.jar:/home/cass/.m2/repository/aopalliance/aopalliance/1.0/aopalliance-1.0.jar:/home/cass/.m2/repository/org/apache/derby/derby/10.11.1.1/derby-10.11.1.1.jar:/home/cass/.m2/repository/net/razorvine/pyrolite/4.9/pyrolite-4.9.jar:/home/cass/.m2/repository/com/univocity/univocity-parsers/2.1.0/univocity-parsers-2.1.0.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-jvm/3.1.2/metrics-jvm-3.1.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-client/2.2.0/hadoop-client-2.2.0.jar:/home/cass/.m2/repository/com/googlecode/javaewah/JavaEWAH/0.3.2/JavaEWAH-0.3.2.jar:/home/cass/.m2/repository/org/fusesource/leveldbjni/leveldbjni-all/1.8/leveldbjni-all-1.8.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-format/2.3.0-incubating/parquet-format-2.3.0-incubating.jar:/home/cass/.m2/repository/org/antlr/stringtemplate/3.2.1/stringtemplate-3.2.1.jar:/home/cass/.m2/repository/org/glassfish/jersey/bundles/repackaged/jersey-guava/2.22.2/jersey-guava-2.22.2.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-json/3.1.2/metrics-json-3.1.2.jar:/home/cass/.m2/repository/net/java/dev/jets3t/jets3t/0.7.1/jets3t-0.7.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-common/2.2.0/hadoop-common-2.2.0.jar:/home/cass/.m2/repository/com/google/inject/guice/3.0/guice-3.0.jar:/home/cass/.m2/repository/commons-io/commons-io/2.4/commons-io-2.4.jar:/home/cass/spark2/spark/sql/core/target/spark-sql_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/commons-dbcp/commons-dbcp/1.4/commons-dbcp-1.4.jar:/home/cass/.m2/repository/org/scala-lang/scala-reflect/2.11.8/scala-reflect-2.11.8.jar:/home/cass/.m2/repository/org/xerial/snappy/snappy-java/1.1.2.4/snappy-java-1.1.2.4.jar:/home/cass/.m2/repository/org/json4s/json4s-jackson_2.11/3.2.11/json4s-jackson_2.11-3.2.11.jar:/home/cass/.m2/repository/com/esotericsoftware/minlog/1.3.0/minlog-1.3.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-auth/2.2.0/hadoop-auth-2.2.0.jar:/home/cass/.m2/repository/org/antlr/ST4/4.0.4/ST4-4.0.4.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-core-asl/1.9.13/jackson-core-asl-1.9.13.jar:/home/cass/.m2/repository/javax/validation/validation-api/1.1.0.Final/validation-api-1.1.0.Final.jar:/home/cass/.m2/repository/net/jpountz/lz4/lz4/1.3.0/lz4-1.3.0.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-common/2.22.2/jersey-common-2.22.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-client/2.2.0/hadoop-yarn-client-2.2.0.jar:/home/cass/.m2/repository/joda-time/joda-time/2.9.3/joda-time-2.9.3.jar:/home/cass/.m2/repository/io/netty/netty/3.8.0.Final/netty-3.8.0.Final.jar:/home/cass/.m2/repository/org/iq80/snappy/snappy/0.2/snappy-0.2.jar:/home/cass/.m2/repository/org/apache/mesos/mesos/0.21.1/mesos-0.21.1-shaded-protobuf.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-annotations/2.5.3/jackson-annotations-2.5.3.jar:/home/cass/.m2/repository/com/google/code/findbugs/jsr305/1.3.9/jsr305-1.3.9.jar:/home/cass/.m2/repository/net/sf/opencsv/opencsv/2.3/opencsv-2.3.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-api/2.4.0-b34/hk2-api-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-server/2.22.2/jersey-server-2.22.2.jar:/home/cass/.m2/repository/net/sf/py4j/py4j/0.10.1/py4j-0.10.1.jar:/home/cass/.m2/repository/commons-lang/commons-lang/2.6/commons-lang-2.6.jar:/home/cass/.m2/repository/com/twitter/chill-java/0.8.0/chill-java-0.8.0.jar:/home/cass/.m2/repository/org/spark-project/hive/hive-exec/1.2.1.spark2/hive-exec-1.2.1.spark2.jar:/home/cass/.m2/repository/org/tukaani/xz/1.0/xz-1.0.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-databind/2.5.3/jackson-databind-2.5.3.jar:/home/cass/.m2/repository/org/codehaus/janino/janino/2.7.8/janino-2.7.8.jar:/home/cass/.m2/repository/javolution/javolution/5.5.1/javolution-5.5.1.jar:/home/cass/.m2/repository/com/jolbox/bonecp/0.8.0.RELEASE/bonecp-0.8.0.RELEASE.jar:/home/cass/.m2/repository/org/codehaus/janino/commons-compiler/2.7.6/commons-compiler-2.7.6.jar:/home/cass/.m2/repository/commons-codec/commons-codec/1.10/commons-codec-1.10.jar:/home/cass/.m2/repository/org/apache/curator/curator-recipes/2.4.0/curator-recipes-2.4.0.jar:/home/cass/.m2/repository/org/javassist/javassist/3.18.1-GA/javassist-3.18.1-GA.jar:/home/cass/.m2/repository/org/apache/ivy/ivy/2.4.0/ivy-2.4.0.jar:/home/cass/.m2/repository/javax/inject/javax.inject/1/javax.inject-1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-core/2.2.0/hadoop-mapreduce-client-core-2.2.0.jar:/home/cass/.m2/repository/com/fasterxml/jackson/module/jackson-module-scala_2.11/2.5.3/jackson-module-scala_2.11-2.5.3.jar:/home/cass/.m2/repository/commons-beanutils/commons-beanutils-core/1.8.0/commons-beanutils-core-1.8.0.jar:/home/cass/.m2/repository/javax/servlet/javax.servlet-api/3.1.0/javax.servlet-api-3.1.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/osgi-resource-locator/1.0.1/osgi-resource-locator-1.0.1.jar:/home/cass/.m2/repository/org/apache/commons/commons-math3/3.4.1/commons-math3-3.4.1.jar:/home/cass/.m2/repository/javax/transaction/jta/1.1/jta-1.1.jar:/home/cass/spark2/spark/common/network-common/target/spark-network-common_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/avro/avro/1.7.7/avro-1.7.7.jar:/home/cass/.m2/repository/org/apache/thrift/libthrift/0.9.2/libthrift-0.9.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-common/2.2.0/hadoop-mapreduce-client-common-2.2.0.jar:/home/cass/.m2/repository/log4j/apache-log4j-extras/1.2.17/apache-log4j-extras-1.2.17.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-utils/2.4.0-b34/hk2-utils-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/hk2/external/aopalliance-repackaged/2.4.0-b34/aopalliance-repackaged-2.4.0-b34.jar:/home/cass/.m2/repository/org/apache/calcite/calcite-core/1.2.0-incubating/calcite-core-1.2.0-incubating.jar:/home/cass/.m2/repository/org/glassfish/hk2/external/javax.inject/2.4.0-b34/javax.inject-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/jersey/containers/jersey-container-servlet-core/2.22.2/jersey-container-servlet-core-2.22.2.jar:/home/cass/.m2/repository/javax/jdo/jdo-api/3.0.1/jdo-api-3.0.1.jar:/home/cass/.m2/repository/oro/oro/2.0.8/oro-2.0.8.jar:/home/cass/.m2/repository/org/scala-lang/scala-compiler/2.11.8/scala-compiler-2.11.8.jar:/home/cass/.m2/repository/org/antlr/antlr-runtime/3.4/antlr-runtime-3.4.jar:/home/cass/.m2/repository/stax/stax-api/1.0.1/stax-api-1.0.1.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-encoding/1.7.0/parquet-encoding-1.7.0.jar:/home/cass/.m2/repository/org/apache/calcite/calcite-avatica/1.2.0-incubating/calcite-avatica-1.2.0-incubating.jar:/home/cass/.m2/repository/org/roaringbitmap/RoaringBitmap/0.5.11/RoaringBitmap-0.5.11.jar:/home/cass/.m2/repository/log4j/log4j/1.2.17/log4j-1.2.17.jar:/home/cass/.m2/repository/com/twitter/parquet-hadoop-bundle/1.6.0/parquet-hadoop-bundle-1.6.0.jar:/home/cass/.m2/repository/org/scala-lang/scala-library/2.11.8/scala-library-2.11.8.jar:/home/cass/.m2/repository/org/datanucleus/datanucleus-core/3.2.10/datanucleus-core-3.2.10.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-hadoop/1.7.0/parquet-hadoop-1.7.0.jar:/home/cass/.m2/repository/jline/jline/2.12/jline-2.12.jar:/home/cass/.m2/repository/org/apache/curator/curator-client/2.4.0/curator-client-2.4.0.jar:/home/cass/.m2/repository/org/apache/commons/commons-compress/1.4.1/commons-compress-1.4.1.jar:/home/cass/.m2/repository/org/apache/calcite/calcite-linq4j/1.2.0-incubating/calcite-linq4j-1.2.0-incubating.jar:/home/cass/.m2/repository/antlr/antlr/2.7.7/antlr-2.7.7.jar:/home/cass/.m2/repository/commons-pool/commons-pool/1.5.4/commons-pool-1.5.4.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-app/2.2.0/hadoop-mapreduce-client-app-2.2.0.jar:/home/cass/.m2/repository/org/slf4j/slf4j-api/1.7.16/slf4j-api-1.7.16.jar:/home/cass/.m2/repository/org/apache/xbean/xbean-asm5-shaded/4.4/xbean-asm5-shaded-4.4.jar:/home/cass/.m2/repository/org/apache/httpcomponents/httpclient/4.5.2/httpclient-4.5.2.jar:/home/cass/.m2/repository/org/json4s/json4s-core_2.11/3.2.11/json4s-core_2.11-3.2.11.jar:/home/cass/.m2/repository/org/mortbay/jetty/jetty-util/6.1.26/jetty-util-6.1.26.jar:/home/cass/.m2/repository/org/jodd/jodd-core/3.5.2/jodd-core-3.5.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-server-common/2.2.0/hadoop-yarn-server-common-2.2.0.jar:/home/cass/.m2/repository/org/apache/thrift/libfb303/0.9.2/libfb303-0.9.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-hdfs/2.2.0/hadoop-hdfs-2.2.0.jar:/home/cass/.m2/repository/net/hydromatic/eigenbase-properties/1.1.5/eigenbase-properties-1.1.5.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-mapper-asl/1.9.13/jackson-mapper-asl-1.9.13.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-api/2.2.0/hadoop-yarn-api-2.2.0.jar:/home/cass/.m2/repository/com/esotericsoftware/kryo-shaded/3.0.3/kryo-shaded-3.0.3.jar:/home/cass/.m2/repository/javax/ws/rs/javax.ws.rs-api/2.0.1/javax.ws.rs-api-2.0.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-common/2.2.0/hadoop-yarn-common-2.2.0.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-client/2.22.2/jersey-client-2.22.2.jar:/home/cass/spark2/spark/common/unsafe/target/spark-unsafe_2.11-2.0.0-SNAPSHOT.jar:/home/cass/spark2/spark/sql/catalyst/target/spark-catalyst_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-column/1.7.0/parquet-column-1.7.0.jar:/home/cass/.m2/repository/org/apache/avro/avro-mapred/1.7.7/avro-mapred-1.7.7-hadoop2.jar:/home/cass/.m2/repository/xmlenc/xmlenc/0.52/xmlenc-0.52.jar:/home/cass/.m2/repository/com/ning/compress-lzf/1.0.3/compress-lzf-1.0.3.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-common/1.7.0/parquet-common-1.7.0.jar:/home/cass/.m2/repository/org/spark-project/hive/hive-metastore/1.2.1.spark2/hive-metastore-1.2.1.spark2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-shuffle/2.2.0/hadoop-mapreduce-client-shuffle-2.2.0.jar:/home/cass/.m2/repository/org/apache/zookeeper/zookeeper/3.4.5/zookeeper-3.4.5.jar:/home/cass/.m2/repository/com/thoughtworks/paranamer/paranamer/2.3/paranamer-2.3.jar:/home/cass/.m2/repository/org/apache/curator/curator-framework/2.4.0/curator-framework-2.4.0.jar:/home/cass/.m2/repository/commons-net/commons-net/2.2/commons-net-2.2.jar:/home/cass/.m2/repository/org/apache/commons/commons-lang3/3.3.2/commons-lang3-3.3.2.jar:/home/cass/.m2/repository/org/json4s/json4s-ast_2.11/3.2.11/json4s-ast_2.11-3.2.11.jar:/home/cass/spark2/spark/launcher/target/spark-launcher_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/scala-lang/scalap/2.11.8/scalap-2.11.8.jar:/home/cass/.m2/repository/com/clearspring/analytics/stream/2.7.0/stream-2.7.0.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-generator/1.7.0/parquet-generator-1.7.0.jar:/home/cass/.m2/repository/org/apache/commons/commons-math/2.1/commons-math-2.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-annotations/2.2.0/hadoop-annotations-2.2.0.jar:/home/cass/.m2/repository/commons-configuration/commons-configuration/1.6/commons-configuration-1.6.jar:/home/cass/.m2/repository/org/glassfish/jersey/containers/jersey-container-servlet/2.22.2/jersey-container-servlet-2.22.2.jar:/home/cass/.m2/repository/commons-digester/commons-digester/1.8/commons-digester-1.8.jar:/home/cass/.m2/repository/org/slf4j/jul-to-slf4j/1.7.16/jul-to-slf4j-1.7.16.jar:/home/cass/.m2/repository/commons-beanutils/commons-beanutils/1.7.0/commons-beanutils-1.7.0.jar:/home/cass/.m2/repository/org/antlr/antlr4-runtime/4.5.2-1/antlr4-runtime-4.5.2-1.jar:/home/cass/spark2/spark/common/network-shuffle/target/spark-network-shuffle_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-xml_2.11/1.0.2/scala-xml_2.11-1.0.2.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-parser-combinators_2.11/1.0.4/scala-parser-combinators_2.11-1.0.4.jar:/home/cass/.m2/repository/commons-cli/commons-cli/1.2/commons-cli-1.2.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-graphite/3.1.2/metrics-graphite-3.1.2.jar:/home/cass/.m2/repository/org/objenesis/objenesis/2.1/objenesis-2.1.jar:/home/cass/.m2/repository/javax/annotation/javax.annotation-api/1.2/javax.annotation-api-1.2.jar:/home/cass/.m2/repository/org/slf4j/slf4j-log4j12/1.7.16/slf4j-log4j12-1.7.16.jar:/home/cass/spark2/spark/common/sketch/target/spark-sketch_2.11-2.0.0-SNAPSHOT.jar:/home/cass/spark2/spark/core/target/spark-core_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/glassfish/jersey/media/jersey-media-jaxb/2.22.2/jersey-media-jaxb-2.22.2.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-core/2.5.3/jackson-core-2.5.3.jar:/home/cass/.m2/repository/org/spark-project/spark/unused/1.0.0/unused-1.0.0.jar:/home/cass/.m2/repository/org/apache/avro/avro-ipc/1.7.7/avro-ipc-1.7.7.jar:/home/cass/.m2/repository/org/datanucleus/datanucleus-rdbms/3.2.9/datanucleus-rdbms-3.2.9.jar:/home/cass/.m2/repository/commons-collections/commons-collections/3.2.2/commons-collections-3.2.2.jar:/home/cass/.m2/repository/com/twitter/chill_2.11/0.8.0/chill_2.11-0.8.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-locator/2.4.0-b34/hk2-locator-2.4.0-b34.jar:/home/cass/spark2/spark/sql/hive/target/spark-hive_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/commons-logging/commons-logging/1.1.3/commons-logging-1.1.3.jar:/home/cass/.m2/repository/org/datanucleus/datanucleus-api-jdo/3.2.6/datanucleus-api-jdo-3.2.6.jar:/home/cass/.m2/repository/org/slf4j/jcl-over-slf4j/1.7.16/jcl-over-slf4j-1.7.16.jar:/home/cass/.m2/repository/org/json/json/20090211/json-20090211.jar:/home/cass/.m2/repository/commons-httpclient/commons-httpclient/3.1/commons-httpclient-3.1.jar:/home/cass/.m2/repository/org/apache/httpcomponents/httpcore/4.4.4/httpcore-4.4.4.jar:/home/cass/.m2/repository/io/netty/netty-all/4.0.29.Final/netty-all-4.0.29.Final.jar:/home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-remote-resources-plugin:1.5:process (default) @ spark-hivecontext-compatibility_2.11 ---
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ spark-hivecontext-compatibility_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/sql/hivecontext-compatibility/src/main/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:compile (scala-compile-first) @ spark-hivecontext-compatibility_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 1 Scala source to /home/cass/spark2/spark/sql/hivecontext-compatibility/target/scala-2.11/classes...
[info] Compile success at May 20, 2016 12:36:35 PM [0.483s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:compile (default-compile) @ spark-hivecontext-compatibility_2.11 ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (create-tmp-dir) @ spark-hivecontext-compatibility_2.11 ---
[INFO] Executing tasks

main:
    [mkdir] Created dir: /home/cass/spark2/spark/sql/hivecontext-compatibility/target/tmp
[INFO] Executed tasks
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ spark-hivecontext-compatibility_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/sql/hivecontext-compatibility/src/test/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:testCompile (scala-test-compile-first) @ spark-hivecontext-compatibility_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 1 Scala source to /home/cass/spark2/spark/sql/hivecontext-compatibility/target/scala-2.11/test-classes...
[warn] /home/cass/spark2/spark/sql/hivecontext-compatibility/src/test/scala/org/apache/spark/sql/hive/HiveContextCompatibilitySuite.scala:28: class HiveContext in package hive is deprecated: Use SparkSession.builder.enableHiveSupport instead
[warn]   private var hc: HiveContext = null
[warn]                   ^
[warn] /home/cass/spark2/spark/sql/hivecontext-compatibility/src/test/scala/org/apache/spark/sql/hive/HiveContextCompatibilitySuite.scala:36: class HiveContext in package hive is deprecated: Use SparkSession.builder.enableHiveSupport instead
[warn]     hc = new HiveContext(sc)
[warn]              ^
[warn] two warnings found
[info] Compile success at May 20, 2016 12:36:36 PM [1.065s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:testCompile (default-testCompile) @ spark-hivecontext-compatibility_2.11 ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (generate-test-classpath) @ spark-hivecontext-compatibility_2.11 ---
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (default-test) @ spark-hivecontext-compatibility_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (test) @ spark-hivecontext-compatibility_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- scalatest-maven-plugin:1.0:test (test) @ spark-hivecontext-compatibility_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (prepare-test-jar) @ spark-hivecontext-compatibility_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/sql/hivecontext-compatibility/target/spark-hivecontext-compatibility_2.11-2.0.0-SNAPSHOT-tests.jar
[INFO]
[INFO] --- maven-jar-plugin:2.6:jar (default-jar) @ spark-hivecontext-compatibility_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/sql/hivecontext-compatibility/target/spark-hivecontext-compatibility_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-site-plugin:3.3:attach-descriptor (attach-descriptor) @ spark-hivecontext-compatibility_2.11 ---
[INFO]
[INFO] --- maven-shade-plugin:2.4.3:shade (default) @ spark-hivecontext-compatibility_2.11 ---
[INFO] Excluding org.apache.spark:spark-hive_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding com.twitter:parquet-hadoop-bundle:jar:1.6.0 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-core_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-sql_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding com.univocity:univocity-parsers:jar:2.1.0 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-sketch_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-catalyst_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.codehaus.janino:janino:jar:2.7.8 from the shaded jar.
[INFO] Excluding org.antlr:antlr4-runtime:jar:4.5.2-1 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-column:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-common:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-encoding:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-generator:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-hadoop:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-format:jar:2.3.0-incubating from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-jackson:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-tags_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.spark-project.hive:hive-exec:jar:1.2.1.spark2 from the shaded jar.
[INFO] Excluding commons-io:commons-io:jar:2.4 from the shaded jar.
[INFO] Excluding commons-lang:commons-lang:jar:2.6 from the shaded jar.
[INFO] Excluding javolution:javolution:jar:5.5.1 from the shaded jar.
[INFO] Excluding log4j:apache-log4j-extras:jar:1.2.17 from the shaded jar.
[INFO] Excluding org.antlr:antlr-runtime:jar:3.4 from the shaded jar.
[INFO] Excluding org.antlr:stringtemplate:jar:3.2.1 from the shaded jar.
[INFO] Excluding antlr:antlr:jar:2.7.7 from the shaded jar.
[INFO] Excluding org.antlr:ST4:jar:4.0.4 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-compress:jar:1.4.1 from the shaded jar.
[INFO] Excluding org.tukaani:xz:jar:1.0 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-core-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding com.googlecode.javaewah:JavaEWAH:jar:0.3.2 from the shaded jar.
[INFO] Excluding org.iq80.snappy:snappy:jar:0.2 from the shaded jar.
[INFO] Excluding org.json:json:jar:20090211 from the shaded jar.
[INFO] Excluding stax:stax-api:jar:1.0.1 from the shaded jar.
[INFO] Excluding net.sf.opencsv:opencsv:jar:2.3 from the shaded jar.
[INFO] Excluding jline:jline:jar:2.12 from the shaded jar.
[INFO] Excluding org.spark-project.hive:hive-metastore:jar:1.2.1.spark2 from the shaded jar.
[INFO] Excluding com.jolbox:bonecp:jar:0.8.0.RELEASE from the shaded jar.
[INFO] Excluding commons-cli:commons-cli:jar:1.2 from the shaded jar.
[INFO] Excluding commons-logging:commons-logging:jar:1.1.3 from the shaded jar.
[INFO] Excluding org.apache.derby:derby:jar:10.11.1.1 from the shaded jar.
[INFO] Excluding org.datanucleus:datanucleus-api-jdo:jar:3.2.6 from the shaded jar.
[INFO] Excluding org.datanucleus:datanucleus-rdbms:jar:3.2.9 from the shaded jar.
[INFO] Excluding commons-pool:commons-pool:jar:1.5.4 from the shaded jar.
[INFO] Excluding commons-dbcp:commons-dbcp:jar:1.4 from the shaded jar.
[INFO] Excluding javax.jdo:jdo-api:jar:3.0.1 from the shaded jar.
[INFO] Excluding javax.transaction:jta:jar:1.1 from the shaded jar.
[INFO] Excluding org.apache.avro:avro:jar:1.7.7 from the shaded jar.
[INFO] Excluding com.thoughtworks.paranamer:paranamer:jar:2.3 from the shaded jar.
[INFO] Excluding org.apache.avro:avro-mapred:jar:hadoop2:1.7.7 from the shaded jar.
[INFO] Excluding org.apache.avro:avro-ipc:jar:1.7.7 from the shaded jar.
[INFO] Excluding commons-httpclient:commons-httpclient:jar:3.1 from the shaded jar.
[INFO] Excluding org.apache.calcite:calcite-avatica:jar:1.2.0-incubating from the shaded jar.
[INFO] Excluding org.apache.calcite:calcite-core:jar:1.2.0-incubating from the shaded jar.
[INFO] Excluding org.apache.calcite:calcite-linq4j:jar:1.2.0-incubating from the shaded jar.
[INFO] Excluding net.hydromatic:eigenbase-properties:jar:1.1.5 from the shaded jar.
[INFO] Excluding org.codehaus.janino:commons-compiler:jar:2.7.6 from the shaded jar.
[INFO] Excluding org.apache.httpcomponents:httpclient:jar:4.5.2 from the shaded jar.
[INFO] Excluding org.apache.httpcomponents:httpcore:jar:4.4.4 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-mapper-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding commons-codec:commons-codec:jar:1.10 from the shaded jar.
[INFO] Excluding joda-time:joda-time:jar:2.9.3 from the shaded jar.
[INFO] Excluding org.jodd:jodd-core:jar:3.5.2 from the shaded jar.
[INFO] Excluding com.google.code.findbugs:jsr305:jar:1.3.9 from the shaded jar.
[INFO] Excluding org.datanucleus:datanucleus-core:jar:3.2.10 from the shaded jar.
[INFO] Excluding org.apache.thrift:libthrift:jar:0.9.2 from the shaded jar.
[INFO] Excluding org.apache.thrift:libfb303:jar:0.9.2 from the shaded jar.
[INFO] Excluding com.twitter:chill_2.11:jar:0.8.0 from the shaded jar.
[INFO] Excluding com.esotericsoftware:kryo-shaded:jar:3.0.3 from the shaded jar.
[INFO] Excluding com.esotericsoftware:minlog:jar:1.3.0 from the shaded jar.
[INFO] Excluding org.objenesis:objenesis:jar:2.1 from the shaded jar.
[INFO] Excluding com.twitter:chill-java:jar:0.8.0 from the shaded jar.
[INFO] Excluding org.apache.xbean:xbean-asm5-shaded:jar:4.4 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-math:jar:2.1 from the shaded jar.
[INFO] Excluding xmlenc:xmlenc:jar:0.52 from the shaded jar.
[INFO] Excluding commons-configuration:commons-configuration:jar:1.6 from the shaded jar.
[INFO] Excluding commons-collections:commons-collections:jar:3.2.2 from the shaded jar.
[INFO] Excluding commons-digester:commons-digester:jar:1.8 from the shaded jar.
[INFO] Excluding commons-beanutils:commons-beanutils:jar:1.7.0 from the shaded jar.
[INFO] Excluding commons-beanutils:commons-beanutils-core:jar:1.8.0 from the shaded jar.
[INFO] Excluding com.google.protobuf:protobuf-java:jar:2.5.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-auth:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-hdfs:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.mortbay.jetty:jetty-util:jar:6.1.26 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-app:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding com.google.inject:guice:jar:3.0 from the shaded jar.
[INFO] Excluding javax.inject:javax.inject:jar:1 from the shaded jar.
[INFO] Excluding aopalliance:aopalliance:jar:1.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-server-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-shuffle:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-api:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-core:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-jobclient:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-annotations:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-launcher_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-network-common_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-network-shuffle_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.fusesource.leveldbjni:leveldbjni-all:jar:1.8 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-annotations:jar:2.5.3 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-unsafe_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding net.java.dev.jets3t:jets3t:jar:0.7.1 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-recipes:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-framework:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-client:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.zookeeper:zookeeper:jar:3.4.5 from the shaded jar.
[INFO] Excluding javax.servlet:javax.servlet-api:jar:3.1.0 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-lang3:jar:3.3.2 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-math3:jar:3.4.1 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-api:jar:1.7.16 from the shaded jar.
[INFO] Excluding org.slf4j:jul-to-slf4j:jar:1.7.16 from the shaded jar.
[INFO] Excluding org.slf4j:jcl-over-slf4j:jar:1.7.16 from the shaded jar.
[INFO] Excluding log4j:log4j:jar:1.2.17 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-log4j12:jar:1.7.16 from the shaded jar.
[INFO] Excluding com.ning:compress-lzf:jar:1.0.3 from the shaded jar.
[INFO] Excluding org.xerial.snappy:snappy-java:jar:1.1.2.4 from the shaded jar.
[INFO] Excluding net.jpountz.lz4:lz4:jar:1.3.0 from the shaded jar.
[INFO] Excluding org.roaringbitmap:RoaringBitmap:jar:0.5.11 from the shaded jar.
[INFO] Excluding commons-net:commons-net:jar:2.2 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-library:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.json4s:json4s-jackson_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.json4s:json4s-core_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.json4s:json4s-ast_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.scala-lang:scalap:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-compiler:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-parser-combinators_2.11:jar:1.0.4 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-client:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.ws.rs:javax.ws.rs-api:jar:2.0.1 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-api:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-utils:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2.external:aopalliance-repackaged:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2.external:javax.inject:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-locator:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.javassist:javassist:jar:3.18.1-GA from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-common:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.annotation:javax.annotation-api:jar:1.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.bundles.repackaged:jersey-guava:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:osgi-resource-locator:jar:1.0.1 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-server:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.media:jersey-media-jaxb:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.validation:validation-api:jar:1.1.0.Final from the shaded jar.
[INFO] Excluding org.glassfish.jersey.containers:jersey-container-servlet:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.containers:jersey-container-servlet-core:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.apache.mesos:mesos:jar:shaded-protobuf:0.21.1 from the shaded jar.
[INFO] Excluding io.netty:netty-all:jar:4.0.29.Final from the shaded jar.
[INFO] Excluding io.netty:netty:jar:3.8.0.Final from the shaded jar.
[INFO] Excluding com.clearspring.analytics:stream:jar:2.7.0 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-core:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-jvm:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-json:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-graphite:jar:3.1.2 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-databind:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-core:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.module:jackson-module-scala_2.11:jar:2.5.3 from the shaded jar.
[INFO] Excluding org.apache.ivy:ivy:jar:2.4.0 from the shaded jar.
[INFO] Excluding oro:oro:jar:2.0.8 from the shaded jar.
[INFO] Excluding net.razorvine:pyrolite:jar:4.9 from the shaded jar.
[INFO] Excluding net.sf.py4j:py4j:jar:0.10.1 from the shaded jar.
[INFO] Including org.spark-project.spark:unused:jar:1.0.0 in the shaded jar.
[INFO] Excluding org.scala-lang:scala-reflect:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-xml_2.11:jar:1.0.2 from the shaded jar.
[INFO] Replacing original artifact with shaded artifact.
[INFO] Replacing /home/cass/spark2/spark/sql/hivecontext-compatibility/target/spark-hivecontext-compatibility_2.11-2.0.0-SNAPSHOT.jar with /home/cass/spark2/spark/sql/hivecontext-compatibility/target/spark-hivecontext-compatibility_2.11-2.0.0-SNAPSHOT-shaded.jar
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/sql/hivecontext-compatibility/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/sql/hivecontext-compatibility/dependency-reduced-pom.xml
[INFO]
[INFO] --- maven-source-plugin:2.4:jar-no-fork (create-source-jar) @ spark-hivecontext-compatibility_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/sql/hivecontext-compatibility/target/spark-hivecontext-compatibility_2.11-2.0.0-SNAPSHOT-sources.jar
[INFO]
[INFO] --- maven-source-plugin:2.4:test-jar-no-fork (create-source-jar) @ spark-hivecontext-compatibility_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/sql/hivecontext-compatibility/target/spark-hivecontext-compatibility_2.11-2.0.0-SNAPSHOT-test-sources.jar
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Spark Project REPL 2.0.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.0.0:clean (default-clean) @ spark-repl_2.11 ---
[INFO]
[INFO] --- maven-enforcer-plugin:1.4.1:enforce (enforce-versions) @ spark-repl_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:add-source (eclipse-add-source) @ spark-repl_2.11 ---
[INFO] Add Source directory: /home/cass/spark2/spark/repl/src/main/scala
[INFO] Add Test Source directory: /home/cass/spark2/spark/repl/src/test/scala
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (default-cli) @ spark-repl_2.11 ---
[INFO] Dependencies classpath:
/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-jobclient/2.2.0/hadoop-mapreduce-client-jobclient-2.2.0.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-jackson/1.7.0/parquet-jackson-1.7.0.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-core/3.1.2/metrics-core-3.1.2.jar:/home/cass/.m2/repository/com/google/protobuf/protobuf-java/2.5.0/protobuf-java-2.5.0.jar:/home/cass/.m2/repository/aopalliance/aopalliance/1.0/aopalliance-1.0.jar:/home/cass/.m2/repository/org/spire-math/spire-macros_2.11/0.7.4/spire-macros_2.11-0.7.4.jar:/home/cass/.m2/repository/net/razorvine/pyrolite/4.9/pyrolite-4.9.jar:/home/cass/.m2/repository/com/univocity/univocity-parsers/2.1.0/univocity-parsers-2.1.0.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-jvm/3.1.2/metrics-jvm-3.1.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-client/2.2.0/hadoop-client-2.2.0.jar:/home/cass/.m2/repository/org/fusesource/leveldbjni/leveldbjni-all/1.8/leveldbjni-all-1.8.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-format/2.3.0-incubating/parquet-format-2.3.0-incubating.jar:/home/cass/.m2/repository/org/glassfish/jersey/bundles/repackaged/jersey-guava/2.22.2/jersey-guava-2.22.2.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-json/3.1.2/metrics-json-3.1.2.jar:/home/cass/.m2/repository/org/spire-math/spire_2.11/0.7.4/spire_2.11-0.7.4.jar:/home/cass/.m2/repository/net/java/dev/jets3t/jets3t/0.7.1/jets3t-0.7.1.jar:/home/cass/spark2/spark/graphx/target/spark-graphx_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-common/2.2.0/hadoop-common-2.2.0.jar:/home/cass/spark2/spark/mllib/target/spark-mllib_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/jpmml/pmml-schema/1.2.7/pmml-schema-1.2.7.jar:/home/cass/.m2/repository/com/google/inject/guice/3.0/guice-3.0.jar:/home/cass/.m2/repository/commons-io/commons-io/2.4/commons-io-2.4.jar:/home/cass/spark2/spark/sql/core/target/spark-sql_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/net/sourceforge/f2j/arpack_combined_all/0.1/arpack_combined_all-0.1.jar:/home/cass/.m2/repository/org/scala-lang/scala-reflect/2.11.8/scala-reflect-2.11.8.jar:/home/cass/.m2/repository/org/xerial/snappy/snappy-java/1.1.2.4/snappy-java-1.1.2.4.jar:/home/cass/.m2/repository/org/json4s/json4s-jackson_2.11/3.2.11/json4s-jackson_2.11-3.2.11.jar:/home/cass/.m2/repository/org/jpmml/pmml-agent/1.2.7/pmml-agent-1.2.7.jar:/home/cass/.m2/repository/com/esotericsoftware/minlog/1.3.0/minlog-1.3.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-auth/2.2.0/hadoop-auth-2.2.0.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-core-asl/1.9.13/jackson-core-asl-1.9.13.jar:/home/cass/.m2/repository/javax/validation/validation-api/1.1.0.Final/validation-api-1.1.0.Final.jar:/home/cass/.m2/repository/net/jpountz/lz4/lz4/1.3.0/lz4-1.3.0.jar:/home/cass/.m2/repository/com/github/rwl/jtransforms/2.4.0/jtransforms-2.4.0.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-common/2.22.2/jersey-common-2.22.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-client/2.2.0/hadoop-yarn-client-2.2.0.jar:/home/cass/.m2/repository/io/netty/netty/3.8.0.Final/netty-3.8.0.Final.jar:/home/cass/.m2/repository/org/apache/mesos/mesos/0.21.1/mesos-0.21.1-shaded-protobuf.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-annotations/2.5.3/jackson-annotations-2.5.3.jar:/home/cass/.m2/repository/com/google/code/findbugs/jsr305/1.3.9/jsr305-1.3.9.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-api/2.4.0-b34/hk2-api-2.4.0-b34.jar:/home/cass/.m2/repository/net/sf/opencsv/opencsv/2.3/opencsv-2.3.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-server/2.22.2/jersey-server-2.22.2.jar:/home/cass/.m2/repository/net/sf/py4j/py4j/0.10.1/py4j-0.10.1.jar:/home/cass/.m2/repository/com/twitter/chill-java/0.8.0/chill-java-0.8.0.jar:/home/cass/.m2/repository/commons-lang/commons-lang/2.6/commons-lang-2.6.jar:/home/cass/.m2/repository/org/tukaani/xz/1.0/xz-1.0.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-databind/2.5.3/jackson-databind-2.5.3.jar:/home/cass/.m2/repository/org/codehaus/janino/janino/2.7.8/janino-2.7.8.jar:/home/cass/.m2/repository/commons-codec/commons-codec/1.10/commons-codec-1.10.jar:/home/cass/.m2/repository/org/apache/curator/curator-recipes/2.4.0/curator-recipes-2.4.0.jar:/home/cass/.m2/repository/org/javassist/javassist/3.18.1-GA/javassist-3.18.1-GA.jar:/home/cass/.m2/repository/org/apache/ivy/ivy/2.4.0/ivy-2.4.0.jar:/home/cass/.m2/repository/javax/inject/javax.inject/1/javax.inject-1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-core/2.2.0/hadoop-mapreduce-client-core-2.2.0.jar:/home/cass/.m2/repository/com/fasterxml/jackson/module/jackson-module-scala_2.11/2.5.3/jackson-module-scala_2.11-2.5.3.jar:/home/cass/.m2/repository/commons-beanutils/commons-beanutils-core/1.8.0/commons-beanutils-core-1.8.0.jar:/home/cass/.m2/repository/javax/servlet/javax.servlet-api/3.1.0/javax.servlet-api-3.1.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/osgi-resource-locator/1.0.1/osgi-resource-locator-1.0.1.jar:/home/cass/.m2/repository/org/apache/commons/commons-math3/3.4.1/commons-math3-3.4.1.jar:/home/cass/spark2/spark/common/network-common/target/spark-network-common_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/avro/avro/1.7.7/avro-1.7.7.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-common/2.2.0/hadoop-mapreduce-client-common-2.2.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-utils/2.4.0-b34/hk2-utils-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/hk2/external/aopalliance-repackaged/2.4.0-b34/aopalliance-repackaged-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/hk2/external/javax.inject/2.4.0-b34/javax.inject-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/jersey/containers/jersey-container-servlet-core/2.22.2/jersey-container-servlet-core-2.22.2.jar:/home/cass/.m2/repository/oro/oro/2.0.8/oro-2.0.8.jar:/home/cass/.m2/repository/org/scala-lang/scala-compiler/2.11.8/scala-compiler-2.11.8.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-encoding/1.7.0/parquet-encoding-1.7.0.jar:/home/cass/.m2/repository/org/roaringbitmap/RoaringBitmap/0.5.11/RoaringBitmap-0.5.11.jar:/home/cass/.m2/repository/log4j/log4j/1.2.17/log4j-1.2.17.jar:/home/cass/.m2/repository/org/scala-lang/scala-library/2.11.8/scala-library-2.11.8.jar:/home/cass/.m2/repository/org/codehaus/janino/commons-compiler/2.7.8/commons-compiler-2.7.8.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-hadoop/1.7.0/parquet-hadoop-1.7.0.jar:/home/cass/.m2/repository/org/apache/curator/curator-client/2.4.0/curator-client-2.4.0.jar:/home/cass/.m2/repository/org/jpmml/pmml-model/1.2.7/pmml-model-1.2.7.jar:/home/cass/.m2/repository/org/apache/commons/commons-compress/1.4.1/commons-compress-1.4.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-app/2.2.0/hadoop-mapreduce-client-app-2.2.0.jar:/home/cass/.m2/repository/org/slf4j/slf4j-api/1.7.16/slf4j-api-1.7.16.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-xml_2.11/1.0.4/scala-xml_2.11-1.0.4.jar:/home/cass/.m2/repository/org/apache/xbean/xbean-asm5-shaded/4.4/xbean-asm5-shaded-4.4.jar:/home/cass/.m2/repository/org/json4s/json4s-core_2.11/3.2.11/json4s-core_2.11-3.2.11.jar:/home/cass/.m2/repository/com/github/fommil/netlib/core/1.1.2/core-1.1.2.jar:/home/cass/.m2/repository/org/mortbay/jetty/jetty-util/6.1.26/jetty-util-6.1.26.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-server-common/2.2.0/hadoop-yarn-server-common-2.2.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-hdfs/2.2.0/hadoop-hdfs-2.2.0.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-mapper-asl/1.9.13/jackson-mapper-asl-1.9.13.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-api/2.2.0/hadoop-yarn-api-2.2.0.jar:/home/cass/.m2/repository/com/esotericsoftware/kryo-shaded/3.0.3/kryo-shaded-3.0.3.jar:/home/cass/.m2/repository/javax/ws/rs/javax.ws.rs-api/2.0.1/javax.ws.rs-api-2.0.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-common/2.2.0/hadoop-yarn-common-2.2.0.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-client/2.22.2/jersey-client-2.22.2.jar:/home/cass/spark2/spark/common/unsafe/target/spark-unsafe_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/avro/avro-mapred/1.7.7/avro-mapred-1.7.7-hadoop2.jar:/home/cass/spark2/spark/sql/catalyst/target/spark-catalyst_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-column/1.7.0/parquet-column-1.7.0.jar:/home/cass/.m2/repository/xmlenc/xmlenc/0.52/xmlenc-0.52.jar:/home/cass/.m2/repository/com/ning/compress-lzf/1.0.3/compress-lzf-1.0.3.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-shuffle/2.2.0/hadoop-mapreduce-client-shuffle-2.2.0.jar:/home/cass/.m2/repository/org/apache/zookeeper/zookeeper/3.4.5/zookeeper-3.4.5.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-common/1.7.0/parquet-common-1.7.0.jar:/home/cass/.m2/repository/org/apache/curator/curator-framework/2.4.0/curator-framework-2.4.0.jar:/home/cass/.m2/repository/commons-net/commons-net/2.2/commons-net-2.2.jar:/home/cass/.m2/repository/org/apache/commons/commons-lang3/3.3.2/commons-lang3-3.3.2.jar:/home/cass/.m2/repository/org/json4s/json4s-ast_2.11/3.2.11/json4s-ast_2.11-3.2.11.jar:/home/cass/spark2/spark/launcher/target/spark-launcher_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/scala-lang/scalap/2.11.8/scalap-2.11.8.jar:/home/cass/.m2/repository/com/clearspring/analytics/stream/2.7.0/stream-2.7.0.jar:/home/cass/.m2/repository/org/apache/commons/commons-math/2.1/commons-math-2.1.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-generator/1.7.0/parquet-generator-1.7.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-annotations/2.2.0/hadoop-annotations-2.2.0.jar:/home/cass/.m2/repository/com/thoughtworks/paranamer/paranamer/2.6/paranamer-2.6.jar:/home/cass/.m2/repository/commons-configuration/commons-configuration/1.6/commons-configuration-1.6.jar:/home/cass/.m2/repository/org/glassfish/jersey/containers/jersey-container-servlet/2.22.2/jersey-container-servlet-2.22.2.jar:/home/cass/.m2/repository/commons-digester/commons-digester/1.8/commons-digester-1.8.jar:/home/cass/.m2/repository/org/slf4j/jul-to-slf4j/1.7.16/jul-to-slf4j-1.7.16.jar:/home/cass/.m2/repository/commons-beanutils/commons-beanutils/1.7.0/commons-beanutils-1.7.0.jar:/home/cass/.m2/repository/org/antlr/antlr4-runtime/4.5.2-1/antlr4-runtime-4.5.2-1.jar:/home/cass/spark2/spark/common/network-shuffle/target/spark-network-shuffle_2.11-2.0.0-SNAPSHOT.jar:/home/cass/spark2/spark/mllib-local/target/spark-mllib-local_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-parser-combinators_2.11/1.0.4/scala-parser-combinators_2.11-1.0.4.jar:/home/cass/.m2/repository/commons-cli/commons-cli/1.2/commons-cli-1.2.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-graphite/3.1.2/metrics-graphite-3.1.2.jar:/home/cass/.m2/repository/org/scalanlp/breeze_2.11/0.11.2/breeze_2.11-0.11.2.jar:/home/cass/.m2/repository/javax/annotation/javax.annotation-api/1.2/javax.annotation-api-1.2.jar:/home/cass/.m2/repository/org/objenesis/objenesis/2.1/objenesis-2.1.jar:/home/cass/.m2/repository/org/slf4j/slf4j-log4j12/1.7.16/slf4j-log4j12-1.7.16.jar:/home/cass/.m2/repository/org/scalanlp/breeze-macros_2.11/0.11.2/breeze-macros_2.11-0.11.2.jar:/home/cass/spark2/spark/common/sketch/target/spark-sketch_2.11-2.0.0-SNAPSHOT.jar:/home/cass/spark2/spark/core/target/spark-core_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/glassfish/jersey/media/jersey-media-jaxb/2.22.2/jersey-media-jaxb-2.22.2.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-core/2.5.3/jackson-core-2.5.3.jar:/home/cass/spark2/spark/streaming/target/spark-streaming_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/spark-project/spark/unused/1.0.0/unused-1.0.0.jar:/home/cass/.m2/repository/org/apache/avro/avro-ipc/1.7.7/avro-ipc-1.7.7.jar:/home/cass/.m2/repository/commons-collections/commons-collections/3.2.2/commons-collections-3.2.2.jar:/home/cass/.m2/repository/com/twitter/chill_2.11/0.8.0/chill_2.11-0.8.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-locator/2.4.0-b34/hk2-locator-2.4.0-b34.jar:/home/cass/.m2/repository/org/slf4j/jcl-over-slf4j/1.7.16/jcl-over-slf4j-1.7.16.jar:/home/cass/.m2/repository/commons-httpclient/commons-httpclient/3.1/commons-httpclient-3.1.jar:/home/cass/.m2/repository/io/netty/netty-all/4.0.29.Final/netty-all-4.0.29.Final.jar:/home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- build-helper-maven-plugin:1.10:add-source (add-scala-sources) @ spark-repl_2.11 ---
[INFO] Source directory: /home/cass/spark2/spark/repl/scala-2.11/src/main/scala added.
[INFO]
[INFO] --- maven-remote-resources-plugin:1.5:process (default) @ spark-repl_2.11 ---
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ spark-repl_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/repl/src/main/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:compile (scala-compile-first) @ spark-repl_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 4 Scala sources to /home/cass/spark2/spark/repl/target/scala-2.11/classes...
[info] Compile success at May 20, 2016 12:36:38 PM [1.090s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:compile (default-compile) @ spark-repl_2.11 ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- build-helper-maven-plugin:1.10:add-test-source (add-scala-test-sources) @ spark-repl_2.11 ---
[INFO] Test Source directory: /home/cass/spark2/spark/repl/scala-2.11/src/test/scala added.
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (create-tmp-dir) @ spark-repl_2.11 ---
[INFO] Executing tasks

main:
    [mkdir] Created dir: /home/cass/spark2/spark/repl/target/tmp
[INFO] Executed tasks
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ spark-repl_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 1 resource
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:testCompile (scala-test-compile-first) @ spark-repl_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 2 Scala sources to /home/cass/spark2/spark/repl/target/scala-2.11/test-classes...
[info] Compile success at May 20, 2016 12:36:39 PM [1.090s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:testCompile (default-testCompile) @ spark-repl_2.11 ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (generate-test-classpath) @ spark-repl_2.11 ---
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (default-test) @ spark-repl_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (test) @ spark-repl_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- scalatest-maven-plugin:1.0:test (test) @ spark-repl_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (prepare-test-jar) @ spark-repl_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/repl/target/spark-repl_2.11-2.0.0-SNAPSHOT-tests.jar
[INFO]
[INFO] --- maven-jar-plugin:2.6:jar (default-jar) @ spark-repl_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/repl/target/spark-repl_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-site-plugin:3.3:attach-descriptor (attach-descriptor) @ spark-repl_2.11 ---
[INFO]
[INFO] --- maven-shade-plugin:2.4.3:shade (default) @ spark-repl_2.11 ---
[INFO] Excluding org.apache.spark:spark-core_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.avro:avro-mapred:jar:hadoop2:1.7.7 from the shaded jar.
[INFO] Excluding org.apache.avro:avro-ipc:jar:1.7.7 from the shaded jar.
[INFO] Excluding org.apache.avro:avro:jar:1.7.7 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-core-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-mapper-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding com.twitter:chill_2.11:jar:0.8.0 from the shaded jar.
[INFO] Excluding com.esotericsoftware:kryo-shaded:jar:3.0.3 from the shaded jar.
[INFO] Excluding com.esotericsoftware:minlog:jar:1.3.0 from the shaded jar.
[INFO] Excluding com.twitter:chill-java:jar:0.8.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding commons-cli:commons-cli:jar:1.2 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-math:jar:2.1 from the shaded jar.
[INFO] Excluding xmlenc:xmlenc:jar:0.52 from the shaded jar.
[INFO] Excluding commons-io:commons-io:jar:2.4 from the shaded jar.
[INFO] Excluding commons-lang:commons-lang:jar:2.6 from the shaded jar.
[INFO] Excluding commons-configuration:commons-configuration:jar:1.6 from the shaded jar.
[INFO] Excluding commons-collections:commons-collections:jar:3.2.2 from the shaded jar.
[INFO] Excluding commons-digester:commons-digester:jar:1.8 from the shaded jar.
[INFO] Excluding commons-beanutils:commons-beanutils:jar:1.7.0 from the shaded jar.
[INFO] Excluding commons-beanutils:commons-beanutils-core:jar:1.8.0 from the shaded jar.
[INFO] Excluding com.google.protobuf:protobuf-java:jar:2.5.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-auth:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-compress:jar:1.4.1 from the shaded jar.
[INFO] Excluding org.tukaani:xz:jar:1.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-hdfs:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.mortbay.jetty:jetty-util:jar:6.1.26 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-app:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding com.google.inject:guice:jar:3.0 from the shaded jar.
[INFO] Excluding javax.inject:javax.inject:jar:1 from the shaded jar.
[INFO] Excluding aopalliance:aopalliance:jar:1.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-server-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-shuffle:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-api:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-core:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-jobclient:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-annotations:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-launcher_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-network-common_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-network-shuffle_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.fusesource.leveldbjni:leveldbjni-all:jar:1.8 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-annotations:jar:2.5.3 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-unsafe_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding net.java.dev.jets3t:jets3t:jar:0.7.1 from the shaded jar.
[INFO] Excluding commons-codec:commons-codec:jar:1.10 from the shaded jar.
[INFO] Excluding commons-httpclient:commons-httpclient:jar:3.1 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-recipes:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-framework:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-client:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.zookeeper:zookeeper:jar:3.4.5 from the shaded jar.
[INFO] Excluding javax.servlet:javax.servlet-api:jar:3.1.0 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-lang3:jar:3.3.2 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-math3:jar:3.4.1 from the shaded jar.
[INFO] Excluding com.google.code.findbugs:jsr305:jar:1.3.9 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-api:jar:1.7.16 from the shaded jar.
[INFO] Excluding org.slf4j:jcl-over-slf4j:jar:1.7.16 from the shaded jar.
[INFO] Excluding log4j:log4j:jar:1.2.17 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-log4j12:jar:1.7.16 from the shaded jar.
[INFO] Excluding com.ning:compress-lzf:jar:1.0.3 from the shaded jar.
[INFO] Excluding org.xerial.snappy:snappy-java:jar:1.1.2.4 from the shaded jar.
[INFO] Excluding net.jpountz.lz4:lz4:jar:1.3.0 from the shaded jar.
[INFO] Excluding org.roaringbitmap:RoaringBitmap:jar:0.5.11 from the shaded jar.
[INFO] Excluding commons-net:commons-net:jar:2.2 from the shaded jar.
[INFO] Excluding org.json4s:json4s-jackson_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.json4s:json4s-core_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.json4s:json4s-ast_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.scala-lang:scalap:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-client:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.ws.rs:javax.ws.rs-api:jar:2.0.1 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-api:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-utils:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2.external:aopalliance-repackaged:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2.external:javax.inject:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-locator:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.javassist:javassist:jar:3.18.1-GA from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-common:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.annotation:javax.annotation-api:jar:1.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.bundles.repackaged:jersey-guava:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:osgi-resource-locator:jar:1.0.1 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-server:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.media:jersey-media-jaxb:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.validation:validation-api:jar:1.1.0.Final from the shaded jar.
[INFO] Excluding org.glassfish.jersey.containers:jersey-container-servlet:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.containers:jersey-container-servlet-core:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.apache.mesos:mesos:jar:shaded-protobuf:0.21.1 from the shaded jar.
[INFO] Excluding io.netty:netty-all:jar:4.0.29.Final from the shaded jar.
[INFO] Excluding io.netty:netty:jar:3.8.0.Final from the shaded jar.
[INFO] Excluding com.clearspring.analytics:stream:jar:2.7.0 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-core:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-jvm:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-json:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-graphite:jar:3.1.2 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-databind:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-core:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.module:jackson-module-scala_2.11:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.thoughtworks.paranamer:paranamer:jar:2.6 from the shaded jar.
[INFO] Excluding org.apache.ivy:ivy:jar:2.4.0 from the shaded jar.
[INFO] Excluding oro:oro:jar:2.0.8 from the shaded jar.
[INFO] Excluding net.razorvine:pyrolite:jar:4.9 from the shaded jar.
[INFO] Excluding net.sf.py4j:py4j:jar:0.10.1 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-mllib_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-streaming_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-graphx_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding com.github.fommil.netlib:core:jar:1.1.2 from the shaded jar.
[INFO] Excluding net.sourceforge.f2j:arpack_combined_all:jar:0.1 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-mllib-local_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.scalanlp:breeze_2.11:jar:0.11.2 from the shaded jar.
[INFO] Excluding org.scalanlp:breeze-macros_2.11:jar:0.11.2 from the shaded jar.
[INFO] Excluding net.sf.opencsv:opencsv:jar:2.3 from the shaded jar.
[INFO] Excluding com.github.rwl:jtransforms:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.spire-math:spire_2.11:jar:0.7.4 from the shaded jar.
[INFO] Excluding org.spire-math:spire-macros_2.11:jar:0.7.4 from the shaded jar.
[INFO] Excluding org.jpmml:pmml-model:jar:1.2.7 from the shaded jar.
[INFO] Excluding org.jpmml:pmml-agent:jar:1.2.7 from the shaded jar.
[INFO] Excluding org.jpmml:pmml-schema:jar:1.2.7 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-sql_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding com.univocity:univocity-parsers:jar:2.1.0 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-sketch_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-catalyst_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.codehaus.janino:janino:jar:2.7.8 from the shaded jar.
[INFO] Excluding org.codehaus.janino:commons-compiler:jar:2.7.8 from the shaded jar.
[INFO] Excluding org.antlr:antlr4-runtime:jar:4.5.2-1 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-column:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-common:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-encoding:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-generator:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-hadoop:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-format:jar:2.3.0-incubating from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-jackson:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-compiler:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-xml_2.11:jar:1.0.4 from the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-parser-combinators_2.11:jar:1.0.4 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-reflect:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.slf4j:jul-to-slf4j:jar:1.7.16 from the shaded jar.
[INFO] Excluding org.objenesis:objenesis:jar:2.1 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-tags_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.xbean:xbean-asm5-shaded:jar:4.4 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-library:jar:2.11.8 from the shaded jar.
[INFO] Including org.spark-project.spark:unused:jar:1.0.0 in the shaded jar.
[INFO] Replacing original artifact with shaded artifact.
[INFO] Replacing /home/cass/spark2/spark/repl/target/spark-repl_2.11-2.0.0-SNAPSHOT.jar with /home/cass/spark2/spark/repl/target/spark-repl_2.11-2.0.0-SNAPSHOT-shaded.jar
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/repl/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/repl/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/repl/dependency-reduced-pom.xml
[INFO]
[INFO] --- maven-source-plugin:2.4:jar-no-fork (create-source-jar) @ spark-repl_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/repl/target/spark-repl_2.11-2.0.0-SNAPSHOT-sources.jar
[INFO]
[INFO] --- maven-source-plugin:2.4:test-jar-no-fork (create-source-jar) @ spark-repl_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/repl/target/spark-repl_2.11-2.0.0-SNAPSHOT-test-sources.jar
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Spark Project Assembly 2.0.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.0.0:clean (default-clean) @ spark-assembly_2.11 ---
[INFO]
[INFO] --- maven-enforcer-plugin:1.4.1:enforce (enforce-versions) @ spark-assembly_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:add-source (eclipse-add-source) @ spark-assembly_2.11 ---
[INFO] Add Source directory: /home/cass/spark2/spark/assembly/src/main/scala
[INFO] Add Test Source directory: /home/cass/spark2/spark/assembly/src/test/scala
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (default-cli) @ spark-assembly_2.11 ---
[INFO] Dependencies classpath:
/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-jobclient/2.2.0/hadoop-mapreduce-client-jobclient-2.2.0.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-jackson/1.7.0/parquet-jackson-1.7.0.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-core/3.1.2/metrics-core-3.1.2.jar:/home/cass/.m2/repository/com/google/protobuf/protobuf-java/2.5.0/protobuf-java-2.5.0.jar:/home/cass/.m2/repository/aopalliance/aopalliance/1.0/aopalliance-1.0.jar:/home/cass/.m2/repository/org/spire-math/spire-macros_2.11/0.7.4/spire-macros_2.11-0.7.4.jar:/home/cass/.m2/repository/net/razorvine/pyrolite/4.9/pyrolite-4.9.jar:/home/cass/.m2/repository/com/univocity/univocity-parsers/2.1.0/univocity-parsers-2.1.0.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-jvm/3.1.2/metrics-jvm-3.1.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-client/2.2.0/hadoop-client-2.2.0.jar:/home/cass/.m2/repository/org/fusesource/leveldbjni/leveldbjni-all/1.8/leveldbjni-all-1.8.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-format/2.3.0-incubating/parquet-format-2.3.0-incubating.jar:/home/cass/.m2/repository/org/glassfish/jersey/bundles/repackaged/jersey-guava/2.22.2/jersey-guava-2.22.2.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-json/3.1.2/metrics-json-3.1.2.jar:/home/cass/.m2/repository/org/spire-math/spire_2.11/0.7.4/spire_2.11-0.7.4.jar:/home/cass/.m2/repository/net/java/dev/jets3t/jets3t/0.7.1/jets3t-0.7.1.jar:/home/cass/spark2/spark/graphx/target/spark-graphx_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-common/2.2.0/hadoop-common-2.2.0.jar:/home/cass/spark2/spark/mllib/target/spark-mllib_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/jpmml/pmml-schema/1.2.7/pmml-schema-1.2.7.jar:/home/cass/.m2/repository/com/google/inject/guice/3.0/guice-3.0.jar:/home/cass/.m2/repository/commons-io/commons-io/2.4/commons-io-2.4.jar:/home/cass/spark2/spark/sql/core/target/spark-sql_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/net/sourceforge/f2j/arpack_combined_all/0.1/arpack_combined_all-0.1.jar:/home/cass/.m2/repository/org/scala-lang/scala-reflect/2.11.8/scala-reflect-2.11.8.jar:/home/cass/.m2/repository/org/xerial/snappy/snappy-java/1.1.2.4/snappy-java-1.1.2.4.jar:/home/cass/.m2/repository/org/json4s/json4s-jackson_2.11/3.2.11/json4s-jackson_2.11-3.2.11.jar:/home/cass/.m2/repository/org/jpmml/pmml-agent/1.2.7/pmml-agent-1.2.7.jar:/home/cass/.m2/repository/com/esotericsoftware/minlog/1.3.0/minlog-1.3.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-auth/2.2.0/hadoop-auth-2.2.0.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-core-asl/1.9.13/jackson-core-asl-1.9.13.jar:/home/cass/.m2/repository/javax/validation/validation-api/1.1.0.Final/validation-api-1.1.0.Final.jar:/home/cass/.m2/repository/net/jpountz/lz4/lz4/1.3.0/lz4-1.3.0.jar:/home/cass/.m2/repository/com/github/rwl/jtransforms/2.4.0/jtransforms-2.4.0.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-common/2.22.2/jersey-common-2.22.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-client/2.2.0/hadoop-yarn-client-2.2.0.jar:/home/cass/.m2/repository/io/netty/netty/3.8.0.Final/netty-3.8.0.Final.jar:/home/cass/.m2/repository/org/apache/mesos/mesos/0.21.1/mesos-0.21.1-shaded-protobuf.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-annotations/2.5.3/jackson-annotations-2.5.3.jar:/home/cass/.m2/repository/com/google/code/findbugs/jsr305/1.3.9/jsr305-1.3.9.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-api/2.4.0-b34/hk2-api-2.4.0-b34.jar:/home/cass/.m2/repository/net/sf/opencsv/opencsv/2.3/opencsv-2.3.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-server/2.22.2/jersey-server-2.22.2.jar:/home/cass/.m2/repository/net/sf/py4j/py4j/0.10.1/py4j-0.10.1.jar:/home/cass/.m2/repository/com/twitter/chill-java/0.8.0/chill-java-0.8.0.jar:/home/cass/.m2/repository/commons-lang/commons-lang/2.6/commons-lang-2.6.jar:/home/cass/.m2/repository/org/tukaani/xz/1.0/xz-1.0.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-databind/2.5.3/jackson-databind-2.5.3.jar:/home/cass/.m2/repository/org/codehaus/janino/janino/2.7.8/janino-2.7.8.jar:/home/cass/.m2/repository/commons-codec/commons-codec/1.10/commons-codec-1.10.jar:/home/cass/.m2/repository/org/apache/curator/curator-recipes/2.4.0/curator-recipes-2.4.0.jar:/home/cass/spark2/spark/repl/target/spark-repl_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/javassist/javassist/3.18.1-GA/javassist-3.18.1-GA.jar:/home/cass/.m2/repository/com/google/guava/guava/14.0.1/guava-14.0.1.jar:/home/cass/.m2/repository/org/apache/ivy/ivy/2.4.0/ivy-2.4.0.jar:/home/cass/.m2/repository/javax/inject/javax.inject/1/javax.inject-1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-core/2.2.0/hadoop-mapreduce-client-core-2.2.0.jar:/home/cass/.m2/repository/com/fasterxml/jackson/module/jackson-module-scala_2.11/2.5.3/jackson-module-scala_2.11-2.5.3.jar:/home/cass/.m2/repository/commons-beanutils/commons-beanutils-core/1.8.0/commons-beanutils-core-1.8.0.jar:/home/cass/.m2/repository/javax/servlet/javax.servlet-api/3.1.0/javax.servlet-api-3.1.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/osgi-resource-locator/1.0.1/osgi-resource-locator-1.0.1.jar:/home/cass/.m2/repository/org/apache/commons/commons-math3/3.4.1/commons-math3-3.4.1.jar:/home/cass/spark2/spark/common/network-common/target/spark-network-common_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/avro/avro/1.7.7/avro-1.7.7.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-common/2.2.0/hadoop-mapreduce-client-common-2.2.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-utils/2.4.0-b34/hk2-utils-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/hk2/external/aopalliance-repackaged/2.4.0-b34/aopalliance-repackaged-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/hk2/external/javax.inject/2.4.0-b34/javax.inject-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/jersey/containers/jersey-container-servlet-core/2.22.2/jersey-container-servlet-core-2.22.2.jar:/home/cass/.m2/repository/oro/oro/2.0.8/oro-2.0.8.jar:/home/cass/.m2/repository/org/scala-lang/scala-compiler/2.11.8/scala-compiler-2.11.8.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-encoding/1.7.0/parquet-encoding-1.7.0.jar:/home/cass/.m2/repository/org/roaringbitmap/RoaringBitmap/0.5.11/RoaringBitmap-0.5.11.jar:/home/cass/.m2/repository/log4j/log4j/1.2.17/log4j-1.2.17.jar:/home/cass/.m2/repository/org/scala-lang/scala-library/2.11.8/scala-library-2.11.8.jar:/home/cass/.m2/repository/org/codehaus/janino/commons-compiler/2.7.8/commons-compiler-2.7.8.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-hadoop/1.7.0/parquet-hadoop-1.7.0.jar:/home/cass/.m2/repository/org/apache/curator/curator-client/2.4.0/curator-client-2.4.0.jar:/home/cass/.m2/repository/org/jpmml/pmml-model/1.2.7/pmml-model-1.2.7.jar:/home/cass/.m2/repository/org/apache/commons/commons-compress/1.4.1/commons-compress-1.4.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-app/2.2.0/hadoop-mapreduce-client-app-2.2.0.jar:/home/cass/.m2/repository/org/slf4j/slf4j-api/1.7.16/slf4j-api-1.7.16.jar:/home/cass/.m2/repository/org/apache/xbean/xbean-asm5-shaded/4.4/xbean-asm5-shaded-4.4.jar:/home/cass/.m2/repository/org/json4s/json4s-core_2.11/3.2.11/json4s-core_2.11-3.2.11.jar:/home/cass/.m2/repository/com/github/fommil/netlib/core/1.1.2/core-1.1.2.jar:/home/cass/.m2/repository/org/mortbay/jetty/jetty-util/6.1.26/jetty-util-6.1.26.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-server-common/2.2.0/hadoop-yarn-server-common-2.2.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-hdfs/2.2.0/hadoop-hdfs-2.2.0.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-mapper-asl/1.9.13/jackson-mapper-asl-1.9.13.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-api/2.2.0/hadoop-yarn-api-2.2.0.jar:/home/cass/.m2/repository/com/esotericsoftware/kryo-shaded/3.0.3/kryo-shaded-3.0.3.jar:/home/cass/.m2/repository/javax/ws/rs/javax.ws.rs-api/2.0.1/javax.ws.rs-api-2.0.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-common/2.2.0/hadoop-yarn-common-2.2.0.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-client/2.22.2/jersey-client-2.22.2.jar:/home/cass/spark2/spark/common/unsafe/target/spark-unsafe_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/avro/avro-mapred/1.7.7/avro-mapred-1.7.7-hadoop2.jar:/home/cass/spark2/spark/sql/catalyst/target/spark-catalyst_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-column/1.7.0/parquet-column-1.7.0.jar:/home/cass/.m2/repository/xmlenc/xmlenc/0.52/xmlenc-0.52.jar:/home/cass/.m2/repository/com/ning/compress-lzf/1.0.3/compress-lzf-1.0.3.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-shuffle/2.2.0/hadoop-mapreduce-client-shuffle-2.2.0.jar:/home/cass/.m2/repository/org/apache/zookeeper/zookeeper/3.4.5/zookeeper-3.4.5.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-common/1.7.0/parquet-common-1.7.0.jar:/home/cass/.m2/repository/org/apache/curator/curator-framework/2.4.0/curator-framework-2.4.0.jar:/home/cass/.m2/repository/commons-net/commons-net/2.2/commons-net-2.2.jar:/home/cass/.m2/repository/org/apache/commons/commons-lang3/3.3.2/commons-lang3-3.3.2.jar:/home/cass/.m2/repository/org/json4s/json4s-ast_2.11/3.2.11/json4s-ast_2.11-3.2.11.jar:/home/cass/spark2/spark/launcher/target/spark-launcher_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/scala-lang/scalap/2.11.8/scalap-2.11.8.jar:/home/cass/.m2/repository/com/clearspring/analytics/stream/2.7.0/stream-2.7.0.jar:/home/cass/.m2/repository/org/apache/commons/commons-math/2.1/commons-math-2.1.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-generator/1.7.0/parquet-generator-1.7.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-annotations/2.2.0/hadoop-annotations-2.2.0.jar:/home/cass/.m2/repository/com/thoughtworks/paranamer/paranamer/2.6/paranamer-2.6.jar:/home/cass/.m2/repository/commons-configuration/commons-configuration/1.6/commons-configuration-1.6.jar:/home/cass/.m2/repository/org/glassfish/jersey/containers/jersey-container-servlet/2.22.2/jersey-container-servlet-2.22.2.jar:/home/cass/.m2/repository/commons-digester/commons-digester/1.8/commons-digester-1.8.jar:/home/cass/.m2/repository/org/slf4j/jul-to-slf4j/1.7.16/jul-to-slf4j-1.7.16.jar:/home/cass/.m2/repository/commons-beanutils/commons-beanutils/1.7.0/commons-beanutils-1.7.0.jar:/home/cass/.m2/repository/org/antlr/antlr4-runtime/4.5.2-1/antlr4-runtime-4.5.2-1.jar:/home/cass/spark2/spark/common/network-shuffle/target/spark-network-shuffle_2.11-2.0.0-SNAPSHOT.jar:/home/cass/spark2/spark/mllib-local/target/spark-mllib-local_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-xml_2.11/1.0.2/scala-xml_2.11-1.0.2.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-parser-combinators_2.11/1.0.4/scala-parser-combinators_2.11-1.0.4.jar:/home/cass/.m2/repository/commons-cli/commons-cli/1.2/commons-cli-1.2.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-graphite/3.1.2/metrics-graphite-3.1.2.jar:/home/cass/.m2/repository/org/scalanlp/breeze_2.11/0.11.2/breeze_2.11-0.11.2.jar:/home/cass/.m2/repository/org/objenesis/objenesis/2.1/objenesis-2.1.jar:/home/cass/.m2/repository/javax/annotation/javax.annotation-api/1.2/javax.annotation-api-1.2.jar:/home/cass/.m2/repository/org/slf4j/slf4j-log4j12/1.7.16/slf4j-log4j12-1.7.16.jar:/home/cass/.m2/repository/org/scalanlp/breeze-macros_2.11/0.11.2/breeze-macros_2.11-0.11.2.jar:/home/cass/spark2/spark/common/sketch/target/spark-sketch_2.11-2.0.0-SNAPSHOT.jar:/home/cass/spark2/spark/core/target/spark-core_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/glassfish/jersey/media/jersey-media-jaxb/2.22.2/jersey-media-jaxb-2.22.2.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-core/2.5.3/jackson-core-2.5.3.jar:/home/cass/spark2/spark/streaming/target/spark-streaming_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/avro/avro-ipc/1.7.7/avro-ipc-1.7.7.jar:/home/cass/.m2/repository/commons-collections/commons-collections/3.2.2/commons-collections-3.2.2.jar:/home/cass/.m2/repository/com/twitter/chill_2.11/0.8.0/chill_2.11-0.8.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-locator/2.4.0-b34/hk2-locator-2.4.0-b34.jar:/home/cass/.m2/repository/org/slf4j/jcl-over-slf4j/1.7.16/jcl-over-slf4j-1.7.16.jar:/home/cass/.m2/repository/commons-httpclient/commons-httpclient/3.1/commons-httpclient-3.1.jar:/home/cass/.m2/repository/io/netty/netty-all/4.0.29.Final/netty-all-4.0.29.Final.jar:/home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-remote-resources-plugin:1.5:process (default) @ spark-assembly_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:compile (scala-compile-first) @ spark-assembly_2.11 ---
[INFO] No sources to compile
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (create-tmp-dir) @ spark-assembly_2.11 ---
[INFO] Executing tasks

main:
    [mkdir] Created dir: /home/cass/spark2/spark/assembly/target/tmp
      [zip] Building zip: /home/cass/spark2/spark/python/lib/pyspark.zip
[INFO] Executed tasks
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:testCompile (scala-test-compile-first) @ spark-assembly_2.11 ---
[INFO] No sources to compile
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (generate-test-classpath) @ spark-assembly_2.11 ---
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (test) @ spark-assembly_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- scalatest-maven-plugin:1.0:test (test) @ spark-assembly_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-site-plugin:3.3:attach-descriptor (attach-descriptor) @ spark-assembly_2.11 ---
[INFO]
[INFO] --- maven-dependency-plugin:2.10:copy-dependencies (copy-module-dependencies) @ spark-assembly_2.11 ---
[INFO] Copying hadoop-mapreduce-client-jobclient-2.2.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/hadoop-mapreduce-client-jobclient-2.2.0.jar
[INFO] Copying parquet-jackson-1.7.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/parquet-jackson-1.7.0.jar
[INFO] Copying metrics-core-3.1.2.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/metrics-core-3.1.2.jar
[INFO] Copying protobuf-java-2.5.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/protobuf-java-2.5.0.jar
[INFO] Copying aopalliance-1.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/aopalliance-1.0.jar
[INFO] Copying spire-macros_2.11-0.7.4.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/spire-macros_2.11-0.7.4.jar
[INFO] Copying pyrolite-4.9.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/pyrolite-4.9.jar
[INFO] Copying univocity-parsers-2.1.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/univocity-parsers-2.1.0.jar
[INFO] Copying metrics-jvm-3.1.2.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/metrics-jvm-3.1.2.jar
[INFO] Copying hadoop-client-2.2.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/hadoop-client-2.2.0.jar
[INFO] Copying leveldbjni-all-1.8.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/leveldbjni-all-1.8.jar
[INFO] Copying parquet-format-2.3.0-incubating.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/parquet-format-2.3.0-incubating.jar
[INFO] Copying jersey-guava-2.22.2.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/jersey-guava-2.22.2.jar
[INFO] Copying metrics-json-3.1.2.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/metrics-json-3.1.2.jar
[INFO] Copying spire_2.11-0.7.4.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/spire_2.11-0.7.4.jar
[INFO] Copying jets3t-0.7.1.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/jets3t-0.7.1.jar
[INFO] Copying spark-graphx_2.11-2.0.0-SNAPSHOT.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/spark-graphx_2.11-2.0.0-SNAPSHOT.jar
[INFO] Copying hadoop-common-2.2.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/hadoop-common-2.2.0.jar
[INFO] Copying spark-mllib_2.11-2.0.0-SNAPSHOT.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/spark-mllib_2.11-2.0.0-SNAPSHOT.jar
[INFO] Copying pmml-schema-1.2.7.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/pmml-schema-1.2.7.jar
[INFO] Copying guice-3.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/guice-3.0.jar
[INFO] Copying commons-io-2.4.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/commons-io-2.4.jar
[INFO] Copying spark-sql_2.11-2.0.0-SNAPSHOT.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/spark-sql_2.11-2.0.0-SNAPSHOT.jar
[INFO] Copying arpack_combined_all-0.1.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/arpack_combined_all-0.1.jar
[INFO] Copying scala-reflect-2.11.8.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/scala-reflect-2.11.8.jar
[INFO] Copying snappy-java-1.1.2.4.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/snappy-java-1.1.2.4.jar
[INFO] Copying json4s-jackson_2.11-3.2.11.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/json4s-jackson_2.11-3.2.11.jar
[INFO] Copying pmml-agent-1.2.7.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/pmml-agent-1.2.7.jar
[INFO] Copying minlog-1.3.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/minlog-1.3.0.jar
[INFO] Copying hadoop-auth-2.2.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/hadoop-auth-2.2.0.jar
[INFO] Copying jackson-core-asl-1.9.13.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/jackson-core-asl-1.9.13.jar
[INFO] Copying validation-api-1.1.0.Final.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/validation-api-1.1.0.Final.jar
[INFO] Copying lz4-1.3.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/lz4-1.3.0.jar
[INFO] Copying jtransforms-2.4.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/jtransforms-2.4.0.jar
[INFO] Copying jersey-common-2.22.2.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/jersey-common-2.22.2.jar
[INFO] Copying hadoop-yarn-client-2.2.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/hadoop-yarn-client-2.2.0.jar
[INFO] Copying netty-3.8.0.Final.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/netty-3.8.0.Final.jar
[INFO] Copying mesos-0.21.1-shaded-protobuf.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/mesos-0.21.1-shaded-protobuf.jar
[INFO] Copying jackson-annotations-2.5.3.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/jackson-annotations-2.5.3.jar
[INFO] Copying jsr305-1.3.9.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/jsr305-1.3.9.jar
[INFO] Copying hk2-api-2.4.0-b34.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/hk2-api-2.4.0-b34.jar
[INFO] Copying opencsv-2.3.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/opencsv-2.3.jar
[INFO] Copying jersey-server-2.22.2.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/jersey-server-2.22.2.jar
[INFO] Copying py4j-0.10.1.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/py4j-0.10.1.jar
[INFO] Copying chill-java-0.8.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/chill-java-0.8.0.jar
[INFO] Copying commons-lang-2.6.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/commons-lang-2.6.jar
[INFO] Copying xz-1.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/xz-1.0.jar
[INFO] Copying jackson-databind-2.5.3.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/jackson-databind-2.5.3.jar
[INFO] Copying janino-2.7.8.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/janino-2.7.8.jar
[INFO] Copying commons-codec-1.10.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/commons-codec-1.10.jar
[INFO] Copying curator-recipes-2.4.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/curator-recipes-2.4.0.jar
[INFO] Copying spark-repl_2.11-2.0.0-SNAPSHOT.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/spark-repl_2.11-2.0.0-SNAPSHOT.jar
[INFO] Copying javassist-3.18.1-GA.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/javassist-3.18.1-GA.jar
[INFO] Copying guava-14.0.1.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/guava-14.0.1.jar
[INFO] Copying ivy-2.4.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/ivy-2.4.0.jar
[INFO] Copying javax.inject-1.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/javax.inject-1.jar
[INFO] Copying hadoop-mapreduce-client-core-2.2.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/hadoop-mapreduce-client-core-2.2.0.jar
[INFO] Copying jackson-module-scala_2.11-2.5.3.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/jackson-module-scala_2.11-2.5.3.jar
[INFO] Copying commons-beanutils-core-1.8.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/commons-beanutils-core-1.8.0.jar
[INFO] Copying javax.servlet-api-3.1.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/javax.servlet-api-3.1.0.jar
[INFO] Copying osgi-resource-locator-1.0.1.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/osgi-resource-locator-1.0.1.jar
[INFO] Copying commons-math3-3.4.1.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/commons-math3-3.4.1.jar
[INFO] Copying spark-network-common_2.11-2.0.0-SNAPSHOT.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/spark-network-common_2.11-2.0.0-SNAPSHOT.jar
[INFO] Copying avro-1.7.7.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/avro-1.7.7.jar
[INFO] Copying hadoop-mapreduce-client-common-2.2.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/hadoop-mapreduce-client-common-2.2.0.jar
[INFO] Copying hk2-utils-2.4.0-b34.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/hk2-utils-2.4.0-b34.jar
[INFO] Copying aopalliance-repackaged-2.4.0-b34.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/aopalliance-repackaged-2.4.0-b34.jar
[INFO] Copying javax.inject-2.4.0-b34.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/javax.inject-2.4.0-b34.jar
[INFO] Copying jersey-container-servlet-core-2.22.2.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/jersey-container-servlet-core-2.22.2.jar
[INFO] Copying oro-2.0.8.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/oro-2.0.8.jar
[INFO] Copying scala-compiler-2.11.8.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/scala-compiler-2.11.8.jar
[INFO] Copying parquet-encoding-1.7.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/parquet-encoding-1.7.0.jar
[INFO] Copying RoaringBitmap-0.5.11.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/RoaringBitmap-0.5.11.jar
[INFO] Copying log4j-1.2.17.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/log4j-1.2.17.jar
[INFO] Copying scala-library-2.11.8.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/scala-library-2.11.8.jar
[INFO] Copying commons-compiler-2.7.8.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/commons-compiler-2.7.8.jar
[INFO] Copying parquet-hadoop-1.7.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/parquet-hadoop-1.7.0.jar
[INFO] Copying curator-client-2.4.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/curator-client-2.4.0.jar
[INFO] Copying pmml-model-1.2.7.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/pmml-model-1.2.7.jar
[INFO] Copying commons-compress-1.4.1.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/commons-compress-1.4.1.jar
[INFO] Copying hadoop-mapreduce-client-app-2.2.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/hadoop-mapreduce-client-app-2.2.0.jar
[INFO] Copying slf4j-api-1.7.16.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/slf4j-api-1.7.16.jar
[INFO] Copying xbean-asm5-shaded-4.4.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/xbean-asm5-shaded-4.4.jar
[INFO] Copying json4s-core_2.11-3.2.11.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/json4s-core_2.11-3.2.11.jar
[INFO] Copying core-1.1.2.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/core-1.1.2.jar
[INFO] Copying jetty-util-6.1.26.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/jetty-util-6.1.26.jar
[INFO] Copying hadoop-yarn-server-common-2.2.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/hadoop-yarn-server-common-2.2.0.jar
[INFO] Copying hadoop-hdfs-2.2.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/hadoop-hdfs-2.2.0.jar
[INFO] Copying jackson-mapper-asl-1.9.13.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/jackson-mapper-asl-1.9.13.jar
[INFO] Copying hadoop-yarn-api-2.2.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/hadoop-yarn-api-2.2.0.jar
[INFO] Copying kryo-shaded-3.0.3.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/kryo-shaded-3.0.3.jar
[INFO] Copying javax.ws.rs-api-2.0.1.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/javax.ws.rs-api-2.0.1.jar
[INFO] Copying hadoop-yarn-common-2.2.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/hadoop-yarn-common-2.2.0.jar
[INFO] Copying jersey-client-2.22.2.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/jersey-client-2.22.2.jar
[INFO] Copying spark-unsafe_2.11-2.0.0-SNAPSHOT.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/spark-unsafe_2.11-2.0.0-SNAPSHOT.jar
[INFO] Copying avro-mapred-1.7.7-hadoop2.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/avro-mapred-1.7.7-hadoop2.jar
[INFO] Copying spark-catalyst_2.11-2.0.0-SNAPSHOT.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/spark-catalyst_2.11-2.0.0-SNAPSHOT.jar
[INFO] Copying parquet-column-1.7.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/parquet-column-1.7.0.jar
[INFO] Copying xmlenc-0.52.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/xmlenc-0.52.jar
[INFO] Copying compress-lzf-1.0.3.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/compress-lzf-1.0.3.jar
[INFO] Copying hadoop-mapreduce-client-shuffle-2.2.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/hadoop-mapreduce-client-shuffle-2.2.0.jar
[INFO] Copying zookeeper-3.4.5.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/zookeeper-3.4.5.jar
[INFO] Copying parquet-common-1.7.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/parquet-common-1.7.0.jar
[INFO] Copying curator-framework-2.4.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/curator-framework-2.4.0.jar
[INFO] Copying commons-net-2.2.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/commons-net-2.2.jar
[INFO] Copying commons-lang3-3.3.2.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/commons-lang3-3.3.2.jar
[INFO] Copying json4s-ast_2.11-3.2.11.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/json4s-ast_2.11-3.2.11.jar
[INFO] Copying spark-launcher_2.11-2.0.0-SNAPSHOT.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/spark-launcher_2.11-2.0.0-SNAPSHOT.jar
[INFO] Copying scalap-2.11.8.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/scalap-2.11.8.jar
[INFO] Copying stream-2.7.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/stream-2.7.0.jar
[INFO] Copying commons-math-2.1.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/commons-math-2.1.jar
[INFO] Copying parquet-generator-1.7.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/parquet-generator-1.7.0.jar
[INFO] Copying hadoop-annotations-2.2.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/hadoop-annotations-2.2.0.jar
[INFO] Copying paranamer-2.6.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/paranamer-2.6.jar
[INFO] Copying commons-configuration-1.6.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/commons-configuration-1.6.jar
[INFO] Copying jersey-container-servlet-2.22.2.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/jersey-container-servlet-2.22.2.jar
[INFO] Copying commons-digester-1.8.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/commons-digester-1.8.jar
[INFO] Copying jul-to-slf4j-1.7.16.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/jul-to-slf4j-1.7.16.jar
[INFO] Copying commons-beanutils-1.7.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/commons-beanutils-1.7.0.jar
[INFO] Copying antlr4-runtime-4.5.2-1.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/antlr4-runtime-4.5.2-1.jar
[INFO] Copying spark-network-shuffle_2.11-2.0.0-SNAPSHOT.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/spark-network-shuffle_2.11-2.0.0-SNAPSHOT.jar
[INFO] Copying spark-mllib-local_2.11-2.0.0-SNAPSHOT.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/spark-mllib-local_2.11-2.0.0-SNAPSHOT.jar
[INFO] Copying scala-xml_2.11-1.0.2.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/scala-xml_2.11-1.0.2.jar
[INFO] Copying scala-parser-combinators_2.11-1.0.4.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/scala-parser-combinators_2.11-1.0.4.jar
[INFO] Copying commons-cli-1.2.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/commons-cli-1.2.jar
[INFO] Copying metrics-graphite-3.1.2.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/metrics-graphite-3.1.2.jar
[INFO] Copying breeze_2.11-0.11.2.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/breeze_2.11-0.11.2.jar
[INFO] Copying objenesis-2.1.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/objenesis-2.1.jar
[INFO] Copying javax.annotation-api-1.2.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/javax.annotation-api-1.2.jar
[INFO] Copying slf4j-log4j12-1.7.16.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/slf4j-log4j12-1.7.16.jar
[INFO] Copying breeze-macros_2.11-0.11.2.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/breeze-macros_2.11-0.11.2.jar
[INFO] Copying spark-sketch_2.11-2.0.0-SNAPSHOT.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/spark-sketch_2.11-2.0.0-SNAPSHOT.jar
[INFO] Copying spark-core_2.11-2.0.0-SNAPSHOT.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/spark-core_2.11-2.0.0-SNAPSHOT.jar
[INFO] Copying jersey-media-jaxb-2.22.2.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/jersey-media-jaxb-2.22.2.jar
[INFO] Copying jackson-core-2.5.3.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/jackson-core-2.5.3.jar
[INFO] Copying spark-streaming_2.11-2.0.0-SNAPSHOT.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/spark-streaming_2.11-2.0.0-SNAPSHOT.jar
[INFO] Copying avro-ipc-1.7.7.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/avro-ipc-1.7.7.jar
[INFO] Copying commons-collections-3.2.2.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/commons-collections-3.2.2.jar
[INFO] Copying chill_2.11-0.8.0.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/chill_2.11-0.8.0.jar
[INFO] Copying hk2-locator-2.4.0-b34.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/hk2-locator-2.4.0-b34.jar
[INFO] Copying jcl-over-slf4j-1.7.16.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/jcl-over-slf4j-1.7.16.jar
[INFO] Copying commons-httpclient-3.1.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/commons-httpclient-3.1.jar
[INFO] Copying netty-all-4.0.29.Final.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/netty-all-4.0.29.Final.jar
[INFO] Copying spark-tags_2.11-2.0.0-SNAPSHOT.jar to /home/cass/spark2/spark/assembly/target/scala-2.11/jars/spark-tags_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-shade-plugin:2.4.3:shade (default) @ spark-assembly_2.11 ---
[INFO] Excluding org.apache.spark:spark-core_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.avro:avro-mapred:jar:hadoop2:1.7.7 from the shaded jar.
[INFO] Excluding org.apache.avro:avro-ipc:jar:1.7.7 from the shaded jar.
[INFO] Excluding org.apache.avro:avro:jar:1.7.7 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-core-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-mapper-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding com.twitter:chill_2.11:jar:0.8.0 from the shaded jar.
[INFO] Excluding com.esotericsoftware:kryo-shaded:jar:3.0.3 from the shaded jar.
[INFO] Excluding com.esotericsoftware:minlog:jar:1.3.0 from the shaded jar.
[INFO] Excluding org.objenesis:objenesis:jar:2.1 from the shaded jar.
[INFO] Excluding com.twitter:chill-java:jar:0.8.0 from the shaded jar.
[INFO] Excluding org.apache.xbean:xbean-asm5-shaded:jar:4.4 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding commons-cli:commons-cli:jar:1.2 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-math:jar:2.1 from the shaded jar.
[INFO] Excluding xmlenc:xmlenc:jar:0.52 from the shaded jar.
[INFO] Excluding commons-io:commons-io:jar:2.4 from the shaded jar.
[INFO] Excluding commons-lang:commons-lang:jar:2.6 from the shaded jar.
[INFO] Excluding commons-configuration:commons-configuration:jar:1.6 from the shaded jar.
[INFO] Excluding commons-collections:commons-collections:jar:3.2.2 from the shaded jar.
[INFO] Excluding commons-digester:commons-digester:jar:1.8 from the shaded jar.
[INFO] Excluding commons-beanutils:commons-beanutils:jar:1.7.0 from the shaded jar.
[INFO] Excluding commons-beanutils:commons-beanutils-core:jar:1.8.0 from the shaded jar.
[INFO] Excluding com.google.protobuf:protobuf-java:jar:2.5.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-auth:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-compress:jar:1.4.1 from the shaded jar.
[INFO] Excluding org.tukaani:xz:jar:1.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-hdfs:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.mortbay.jetty:jetty-util:jar:6.1.26 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-app:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding com.google.inject:guice:jar:3.0 from the shaded jar.
[INFO] Excluding javax.inject:javax.inject:jar:1 from the shaded jar.
[INFO] Excluding aopalliance:aopalliance:jar:1.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-server-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-shuffle:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-api:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-core:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-jobclient:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-annotations:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-launcher_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-network-common_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-network-shuffle_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.fusesource.leveldbjni:leveldbjni-all:jar:1.8 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-annotations:jar:2.5.3 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-unsafe_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding net.java.dev.jets3t:jets3t:jar:0.7.1 from the shaded jar.
[INFO] Excluding commons-codec:commons-codec:jar:1.10 from the shaded jar.
[INFO] Excluding commons-httpclient:commons-httpclient:jar:3.1 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-recipes:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-framework:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-client:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.zookeeper:zookeeper:jar:3.4.5 from the shaded jar.
[INFO] Excluding javax.servlet:javax.servlet-api:jar:3.1.0 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-lang3:jar:3.3.2 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-math3:jar:3.4.1 from the shaded jar.
[INFO] Excluding com.google.code.findbugs:jsr305:jar:1.3.9 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-api:jar:1.7.16 from the shaded jar.
[INFO] Excluding org.slf4j:jul-to-slf4j:jar:1.7.16 from the shaded jar.
[INFO] Excluding org.slf4j:jcl-over-slf4j:jar:1.7.16 from the shaded jar.
[INFO] Excluding log4j:log4j:jar:1.2.17 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-log4j12:jar:1.7.16 from the shaded jar.
[INFO] Excluding com.ning:compress-lzf:jar:1.0.3 from the shaded jar.
[INFO] Excluding org.xerial.snappy:snappy-java:jar:1.1.2.4 from the shaded jar.
[INFO] Excluding net.jpountz.lz4:lz4:jar:1.3.0 from the shaded jar.
[INFO] Excluding org.roaringbitmap:RoaringBitmap:jar:0.5.11 from the shaded jar.
[INFO] Excluding commons-net:commons-net:jar:2.2 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-library:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.json4s:json4s-jackson_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.json4s:json4s-core_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.json4s:json4s-ast_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.scala-lang:scalap:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-client:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.ws.rs:javax.ws.rs-api:jar:2.0.1 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-api:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-utils:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2.external:aopalliance-repackaged:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2.external:javax.inject:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-locator:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.javassist:javassist:jar:3.18.1-GA from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-common:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.annotation:javax.annotation-api:jar:1.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.bundles.repackaged:jersey-guava:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:osgi-resource-locator:jar:1.0.1 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-server:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.media:jersey-media-jaxb:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.validation:validation-api:jar:1.1.0.Final from the shaded jar.
[INFO] Excluding org.glassfish.jersey.containers:jersey-container-servlet:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.containers:jersey-container-servlet-core:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.apache.mesos:mesos:jar:shaded-protobuf:0.21.1 from the shaded jar.
[INFO] Excluding io.netty:netty-all:jar:4.0.29.Final from the shaded jar.
[INFO] Excluding io.netty:netty:jar:3.8.0.Final from the shaded jar.
[INFO] Excluding com.clearspring.analytics:stream:jar:2.7.0 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-core:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-jvm:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-json:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-graphite:jar:3.1.2 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-databind:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-core:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.module:jackson-module-scala_2.11:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.thoughtworks.paranamer:paranamer:jar:2.6 from the shaded jar.
[INFO] Excluding org.apache.ivy:ivy:jar:2.4.0 from the shaded jar.
[INFO] Excluding oro:oro:jar:2.0.8 from the shaded jar.
[INFO] Excluding net.razorvine:pyrolite:jar:4.9 from the shaded jar.
[INFO] Excluding net.sf.py4j:py4j:jar:0.10.1 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-tags_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-mllib_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-mllib-local_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.scalanlp:breeze_2.11:jar:0.11.2 from the shaded jar.
[INFO] Excluding org.scalanlp:breeze-macros_2.11:jar:0.11.2 from the shaded jar.
[INFO] Excluding net.sf.opencsv:opencsv:jar:2.3 from the shaded jar.
[INFO] Excluding com.github.rwl:jtransforms:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.spire-math:spire_2.11:jar:0.7.4 from the shaded jar.
[INFO] Excluding org.spire-math:spire-macros_2.11:jar:0.7.4 from the shaded jar.
[INFO] Excluding org.jpmml:pmml-model:jar:1.2.7 from the shaded jar.
[INFO] Excluding org.jpmml:pmml-agent:jar:1.2.7 from the shaded jar.
[INFO] Excluding org.jpmml:pmml-schema:jar:1.2.7 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-streaming_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-graphx_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding com.github.fommil.netlib:core:jar:1.1.2 from the shaded jar.
[INFO] Excluding net.sourceforge.f2j:arpack_combined_all:jar:0.1 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-sql_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding com.univocity:univocity-parsers:jar:2.1.0 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-sketch_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-catalyst_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.codehaus.janino:janino:jar:2.7.8 from the shaded jar.
[INFO] Excluding org.codehaus.janino:commons-compiler:jar:2.7.8 from the shaded jar.
[INFO] Excluding org.antlr:antlr4-runtime:jar:4.5.2-1 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-column:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-common:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-encoding:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-generator:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-hadoop:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-format:jar:2.3.0-incubating from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-jackson:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-repl_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.scala-lang:scala-compiler:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-parser-combinators_2.11:jar:1.0.4 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-reflect:jar:2.11.8 from the shaded jar.
[INFO] Including com.google.guava:guava:jar:14.0.1 in the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-xml_2.11:jar:1.0.2 from the shaded jar.
[INFO] Replacing original artifact with shaded artifact.
[INFO]
[INFO] --- maven-source-plugin:2.4:jar-no-fork (create-source-jar) @ spark-assembly_2.11 ---
[INFO]
[INFO] --- maven-source-plugin:2.4:test-jar-no-fork (create-source-jar) @ spark-assembly_2.11 ---
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (default) @ spark-assembly_2.11 ---
[INFO] Executing tasks

main:
[INFO] Executed tasks
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Spark Project External Flume Sink 2.0.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.0.0:clean (default-clean) @ spark-streaming-flume-sink_2.11 ---
[INFO]
[INFO] --- maven-enforcer-plugin:1.4.1:enforce (enforce-versions) @ spark-streaming-flume-sink_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:add-source (eclipse-add-source) @ spark-streaming-flume-sink_2.11 ---
[INFO] Add Source directory: /home/cass/spark2/spark/external/flume-sink/src/main/scala
[INFO] Add Test Source directory: /home/cass/spark2/spark/external/flume-sink/src/test/scala
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (default-cli) @ spark-streaming-flume-sink_2.11 ---
[INFO] Dependencies classpath:
/home/cass/.m2/repository/joda-time/joda-time/2.9.3/joda-time-2.9.3.jar:/home/cass/.m2/repository/log4j/log4j/1.2.17/log4j-1.2.17.jar:/home/cass/.m2/repository/org/scala-lang/scala-library/2.11.8/scala-library-2.11.8.jar:/home/cass/.m2/repository/commons-lang/commons-lang/2.6/commons-lang-2.6.jar:/home/cass/.m2/repository/org/apache/mina/mina-core/2.0.4/mina-core-2.0.4.jar:/home/cass/.m2/repository/org/apache/commons/commons-compress/1.4.1/commons-compress-1.4.1.jar:/home/cass/.m2/repository/org/tukaani/xz/1.0/xz-1.0.jar:/home/cass/.m2/repository/org/slf4j/slf4j-api/1.7.16/slf4j-api-1.7.16.jar:/home/cass/.m2/repository/commons-cli/commons-cli/1.2/commons-cli-1.2.jar:/home/cass/.m2/repository/commons-codec/commons-codec/1.10/commons-codec-1.10.jar:/home/cass/.m2/repository/org/slf4j/slf4j-log4j12/1.7.16/slf4j-log4j12-1.7.16.jar:/home/cass/.m2/repository/org/mortbay/jetty/jetty-util/6.1.26/jetty-util-6.1.26.jar:/home/cass/.m2/repository/com/google/code/gson/gson/2.2.2/gson-2.2.2.jar:/home/cass/.m2/repository/org/apache/flume/flume-ng-sdk/1.6.0/flume-ng-sdk-1.6.0.jar:/home/cass/.m2/repository/org/spark-project/spark/unused/1.0.0/unused-1.0.0.jar:/home/cass/.m2/repository/org/apache/avro/avro-ipc/1.7.7/avro-ipc-1.7.7.jar:/home/cass/.m2/repository/commons-io/commons-io/2.4/commons-io-2.4.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-mapper-asl/1.9.13/jackson-mapper-asl-1.9.13.jar:/home/cass/.m2/repository/org/apache/avro/avro/1.7.7/avro-1.7.7.jar:/home/cass/.m2/repository/org/xerial/snappy/snappy-java/1.1.2.4/snappy-java-1.1.2.4.jar:/home/cass/.m2/repository/org/apache/flume/flume-ng-core/1.6.0/flume-ng-core-1.6.0.jar:/home/cass/.m2/repository/org/mortbay/jetty/jetty/6.1.26/jetty-6.1.26.jar:/home/cass/.m2/repository/com/thoughtworks/paranamer/paranamer/2.3/paranamer-2.3.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-core-asl/1.9.13/jackson-core-asl-1.9.13.jar:/home/cass/.m2/repository/org/apache/flume/flume-ng-configuration/1.6.0/flume-ng-configuration-1.6.0.jar:/home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- avro-maven-plugin:1.7.7:idl-protocol (default) @ spark-streaming-flume-sink_2.11 ---
[INFO]
[INFO] --- maven-remote-resources-plugin:1.5:process (default) @ spark-streaming-flume-sink_2.11 ---
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ spark-streaming-flume-sink_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/external/flume-sink/src/main/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:compile (scala-compile-first) @ spark-streaming-flume-sink_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 6 Scala sources and 3 Java sources to /home/cass/spark2/spark/external/flume-sink/target/scala-2.11/classes...
[warn] Class org.jboss.netty.channel.ChannelFactory not found - continuing with a stub.
[warn] Class org.jboss.netty.channel.ChannelFactory not found - continuing with a stub.
[warn] Class org.jboss.netty.channel.ChannelPipelineFactory not found - continuing with a stub.
[warn] Class org.jboss.netty.handler.execution.ExecutionHandler not found - continuing with a stub.
[warn] Class org.jboss.netty.channel.ChannelFactory not found - continuing with a stub.
[warn] Class org.jboss.netty.handler.execution.ExecutionHandler not found - continuing with a stub.
[warn] Class org.jboss.netty.channel.group.ChannelGroup not found - continuing with a stub.
[warn] Class com.google.common.collect.ImmutableMap not found - continuing with a stub.
[warn] Class com.google.common.collect.ImmutableMap not found - continuing with a stub.
[warn] Class com.google.common.collect.ImmutableMap not found - continuing with a stub.
[warn] Class com.google.common.collect.ImmutableMap not found - continuing with a stub.
[warn] 11 warnings found
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] /home/cass/spark2/spark/external/flume-sink/target/scala-2.11/src_managed/main/compiled_avro/org/apache/spark/streaming/flume/sink/EventBatch.java:243: warning: [unchecked] unchecked cast
[warn]         record.events = fieldSetFlags()[2] ? this.events : (java.util.List<org.apache.spark.streaming.flume.sink.SparkSinkEvent>) defaultValue(fields()[2]);
[warn]                                                                                                                                               ^
[warn]   required: List<SparkSinkEvent>
[warn]   found:    Object
[warn] /home/cass/spark2/spark/external/flume-sink/target/scala-2.11/src_managed/main/compiled_avro/org/apache/spark/streaming/flume/sink/SparkSinkEvent.java:188: warning: [unchecked] unchecked cast
[warn]         record.headers = fieldSetFlags()[0] ? this.headers : (java.util.Map<java.lang.CharSequence,java.lang.CharSequence>) defaultValue(fields()[0]);
[warn]                                                                                                                                         ^
[warn]   required: Map<CharSequence,CharSequence>
[warn]   found:    Object
[warn] 3 warnings
[info] Compile success at May 20, 2016 12:36:44 PM [1.732s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:compile (default-compile) @ spark-streaming-flume-sink_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 3 source files to /home/cass/spark2/spark/external/flume-sink/target/scala-2.11/classes
[WARNING] /home/cass/spark2/spark/external/flume-sink/target/scala-2.11/src_managed/main/compiled_avro/org/apache/spark/streaming/flume/sink/SparkSinkEvent.java:[188,136] [unchecked] unchecked cast
[WARNING]   required: Map<CharSequence,CharSequence>
  found:    Object
/home/cass/spark2/spark/external/flume-sink/target/scala-2.11/src_managed/main/compiled_avro/org/apache/spark/streaming/flume/sink/EventBatch.java:[243,142] [unchecked] unchecked cast
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (create-tmp-dir) @ spark-streaming-flume-sink_2.11 ---
[INFO] Executing tasks

main:
    [mkdir] Created dir: /home/cass/spark2/spark/external/flume-sink/target/tmp
[INFO] Executed tasks
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ spark-streaming-flume-sink_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 1 resource
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:testCompile (scala-test-compile-first) @ spark-streaming-flume-sink_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 1 Scala source to /home/cass/spark2/spark/external/flume-sink/target/scala-2.11/test-classes...
[info] Compile success at May 20, 2016 12:36:46 PM [0.795s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:testCompile (default-testCompile) @ spark-streaming-flume-sink_2.11 ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (generate-test-classpath) @ spark-streaming-flume-sink_2.11 ---
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (default-test) @ spark-streaming-flume-sink_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (test) @ spark-streaming-flume-sink_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- scalatest-maven-plugin:1.0:test (test) @ spark-streaming-flume-sink_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (prepare-test-jar) @ spark-streaming-flume-sink_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/external/flume-sink/target/spark-streaming-flume-sink_2.11-2.0.0-SNAPSHOT-tests.jar
[INFO]
[INFO] --- maven-jar-plugin:2.6:jar (default-jar) @ spark-streaming-flume-sink_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/external/flume-sink/target/spark-streaming-flume-sink_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-site-plugin:3.3:attach-descriptor (attach-descriptor) @ spark-streaming-flume-sink_2.11 ---
[INFO]
[INFO] --- maven-shade-plugin:2.4.3:shade (default) @ spark-streaming-flume-sink_2.11 ---
[INFO] Excluding org.apache.flume:flume-ng-sdk:jar:1.6.0 from the shaded jar.
[INFO] Excluding org.apache.avro:avro:jar:1.7.7 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-core-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-mapper-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding com.thoughtworks.paranamer:paranamer:jar:2.3 from the shaded jar.
[INFO] Excluding org.xerial.snappy:snappy-java:jar:1.1.2.4 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-compress:jar:1.4.1 from the shaded jar.
[INFO] Excluding org.tukaani:xz:jar:1.0 from the shaded jar.
[INFO] Excluding org.apache.avro:avro-ipc:jar:1.7.7 from the shaded jar.
[INFO] Excluding org.apache.flume:flume-ng-core:jar:1.6.0 from the shaded jar.
[INFO] Excluding org.apache.flume:flume-ng-configuration:jar:1.6.0 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-api:jar:1.7.16 from the shaded jar.
[INFO] Excluding commons-io:commons-io:jar:2.4 from the shaded jar.
[INFO] Excluding commons-codec:commons-codec:jar:1.10 from the shaded jar.
[INFO] Excluding log4j:log4j:jar:1.2.17 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-log4j12:jar:1.7.16 from the shaded jar.
[INFO] Excluding commons-cli:commons-cli:jar:1.2 from the shaded jar.
[INFO] Excluding commons-lang:commons-lang:jar:2.6 from the shaded jar.
[INFO] Excluding joda-time:joda-time:jar:2.9.3 from the shaded jar.
[INFO] Excluding org.mortbay.jetty:jetty-util:jar:6.1.26 from the shaded jar.
[INFO] Excluding org.mortbay.jetty:jetty:jar:6.1.26 from the shaded jar.
[INFO] Excluding com.google.code.gson:gson:jar:2.2.2 from the shaded jar.
[INFO] Excluding org.apache.mina:mina-core:jar:2.0.4 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-library:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-tags_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Including org.spark-project.spark:unused:jar:1.0.0 in the shaded jar.
[INFO] Replacing original artifact with shaded artifact.
[INFO] Replacing /home/cass/spark2/spark/external/flume-sink/target/spark-streaming-flume-sink_2.11-2.0.0-SNAPSHOT.jar with /home/cass/spark2/spark/external/flume-sink/target/spark-streaming-flume-sink_2.11-2.0.0-SNAPSHOT-shaded.jar
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/external/flume-sink/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/external/flume-sink/dependency-reduced-pom.xml
[INFO]
[INFO] --- maven-source-plugin:2.4:jar-no-fork (create-source-jar) @ spark-streaming-flume-sink_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/external/flume-sink/target/spark-streaming-flume-sink_2.11-2.0.0-SNAPSHOT-sources.jar
[INFO]
[INFO] --- maven-source-plugin:2.4:test-jar-no-fork (create-source-jar) @ spark-streaming-flume-sink_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/external/flume-sink/target/spark-streaming-flume-sink_2.11-2.0.0-SNAPSHOT-test-sources.jar
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Spark Project External Flume 2.0.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.0.0:clean (default-clean) @ spark-streaming-flume_2.11 ---
[INFO]
[INFO] --- maven-enforcer-plugin:1.4.1:enforce (enforce-versions) @ spark-streaming-flume_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:add-source (eclipse-add-source) @ spark-streaming-flume_2.11 ---
[INFO] Add Source directory: /home/cass/spark2/spark/external/flume/src/main/scala
[INFO] Add Test Source directory: /home/cass/spark2/spark/external/flume/src/test/scala
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (default-cli) @ spark-streaming-flume_2.11 ---
[INFO] Dependencies classpath:
/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-jobclient/2.2.0/hadoop-mapreduce-client-jobclient-2.2.0.jar:/home/cass/.m2/repository/log4j/log4j/1.2.17/log4j-1.2.17.jar:/home/cass/.m2/repository/org/scala-lang/scala-library/2.11.8/scala-library-2.11.8.jar:/home/cass/.m2/repository/com/google/protobuf/protobuf-java/2.5.0/protobuf-java-2.5.0.jar:/home/cass/.m2/repository/aopalliance/aopalliance/1.0/aopalliance-1.0.jar:/home/cass/.m2/repository/org/apache/curator/curator-client/2.4.0/curator-client-2.4.0.jar:/home/cass/.m2/repository/org/apache/mina/mina-core/2.0.4/mina-core-2.0.4.jar:/home/cass/.m2/repository/org/apache/commons/commons-compress/1.4.1/commons-compress-1.4.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-client/2.2.0/hadoop-client-2.2.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-app/2.2.0/hadoop-mapreduce-client-app-2.2.0.jar:/home/cass/.m2/repository/org/slf4j/slf4j-api/1.7.16/slf4j-api-1.7.16.jar:/home/cass/.m2/repository/net/java/dev/jets3t/jets3t/0.7.1/jets3t-0.7.1.jar:/home/cass/.m2/repository/org/mortbay/jetty/jetty-util/6.1.26/jetty-util-6.1.26.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-server-common/2.2.0/hadoop-yarn-server-common-2.2.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-common/2.2.0/hadoop-common-2.2.0.jar:/home/cass/.m2/repository/com/google/inject/guice/3.0/guice-3.0.jar:/home/cass/.m2/repository/commons-io/commons-io/2.4/commons-io-2.4.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-hdfs/2.2.0/hadoop-hdfs-2.2.0.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-mapper-asl/1.9.13/jackson-mapper-asl-1.9.13.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-api/2.2.0/hadoop-yarn-api-2.2.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-common/2.2.0/hadoop-yarn-common-2.2.0.jar:/home/cass/.m2/repository/org/xerial/snappy/snappy-java/1.1.2.4/snappy-java-1.1.2.4.jar:/home/cass/.m2/repository/org/apache/flume/flume-ng-core/1.6.0/flume-ng-core-1.6.0.jar:/home/cass/.m2/repository/org/apache/avro/avro-mapred/1.7.7/avro-mapred-1.7.7-hadoop2.jar:/home/cass/.m2/repository/xmlenc/xmlenc/0.52/xmlenc-0.52.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-shuffle/2.2.0/hadoop-mapreduce-client-shuffle-2.2.0.jar:/home/cass/.m2/repository/org/apache/zookeeper/zookeeper/3.4.5/zookeeper-3.4.5.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-auth/2.2.0/hadoop-auth-2.2.0.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-core-asl/1.9.13/jackson-core-asl-1.9.13.jar:/home/cass/.m2/repository/org/apache/curator/curator-framework/2.4.0/curator-framework-2.4.0.jar:/home/cass/spark2/spark/external/flume-sink/target/spark-streaming-flume-sink_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/commons-net/commons-net/2.2/commons-net-2.2.jar:/home/cass/.m2/repository/org/apache/flume/flume-ng-configuration/1.6.0/flume-ng-configuration-1.6.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-client/2.2.0/hadoop-yarn-client-2.2.0.jar:/home/cass/.m2/repository/org/apache/commons/commons-math/2.1/commons-math-2.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-annotations/2.2.0/hadoop-annotations-2.2.0.jar:/home/cass/.m2/repository/joda-time/joda-time/2.9.3/joda-time-2.9.3.jar:/home/cass/.m2/repository/com/thoughtworks/paranamer/paranamer/2.6/paranamer-2.6.jar:/home/cass/.m2/repository/commons-configuration/commons-configuration/1.6/commons-configuration-1.6.jar:/home/cass/.m2/repository/commons-digester/commons-digester/1.8/commons-digester-1.8.jar:/home/cass/.m2/repository/commons-beanutils/commons-beanutils/1.7.0/commons-beanutils-1.7.0.jar:/home/cass/.m2/repository/commons-lang/commons-lang/2.6/commons-lang-2.6.jar:/home/cass/.m2/repository/org/tukaani/xz/1.0/xz-1.0.jar:/home/cass/.m2/repository/commons-cli/commons-cli/1.2/commons-cli-1.2.jar:/home/cass/.m2/repository/org/apache/curator/curator-recipes/2.4.0/curator-recipes-2.4.0.jar:/home/cass/.m2/repository/commons-codec/commons-codec/1.10/commons-codec-1.10.jar:/home/cass/.m2/repository/org/slf4j/slf4j-log4j12/1.7.16/slf4j-log4j12-1.7.16.jar:/home/cass/.m2/repository/com/google/code/gson/gson/2.2.2/gson-2.2.2.jar:/home/cass/.m2/repository/org/apache/flume/flume-ng-sdk/1.6.0/flume-ng-sdk-1.6.0.jar:/home/cass/.m2/repository/javax/inject/javax.inject/1/javax.inject-1.jar:/home/cass/.m2/repository/org/spark-project/spark/unused/1.0.0/unused-1.0.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-core/2.2.0/hadoop-mapreduce-client-core-2.2.0.jar:/home/cass/.m2/repository/org/apache/avro/avro-ipc/1.7.7/avro-ipc-1.7.7.jar:/home/cass/.m2/repository/commons-beanutils/commons-beanutils-core/1.8.0/commons-beanutils-core-1.8.0.jar:/home/cass/.m2/repository/commons-collections/commons-collections/3.2.2/commons-collections-3.2.2.jar:/home/cass/.m2/repository/org/apache/avro/avro/1.7.7/avro-1.7.7.jar:/home/cass/.m2/repository/org/mortbay/jetty/jetty/6.1.26/jetty-6.1.26.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-common/2.2.0/hadoop-mapreduce-client-common-2.2.0.jar:/home/cass/.m2/repository/commons-httpclient/commons-httpclient/3.1/commons-httpclient-3.1.jar:/home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-remote-resources-plugin:1.5:process (default) @ spark-streaming-flume_2.11 ---
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ spark-streaming-flume_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/external/flume/src/main/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:compile (scala-compile-first) @ spark-streaming-flume_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 8 Scala sources and 1 Java source to /home/cass/spark2/spark/external/flume/target/scala-2.11/classes...
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] 1 warning
[info] Compile success at May 20, 2016 12:36:50 PM [1.888s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:compile (default-compile) @ spark-streaming-flume_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 1 source file to /home/cass/spark2/spark/external/flume/target/scala-2.11/classes
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (create-tmp-dir) @ spark-streaming-flume_2.11 ---
[INFO] Executing tasks

main:
    [mkdir] Created dir: /home/cass/spark2/spark/external/flume/target/tmp
[INFO] Executed tasks
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ spark-streaming-flume_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 1 resource
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:testCompile (scala-test-compile-first) @ spark-streaming-flume_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 3 Scala sources and 3 Java sources to /home/cass/spark2/spark/external/flume/target/scala-2.11/test-classes...
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] 1 warning
[info] Compile success at May 20, 2016 12:36:53 PM [2.079s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:testCompile (default-testCompile) @ spark-streaming-flume_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 3 source files to /home/cass/spark2/spark/external/flume/target/scala-2.11/test-classes
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (generate-test-classpath) @ spark-streaming-flume_2.11 ---
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (default-test) @ spark-streaming-flume_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (test) @ spark-streaming-flume_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- scalatest-maven-plugin:1.0:test (test) @ spark-streaming-flume_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (prepare-test-jar) @ spark-streaming-flume_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/external/flume/target/spark-streaming-flume_2.11-2.0.0-SNAPSHOT-tests.jar
[INFO]
[INFO] --- maven-jar-plugin:2.6:jar (default-jar) @ spark-streaming-flume_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/external/flume/target/spark-streaming-flume_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-site-plugin:3.3:attach-descriptor (attach-descriptor) @ spark-streaming-flume_2.11 ---
[INFO]
[INFO] --- maven-shade-plugin:2.4.3:shade (default) @ spark-streaming-flume_2.11 ---
[INFO] Excluding org.scala-lang:scala-library:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.apache.avro:avro-mapred:jar:hadoop2:1.7.7 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-core-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-mapper-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-math:jar:2.1 from the shaded jar.
[INFO] Excluding xmlenc:xmlenc:jar:0.52 from the shaded jar.
[INFO] Excluding commons-configuration:commons-configuration:jar:1.6 from the shaded jar.
[INFO] Excluding commons-collections:commons-collections:jar:3.2.2 from the shaded jar.
[INFO] Excluding commons-digester:commons-digester:jar:1.8 from the shaded jar.
[INFO] Excluding commons-beanutils:commons-beanutils:jar:1.7.0 from the shaded jar.
[INFO] Excluding commons-beanutils:commons-beanutils-core:jar:1.8.0 from the shaded jar.
[INFO] Excluding com.google.protobuf:protobuf-java:jar:2.5.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-auth:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-hdfs:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-app:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding com.google.inject:guice:jar:3.0 from the shaded jar.
[INFO] Excluding javax.inject:javax.inject:jar:1 from the shaded jar.
[INFO] Excluding aopalliance:aopalliance:jar:1.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-server-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-shuffle:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-api:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-core:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-jobclient:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-annotations:jar:2.2.0 from the shaded jar.
[INFO] Excluding net.java.dev.jets3t:jets3t:jar:0.7.1 from the shaded jar.
[INFO] Excluding commons-httpclient:commons-httpclient:jar:3.1 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-recipes:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-framework:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-client:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.zookeeper:zookeeper:jar:3.4.5 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-api:jar:1.7.16 from the shaded jar.
[INFO] Excluding log4j:log4j:jar:1.2.17 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-log4j12:jar:1.7.16 from the shaded jar.
[INFO] Excluding org.xerial.snappy:snappy-java:jar:1.1.2.4 from the shaded jar.
[INFO] Excluding commons-net:commons-net:jar:2.2 from the shaded jar.
[INFO] Excluding com.thoughtworks.paranamer:paranamer:jar:2.6 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-streaming-flume-sink_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.flume:flume-ng-core:jar:1.6.0 from the shaded jar.
[INFO] Excluding org.apache.flume:flume-ng-configuration:jar:1.6.0 from the shaded jar.
[INFO] Excluding commons-io:commons-io:jar:2.4 from the shaded jar.
[INFO] Excluding commons-codec:commons-codec:jar:1.10 from the shaded jar.
[INFO] Excluding commons-cli:commons-cli:jar:1.2 from the shaded jar.
[INFO] Excluding commons-lang:commons-lang:jar:2.6 from the shaded jar.
[INFO] Excluding org.apache.avro:avro:jar:1.7.7 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-compress:jar:1.4.1 from the shaded jar.
[INFO] Excluding org.tukaani:xz:jar:1.0 from the shaded jar.
[INFO] Excluding org.apache.avro:avro-ipc:jar:1.7.7 from the shaded jar.
[INFO] Excluding joda-time:joda-time:jar:2.9.3 from the shaded jar.
[INFO] Excluding org.mortbay.jetty:jetty-util:jar:6.1.26 from the shaded jar.
[INFO] Excluding org.mortbay.jetty:jetty:jar:6.1.26 from the shaded jar.
[INFO] Excluding com.google.code.gson:gson:jar:2.2.2 from the shaded jar.
[INFO] Excluding org.apache.mina:mina-core:jar:2.0.4 from the shaded jar.
[INFO] Excluding org.apache.flume:flume-ng-sdk:jar:1.6.0 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-tags_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Including org.spark-project.spark:unused:jar:1.0.0 in the shaded jar.
[INFO] Replacing original artifact with shaded artifact.
[INFO] Replacing /home/cass/spark2/spark/external/flume/target/spark-streaming-flume_2.11-2.0.0-SNAPSHOT.jar with /home/cass/spark2/spark/external/flume/target/spark-streaming-flume_2.11-2.0.0-SNAPSHOT-shaded.jar
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/external/flume/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/external/flume/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/external/flume/dependency-reduced-pom.xml
[INFO]
[INFO] --- maven-source-plugin:2.4:jar-no-fork (create-source-jar) @ spark-streaming-flume_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/external/flume/target/spark-streaming-flume_2.11-2.0.0-SNAPSHOT-sources.jar
[INFO]
[INFO] --- maven-source-plugin:2.4:test-jar-no-fork (create-source-jar) @ spark-streaming-flume_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/external/flume/target/spark-streaming-flume_2.11-2.0.0-SNAPSHOT-test-sources.jar
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Spark Project External Flume Assembly 2.0.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.0.0:clean (default-clean) @ spark-streaming-flume-assembly_2.11 ---
[INFO]
[INFO] --- maven-enforcer-plugin:1.4.1:enforce (enforce-versions) @ spark-streaming-flume-assembly_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:add-source (eclipse-add-source) @ spark-streaming-flume-assembly_2.11 ---
[INFO] Add Source directory: /home/cass/spark2/spark/external/flume-assembly/src/main/scala
[INFO] Add Test Source directory: /home/cass/spark2/spark/external/flume-assembly/src/test/scala
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (default-cli) @ spark-streaming-flume-assembly_2.11 ---
[INFO] Dependencies classpath:
/home/cass/.m2/repository/com/google/code/gson/gson/2.2.2/gson-2.2.2.jar:/home/cass/.m2/repository/joda-time/joda-time/2.9.3/joda-time-2.9.3.jar:/home/cass/.m2/repository/org/apache/mina/mina-core/2.0.4/mina-core-2.0.4.jar:/home/cass/.m2/repository/org/apache/flume/flume-ng-sdk/1.6.0/flume-ng-sdk-1.6.0.jar:/home/cass/.m2/repository/org/spark-project/spark/unused/1.0.0/unused-1.0.0.jar:/home/cass/spark2/spark/external/flume/target/spark-streaming-flume_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/commons-io/commons-io/2.4/commons-io-2.4.jar:/home/cass/spark2/spark/external/flume-sink/target/spark-streaming-flume-sink_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/commons-cli/commons-cli/1.2/commons-cli-1.2.jar:/home/cass/.m2/repository/org/apache/flume/flume-ng-configuration/1.6.0/flume-ng-configuration-1.6.0.jar:/home/cass/.m2/repository/org/apache/flume/flume-ng-core/1.6.0/flume-ng-core-1.6.0.jar:/home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-remote-resources-plugin:1.5:process (default) @ spark-streaming-flume-assembly_2.11 ---
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ spark-streaming-flume-assembly_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/external/flume-assembly/src/main/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:compile (scala-compile-first) @ spark-streaming-flume-assembly_2.11 ---
[INFO] No sources to compile
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:compile (default-compile) @ spark-streaming-flume-assembly_2.11 ---
[INFO] No sources to compile
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (create-tmp-dir) @ spark-streaming-flume-assembly_2.11 ---
[INFO] Executing tasks

main:
    [mkdir] Created dir: /home/cass/spark2/spark/external/flume-assembly/target/tmp
[INFO] Executed tasks
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ spark-streaming-flume-assembly_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/external/flume-assembly/src/test/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:testCompile (scala-test-compile-first) @ spark-streaming-flume-assembly_2.11 ---
[INFO] No sources to compile
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:testCompile (default-testCompile) @ spark-streaming-flume-assembly_2.11 ---
[INFO] No sources to compile
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (generate-test-classpath) @ spark-streaming-flume-assembly_2.11 ---
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (default-test) @ spark-streaming-flume-assembly_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (test) @ spark-streaming-flume-assembly_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- scalatest-maven-plugin:1.0:test (test) @ spark-streaming-flume-assembly_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (prepare-test-jar) @ spark-streaming-flume-assembly_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/external/flume-assembly/target/spark-streaming-flume-assembly_2.11-2.0.0-SNAPSHOT-tests.jar
[INFO]
[INFO] --- maven-jar-plugin:2.6:jar (default-jar) @ spark-streaming-flume-assembly_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/external/flume-assembly/target/spark-streaming-flume-assembly_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-site-plugin:3.3:attach-descriptor (attach-descriptor) @ spark-streaming-flume-assembly_2.11 ---
[INFO]
[INFO] --- maven-shade-plugin:2.4.3:shade (default) @ spark-streaming-flume-assembly_2.11 ---
[INFO] Including org.apache.spark:spark-streaming-flume_2.11:jar:2.0.0-SNAPSHOT in the shaded jar.
[INFO] Including org.apache.spark:spark-streaming-flume-sink_2.11:jar:2.0.0-SNAPSHOT in the shaded jar.
[INFO] Including org.apache.flume:flume-ng-core:jar:1.6.0 in the shaded jar.
[INFO] Including org.apache.flume:flume-ng-configuration:jar:1.6.0 in the shaded jar.
[INFO] Including commons-io:commons-io:jar:2.4 in the shaded jar.
[INFO] Including commons-cli:commons-cli:jar:1.2 in the shaded jar.
[INFO] Including joda-time:joda-time:jar:2.9.3 in the shaded jar.
[INFO] Including com.google.code.gson:gson:jar:2.2.2 in the shaded jar.
[INFO] Including org.apache.mina:mina-core:jar:2.0.4 in the shaded jar.
[INFO] Including org.apache.flume:flume-ng-sdk:jar:1.6.0 in the shaded jar.
[INFO] Including org.apache.spark:spark-tags_2.11:jar:2.0.0-SNAPSHOT in the shaded jar.
[INFO] Including org.spark-project.spark:unused:jar:1.0.0 in the shaded jar.
[WARNING] unused-1.0.0.jar, spark-tags_2.11-2.0.0-SNAPSHOT.jar, spark-streaming-flume_2.11-2.0.0-SNAPSHOT.jar, spark-streaming-flume-sink_2.11-2.0.0-SNAPSHOT.jar define 1 overlapping classes:
[WARNING]   - org.apache.spark.unused.UnusedStubClass
[WARNING] maven-shade-plugin has detected that some class files are
[WARNING] present in two or more JARs. When this happens, only one
[WARNING] single version of the class is copied to the uber jar.
[WARNING] Usually this is not harmful and you can skip these warnings,
[WARNING] otherwise try to manually exclude artifacts based on
[WARNING] mvn dependency:tree -Ddetail=true and the above output.
[WARNING] See http://maven.apache.org/plugins/maven-shade-plugin/
[INFO] Replacing original artifact with shaded artifact.
[INFO] Replacing /home/cass/spark2/spark/external/flume-assembly/target/spark-streaming-flume-assembly_2.11-2.0.0-SNAPSHOT.jar with /home/cass/spark2/spark/external/flume-assembly/target/spark-streaming-flume-assembly_2.11-2.0.0-SNAPSHOT-shaded.jar
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/external/flume-assembly/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/external/flume-assembly/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/external/flume-assembly/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/external/flume-assembly/dependency-reduced-pom.xml
[INFO]
[INFO] --- maven-source-plugin:2.4:jar-no-fork (create-source-jar) @ spark-streaming-flume-assembly_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/external/flume-assembly/target/spark-streaming-flume-assembly_2.11-2.0.0-SNAPSHOT-sources.jar
[INFO]
[INFO] --- maven-source-plugin:2.4:test-jar-no-fork (create-source-jar) @ spark-streaming-flume-assembly_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/external/flume-assembly/target/spark-streaming-flume-assembly_2.11-2.0.0-SNAPSHOT-test-sources.jar
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Spark Integration for Kafka 0.8 2.0.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.0.0:clean (default-clean) @ spark-streaming-kafka-0-8_2.11 ---
[INFO]
[INFO] --- maven-enforcer-plugin:1.4.1:enforce (enforce-versions) @ spark-streaming-kafka-0-8_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:add-source (eclipse-add-source) @ spark-streaming-kafka-0-8_2.11 ---
[INFO] Add Source directory: /home/cass/spark2/spark/external/kafka-0-8/src/main/scala
[INFO] Add Test Source directory: /home/cass/spark2/spark/external/kafka-0-8/src/test/scala
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (default-cli) @ spark-streaming-kafka-0-8_2.11 ---
[INFO] Dependencies classpath:
/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-jobclient/2.2.0/hadoop-mapreduce-client-jobclient-2.2.0.jar:/home/cass/.m2/repository/log4j/log4j/1.2.17/log4j-1.2.17.jar:/home/cass/.m2/repository/org/scala-lang/scala-library/2.11.8/scala-library-2.11.8.jar:/home/cass/.m2/repository/com/google/protobuf/protobuf-java/2.5.0/protobuf-java-2.5.0.jar:/home/cass/.m2/repository/aopalliance/aopalliance/1.0/aopalliance-1.0.jar:/home/cass/.m2/repository/org/apache/curator/curator-client/2.4.0/curator-client-2.4.0.jar:/home/cass/.m2/repository/org/apache/commons/commons-compress/1.4.1/commons-compress-1.4.1.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-parser-combinators_2.11/1.0.2/scala-parser-combinators_2.11-1.0.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-client/2.2.0/hadoop-client-2.2.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-app/2.2.0/hadoop-mapreduce-client-app-2.2.0.jar:/home/cass/.m2/repository/org/slf4j/slf4j-api/1.7.16/slf4j-api-1.7.16.jar:/home/cass/.m2/repository/net/java/dev/jets3t/jets3t/0.7.1/jets3t-0.7.1.jar:/home/cass/.m2/repository/org/mortbay/jetty/jetty-util/6.1.26/jetty-util-6.1.26.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-server-common/2.2.0/hadoop-yarn-server-common-2.2.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-common/2.2.0/hadoop-common-2.2.0.jar:/home/cass/.m2/repository/com/google/inject/guice/3.0/guice-3.0.jar:/home/cass/.m2/repository/commons-io/commons-io/2.4/commons-io-2.4.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-hdfs/2.2.0/hadoop-hdfs-2.2.0.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-mapper-asl/1.9.13/jackson-mapper-asl-1.9.13.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-api/2.2.0/hadoop-yarn-api-2.2.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-common/2.2.0/hadoop-yarn-common-2.2.0.jar:/home/cass/.m2/repository/org/xerial/snappy/snappy-java/1.1.2.4/snappy-java-1.1.2.4.jar:/home/cass/.m2/repository/org/apache/avro/avro-mapred/1.7.7/avro-mapred-1.7.7-hadoop2.jar:/home/cass/.m2/repository/xmlenc/xmlenc/0.52/xmlenc-0.52.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-shuffle/2.2.0/hadoop-mapreduce-client-shuffle-2.2.0.jar:/home/cass/.m2/repository/org/apache/zookeeper/zookeeper/3.4.5/zookeeper-3.4.5.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-auth/2.2.0/hadoop-auth-2.2.0.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-core-asl/1.9.13/jackson-core-asl-1.9.13.jar:/home/cass/.m2/repository/org/apache/curator/curator-framework/2.4.0/curator-framework-2.4.0.jar:/home/cass/.m2/repository/commons-net/commons-net/2.2/commons-net-2.2.jar:/home/cass/.m2/repository/net/jpountz/lz4/lz4/1.3.0/lz4-1.3.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-client/2.2.0/hadoop-yarn-client-2.2.0.jar:/home/cass/.m2/repository/org/apache/commons/commons-math/2.1/commons-math-2.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-annotations/2.2.0/hadoop-annotations-2.2.0.jar:/home/cass/.m2/repository/com/thoughtworks/paranamer/paranamer/2.6/paranamer-2.6.jar:/home/cass/.m2/repository/commons-configuration/commons-configuration/1.6/commons-configuration-1.6.jar:/home/cass/.m2/repository/commons-digester/commons-digester/1.8/commons-digester-1.8.jar:/home/cass/.m2/repository/commons-beanutils/commons-beanutils/1.7.0/commons-beanutils-1.7.0.jar:/home/cass/.m2/repository/commons-lang/commons-lang/2.6/commons-lang-2.6.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-xml_2.11/1.0.2/scala-xml_2.11-1.0.2.jar:/home/cass/.m2/repository/com/yammer/metrics/metrics-core/2.2.0/metrics-core-2.2.0.jar:/home/cass/.m2/repository/org/tukaani/xz/1.0/xz-1.0.jar:/home/cass/.m2/repository/commons-cli/commons-cli/1.2/commons-cli-1.2.jar:/home/cass/.m2/repository/commons-codec/commons-codec/1.10/commons-codec-1.10.jar:/home/cass/.m2/repository/org/apache/curator/curator-recipes/2.4.0/curator-recipes-2.4.0.jar:/home/cass/.m2/repository/org/slf4j/slf4j-log4j12/1.7.16/slf4j-log4j12-1.7.16.jar:/home/cass/.m2/repository/javax/inject/javax.inject/1/javax.inject-1.jar:/home/cass/.m2/repository/org/spark-project/spark/unused/1.0.0/unused-1.0.0.jar:/home/cass/.m2/repository/org/apache/avro/avro-ipc/1.7.7/avro-ipc-1.7.7.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-core/2.2.0/hadoop-mapreduce-client-core-2.2.0.jar:/home/cass/.m2/repository/commons-beanutils/commons-beanutils-core/1.8.0/commons-beanutils-core-1.8.0.jar:/home/cass/.m2/repository/org/apache/kafka/kafka-clients/0.8.2.1/kafka-clients-0.8.2.1.jar:/home/cass/.m2/repository/commons-collections/commons-collections/3.2.2/commons-collections-3.2.2.jar:/home/cass/.m2/repository/org/apache/kafka/kafka_2.11/0.8.2.1/kafka_2.11-0.8.2.1.jar:/home/cass/.m2/repository/org/apache/avro/avro/1.7.7/avro-1.7.7.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-common/2.2.0/hadoop-mapreduce-client-common-2.2.0.jar:/home/cass/.m2/repository/com/101tec/zkclient/0.3/zkclient-0.3.jar:/home/cass/.m2/repository/commons-httpclient/commons-httpclient/3.1/commons-httpclient-3.1.jar:/home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-remote-resources-plugin:1.5:process (default) @ spark-streaming-kafka-0-8_2.11 ---
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ spark-streaming-kafka-0-8_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/external/kafka-0-8/src/main/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:compile (scala-compile-first) @ spark-streaming-kafka-0-8_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 11 Scala sources and 1 Java source to /home/cass/spark2/spark/external/kafka-0-8/target/scala-2.11/classes...
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] 1 warning
[info] Compile success at May 20, 2016 12:36:59 PM [3.649s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:compile (default-compile) @ spark-streaming-kafka-0-8_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 1 source file to /home/cass/spark2/spark/external/kafka-0-8/target/scala-2.11/classes
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (create-tmp-dir) @ spark-streaming-kafka-0-8_2.11 ---
[INFO] Executing tasks

main:
    [mkdir] Created dir: /home/cass/spark2/spark/external/kafka-0-8/target/tmp
[INFO] Executed tasks
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ spark-streaming-kafka-0-8_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 1 resource
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:testCompile (scala-test-compile-first) @ spark-streaming-kafka-0-8_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 5 Scala sources and 3 Java sources to /home/cass/spark2/spark/external/kafka-0-8/target/scala-2.11/test-classes...
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] 1 warning
[info] Compile success at May 20, 2016 12:37:04 PM [3.492s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:testCompile (default-testCompile) @ spark-streaming-kafka-0-8_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 3 source files to /home/cass/spark2/spark/external/kafka-0-8/target/scala-2.11/test-classes
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (generate-test-classpath) @ spark-streaming-kafka-0-8_2.11 ---
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (default-test) @ spark-streaming-kafka-0-8_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (test) @ spark-streaming-kafka-0-8_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- scalatest-maven-plugin:1.0:test (test) @ spark-streaming-kafka-0-8_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (prepare-test-jar) @ spark-streaming-kafka-0-8_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/external/kafka-0-8/target/spark-streaming-kafka-0-8_2.11-2.0.0-SNAPSHOT-tests.jar
[INFO]
[INFO] --- maven-jar-plugin:2.6:jar (default-jar) @ spark-streaming-kafka-0-8_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/external/kafka-0-8/target/spark-streaming-kafka-0-8_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-site-plugin:3.3:attach-descriptor (attach-descriptor) @ spark-streaming-kafka-0-8_2.11 ---
[INFO]
[INFO] --- maven-shade-plugin:2.4.3:shade (default) @ spark-streaming-kafka-0-8_2.11 ---
[INFO] Excluding org.scala-lang:scala-library:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.apache.avro:avro-mapred:jar:hadoop2:1.7.7 from the shaded jar.
[INFO] Excluding org.apache.avro:avro-ipc:jar:1.7.7 from the shaded jar.
[INFO] Excluding org.apache.avro:avro:jar:1.7.7 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-core-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-mapper-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding commons-cli:commons-cli:jar:1.2 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-math:jar:2.1 from the shaded jar.
[INFO] Excluding xmlenc:xmlenc:jar:0.52 from the shaded jar.
[INFO] Excluding commons-io:commons-io:jar:2.4 from the shaded jar.
[INFO] Excluding commons-lang:commons-lang:jar:2.6 from the shaded jar.
[INFO] Excluding commons-configuration:commons-configuration:jar:1.6 from the shaded jar.
[INFO] Excluding commons-collections:commons-collections:jar:3.2.2 from the shaded jar.
[INFO] Excluding commons-digester:commons-digester:jar:1.8 from the shaded jar.
[INFO] Excluding commons-beanutils:commons-beanutils:jar:1.7.0 from the shaded jar.
[INFO] Excluding commons-beanutils:commons-beanutils-core:jar:1.8.0 from the shaded jar.
[INFO] Excluding com.google.protobuf:protobuf-java:jar:2.5.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-auth:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-compress:jar:1.4.1 from the shaded jar.
[INFO] Excluding org.tukaani:xz:jar:1.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-hdfs:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.mortbay.jetty:jetty-util:jar:6.1.26 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-app:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding com.google.inject:guice:jar:3.0 from the shaded jar.
[INFO] Excluding javax.inject:javax.inject:jar:1 from the shaded jar.
[INFO] Excluding aopalliance:aopalliance:jar:1.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-server-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-shuffle:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-api:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-core:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-jobclient:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-annotations:jar:2.2.0 from the shaded jar.
[INFO] Excluding net.java.dev.jets3t:jets3t:jar:0.7.1 from the shaded jar.
[INFO] Excluding commons-codec:commons-codec:jar:1.10 from the shaded jar.
[INFO] Excluding commons-httpclient:commons-httpclient:jar:3.1 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-recipes:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-framework:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-client:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.zookeeper:zookeeper:jar:3.4.5 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-api:jar:1.7.16 from the shaded jar.
[INFO] Excluding log4j:log4j:jar:1.2.17 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-log4j12:jar:1.7.16 from the shaded jar.
[INFO] Excluding org.xerial.snappy:snappy-java:jar:1.1.2.4 from the shaded jar.
[INFO] Excluding net.jpountz.lz4:lz4:jar:1.3.0 from the shaded jar.
[INFO] Excluding commons-net:commons-net:jar:2.2 from the shaded jar.
[INFO] Excluding com.thoughtworks.paranamer:paranamer:jar:2.6 from the shaded jar.
[INFO] Excluding org.apache.kafka:kafka_2.11:jar:0.8.2.1 from the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-xml_2.11:jar:1.0.2 from the shaded jar.
[INFO] Excluding com.yammer.metrics:metrics-core:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-parser-combinators_2.11:jar:1.0.2 from the shaded jar.
[INFO] Excluding com.101tec:zkclient:jar:0.3 from the shaded jar.
[INFO] Excluding org.apache.kafka:kafka-clients:jar:0.8.2.1 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-tags_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Including org.spark-project.spark:unused:jar:1.0.0 in the shaded jar.
[INFO] Replacing original artifact with shaded artifact.
[INFO] Replacing /home/cass/spark2/spark/external/kafka-0-8/target/spark-streaming-kafka-0-8_2.11-2.0.0-SNAPSHOT.jar with /home/cass/spark2/spark/external/kafka-0-8/target/spark-streaming-kafka-0-8_2.11-2.0.0-SNAPSHOT-shaded.jar
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/external/kafka-0-8/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/external/kafka-0-8/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/external/kafka-0-8/dependency-reduced-pom.xml
[INFO]
[INFO] --- maven-source-plugin:2.4:jar-no-fork (create-source-jar) @ spark-streaming-kafka-0-8_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/external/kafka-0-8/target/spark-streaming-kafka-0-8_2.11-2.0.0-SNAPSHOT-sources.jar
[INFO]
[INFO] --- maven-source-plugin:2.4:test-jar-no-fork (create-source-jar) @ spark-streaming-kafka-0-8_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/external/kafka-0-8/target/spark-streaming-kafka-0-8_2.11-2.0.0-SNAPSHOT-test-sources.jar
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Spark Project Examples 2.0.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.0.0:clean (default-clean) @ spark-examples_2.11 ---
[INFO]
[INFO] --- maven-enforcer-plugin:1.4.1:enforce (enforce-versions) @ spark-examples_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:add-source (eclipse-add-source) @ spark-examples_2.11 ---
[INFO] Add Source directory: /home/cass/spark2/spark/examples/src/main/scala
[INFO] Add Test Source directory: /home/cass/spark2/spark/examples/src/test/scala
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (default-cli) @ spark-examples_2.11 ---
[INFO] Dependencies classpath:
/home/cass/.m2/repository/com/github/scopt/scopt_2.11/3.3.0/scopt_2.11-3.3.0.jar
[INFO]
[INFO] --- maven-remote-resources-plugin:1.5:process (default) @ spark-examples_2.11 ---
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ spark-examples_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 7 resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:compile (scala-compile-first) @ spark-examples_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 167 Scala sources and 110 Java sources to /home/cass/spark2/spark/examples/target/scala-2.11/classes...
[warn] /home/cass/spark2/spark/examples/src/main/scala/org/apache/spark/examples/ml/DecisionTreeExample.scala:324: value precision in class MulticlassMetrics is deprecated: Use accuracy.
[warn]     val accuracy = new MulticlassMetrics(predictions.zip(labels)).precision
[warn]                                                                   ^
[warn] /home/cass/spark2/spark/examples/src/main/scala/org/apache/spark/examples/mllib/AbstractParams.scala:41: method declarations in class TypeApi is deprecated: Use `decls` instead
[warn]     val allAccessors = tpe.declarations.collect {
[warn]                            ^
[warn] /home/cass/spark2/spark/examples/src/main/scala/org/apache/spark/examples/mllib/DecisionTreeRunner.scala:299: value precision in class MulticlassMetrics is deprecated: Use accuracy.
[warn]             .precision
[warn]              ^
[warn] /home/cass/spark2/spark/examples/src/main/scala/org/apache/spark/examples/mllib/DecisionTreeRunner.scala:302: value precision in class MulticlassMetrics is deprecated: Use accuracy.
[warn]           new MulticlassMetrics(test.map(lp => (model.predict(lp.features), lp.label))).precision
[warn]                                                                                         ^
[warn] /home/cass/spark2/spark/examples/src/main/scala/org/apache/spark/examples/mllib/DecisionTreeRunner.scala:326: value precision in class MulticlassMetrics is deprecated: Use accuracy.
[warn]             .precision
[warn]              ^
[warn] /home/cass/spark2/spark/examples/src/main/scala/org/apache/spark/examples/mllib/DecisionTreeRunner.scala:329: value precision in class MulticlassMetrics is deprecated: Use accuracy.
[warn]           new MulticlassMetrics(test.map(lp => (model.predict(lp.features), lp.label))).precision
[warn]                                                                                         ^
[warn] /home/cass/spark2/spark/examples/src/main/scala/org/apache/spark/examples/mllib/GradientBoostedTreesRunner.scala:124: value precision in class MulticlassMetrics is deprecated: Use accuracy.
[warn]           .precision
[warn]            ^
[warn] /home/cass/spark2/spark/examples/src/main/scala/org/apache/spark/examples/mllib/GradientBoostedTreesRunner.scala:127: value precision in class MulticlassMetrics is deprecated: Use accuracy.
[warn]         new MulticlassMetrics(test.map(lp => (model.predict(lp.features), lp.label))).precision
[warn]                                                                                       ^
[warn] /home/cass/spark2/spark/examples/src/main/scala/org/apache/spark/examples/mllib/LinearRegression.scala:115: class LinearRegressionWithSGD in package regression is deprecated: Use ml.regression.LinearRegression or LBFGS
[warn]     val algorithm = new LinearRegressionWithSGD()
[warn]                         ^
[warn] /home/cass/spark2/spark/examples/src/main/scala/org/apache/spark/examples/mllib/LinearRegressionWithSGDExample.scala:46: object LinearRegressionWithSGD in package regression is deprecated: Use ml.regression.LinearRegression or LBFGS
[warn]     val model = LinearRegressionWithSGD.train(parsedData, numIterations, stepSize)
[warn]                 ^
[warn] /home/cass/spark2/spark/examples/src/main/scala/org/apache/spark/examples/mllib/LogisticRegressionWithLBFGSExample.scala:57: value precision in class MulticlassMetrics is deprecated: Use accuracy.
[warn]     val precision = metrics.precision
[warn]                             ^
[warn] /home/cass/spark2/spark/examples/src/main/scala/org/apache/spark/examples/mllib/MulticlassMetricsExample.scala:62: value precision in class MulticlassMetrics is deprecated: Use accuracy.
[warn]     val precision = metrics.precision
[warn]                             ^
[warn] /home/cass/spark2/spark/examples/src/main/scala/org/apache/spark/examples/mllib/MulticlassMetricsExample.scala:63: value recall in class MulticlassMetrics is deprecated: Use accuracy.
[warn]     val recall = metrics.recall // same as true positive rate
[warn]                          ^
[warn] /home/cass/spark2/spark/examples/src/main/scala/org/apache/spark/examples/mllib/MulticlassMetricsExample.scala:64: value fMeasure in class MulticlassMetrics is deprecated: Use accuracy.
[warn]     val f1Score = metrics.fMeasure
[warn]                           ^
[warn] /home/cass/spark2/spark/examples/src/main/scala/org/apache/spark/examples/mllib/PCAExample.scala:51: object LinearRegressionWithSGD in package regression is deprecated: Use ml.regression.LinearRegression or LBFGS
[warn]     val model = LinearRegressionWithSGD.train(training, numIterations)
[warn]                 ^
[warn] /home/cass/spark2/spark/examples/src/main/scala/org/apache/spark/examples/mllib/PCAExample.scala:52: object LinearRegressionWithSGD in package regression is deprecated: Use ml.regression.LinearRegression or LBFGS
[warn]     val model_pca = LinearRegressionWithSGD.train(training_pca, numIterations)
[warn]                     ^
[warn] /home/cass/spark2/spark/examples/src/main/scala/org/apache/spark/examples/mllib/RegressionMetricsExample.scala:43: object LinearRegressionWithSGD in package regression is deprecated: Use ml.regression.LinearRegression or LBFGS
[warn]     val model = LinearRegressionWithSGD.train(data, numIterations)
[warn]                 ^
[warn] 17 warnings found
[warn] warning: [options] bootstrap class path not set in conjunction with -source 1.7
[warn] /home/cass/spark2/spark/examples/src/main/java/org/apache/spark/examples/mllib/JavaLinearRegressionWithSGDExample.java:32: warning: [deprecation] LinearRegressionWithSGD in org.apache.spark.mllib.regression has been deprecated
[warn] import org.apache.spark.mllib.regression.LinearRegressionWithSGD;
[warn]                                         ^
[warn] /home/cass/spark2/spark/examples/src/main/java/org/apache/spark/examples/mllib/JavaRegressionMetricsExample.java:28: warning: [deprecation] LinearRegressionWithSGD in org.apache.spark.mllib.regression has been deprecated
[warn] import org.apache.spark.mllib.regression.LinearRegressionWithSGD;
[warn]                                         ^
[warn] /home/cass/spark2/spark/examples/src/main/java/org/apache/spark/examples/streaming/JavaRecoverableNetworkWordCount.java:32: warning: [deprecation] Accumulator in org.apache.spark has been deprecated
[warn] import org.apache.spark.Accumulator;
[warn]                        ^
[warn] /home/cass/spark2/spark/examples/src/main/java/org/apache/spark/examples/mllib/JavaLinearRegressionWithSGDExample.java:66: warning: [deprecation] LinearRegressionWithSGD in org.apache.spark.mllib.regression has been deprecated
[warn]       LinearRegressionWithSGD.train(JavaRDD.toRDD(parsedData), numIterations, stepSize);
[warn]       ^
[warn] /home/cass/spark2/spark/examples/src/main/java/org/apache/spark/examples/mllib/JavaLogisticRegressionWithLBFGSExample.java:68: warning: [deprecation] precision() in MulticlassMetrics has been deprecated
[warn]     double precision = metrics.precision();
[warn]                               ^
[warn] /home/cass/spark2/spark/examples/src/main/java/org/apache/spark/examples/mllib/JavaMulticlassClassificationMetricsExample.java:71: warning: [deprecation] precision() in MulticlassMetrics has been deprecated
[warn]     System.out.println("Precision = " + metrics.precision());
[warn]                                                ^
[warn] /home/cass/spark2/spark/examples/src/main/java/org/apache/spark/examples/mllib/JavaMulticlassClassificationMetricsExample.java:72: warning: [deprecation] recall() in MulticlassMetrics has been deprecated
[warn]     System.out.println("Recall = " + metrics.recall());
[warn]                                             ^
[warn] /home/cass/spark2/spark/examples/src/main/java/org/apache/spark/examples/mllib/JavaMulticlassClassificationMetricsExample.java:73: warning: [deprecation] fMeasure() in MulticlassMetrics has been deprecated
[warn]     System.out.println("F1 Score = " + metrics.fMeasure());
[warn]                                               ^
[warn] /home/cass/spark2/spark/examples/src/main/java/org/apache/spark/examples/mllib/JavaRegressionMetricsExample.java:57: warning: [deprecation] LinearRegressionWithSGD in org.apache.spark.mllib.regression has been deprecated
[warn]     final LinearRegressionModel model = LinearRegressionWithSGD.train(JavaRDD.toRDD(parsedData),
[warn]                                         ^
[warn] /home/cass/spark2/spark/examples/src/main/java/org/apache/spark/examples/streaming/JavaRecoverableNetworkWordCount.java:70: warning: [deprecation] Accumulator in org.apache.spark has been deprecated
[warn]   private static volatile Accumulator<Integer> instance = null;
[warn]                           ^
[warn] /home/cass/spark2/spark/examples/src/main/java/org/apache/spark/examples/streaming/JavaRecoverableNetworkWordCount.java:72: warning: [deprecation] Accumulator in org.apache.spark has been deprecated
[warn]   public static Accumulator<Integer> getInstance(JavaSparkContext jsc) {
[warn]                 ^
[warn] /home/cass/spark2/spark/examples/src/main/java/org/apache/spark/examples/streaming/JavaRecoverableNetworkWordCount.java:161: warning: [deprecation] Accumulator in org.apache.spark has been deprecated
[warn]         final Accumulator<Integer> droppedWordsCounter =
[warn]               ^
[warn] 13 warnings
[info] Compile success at May 20, 2016 12:37:18 PM [11.060s]
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:compile (default-compile) @ spark-examples_2.11 ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 110 source files to /home/cass/spark2/spark/examples/target/scala-2.11/classes
[WARNING] /home/cass/spark2/spark/examples/src/main/java/org/apache/spark/examples/mllib/JavaRegressionMetricsExample.java:[28,40] [deprecation] LinearRegressionWithSGD in org.apache.spark.mllib.regression has been deprecated
[WARNING] /home/cass/spark2/spark/examples/src/main/java/org/apache/spark/examples/streaming/JavaRecoverableNetworkWordCount.java:[32,23] [deprecation] Accumulator in org.apache.spark has been deprecated
[WARNING] /home/cass/spark2/spark/examples/src/main/java/org/apache/spark/examples/mllib/JavaLinearRegressionWithSGDExample.java:[32,40] [deprecation] LinearRegressionWithSGD in org.apache.spark.mllib.regression has been deprecated
[WARNING] /home/cass/spark2/spark/examples/src/main/java/org/apache/spark/examples/mllib/JavaLogisticRegressionWithLBFGSExample.java:[68,30] [deprecation] precision() in MulticlassMetrics has been deprecated
[WARNING] /home/cass/spark2/spark/examples/src/main/java/org/apache/spark/examples/mllib/JavaRegressionMetricsExample.java:[57,40] [deprecation] LinearRegressionWithSGD in org.apache.spark.mllib.regression has been deprecated
[WARNING] /home/cass/spark2/spark/examples/src/main/java/org/apache/spark/examples/streaming/JavaRecoverableNetworkWordCount.java:[70,26] [deprecation] Accumulator in org.apache.spark has been deprecated
[WARNING] /home/cass/spark2/spark/examples/src/main/java/org/apache/spark/examples/streaming/JavaRecoverableNetworkWordCount.java:[72,16] [deprecation] Accumulator in org.apache.spark has been deprecated
[WARNING] /home/cass/spark2/spark/examples/src/main/java/org/apache/spark/examples/streaming/JavaRecoverableNetworkWordCount.java:[161,14] [deprecation] Accumulator in org.apache.spark has been deprecated
[WARNING] /home/cass/spark2/spark/examples/src/main/java/org/apache/spark/examples/mllib/JavaMulticlassClassificationMetricsExample.java:[71,47] [deprecation] precision() in MulticlassMetrics has been deprecated
[WARNING] /home/cass/spark2/spark/examples/src/main/java/org/apache/spark/examples/mllib/JavaMulticlassClassificationMetricsExample.java:[72,44] [deprecation] recall() in MulticlassMetrics has been deprecated
[WARNING] /home/cass/spark2/spark/examples/src/main/java/org/apache/spark/examples/mllib/JavaMulticlassClassificationMetricsExample.java:[73,46] [deprecation] fMeasure() in MulticlassMetrics has been deprecated
[WARNING] /home/cass/spark2/spark/examples/src/main/java/org/apache/spark/examples/mllib/JavaLinearRegressionWithSGDExample.java:[66,6] [deprecation] LinearRegressionWithSGD in org.apache.spark.mllib.regression has been deprecated
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (create-tmp-dir) @ spark-examples_2.11 ---
[INFO] Executing tasks

main:
    [mkdir] Created dir: /home/cass/spark2/spark/examples/target/tmp
[INFO] Executed tasks
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ spark-examples_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/examples/src/test/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:testCompile (scala-test-compile-first) @ spark-examples_2.11 ---
[INFO] No sources to compile
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:testCompile (default-testCompile) @ spark-examples_2.11 ---
[INFO] No sources to compile
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (generate-test-classpath) @ spark-examples_2.11 ---
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (default-test) @ spark-examples_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (test) @ spark-examples_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- scalatest-maven-plugin:1.0:test (test) @ spark-examples_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-jar-plugin:2.6:jar (default-jar) @ spark-examples_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/examples/target/scala-2.11/jars/spark-examples_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-site-plugin:3.3:attach-descriptor (attach-descriptor) @ spark-examples_2.11 ---
[INFO]
[INFO] --- maven-dependency-plugin:2.10:copy-dependencies (copy-module-dependencies) @ spark-examples_2.11 ---
[INFO] Copying scopt_2.11-3.3.0.jar to /home/cass/spark2/spark/examples/target/scala-2.11/jars/scopt_2.11-3.3.0.jar
[INFO]
[INFO] --- maven-shade-plugin:2.4.3:shade (default) @ spark-examples_2.11 ---
[INFO] Excluding com.github.scopt:scopt_2.11:jar:3.3.0 from the shaded jar.
[INFO] Replacing original artifact with shaded artifact.
[INFO] Replacing /home/cass/spark2/spark/examples/target/scala-2.11/jars/spark-examples_2.11-2.0.0-SNAPSHOT.jar with /home/cass/spark2/spark/examples/target/spark-examples_2.11-2.0.0-SNAPSHOT-shaded.jar
[INFO]
[INFO] --- maven-source-plugin:2.4:jar-no-fork (create-source-jar) @ spark-examples_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/examples/target/spark-examples_2.11-2.0.0-SNAPSHOT-sources.jar
[INFO]
[INFO] --- maven-source-plugin:2.4:test-jar-no-fork (create-source-jar) @ spark-examples_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/examples/target/spark-examples_2.11-2.0.0-SNAPSHOT-test-sources.jar
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Spark Project External Kafka Assembly 2.0.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.0.0:clean (default-clean) @ spark-streaming-kafka-0-8-assembly_2.11 ---
[INFO]
[INFO] --- maven-enforcer-plugin:1.4.1:enforce (enforce-versions) @ spark-streaming-kafka-0-8-assembly_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:add-source (eclipse-add-source) @ spark-streaming-kafka-0-8-assembly_2.11 ---
[INFO] Add Source directory: /home/cass/spark2/spark/external/kafka-0-8-assembly/src/main/scala
[INFO] Add Test Source directory: /home/cass/spark2/spark/external/kafka-0-8-assembly/src/test/scala
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (default-cli) @ spark-streaming-kafka-0-8-assembly_2.11 ---
[INFO] Dependencies classpath:
/home/cass/spark2/spark/external/kafka-0-8/target/spark-streaming-kafka-0-8_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/javax/inject/javax.inject/1/javax.inject-1.jar:/home/cass/.m2/repository/org/spark-project/spark/unused/1.0.0/unused-1.0.0.jar:/home/cass/.m2/repository/com/thoughtworks/paranamer/paranamer/2.6/paranamer-2.6.jar:/home/cass/.m2/repository/com/google/inject/guice/3.0/guice-3.0.jar:/home/cass/.m2/repository/org/apache/avro/avro-ipc/1.7.7/avro-ipc-1.7.7.jar:/home/cass/.m2/repository/commons-io/commons-io/2.4/commons-io-2.4.jar:/home/cass/.m2/repository/org/apache/kafka/kafka-clients/0.8.2.1/kafka-clients-0.8.2.1.jar:/home/cass/.m2/repository/aopalliance/aopalliance/1.0/aopalliance-1.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-api/2.2.0/hadoop-yarn-api-2.2.0.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-mapper-asl/1.9.13/jackson-mapper-asl-1.9.13.jar:/home/cass/.m2/repository/org/apache/kafka/kafka_2.11/0.8.2.1/kafka_2.11-0.8.2.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-common/2.2.0/hadoop-yarn-common-2.2.0.jar:/home/cass/.m2/repository/org/apache/avro/avro/1.7.7/avro-1.7.7.jar:/home/cass/.m2/repository/org/apache/commons/commons-compress/1.4.1/commons-compress-1.4.1.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-xml_2.11/1.0.2/scala-xml_2.11-1.0.2.jar:/home/cass/.m2/repository/com/101tec/zkclient/0.3/zkclient-0.3.jar:/home/cass/.m2/repository/com/yammer/metrics/metrics-core/2.2.0/metrics-core-2.2.0.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-parser-combinators_2.11/1.0.2/scala-parser-combinators_2.11-1.0.2.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-core-asl/1.9.13/jackson-core-asl-1.9.13.jar:/home/cass/.m2/repository/org/tukaani/xz/1.0/xz-1.0.jar:/home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-client/2.2.0/hadoop-yarn-client-2.2.0.jar
[INFO]
[INFO] --- maven-remote-resources-plugin:1.5:process (default) @ spark-streaming-kafka-0-8-assembly_2.11 ---
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ spark-streaming-kafka-0-8-assembly_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/external/kafka-0-8-assembly/src/main/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:compile (scala-compile-first) @ spark-streaming-kafka-0-8-assembly_2.11 ---
[INFO] No sources to compile
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:compile (default-compile) @ spark-streaming-kafka-0-8-assembly_2.11 ---
[INFO] No sources to compile
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (create-tmp-dir) @ spark-streaming-kafka-0-8-assembly_2.11 ---
[INFO] Executing tasks

main:
    [mkdir] Created dir: /home/cass/spark2/spark/external/kafka-0-8-assembly/target/tmp
[INFO] Executed tasks
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ spark-streaming-kafka-0-8-assembly_2.11 ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] skip non existing resourceDirectory /home/cass/spark2/spark/external/kafka-0-8-assembly/src/test/resources
[INFO] Copying 3 resources
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:testCompile (scala-test-compile-first) @ spark-streaming-kafka-0-8-assembly_2.11 ---
[INFO] No sources to compile
[INFO]
[INFO] --- maven-compiler-plugin:3.5.1:testCompile (default-testCompile) @ spark-streaming-kafka-0-8-assembly_2.11 ---
[INFO] No sources to compile
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (generate-test-classpath) @ spark-streaming-kafka-0-8-assembly_2.11 ---
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (default-test) @ spark-streaming-kafka-0-8-assembly_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (test) @ spark-streaming-kafka-0-8-assembly_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- scalatest-maven-plugin:1.0:test (test) @ spark-streaming-kafka-0-8-assembly_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (prepare-test-jar) @ spark-streaming-kafka-0-8-assembly_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/external/kafka-0-8-assembly/target/spark-streaming-kafka-0-8-assembly_2.11-2.0.0-SNAPSHOT-tests.jar
[INFO]
[INFO] --- maven-jar-plugin:2.6:jar (default-jar) @ spark-streaming-kafka-0-8-assembly_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/external/kafka-0-8-assembly/target/spark-streaming-kafka-0-8-assembly_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-site-plugin:3.3:attach-descriptor (attach-descriptor) @ spark-streaming-kafka-0-8-assembly_2.11 ---
[INFO]
[INFO] --- maven-shade-plugin:2.4.3:shade (default) @ spark-streaming-kafka-0-8-assembly_2.11 ---
[INFO] Including org.apache.spark:spark-streaming-kafka-0-8_2.11:jar:2.0.0-SNAPSHOT in the shaded jar.
[INFO] Including org.apache.kafka:kafka_2.11:jar:0.8.2.1 in the shaded jar.
[INFO] Including com.yammer.metrics:metrics-core:jar:2.2.0 in the shaded jar.
[INFO] Including org.scala-lang.modules:scala-parser-combinators_2.11:jar:1.0.2 in the shaded jar.
[INFO] Including com.101tec:zkclient:jar:0.3 in the shaded jar.
[INFO] Including org.apache.kafka:kafka-clients:jar:0.8.2.1 in the shaded jar.
[INFO] Including org.apache.spark:spark-tags_2.11:jar:2.0.0-SNAPSHOT in the shaded jar.
[INFO] Including com.thoughtworks.paranamer:paranamer:jar:2.6 in the shaded jar.
[INFO] Including commons-io:commons-io:jar:2.4 in the shaded jar.
[INFO] Including org.apache.avro:avro:jar:1.7.7 in the shaded jar.
[INFO] Including org.apache.commons:commons-compress:jar:1.4.1 in the shaded jar.
[INFO] Including org.tukaani:xz:jar:1.0 in the shaded jar.
[INFO] Including org.apache.hadoop:hadoop-yarn-client:jar:2.2.0 in the shaded jar.
[INFO] Including com.google.inject:guice:jar:3.0 in the shaded jar.
[INFO] Including javax.inject:javax.inject:jar:1 in the shaded jar.
[INFO] Including aopalliance:aopalliance:jar:1.0 in the shaded jar.
[INFO] Including org.apache.hadoop:hadoop-yarn-api:jar:2.2.0 in the shaded jar.
[INFO] Including org.apache.hadoop:hadoop-yarn-common:jar:2.2.0 in the shaded jar.
[INFO] Including org.apache.avro:avro-ipc:jar:1.7.7 in the shaded jar.
[INFO] Including org.codehaus.jackson:jackson-core-asl:jar:1.9.13 in the shaded jar.
[INFO] Including org.codehaus.jackson:jackson-mapper-asl:jar:1.9.13 in the shaded jar.
[INFO] Including org.spark-project.spark:unused:jar:1.0.0 in the shaded jar.
[INFO] Including org.scala-lang.modules:scala-xml_2.11:jar:1.0.2 in the shaded jar.
[WARNING] hadoop-yarn-common-2.2.0.jar, hadoop-yarn-api-2.2.0.jar define 3 overlapping classes:
[WARNING]   - org.apache.hadoop.yarn.util.package-info
[WARNING]   - org.apache.hadoop.yarn.factories.package-info
[WARNING]   - org.apache.hadoop.yarn.factory.providers.package-info
[WARNING] unused-1.0.0.jar, spark-tags_2.11-2.0.0-SNAPSHOT.jar, spark-streaming-kafka-0-8_2.11-2.0.0-SNAPSHOT.jar define 1 overlapping classes:
[WARNING]   - org.apache.spark.unused.UnusedStubClass
[WARNING] maven-shade-plugin has detected that some class files are
[WARNING] present in two or more JARs. When this happens, only one
[WARNING] single version of the class is copied to the uber jar.
[WARNING] Usually this is not harmful and you can skip these warnings,
[WARNING] otherwise try to manually exclude artifacts based on
[WARNING] mvn dependency:tree -Ddetail=true and the above output.
[WARNING] See http://maven.apache.org/plugins/maven-shade-plugin/
[INFO] Replacing original artifact with shaded artifact.
[INFO] Replacing /home/cass/spark2/spark/external/kafka-0-8-assembly/target/spark-streaming-kafka-0-8-assembly_2.11-2.0.0-SNAPSHOT.jar with /home/cass/spark2/spark/external/kafka-0-8-assembly/target/spark-streaming-kafka-0-8-assembly_2.11-2.0.0-SNAPSHOT-shaded.jar
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/external/kafka-0-8-assembly/dependency-reduced-pom.xml
[INFO] Dependency-reduced POM written at: /home/cass/spark2/spark/external/kafka-0-8-assembly/dependency-reduced-pom.xml
[INFO]
[INFO] --- maven-source-plugin:2.4:jar-no-fork (create-source-jar) @ spark-streaming-kafka-0-8-assembly_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/external/kafka-0-8-assembly/target/spark-streaming-kafka-0-8-assembly_2.11-2.0.0-SNAPSHOT-sources.jar
[INFO]
[INFO] --- maven-source-plugin:2.4:test-jar-no-fork (create-source-jar) @ spark-streaming-kafka-0-8-assembly_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/external/kafka-0-8-assembly/target/spark-streaming-kafka-0-8-assembly_2.11-2.0.0-SNAPSHOT-test-sources.jar
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Spark Project Java 8 Tests 2.0.0-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-clean-plugin:3.0.0:clean (default-clean) @ java8-tests_2.11 ---
[INFO]
[INFO] --- maven-enforcer-plugin:1.4.1:enforce (enforce-versions) @ java8-tests_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:add-source (eclipse-add-source) @ java8-tests_2.11 ---
[INFO] Add Source directory: /home/cass/spark2/spark/external/java8-tests/src/main/scala
[INFO] Add Test Source directory: /home/cass/spark2/spark/external/java8-tests/src/test/scala
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (default-cli) @ java8-tests_2.11 ---
[INFO] Dependencies classpath:
/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-jobclient/2.2.0/hadoop-mapreduce-client-jobclient-2.2.0.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-jackson/1.7.0/parquet-jackson-1.7.0.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-core/3.1.2/metrics-core-3.1.2.jar:/home/cass/.m2/repository/com/google/protobuf/protobuf-java/2.5.0/protobuf-java-2.5.0.jar:/home/cass/.m2/repository/aopalliance/aopalliance/1.0/aopalliance-1.0.jar:/home/cass/.m2/repository/net/razorvine/pyrolite/4.9/pyrolite-4.9.jar:/home/cass/.m2/repository/com/univocity/univocity-parsers/2.1.0/univocity-parsers-2.1.0.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-jvm/3.1.2/metrics-jvm-3.1.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-client/2.2.0/hadoop-client-2.2.0.jar:/home/cass/.m2/repository/org/fusesource/leveldbjni/leveldbjni-all/1.8/leveldbjni-all-1.8.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-format/2.3.0-incubating/parquet-format-2.3.0-incubating.jar:/home/cass/.m2/repository/org/glassfish/jersey/bundles/repackaged/jersey-guava/2.22.2/jersey-guava-2.22.2.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-json/3.1.2/metrics-json-3.1.2.jar:/home/cass/.m2/repository/net/java/dev/jets3t/jets3t/0.7.1/jets3t-0.7.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-common/2.2.0/hadoop-common-2.2.0.jar:/home/cass/.m2/repository/com/google/inject/guice/3.0/guice-3.0.jar:/home/cass/.m2/repository/commons-io/commons-io/2.4/commons-io-2.4.jar:/home/cass/spark2/spark/sql/core/target/spark-sql_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/scala-lang/scala-reflect/2.11.8/scala-reflect-2.11.8.jar:/home/cass/.m2/repository/org/xerial/snappy/snappy-java/1.1.2.4/snappy-java-1.1.2.4.jar:/home/cass/.m2/repository/org/json4s/json4s-jackson_2.11/3.2.11/json4s-jackson_2.11-3.2.11.jar:/home/cass/.m2/repository/com/esotericsoftware/minlog/1.3.0/minlog-1.3.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-auth/2.2.0/hadoop-auth-2.2.0.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-core-asl/1.9.13/jackson-core-asl-1.9.13.jar:/home/cass/.m2/repository/javax/validation/validation-api/1.1.0.Final/validation-api-1.1.0.Final.jar:/home/cass/.m2/repository/net/jpountz/lz4/lz4/1.3.0/lz4-1.3.0.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-common/2.22.2/jersey-common-2.22.2.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-client/2.2.0/hadoop-yarn-client-2.2.0.jar:/home/cass/.m2/repository/io/netty/netty/3.8.0.Final/netty-3.8.0.Final.jar:/home/cass/.m2/repository/org/apache/mesos/mesos/0.21.1/mesos-0.21.1-shaded-protobuf.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-annotations/2.5.3/jackson-annotations-2.5.3.jar:/home/cass/.m2/repository/com/google/code/findbugs/jsr305/1.3.9/jsr305-1.3.9.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-api/2.4.0-b34/hk2-api-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-server/2.22.2/jersey-server-2.22.2.jar:/home/cass/.m2/repository/net/sf/py4j/py4j/0.10.1/py4j-0.10.1.jar:/home/cass/.m2/repository/com/twitter/chill-java/0.8.0/chill-java-0.8.0.jar:/home/cass/.m2/repository/commons-lang/commons-lang/2.6/commons-lang-2.6.jar:/home/cass/.m2/repository/org/tukaani/xz/1.0/xz-1.0.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-databind/2.5.3/jackson-databind-2.5.3.jar:/home/cass/.m2/repository/org/codehaus/janino/janino/2.7.8/janino-2.7.8.jar:/home/cass/.m2/repository/commons-codec/commons-codec/1.10/commons-codec-1.10.jar:/home/cass/.m2/repository/org/apache/curator/curator-recipes/2.4.0/curator-recipes-2.4.0.jar:/home/cass/.m2/repository/org/javassist/javassist/3.18.1-GA/javassist-3.18.1-GA.jar:/home/cass/.m2/repository/org/apache/ivy/ivy/2.4.0/ivy-2.4.0.jar:/home/cass/.m2/repository/javax/inject/javax.inject/1/javax.inject-1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-core/2.2.0/hadoop-mapreduce-client-core-2.2.0.jar:/home/cass/.m2/repository/com/fasterxml/jackson/module/jackson-module-scala_2.11/2.5.3/jackson-module-scala_2.11-2.5.3.jar:/home/cass/.m2/repository/commons-beanutils/commons-beanutils-core/1.8.0/commons-beanutils-core-1.8.0.jar:/home/cass/.m2/repository/javax/servlet/javax.servlet-api/3.1.0/javax.servlet-api-3.1.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/osgi-resource-locator/1.0.1/osgi-resource-locator-1.0.1.jar:/home/cass/.m2/repository/org/apache/commons/commons-math3/3.4.1/commons-math3-3.4.1.jar:/home/cass/spark2/spark/common/network-common/target/spark-network-common_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/avro/avro/1.7.7/avro-1.7.7.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-common/2.2.0/hadoop-mapreduce-client-common-2.2.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-utils/2.4.0-b34/hk2-utils-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/hk2/external/aopalliance-repackaged/2.4.0-b34/aopalliance-repackaged-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/hk2/external/javax.inject/2.4.0-b34/javax.inject-2.4.0-b34.jar:/home/cass/.m2/repository/org/glassfish/jersey/containers/jersey-container-servlet-core/2.22.2/jersey-container-servlet-core-2.22.2.jar:/home/cass/.m2/repository/oro/oro/2.0.8/oro-2.0.8.jar:/home/cass/.m2/repository/org/scala-lang/scala-compiler/2.11.8/scala-compiler-2.11.8.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-encoding/1.7.0/parquet-encoding-1.7.0.jar:/home/cass/.m2/repository/org/roaringbitmap/RoaringBitmap/0.5.11/RoaringBitmap-0.5.11.jar:/home/cass/.m2/repository/log4j/log4j/1.2.17/log4j-1.2.17.jar:/home/cass/.m2/repository/org/scala-lang/scala-library/2.11.8/scala-library-2.11.8.jar:/home/cass/.m2/repository/org/codehaus/janino/commons-compiler/2.7.8/commons-compiler-2.7.8.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-hadoop/1.7.0/parquet-hadoop-1.7.0.jar:/home/cass/.m2/repository/org/apache/curator/curator-client/2.4.0/curator-client-2.4.0.jar:/home/cass/.m2/repository/org/apache/commons/commons-compress/1.4.1/commons-compress-1.4.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-app/2.2.0/hadoop-mapreduce-client-app-2.2.0.jar:/home/cass/.m2/repository/org/slf4j/slf4j-api/1.7.16/slf4j-api-1.7.16.jar:/home/cass/.m2/repository/org/apache/xbean/xbean-asm5-shaded/4.4/xbean-asm5-shaded-4.4.jar:/home/cass/.m2/repository/org/json4s/json4s-core_2.11/3.2.11/json4s-core_2.11-3.2.11.jar:/home/cass/.m2/repository/org/mortbay/jetty/jetty-util/6.1.26/jetty-util-6.1.26.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-server-common/2.2.0/hadoop-yarn-server-common-2.2.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-hdfs/2.2.0/hadoop-hdfs-2.2.0.jar:/home/cass/.m2/repository/org/codehaus/jackson/jackson-mapper-asl/1.9.13/jackson-mapper-asl-1.9.13.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-api/2.2.0/hadoop-yarn-api-2.2.0.jar:/home/cass/.m2/repository/com/esotericsoftware/kryo-shaded/3.0.3/kryo-shaded-3.0.3.jar:/home/cass/.m2/repository/javax/ws/rs/javax.ws.rs-api/2.0.1/javax.ws.rs-api-2.0.1.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-yarn-common/2.2.0/hadoop-yarn-common-2.2.0.jar:/home/cass/.m2/repository/org/glassfish/jersey/core/jersey-client/2.22.2/jersey-client-2.22.2.jar:/home/cass/spark2/spark/common/unsafe/target/spark-unsafe_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/avro/avro-mapred/1.7.7/avro-mapred-1.7.7-hadoop2.jar:/home/cass/spark2/spark/sql/catalyst/target/spark-catalyst_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-column/1.7.0/parquet-column-1.7.0.jar:/home/cass/.m2/repository/xmlenc/xmlenc/0.52/xmlenc-0.52.jar:/home/cass/.m2/repository/com/ning/compress-lzf/1.0.3/compress-lzf-1.0.3.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-mapreduce-client-shuffle/2.2.0/hadoop-mapreduce-client-shuffle-2.2.0.jar:/home/cass/.m2/repository/org/apache/zookeeper/zookeeper/3.4.5/zookeeper-3.4.5.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-common/1.7.0/parquet-common-1.7.0.jar:/home/cass/.m2/repository/org/apache/curator/curator-framework/2.4.0/curator-framework-2.4.0.jar:/home/cass/.m2/repository/commons-net/commons-net/2.2/commons-net-2.2.jar:/home/cass/.m2/repository/org/apache/commons/commons-lang3/3.3.2/commons-lang3-3.3.2.jar:/home/cass/.m2/repository/org/json4s/json4s-ast_2.11/3.2.11/json4s-ast_2.11-3.2.11.jar:/home/cass/spark2/spark/launcher/target/spark-launcher_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/scala-lang/scalap/2.11.8/scalap-2.11.8.jar:/home/cass/.m2/repository/com/clearspring/analytics/stream/2.7.0/stream-2.7.0.jar:/home/cass/.m2/repository/org/apache/commons/commons-math/2.1/commons-math-2.1.jar:/home/cass/.m2/repository/org/apache/parquet/parquet-generator/1.7.0/parquet-generator-1.7.0.jar:/home/cass/.m2/repository/org/apache/hadoop/hadoop-annotations/2.2.0/hadoop-annotations-2.2.0.jar:/home/cass/.m2/repository/com/thoughtworks/paranamer/paranamer/2.6/paranamer-2.6.jar:/home/cass/.m2/repository/commons-configuration/commons-configuration/1.6/commons-configuration-1.6.jar:/home/cass/.m2/repository/org/glassfish/jersey/containers/jersey-container-servlet/2.22.2/jersey-container-servlet-2.22.2.jar:/home/cass/.m2/repository/commons-digester/commons-digester/1.8/commons-digester-1.8.jar:/home/cass/.m2/repository/org/slf4j/jul-to-slf4j/1.7.16/jul-to-slf4j-1.7.16.jar:/home/cass/.m2/repository/commons-beanutils/commons-beanutils/1.7.0/commons-beanutils-1.7.0.jar:/home/cass/.m2/repository/org/antlr/antlr4-runtime/4.5.2-1/antlr4-runtime-4.5.2-1.jar:/home/cass/spark2/spark/common/network-shuffle/target/spark-network-shuffle_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-xml_2.11/1.0.2/scala-xml_2.11-1.0.2.jar:/home/cass/.m2/repository/org/scala-lang/modules/scala-parser-combinators_2.11/1.0.4/scala-parser-combinators_2.11-1.0.4.jar:/home/cass/.m2/repository/commons-cli/commons-cli/1.2/commons-cli-1.2.jar:/home/cass/.m2/repository/io/dropwizard/metrics/metrics-graphite/3.1.2/metrics-graphite-3.1.2.jar:/home/cass/.m2/repository/org/objenesis/objenesis/2.1/objenesis-2.1.jar:/home/cass/.m2/repository/javax/annotation/javax.annotation-api/1.2/javax.annotation-api-1.2.jar:/home/cass/.m2/repository/org/slf4j/slf4j-log4j12/1.7.16/slf4j-log4j12-1.7.16.jar:/home/cass/spark2/spark/common/sketch/target/spark-sketch_2.11-2.0.0-SNAPSHOT.jar:/home/cass/spark2/spark/core/target/spark-core_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/glassfish/jersey/media/jersey-media-jaxb/2.22.2/jersey-media-jaxb-2.22.2.jar:/home/cass/.m2/repository/com/fasterxml/jackson/core/jackson-core/2.5.3/jackson-core-2.5.3.jar:/home/cass/spark2/spark/streaming/target/spark-streaming_2.11-2.0.0-SNAPSHOT.jar:/home/cass/.m2/repository/org/spark-project/spark/unused/1.0.0/unused-1.0.0.jar:/home/cass/.m2/repository/org/apache/avro/avro-ipc/1.7.7/avro-ipc-1.7.7.jar:/home/cass/.m2/repository/commons-collections/commons-collections/3.2.2/commons-collections-3.2.2.jar:/home/cass/.m2/repository/com/twitter/chill_2.11/0.8.0/chill_2.11-0.8.0.jar:/home/cass/.m2/repository/org/glassfish/hk2/hk2-locator/2.4.0-b34/hk2-locator-2.4.0-b34.jar:/home/cass/.m2/repository/org/slf4j/jcl-over-slf4j/1.7.16/jcl-over-slf4j-1.7.16.jar:/home/cass/.m2/repository/commons-httpclient/commons-httpclient/3.1/commons-httpclient-3.1.jar:/home/cass/.m2/repository/io/netty/netty-all/4.0.29.Final/netty-all-4.0.29.Final.jar:/home/cass/spark2/spark/common/tags/target/spark-tags_2.11-2.0.0-SNAPSHOT.jar
[INFO]
[INFO] --- maven-remote-resources-plugin:1.5:process (default) @ java8-tests_2.11 ---
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:compile (scala-compile-first) @ java8-tests_2.11 ---
[INFO] No sources to compile
[INFO]
[INFO] --- maven-antrun-plugin:1.8:run (create-tmp-dir) @ java8-tests_2.11 ---
[INFO] Executing tasks

main:
    [mkdir] Created dir: /home/cass/spark2/spark/external/java8-tests/target/tmp
[INFO] Executed tasks
[INFO]
[INFO] --- scala-maven-plugin:3.2.2:testCompile (scala-test-compile-first) @ java8-tests_2.11 ---
[INFO] Using zinc server for incremental compilation
[warn] Pruning sources from previous analysis, due to incompatible CompileSetup.
[info] Compiling 1 Scala source and 3 Java sources to /home/cass/spark2/spark/external/java8-tests/target/test-classes...
[warn] /home/cass/spark2/spark/external/java8-tests/src/test/java/org/apache/spark/streaming/Java8APISuite.java:30: warning: [deprecation] Accumulator in org.apache.spark has been deprecated
[warn] import org.apache.spark.Accumulator;
[warn]                        ^
[warn] /home/cass/spark2/spark/external/java8-tests/src/test/java/org/apache/spark/Java8APISuite.java:307: warning: [deprecation] Accumulator in org.apache.spark has been deprecated
[warn]     Accumulator<Integer> intAccum = sc.intAccumulator(10);
[warn]     ^
[warn] /home/cass/spark2/spark/external/java8-tests/src/test/java/org/apache/spark/Java8APISuite.java:311: warning: [deprecation] Accumulator in org.apache.spark has been deprecated
[warn]     Accumulator<Double> doubleAccum = sc.doubleAccumulator(10.0);
[warn]     ^
[warn] /home/cass/spark2/spark/external/java8-tests/src/test/java/org/apache/spark/Java8APISuite.java:316: warning: [deprecation] AccumulatorParam in org.apache.spark has been deprecated
[warn]     AccumulatorParam<Float> floatAccumulatorParam = new AccumulatorParam<Float>() {
[warn]     ^
[warn] /home/cass/spark2/spark/external/java8-tests/src/test/java/org/apache/spark/Java8APISuite.java:316: warning: [deprecation] AccumulatorParam in org.apache.spark has been deprecated
[warn]     AccumulatorParam<Float> floatAccumulatorParam = new AccumulatorParam<Float>() {
[warn]                                                         ^
[warn] /home/cass/spark2/spark/external/java8-tests/src/test/java/org/apache/spark/Java8APISuite.java:331: warning: [deprecation] Accumulator in org.apache.spark has been deprecated
[warn]     Accumulator<Float> floatAccum = sc.accumulator(10.0f, floatAccumulatorParam);
[warn]     ^
[warn] /home/cass/spark2/spark/external/java8-tests/src/test/java/org/apache/spark/streaming/Java8APISuite.java:365: warning: [deprecation] Accumulator in org.apache.spark has been deprecated
[warn]     final Accumulator<Integer> accumRdd = ssc.sparkContext().accumulator(0);
[warn]           ^
[warn] /home/cass/spark2/spark/external/java8-tests/src/test/java/org/apache/spark/streaming/Java8APISuite.java:366: warning: [deprecation] Accumulator in org.apache.spark has been deprecated
[warn]     final Accumulator<Integer> accumEle = ssc.sparkContext().accumulator(0);
[warn]           ^
[warn] 8 warnings
[info] Compile success at May 20, 2016 12:37:29 PM [3.919s]
[INFO]
[INFO] --- maven-dependency-plugin:2.10:build-classpath (generate-test-classpath) @ java8-tests_2.11 ---
[INFO]
[INFO] --- maven-surefire-plugin:2.19.1:test (test) @ java8-tests_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- scalatest-maven-plugin:1.0:test (test) @ java8-tests_2.11 ---
[INFO] Tests are skipped.
[INFO]
[INFO] --- maven-jar-plugin:2.6:test-jar (prepare-test-jar) @ java8-tests_2.11 ---
[INFO] Building jar: /home/cass/spark2/spark/external/java8-tests/target/java8-tests_2.11-2.0.0-SNAPSHOT-tests.jar
[INFO]
[INFO] --- maven-site-plugin:3.3:attach-descriptor (attach-descriptor) @ java8-tests_2.11 ---
[INFO]
[INFO] --- maven-shade-plugin:2.4.3:shade (default) @ java8-tests_2.11 ---
[INFO] Excluding org.apache.spark:spark-core_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.avro:avro-mapred:jar:hadoop2:1.7.7 from the shaded jar.
[INFO] Excluding org.apache.avro:avro-ipc:jar:1.7.7 from the shaded jar.
[INFO] Excluding org.apache.avro:avro:jar:1.7.7 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-core-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding org.codehaus.jackson:jackson-mapper-asl:jar:1.9.13 from the shaded jar.
[INFO] Excluding com.twitter:chill_2.11:jar:0.8.0 from the shaded jar.
[INFO] Excluding com.esotericsoftware:kryo-shaded:jar:3.0.3 from the shaded jar.
[INFO] Excluding com.esotericsoftware:minlog:jar:1.3.0 from the shaded jar.
[INFO] Excluding org.objenesis:objenesis:jar:2.1 from the shaded jar.
[INFO] Excluding com.twitter:chill-java:jar:0.8.0 from the shaded jar.
[INFO] Excluding org.apache.xbean:xbean-asm5-shaded:jar:4.4 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding commons-cli:commons-cli:jar:1.2 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-math:jar:2.1 from the shaded jar.
[INFO] Excluding xmlenc:xmlenc:jar:0.52 from the shaded jar.
[INFO] Excluding commons-io:commons-io:jar:2.4 from the shaded jar.
[INFO] Excluding commons-lang:commons-lang:jar:2.6 from the shaded jar.
[INFO] Excluding commons-configuration:commons-configuration:jar:1.6 from the shaded jar.
[INFO] Excluding commons-collections:commons-collections:jar:3.2.2 from the shaded jar.
[INFO] Excluding commons-digester:commons-digester:jar:1.8 from the shaded jar.
[INFO] Excluding commons-beanutils:commons-beanutils:jar:1.7.0 from the shaded jar.
[INFO] Excluding commons-beanutils:commons-beanutils-core:jar:1.8.0 from the shaded jar.
[INFO] Excluding com.google.protobuf:protobuf-java:jar:2.5.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-auth:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-compress:jar:1.4.1 from the shaded jar.
[INFO] Excluding org.tukaani:xz:jar:1.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-hdfs:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.mortbay.jetty:jetty-util:jar:6.1.26 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-app:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-client:jar:2.2.0 from the shaded jar.
[INFO] Excluding com.google.inject:guice:jar:3.0 from the shaded jar.
[INFO] Excluding javax.inject:javax.inject:jar:1 from the shaded jar.
[INFO] Excluding aopalliance:aopalliance:jar:1.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-server-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-shuffle:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-api:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-core:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-yarn-common:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-mapreduce-client-jobclient:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.hadoop:hadoop-annotations:jar:2.2.0 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-launcher_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-network-common_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-network-shuffle_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.fusesource.leveldbjni:leveldbjni-all:jar:1.8 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-annotations:jar:2.5.3 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-unsafe_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding net.java.dev.jets3t:jets3t:jar:0.7.1 from the shaded jar.
[INFO] Excluding commons-codec:commons-codec:jar:1.10 from the shaded jar.
[INFO] Excluding commons-httpclient:commons-httpclient:jar:3.1 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-recipes:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-framework:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.curator:curator-client:jar:2.4.0 from the shaded jar.
[INFO] Excluding org.apache.zookeeper:zookeeper:jar:3.4.5 from the shaded jar.
[INFO] Excluding javax.servlet:javax.servlet-api:jar:3.1.0 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-lang3:jar:3.3.2 from the shaded jar.
[INFO] Excluding org.apache.commons:commons-math3:jar:3.4.1 from the shaded jar.
[INFO] Excluding com.google.code.findbugs:jsr305:jar:1.3.9 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-api:jar:1.7.16 from the shaded jar.
[INFO] Excluding org.slf4j:jul-to-slf4j:jar:1.7.16 from the shaded jar.
[INFO] Excluding org.slf4j:jcl-over-slf4j:jar:1.7.16 from the shaded jar.
[INFO] Excluding log4j:log4j:jar:1.2.17 from the shaded jar.
[INFO] Excluding org.slf4j:slf4j-log4j12:jar:1.7.16 from the shaded jar.
[INFO] Excluding com.ning:compress-lzf:jar:1.0.3 from the shaded jar.
[INFO] Excluding org.xerial.snappy:snappy-java:jar:1.1.2.4 from the shaded jar.
[INFO] Excluding net.jpountz.lz4:lz4:jar:1.3.0 from the shaded jar.
[INFO] Excluding org.roaringbitmap:RoaringBitmap:jar:0.5.11 from the shaded jar.
[INFO] Excluding commons-net:commons-net:jar:2.2 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-library:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.json4s:json4s-jackson_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.json4s:json4s-core_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.json4s:json4s-ast_2.11:jar:3.2.11 from the shaded jar.
[INFO] Excluding org.scala-lang:scalap:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang:scala-compiler:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-parser-combinators_2.11:jar:1.0.4 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-client:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.ws.rs:javax.ws.rs-api:jar:2.0.1 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-api:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-utils:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2.external:aopalliance-repackaged:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2.external:javax.inject:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:hk2-locator:jar:2.4.0-b34 from the shaded jar.
[INFO] Excluding org.javassist:javassist:jar:3.18.1-GA from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-common:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.annotation:javax.annotation-api:jar:1.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.bundles.repackaged:jersey-guava:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.hk2:osgi-resource-locator:jar:1.0.1 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.core:jersey-server:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.media:jersey-media-jaxb:jar:2.22.2 from the shaded jar.
[INFO] Excluding javax.validation:validation-api:jar:1.1.0.Final from the shaded jar.
[INFO] Excluding org.glassfish.jersey.containers:jersey-container-servlet:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.glassfish.jersey.containers:jersey-container-servlet-core:jar:2.22.2 from the shaded jar.
[INFO] Excluding org.apache.mesos:mesos:jar:shaded-protobuf:0.21.1 from the shaded jar.
[INFO] Excluding io.netty:netty-all:jar:4.0.29.Final from the shaded jar.
[INFO] Excluding io.netty:netty:jar:3.8.0.Final from the shaded jar.
[INFO] Excluding com.clearspring.analytics:stream:jar:2.7.0 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-core:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-jvm:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-json:jar:3.1.2 from the shaded jar.
[INFO] Excluding io.dropwizard.metrics:metrics-graphite:jar:3.1.2 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-databind:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.core:jackson-core:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.fasterxml.jackson.module:jackson-module-scala_2.11:jar:2.5.3 from the shaded jar.
[INFO] Excluding com.thoughtworks.paranamer:paranamer:jar:2.6 from the shaded jar.
[INFO] Excluding org.apache.ivy:ivy:jar:2.4.0 from the shaded jar.
[INFO] Excluding oro:oro:jar:2.0.8 from the shaded jar.
[INFO] Excluding net.razorvine:pyrolite:jar:4.9 from the shaded jar.
[INFO] Excluding net.sf.py4j:py4j:jar:0.10.1 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-streaming_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-sql_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding com.univocity:univocity-parsers:jar:2.1.0 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-sketch_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.apache.spark:spark-catalyst_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Excluding org.codehaus.janino:janino:jar:2.7.8 from the shaded jar.
[INFO] Excluding org.codehaus.janino:commons-compiler:jar:2.7.8 from the shaded jar.
[INFO] Excluding org.antlr:antlr4-runtime:jar:4.5.2-1 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-column:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-common:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-encoding:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-generator:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-hadoop:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-format:jar:2.3.0-incubating from the shaded jar.
[INFO] Excluding org.apache.parquet:parquet-jackson:jar:1.7.0 from the shaded jar.
[INFO] Excluding org.apache.spark:spark-tags_2.11:jar:2.0.0-SNAPSHOT from the shaded jar.
[INFO] Including org.spark-project.spark:unused:jar:1.0.0 in the shaded jar.
[INFO] Excluding org.scala-lang:scala-reflect:jar:2.11.8 from the shaded jar.
[INFO] Excluding org.scala-lang.modules:scala-xml_2.11:jar:1.0.2 from the shaded jar.
[INFO] Replacing original artifact with shaded artifact.
[INFO]
[INFO] --- maven-source-plugin:2.4:jar-no-fork (create-source-jar) @ java8-tests_2.11 ---
[INFO]
[INFO] --- maven-source-plugin:2.4:test-jar-no-fork (create-source-jar) @ java8-tests_2.11 ---
[INFO] ------------------------------------------------------------------------
[INFO] Reactor Summary:
[INFO]
[INFO] Spark Project Parent POM ........................... SUCCESS [  7.072 s]
[INFO] Spark Project Tags ................................. SUCCESS [  8.367 s]
[INFO] Spark Project Sketch ............................... SUCCESS [  6.058 s]
[INFO] Spark Project Networking ........................... SUCCESS [  7.929 s]
[INFO] Spark Project Shuffle Streaming Service ............ SUCCESS [  5.086 s]
[INFO] Spark Project Unsafe ............................... SUCCESS [  7.547 s]
[INFO] Spark Project Launcher ............................. SUCCESS [  6.654 s]
[INFO] Spark Project Core ................................. SUCCESS [02:00 min]
[INFO] Spark Project GraphX ............................... SUCCESS [ 11.730 s]
[INFO] Spark Project Streaming ............................ SUCCESS [ 27.599 s]
[INFO] Spark Project Catalyst ............................. SUCCESS [01:00 min]
[INFO] Spark Project SQL .................................. SUCCESS [01:17 min]
[INFO] Spark Project ML Local Library ..................... SUCCESS [  5.736 s]
[INFO] Spark Project ML Library ........................... SUCCESS [01:10 min]
[INFO] Spark Project Tools ................................ SUCCESS [  1.087 s]
[INFO] Spark Project Hive ................................. SUCCESS [ 34.424 s]
[INFO] Spark Project HiveContext Compatibility ............ SUCCESS [  3.505 s]
[INFO] Spark Project REPL ................................. SUCCESS [  3.263 s]
[INFO] Spark Project Assembly ............................. SUCCESS [  2.034 s]
[INFO] Spark Project External Flume Sink .................. SUCCESS [  4.851 s]
[INFO] Spark Project External Flume ....................... SUCCESS [  7.824 s]
[INFO] Spark Project External Flume Assembly .............. SUCCESS [  1.747 s]
[INFO] Spark Integration for Kafka 0.8 .................... SUCCESS [  9.528 s]
[INFO] Spark Project Examples ............................. SUCCESS [ 16.023 s]
[INFO] Spark Project External Kafka Assembly .............. SUCCESS [  3.564 s]
[INFO] Spark Project Java 8 Tests ......................... SUCCESS [  4.608 s]
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time: 08:35 min
[INFO] Finished at: 2016-05-20T12:37:29-04:00
[INFO] Final Memory: 78M/950M
[INFO] ------------------------------------------------------------------------

[cass@compile spark]$
```
