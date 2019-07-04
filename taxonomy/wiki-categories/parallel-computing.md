Parallel computing


Embarrassingly parallel 
 Connected to: Inherently serial problem Graphics processing unit Password cracking
From Wikipedia, the free encyclopedia
In parallel computing, an embarrassingly parallel workload or problem (also called perfectly parallel or pleasingly parallel) is one where little or no effort is needed to separate the problem into a number of parallel tasks.[1] This is often the case where there is little or no dependency or need for communication between those parallel tasks, or for results between them.[2]

Thus, these are different from distributed computing problems that need communication between tasks, especially communication of intermediate results. They are easy to perform on server farms which lack the special infrastructure used in a true supercomputer cluster. They are thus well suited to large, Internet-based distributed platforms such as BOINC, and do not suffer from parallel slowdown. The opposite of embarrassingly parallel problems are inherently serial problems, which cannot be parallelized at all.

A common example of an embarrassingly parallel problem is 3D video rendering handled by a graphics processing unit, where each frame (forward method) or pixel (ray tracing method) can be handled with no interdependency. Password cracking is another embarrassingly parallel task that is easily distributed on central processing units, CPU cores, or clusters.

Etymology
"Embarrassingly" is used here in the same sense as in the phrase "an embarrassment of riches", meaning an overabundance—here referring to parallelization problems which are "embarrassingly easy".[3] The term may also imply embarrassment on the part of developers or compilers: "Because so many important problems remain unsolved mainly due to their intrinsic computational complexity, it would be embarrassing not to develop parallel implementations of polynomial homotopy continuation methods."[4] The term is first found in the literature in a 1986 book on multiprocessors by MATLAB's co-founder Cleve Moler,[5] who claims to have invented the term.[6]

An alternative term, pleasingly parallel, has gained some use, perhaps to avoid the negative connotations of embarrassment in favor of a positive reflection on the parallelizability of the problems: "Of course, there is nothing embarrassing about these programs at all."[7]

Examples
Some examples of embarrassingly parallel problems include:

Distributed relational database queries using distributed set processing.
Serving static files on a webserver to multiple users at once.
The Mandelbrot set, Perlin noise and similar images, where each point is calculated independently.
Rendering of computer graphics. In computer animation, each frame or pixel may be rendered independently (see parallel rendering).
Brute-force searches in cryptography.[8] Notable real-world examples include distributed.net and proof-of-work systems used in cryptocurrency.
BLAST searches in bioinformatics for multiple queries (but not for individual large queries).[9]
Large scale facial recognition systems that compare thousands of arbitrary acquired faces (e.g., a security or surveillance video via closed-circuit television) with similarly large number of previously stored faces (e.g., a rogues gallery or similar watch list).[10]
Computer simulations comparing many independent scenarios, such as climate models.
Evolutionary computation metaheuristics such as genetic algorithms.
Ensemble calculations of numerical weather prediction.
Event simulation and reconstruction in particle physics.
The marching squares algorithm.
Sieving step of the quadratic sieve and the number field sieve.
Tree growth step of the random forest machine learning technique.
Discrete Fourier transform where each harmonic is independently calculated.
Convolutional neural networks running on GPUs.
Hyperparameter grid search in machine learning.
Implementations
In R (programming language) – The Simple Network of Workstations (SNOW) package implements a simple mechanism for using a set of workstations or a Beowulf cluster for embarrassingly parallel computations.[11]
Amdahl's law defines value P, which would be almost or exactly equal to 1 for embarrassingly parallel problems.
Map (parallel pattern)
Multiprocessing
Massively parallel
Parallel computing
Process oriented programming
Shared nothing architecture (SN)
Symmetric multiprocessing (SMP)
Connection Machine
Cellular automaton
CUDA framework
Manycore processor
Vector processor
^ Herlihy, Maurice; Shavit, Nir (2012). The Art of Multiprocessor Programming, Revised Reprint (revised ed.). Elsevier. p. 14. ISBN 9780123977953. Retrieved 28 February 2016. Some computational problems are “embarrassingly parallel”: they can easily be divided into components that can be executed concurrently.
^ Section 1.4.4 of: Foster, Ian (1995). "Designing and Building Parallel Programs". Addison–Wesley (ISBN 9780201575941). Archived from the original on 2011-02-21.
^ Matloff, Norman (2011). The Art of R Programming: A Tour of Statistical Software Design, p.347. No Starch. ISBN 9781593274108.
^ Leykin, Anton; Verschelde, Jan; Zhuang, Yan (2006). "Parallel Homotopy Algorithms to Solve Polynomial Systems". Proceedings of ICMS 2006.
^ Moler, Cleve (1986). Heath, Michael T., ed. "Matrix Computation on Distributed Memory Multiprocessors". Hypercube Multiprocessors. Society for Industrial and Applied Mathematics, Philadelphia. ISBN 0898712092.
^ The Intel hypercube part 2 reposted on Cleve's Corner blog on The MathWorks website
^ Kepner, Jeremy (2009). Parallel MATLAB for Multicore and Multinode Computers, p.12. SIAM. ISBN 9780898716733.
^ Simon, Josefsson; Colin, Percival (August 2016). "The scrypt Password-Based Key Derivation Function". tools.ietf.org. Retrieved 2016-12-12.
^ SeqAnswers forum
^ How we made our face recognizer 25 times faster (developer blog post)
^ Simple Network of Workstations (SNOW) package
Embarrassingly Parallel Computations, Engineering a Beowulf-style Compute Cluster
"Star-P: High Productivity Parallel Computing"
[hide]
Parallel computing
General	
Distributed computing Parallel computing Massively parallel Cloud computing High-performance computing Multiprocessing Manycore processor GPGPU Computer network Systolic array
Levels	
Bit Instruction Thread Task Data Memory Loop Pipeline
Multithreading	
Temporal Simultaneous (SMT) Speculative (SpMT) Preemptive Cooperative Clustered Multi-Thread (CMT) Hardware scout
Theory	
PRAM model Analysis of parallel algorithms Amdahl's law Gustafson's law Cost efficiency Karp–Flatt metric Slowdown Speedup
Elements	
Process Thread Fiber Instruction window
Coordination	
Multiprocessing Memory coherency Cache coherency Cache invalidation Barrier Synchronization Application checkpointing
Programming	
Stream processing Dataflow programming Models Implicit parallelism Explicit parallelism Concurrency Non-blocking algorithm
Hardware	
Flynn's taxonomy SISD SIMD SIMT MISD MIMD Dataflow architecture Pipelined processor Superscalar processor Vector processor Multiprocessor symmetric asymmetric Memory shared distributed distributed shared UMA NUMA COMA Massively parallel computer Computer cluster Grid computer
APIs	
Ateji PX Boost.Thread Chapel Charm++ Cilk Coarray Fortran CUDA Dryad C++ AMP Global Arrays MPI OpenMP OpenCL OpenHMPP OpenACC TPL PLINQ PVM POSIX Threads RaftLib UPC TBB ZPL
Problems	
Deadlock Livelock Deterministic algorithm Embarrassingly parallel Parallel slowdown Race condition Software lockout Scalability Starvation
Category Category: parallel computing Commons page Media related to Parallel computing at Wikimedia Commons
 Related topics
Berkeley Open Infrastructure for Network Computing
The Berkeley Open Infrastructure for Network Computing (BOINC, pronounced /bɔɪŋk/ - rhymes with "oink"), an open-source middleware system, supports volunteer and grid computing. Originally developed to support the SETI@home project, it became generalized as a platform for other distributed applications in areas as diverse as mathematics, medicine, molecular biology, climatology, environmental...
Supercomputer
A supercomputer is a computer with a high-level computational capacity compared to a general-purpose computer. Performance of a supercomputer is measured in floating point operations per second (FLOPS) instead of million instructions per second (MIPS).
Server farm
A server farm or server cluster is a collection of computer servers - usually maintained by an organization to supply server functionality far beyond the capability of a single machine. Server farms often consist of thousands of computers which require a large amount of power to run and to keep cool.
This page is based on a Wikipedia article written by contributors (read/edit).
Text is available under the CC BY-SA 4.0 license; additional terms may apply.
Images, videos and audio are available under their respective licenses.
Tell your friends about Wikiwand!
Gmail Facebook Twitter  
http://www.wikiwand.com/
Link 

Home About Press Site Map Terms Of Service Privacy Policy
Embarrassingly parallel

---

wikimedia: Category: Concurrent programming
https://commons.wikimedia.org/wiki/Category:Concurrent_programming

Foundations of Actor Semantics
https://dspace.mit.edu/handle/1721.1/6935

The Intel Hypercube, part 2, reposted
Posted by Cleve Moler, November 12, 2013
https://blogs.mathworks.com/cleve/2013/11/12/the-intel-hypercube-part-2-reposted/#096367ea-045e-4f28-8fa2-9f7db8fb7b01

How We Made Our Face Recognizer 25x Faster
Posted by Louis Brandy on 27 October 2008
http://lbrandy.com/blog/2008/10/how-we-made-our-face-recognizer-25-times-faster/


Coordinated Computing
Tools and Techniques for Distributed Software
Robert E. Filman and Daniel P. Friedman
https://web.archive.org/web/20070516135233/http://ic.arc.nasa.gov/people/filman/text/dpl/dpl.html

https://dl.acm.org/citation.cfm?doid=242223.242252

Parallel Homotopy Algorithms to Solve Polynomial Systems
https://link.springer.com/chapter/10.1007%2F11832225_22#page-1

Parallel Algorithms
https://www.webcitation.org/5wfSkP1Ia?url=http://www.mcs.anl.gov/~itf/dbpp/text/node10.html

Embarrassingly Parallel Computations
http://webhome.phy.duke.edu/~rgb/Beowulf/beowulf_book/beowulf_book/node30.html

Engineering a Beowulf-style Compute Cluster
http://webhome.phy.duke.edu/~rgb/Beowulf/beowulf_book/beowulf_book/node1.html

---
https://commons.wikimedia.org/wiki/Category:Concurrency_(computer_science)

https://en.wikipedia.org/wiki/Category:Concurrency_(computer_science)?oldformat=true


Search Wikipedia
 
Collected from: [Embarrassingly parallel](https://en.wikipedia.org/wiki/Embarrassingly_parallel)


- [Parallel computing](https://en.wikipedia.org/wiki/Parallel_computing)
- [Distributed computing](https://en.wikipedia.org/wiki/Distributed_computing)
- [Massively parallel](https://en.wikipedia.org/wiki/Massively_parallel)
- [Cloud computing](https://en.wikipedia.org/wiki/Cloud_computing)
- [Supercomputer](https://en.wikipedia.org/wiki/Supercomputer)
- [Multiprocessing](https://en.wikipedia.org/wiki/Multiprocessing)
- [Manycore processor](https://en.wikipedia.org/wiki/Manycore_processor)
- [General-purpose computing on graphics processing u](https://en.wikipedia.org/wiki/General-purpose_computing_on_graphics_processing_units)
- [Computer network](https://en.wikipedia.org/wiki/Computer_network)
- [Systolic array](https://en.wikipedia.org/wiki/Systolic_array)
- [Bit-level parallelism](https://en.wikipedia.org/wiki/Bit-level_parallelism)
- [Instruction-level parallelism](https://en.wikipedia.org/wiki/Instruction-level_parallelism)
- [Task parallelism](https://en.wikipedia.org/wiki/Task_parallelism)
- [Data parallelism](https://en.wikipedia.org/wiki/Data_parallelism)
- [Memory-level parallelism](https://en.wikipedia.org/wiki/Memory-level_parallelism)
- [Loop-level parallelism](https://en.wikipedia.org/wiki/Loop-level_parallelism)
- [Pipeline (computing)](https://en.wikipedia.org/wiki/Pipeline_(computing))
- [Multithreading (computer architecture)](https://en.wikipedia.org/wiki/Multithreading_(computer_architecture))
- [Temporal multithreading](https://en.wikipedia.org/wiki/Temporal_multithreading)
- [Simultaneous](https://en.wikipedia.org/wiki/Simultaneous_multithreading)
- [Speculative multithreading](https://en.wikipedia.org/wiki/Speculative_multithreading)
- [Preemptive](https://en.wikipedia.org/wiki/Preemption_(computing))
- [Computer multitasking](https://en.wikipedia.org/wiki/Computer_multitasking#Cooperative_multitasking)
- [Bulldozer (microarchitecture)](https://en.wikipedia.org/wiki/Bulldozer_(microarchitecture)#Bulldozer_core)
- [Hardware scout](https://en.wikipedia.org/wiki/Hardware_scout)
- [Parallel random-access machine](https://en.wikipedia.org/wiki/Parallel_random-access_machine)
- [Analysis of parallel algorithms](https://en.wikipedia.org/wiki/Analysis_of_parallel_algorithms)
- [Amdahl's law](https://en.wikipedia.org/wiki/Amdahl%27s_law)
- [Gustafson's law](https://en.wikipedia.org/wiki/Gustafson%27s_law)
- [Cost efficiency](https://en.wikipedia.org/wiki/Cost_efficiency)
- [Karp–Flatt metric](https://en.wikipedia.org/wiki/Karp%E2%80%93Flatt_metric)
- [Parallel slowdown](https://en.wikipedia.org/wiki/Parallel_slowdown)
- [Speedup](https://en.wikipedia.org/wiki/Speedup)
- [Process (computing)](https://en.wikipedia.org/wiki/Process_(computing))
- [Thread (computing)](https://en.wikipedia.org/wiki/Thread_(computing))
- [Fiber (computer science)](https://en.wikipedia.org/wiki/Fiber_(computer_science))
- [Instruction window](https://en.wikipedia.org/wiki/Instruction_window)
- [Memory coherence](https://en.wikipedia.org/wiki/Memory_coherence)
- [Cache coherence](https://en.wikipedia.org/wiki/Cache_coherence)
- [Cache invalidation](https://en.wikipedia.org/wiki/Cache_invalidation)
- [Barrier (computer science)](https://en.wikipedia.org/wiki/Barrier_(computer_science))
- [Synchronization (computer science)](https://en.wikipedia.org/wiki/Synchronization_(computer_science))
- [Application checkpointing](https://en.wikipedia.org/wiki/Application_checkpointing)
- [Computer programming](https://en.wikipedia.org/wiki/Computer_programming)
- [Stream processing](https://en.wikipedia.org/wiki/Stream_processing)
- [Dataflow programming](https://en.wikipedia.org/wiki/Dataflow_programming)
- [Parallel programming model](https://en.wikipedia.org/wiki/Parallel_programming_model)
- [Implicit parallelism](https://en.wikipedia.org/wiki/Implicit_parallelism)
- [Explicit parallelism](https://en.wikipedia.org/wiki/Explicit_parallelism)
- [Concurrency (computer science)](https://en.wikipedia.org/wiki/Concurrency_(computer_science))
- [Non-blocking algorithm](https://en.wikipedia.org/wiki/Non-blocking_algorithm)
- [Computer hardware](https://en.wikipedia.org/wiki/Computer_hardware)
- [Flynn's taxonomy](https://en.wikipedia.org/wiki/Flynn%27s_taxonomy)
- [SISD](https://en.wikipedia.org/wiki/SISD)
- [SIMD](https://en.wikipedia.org/wiki/SIMD)
- [Single instruction, multiple threads](https://en.wikipedia.org/wiki/Single_instruction,_multiple_threads)
- [MISD](https://en.wikipedia.org/wiki/MISD)
- [MIMD](https://en.wikipedia.org/wiki/MIMD)
- [Dataflow architecture](https://en.wikipedia.org/wiki/Dataflow_architecture)
- [Instruction pipelining](https://en.wikipedia.org/wiki/Instruction_pipelining)
- [Superscalar processor](https://en.wikipedia.org/wiki/Superscalar_processor)
- [Vector processor](https://en.wikipedia.org/wiki/Vector_processor)
- [Symmetric multiprocessing](https://en.wikipedia.org/wiki/Symmetric_multiprocessing)
- [Asymmetric multiprocessing](https://en.wikipedia.org/wiki/Asymmetric_multiprocessing)
- [Semiconductor memory](https://en.wikipedia.org/wiki/Semiconductor_memory)
- [Shared memory](https://en.wikipedia.org/wiki/Shared_memory)
- [Distributed memory](https://en.wikipedia.org/wiki/Distributed_memory)
- [Distributed shared memory](https://en.wikipedia.org/wiki/Distributed_shared_memory)
- [Uniform memory access](https://en.wikipedia.org/wiki/Uniform_memory_access)
- [Non-uniform memory access](https://en.wikipedia.org/wiki/Non-uniform_memory_access)
- [Cache-only memory architecture](https://en.wikipedia.org/wiki/Cache-only_memory_architecture)
- [Computer cluster](https://en.wikipedia.org/wiki/Computer_cluster)
- [Grid computing](https://en.wikipedia.org/wiki/Grid_computing)
- [Application programming interface](https://en.wikipedia.org/wiki/Application_programming_interface)
- [Ateji PX](https://en.wikipedia.org/wiki/Ateji_PX)
- [Boost (C++ libraries)](https://en.wikipedia.org/wiki/Boost_(C%2B%2B_libraries)#Multithreading_%E2%80%93_Boost.Thread)
- [Chapel (programming language)](https://en.wikipedia.org/wiki/Chapel_(programming_language))
- [Charm++](https://en.wikipedia.org/wiki/Charm%2B%2B)
- [Cilk](https://en.wikipedia.org/wiki/Cilk)
- [Coarray Fortran](https://en.wikipedia.org/wiki/Coarray_Fortran)
- [CUDA](https://en.wikipedia.org/wiki/CUDA)
- [Dryad (programming)](https://en.wikipedia.org/wiki/Dryad_(programming))
- [C++ AMP](https://en.wikipedia.org/wiki/C%2B%2B_AMP)
- [Global Arrays](https://en.wikipedia.org/wiki/Global_Arrays)
- [Message Passing Interface](https://en.wikipedia.org/wiki/Message_Passing_Interface)
- [OpenMP](https://en.wikipedia.org/wiki/OpenMP)
- [OpenCL](https://en.wikipedia.org/wiki/OpenCL)
- [OpenHMPP](https://en.wikipedia.org/wiki/OpenHMPP)
- [OpenACC](https://en.wikipedia.org/wiki/OpenACC)
- [Parallel Extensions](https://en.wikipedia.org/wiki/Parallel_Extensions#Task_Parallel_Library)
- [Parallel Extensions](https://en.wikipedia.org/wiki/Parallel_Extensions#PLINQ)
- [Parallel Virtual Machine](https://en.wikipedia.org/wiki/Parallel_Virtual_Machine)
- [POSIX Threads](https://en.wikipedia.org/wiki/POSIX_Threads)
- [RaftLib](https://en.wikipedia.org/wiki/RaftLib)
- [Unified Parallel C](https://en.wikipedia.org/wiki/Unified_Parallel_C)
- [Threading Building Blocks](https://en.wikipedia.org/wiki/Threading_Building_Blocks)
- [ZPL (programming language)](https://en.wikipedia.org/wiki/ZPL_(programming_language))
- [Deadlock](https://en.wikipedia.org/wiki/Deadlock)
- [Deadlock](https://en.wikipedia.org/wiki/Deadlock#Livelock)
- [Deterministic algorithm](https://en.wikipedia.org/wiki/Deterministic_algorithm)
- [Embarrassingly parallel](https://en.wikipedia.org/wiki/undefined)
- [Race condition](https://en.wikipedia.org/wiki/Race_condition#Computing)
- [Software lockout](https://en.wikipedia.org/wiki/Software_lockout)
- [Scalability](https://en.wikipedia.org/wiki/Scalability)
- [Starvation (computer science)](https://en.wikipedia.org/wiki/Starvation_(computer_science))
- [Category:Parallel computing](https://en.wikipedia.org/wiki/Category:Parallel_computing)
- [c:Category:Parallel computing](https://commons.wikimedia.org/wiki/Category:Parallel_computing)

