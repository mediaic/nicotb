---
layout: default
title: Build Nicotb
---
# Dependencies

* numpy and development package (TODO: version?)
* Google glog development packages (TODO: version?)
* Python (>= 3.3 ?)
* ncverilog (TODO: how about other tools which also support VPI)
* Linux (TODO: how to port?)

# Build Nicotb

First you should build the VPI library.

```bash
make -C lib/cpp
```

The examples are under the sim/ directory.
To run the examples, we have prepared a Makefile.
There are but roughly
Currently there are 2 examples, and you will lanuch the simulation
roughly like this.

```bash
cd sim/OOO
make -f ../Makefile XXX
```

where XXX is the name of toplevel Python and Verilog files.

However, you might face many problems when building the VPI library.
The Makefile is based on the configuration of my system,
and I am not familiar with the numpy/Python build flow.
Moreover, I could not access more platforms now,
so library/include paths should be modified accordingly.
