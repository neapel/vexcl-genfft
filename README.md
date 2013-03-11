This is a branch of [FFTw's](http://fftw.org/) kernel generator for use in [VexCL's](http://ddemidov.github.com/vexcl/) FFT.

The original files are from the `genfft` folder in fftw3-3.3.2, the OpenCL specific generator is in `cl_gen_notw.ml`.

Compile with `ocamlbuild -libs unix,nums cl_gen_notw.native`

The kernels used in VexCL are generated using `./kernels.sh > vexcl/fft/unrolled_dft.hpp`.
