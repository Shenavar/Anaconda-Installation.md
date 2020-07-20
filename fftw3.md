# Fast Fourier Transform

## I. What is it?

Fourier transform converts a physical-space (or time series) representation of a function into frequency-space in one or more dimensions.
Owing to its vast application in science and engineering, it is vital to compute it as fast as possible.
Fast Fourier transform (FFT) is a way to compute discrete Fourier transform (DFT) with the algorithm complexity of N log N instead of N^2.

Because of its importance, there are many implication of FFT, namely [fftw](http://fftw.org/) (C and FORTRAN),
[pyFFTW](https://pyfftw.readthedocs.io/en/latest/), [numpy.fft](https://numpy.org/doc/stable/reference/routines.fft.html),
[scipy.fft](https://docs.scipy.org/doc/scipy/reference/tutorial/fft.html) (python)
and [fftw.jl](https://github.com/JuliaMath/FFTW.jl) (Julia).

For the NA2020 crash course, you will need a working FFT library on your computer. In the following we will tell you how simply you can install it in a Gnu/Linux OS.

## II. How to install FFT (C and FORTRAN)(ubuntu based distros)

**fftw** is a well-known FFT library which is implemented in C with an interface
for FORTRAN.


To install **fftw** library version 3, run

```sh
sudo apt-get update
````

in terminal. Then run

```sh
sudo apt-get install libfftw3-dev
````

Now **fftw3** is installed on your system. You can list all the files installed by
this package as

```sh
dpkg -L libfftw3-dev
```

## III. How to use the library fftw3 in c++ codes

Usually, the library is installed in the following directory

```sh
/usr/include/
````

Imagine that your c++ code is saved as

```sh
example.cpp
````

Then, to execute your c++ code, you need to run the  following command in terminal

```sh
g++ example.cpp -I/usr/include -lm -lfftw3
````

## IV. Install pyFFTW (python wrapper)

Just run in terminal

```sh
pip install pyfftw
```

or if you prefer to install via conda, run

```sh
conda install -c conda-forge pyfftw
```
