# I. How to install fftw3

This tutorial for installing **fftw3** is written based on
[How To Install "fftw3" Package on Ubuntu](https://zoomadmin.com/HowToInstall/UbuntuPackage/fftw3)
. You need to be connected to internet to install **fftw3**. To install **fftw3** run 

```sh
sudo apt-get update -y
````

in tterminal. Then run

```sh
sudo apt-get install -y fftw3
````

Now **fftw3** is installed on your system.

# I. How to use the library fftw3 in c++ codes

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
g++ example.cpp -I/usr/include/ffttw.h -lm -lfftw3
````
