# Optimizing Common Table Expressions in Apache Hive with Calcite

*Where:*  Caclite Hybrid Meetup

*When:* February 21, 2025

*Duration:* 25 minutes

*Abstract:*
In many real-world queries, certain expressions may appear multiple times, requiring repeated computations to construct the final result. These recurring computations, known as common table expressions (CTEs), can be explicitly defined in SQL queries using the WITH clause or implicitly derived through transformation rules. Identifying and leveraging CTEs is essential for reducing the cost of executing complex queries and is a critical component of modern data management systems.

Apache Hive, a SQL-based data management system, provides powerful mechanisms to detect and exploit CTEs through heuristic and cost-based optimization techniques.
This talk delves into the internals of Hive's planner, focusing on its integration with Apache Calcite for CTE optimization. We will begin with a high-level overview of Hive's planner architecture and its reliance on Calcite in various planning phases. The discussion will then shift to the CTE rewriting phase, highlighting key Calcite concepts and demonstrating how they are employed to optimize CTEs effectively.
