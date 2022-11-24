# Issue about the compilation of mechsys
With Ubuntu 20 or higher version, a problem may happen occasionally, i.e.,

```
usr/bin/ld cannot find -lgfortran
```

This issure can be solved by using lower version of g++, gcc and gfortran.


sudo update-alternatives --install /usr/bin/g++ g++ /usr/bin/g++-7 20

sudo update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-7 20

sudo update-alternatives --install /usr/bin/gfortran gfortran /usr/bin/gfortran-7 20
