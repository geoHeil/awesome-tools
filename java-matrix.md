# java matrix tools

## whishlist

- multiplication
- addition
- matrix decomposition
- not only java based (option for BLAS)
- vectorized (SIMD)
- fast

## benchmarks:
- https://github.com/optimatika/ojAlgo/wiki/Java-Matrix-Benchmark
- https://java-matrix.org
- https://www.reddit.com/r/scala/comments/5fcjo3/breeze_vs_nd4s/

## available libraries
- https://github.com/scalanlp/breeze
  - included into spark
  - netlib java blas backend for labpack and netlib which optimally are compiled with MKL support
- https://nd4j.org
  - switching backend is transparent (BLAS, GPU)
  - commercially supported
- http://ejml.org/wiki/index.php?title=Main_Page
  - no BLAS, pure java
  - free
  - 202 stars
  - apache 2.0
  - recommendation: nice, but only pure java. probably easy to get started with, not the most performance. a lot of algorithms implemented

- https://github.com/optimatika/ojAlgo
  - no native code
  - 189 stars
  
- https://scicomp.stackexchange.com/questions/2486/parallel-scientific-computation-software-development-language
- intel MKL https://software.intel.com/en-us/articles/performance-tools-for-software-developers-how-do-i-use-intel-mkl-with-java/
  - commercial licensing
- https://ujmp.org
- https://github.com/fommil/netlib-java/
- https://github.com/fommil/matrix-toolkits-java and https://github.com/andreas-solti/matrix-toolkits-java
- https://github.com/hughperkins/jeigen
  - java wrapper around C library
