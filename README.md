<!-- Copyright (c) 2022 Christopher Taylor                                          -->
<!--                                                                                -->
<!--   Distributed under the Boost Software License, Version 1.0. (See accompanying -->
<!--   file LICENSE_1_0.txt or copy at http://www.boost.org/LICENSE_1_0.txt)        -->
# [codon_openshmem](https://github.com/ct-clmsn/codon_openshmem)

`codon_openshmem` (COS) wraps the existing [Sandia OpenSHMEM](https://github.com/Sandia-OpenSHMEM/SOS) library implemented by Sandia National Laboratory. COS provides the [codon](https://github.com/exaloop/codon) Python compiler Partitioned Global Address Space (PGAS) support.

Users are able to interact with OpenSHMEM using a handful of the existing OpenSHMEM functions or users are able to interact with OpenSHMEM through a class called Runtime. Users can create distributed symmetric arrays using a templated SymmetricArray class. Users can additionally leverage Codon's support for the [static keyword](https://docs.exaloop.io/codon/language/statics) with COS.

COS HPC users can benefit from Codon's native support for [OpenMP](https://docs.exaloop.io/codon/advanced/parallel), [GPUs](https://docs.exaloop.io/codon/advanced/gpu), existing [Python extensions](https://docs.exaloop.io/codon/interoperability/pyext), and portable assembly using the [LLVM IR](https://docs.exaloop.io/codon/language/llvm) interface. 


### Developer Notes

A simple example application is provided in the `./test` directory along with a Makefile. The COS implementation is provided in the `./src` directory, users only need to copy that file into their project directory. COS is implemented using Codon's [FFI](https://docs.exaloop.io/codon/language/ffi) interface. Additional details on Codon's C/C++ interface are available [here](https://docs.exaloop.io/codon/interoperability/cpp).

### Licenses

* [Boost](https://www.boost.org/users/license.html) Version 1.0 (2022-)

### Author

Christopher Taylor

### Special Thanks

* The OpenSHMEM developers and committee
* Sandia National Labs/US Department of Energy

### Dependencies

* [Sandia OpenSHMEM](https://github.com/Sandia-OpenSHMEM/SOS)
