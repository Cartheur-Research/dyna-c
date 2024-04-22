## dyna-c

The clean version for the Robotis motor control in Linux.

### How to use this repo

Inside the `build` folder are the makefiles for `arm`, `x86`, and `x64` versions of Linux. Ensure that your system has the build tools installedddd:

`apt install build-essential`

### Building & linking

The codebase was obtained from a customer where the last working date-stamp was 20160609, which noted gcc-5.4. The standard has changed so the line:

`LDFLAGS="-Wl,-allow-multiple-definition"`

has been added to resolve the multiple definitions that should be fixed, when there is time. However, other issues still remain that will be addressed when there is time away from robotics development itself.

Note that there is dummy `hello.c` file that is added as a source to the makefile.