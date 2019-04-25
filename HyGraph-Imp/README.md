# Improving Graph Processing on Heterogeneous Platforms

HyGraph [1] is a graph-processing system designed for hybrid platforms consisting of a multi-core CPU and a NVIDIA GPU. It solves the issue of workload imbalance in hybrid graph processing by replicating vertex state into both CPU and GPU memory and scheduling task onto both CPU and GPU in a dynamic fashion. This projects improves HyGraph by packing some operations and inlining some functions, also a job distributor is designed for better workload balancing.


To run HyGraph, run `main`.

```
./main [graph file] [algorithm]
```

Where algorithm should be one of the following: `bfs` (Breadth-first search), `pr` (PageRank), `sssp` (Single-Source Shortest Path), `cc` (Connected components). The graph file should be in human-readable format containing one edge per line where each edge consists of a pair of two number. Duplicate edges, empty lines or comments (start with `#` or `*` or `-`) are ignored.




# HyGraph Author
[1] Heldens S., Varbanescu A. L., Iosup A., HyGraph: Fast Graph Processing on Hybrid CPU-GPU Platforms by Dynamic Load-Balancing, 2016. Manuscript submitted for publication.

