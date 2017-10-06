# gcc-chrome-os-binary
GCC binary for Chrome OS

This is the (Intel x86_64) Chrome OS binary for the stable release of GCC 7.2, this file is provided for your convenience, if you prefer to compile yourself gcc-7.2 visit the tutorial webpage for build instructions:

[https://solarianprogrammer.com/2017/10/05/building-gcc-chromebook-chrome-os/](https://solarianprogrammer.com/2017/10/05/building-gcc-chromebook-chrome-os/)

You need to have the [Developer Mode](https://solarianprogrammer.com/2017/09/11/two-weeks-programming-chromebook-challenge/#dev_mod) enabled on your Chrome OS device.

**Clone (download) the archive on your machine with:**

git clone https://github.com/sol-prog/gcc-chrome-os-binary.git

In order to install this binary extract gcc-7.2.0.tar.bz2 and copy the extracted folder (gcc-7.2) in your /usr/local folder.

Using the new compilers (gcc-7.2, g++-7.2 and gfortran-7.2) require that you modify your path, paste the next line in a shell tab:

export PATH=/usr/local/gcc-7.2/bin:$PATH
export LIBRARY_PATH=/usr/local/lib64:$LIBRARY_PATH

The above will modify temporarily your path (closing the Terminal will revert to the default path). If you want to add this permanently to your path add the above line in the .bashrc file from your Home.

Compiling a C++14 code is as simple as:

g++-7.2 file_name.cpp -o file_name:

If you need more help leave me a comment at:

[https://solarianprogrammer.com/2017/10/05/building-gcc-chromebook-chrome-os/](https://solarianprogrammer.com/2017/10/05/building-gcc-chromebook-chrome-os/)
