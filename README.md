# Hello Abduction

A demo of abduction using the MISTRAL SMT solver.

### Prerequisites
On an Ubuntu machine, run this command to install Mistral's dependencies:
```
sudo apt install libc6-dev-i386 gettext gawk flex libmpfr-dev cmake \
kdelibs5-dev libgtkmm-2.4-dev libboost-thread-dev libboost-serialization-dev \
libglademm-2.4-dev graphviz doxygen g++ libgmp-dev build-essential flex bison \
binutils-gold libgmp10
```

You can probably use yum or other installers similarly, but this has not been
tested.

### Setup

1. Clone this repo and enter into the repo directory.

2. Run `git submodule update --init --recursive` to load the ext/mistral subdirectory.

3. Run `./build.sh` to build the demo.

### Executing

The demo can be found in the build/bin/ directory.

You can execute it with the line `build/bin/HelloAbduction`.
