## Accelerating distributed joins in Apache Hive: Runtime filtering-enhancements

*Where:* ApacheCon

*When:* September 29, 2020

*Duration:* 40 minutes

*Abstract:*

Apache Hive is an open-source relational database system that is widely adopted by several organizations for big data analytic workloads. It combines traditional MPP (massively parallel processing) techniques with more recent cloud computing concepts to achieve the increased scalability and high performance needed by modern data intensive applications. Even though it was originally tailored towards long running data warehousing queries, its architecture recently changed with the introduction of LLAP (Live Long and Process) layer. Instead of regular containers, LLAP utilizes long-running executors to exploit data sharing and caching possibilities within and across queries. Executors eliminate unnecessary disk IO overhead and thus reduce the latency of interactive BI (business intelligence) queries by orders of magnitude. However, as container startup cost and IO overhead is now minimized, the need to effectively utilize memory and CPU resources across long-running executors in the cluster is becoming increasingly essential. For instance, in a variety of production workloads, we noticed that the memory bandwidth of early decoding all table columns for every row, even when this row is dropped later on, is starting to overwhelm the performance of single query execution. In this talk, we focus on some of the optimizations we introduced in Hive 4.0 to increase CPU efficiency and save memory allocations. In particular, we describe the lazy decoding (or row-level filtering) and composite bloom-filters optimizations that greatly improve the performance of queries containing broadcast joins, reducing their runtime by up to 50%. Over several production and synthetic workloads, we show the benefit of the newly introduced optimizations as part of Cloudera’s cloud-native Data Warehouse engine. At the same time, the community can directly benefit from the presented features as are they 100% open-source!

*Video:* https://www.youtube.com/watch?v=P5Q5GZheAEk
