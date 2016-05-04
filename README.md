# uQlust-ver1.0
This repository contains the uQlust package ver. 1.0  for ultrafast ranking and clustering of macromolecular structures. 

uQlust combines versatile structural profiles of both proteins and nucleic acids with linear time algorithm for comparison of all pairs of models using 1D-jury (Adamczak and Meller, 2011), and profile hashing for efficient and low memory footprint clustering of macromolecular structures, including hierarchical clustering. While reducing the computation time by orders of magnitude with respect to existing methods, uQlust yields comparable accuracies in protein and RNA clustering and model quality assessment. Even though it has been primarily developed for large scale structure prediction and molecular simulations for both proteins and RNA, uQlust can also be used in conjunction with an arbitrary profile, such as the FragBag structural motif frequency profile.

uQlust was written (in C#) by Rafal Adamczak, based on a joined work with Jarek Meller (Adamczak & Meller, uQlust: Ultrafast Ranking and Clustering of Macromolecular Structures, to be published). The code should be easily portable between different operating systems (pre-compiled executable are available for Linux and 64-bit Windows operating systems). Multithreading is enabled to speed up profile pre-processing, ranking and clustering. For vector hashing, C# Dictionary Type with a hash function default method GetHashCode() is used. The source code, pre-compiled executables, user manual and a number of utilities and benchmarks and examples are available as part of this package. 