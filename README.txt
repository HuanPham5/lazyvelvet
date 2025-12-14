Project Description
This project is a research-oriented modification of the Velvet de novo genome assembler. The goal is to replace Velvet’s original exhaustive graph traversal strategy with a lazy traversal approach. Instead of fully traversing and simplifying the de Bruijn graph upfront, the lazy traversal defers exploration until it is required, with the aim of reducing unnecessary computation while preserving assembly quality. This work is intended for algorithmic experimentation and performance analysis rather than as a production-ready assembler.

Motivation
Velvet performs aggressive graph simplification and traversal to generate contigs from short-read sequencing data. While effective, this approach can be computationally expensive, especially on large or complex graphs. Lazy traversal explores only relevant portions of the graph on demand, potentially reducing runtime and memory usage. This project investigates whether such a strategy can be integrated into Velvet’s architecture without compromising correctness.

Acknowledgment
This project is based on the original Velvet genome assembler developed by Daniel Zerbino and Ewan Birney. The original Velvet source code, algorithms, and design form the foundation of this work. All credit for the original implementation and methodology belongs to the original authors. This repository contains experimental modifications for research and educational purposes only.

License and Attribution
This work retains the original Velvet license. Redistribution and use of this code must comply with the terms of that license. Removing Git history does not remove the obligation to acknowledge the original authors or preserve the license text.

Status
This project is experimental. The lazy traversal implementation is a prototype and has not been validated across all datasets or edge cases supported by the original Velvet assembler.
