# Apache Calcite Tutorial

*Where:* BOSS 2021 (https://boss-workshop.github.io/boss-2021/)

*When:* August 21, 2021

*Duration:* 45 minutes

*Abstract:*

Apache Calcite is a dynamic data management framework.
Think of it as a toolkit for building databases: it has an industry-standard SQL parser, validator, highly customizable optimizer (with pluggable transformation rules and cost functions, relational algebra, and an extensive library of rules), but it has no preferred storage primitives.
In this tutorial, the attendees will use Apache Calcite to build a fully fledged query processor from scratch with very few lines of code.
This processor is a full implementation of SQL over an Apache Lucene storage engine.
(Lucene does not support SQL queries and lacks a declarative language for performing complex operations such as joins or aggregations.)
Attendees will also learn how to use Calcite as an effective tool for research.

