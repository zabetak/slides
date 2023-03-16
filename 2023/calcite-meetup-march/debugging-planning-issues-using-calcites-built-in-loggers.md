# Debugging Planning Issues Using Calcite's Built-in Loggers

*Where:*  Caclite Virtual Meetup

*When:* March 15, 2023

*Duration:* 40 minutes

*Abstract:*

Wrong results, high memory usage (OutOfMemoryError, GC pauses, etc), unresponsive server, infinite planning time, are some common issues that may arise when using Calcite and in general a query processor in production systems.

In this talk, we will demonstrate how we can exploit Calcite's built-in loggers (notably [CALCITE-4704](https://issues.apache.org/jira/browse/CALCITE-4704), and [CALCITE-4991](https://issues.apache.org/jira/browse/CALCITE-4991)) to debug such issues through use-cases from Apache Hive.

