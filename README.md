oc_jpegencode_vdt
=================
This repository is fork of a fork - it is taken from [https://github.com/chiggs/oc_jpegencode](https://github.com/chiggs/oc_jpegencode),
just added Eclipse/[VDT](https://github.com/Elphel/vdt-plugin) project files, made a few other changes
so it can be imported into IDE as Eclipse project and run there.

__These Verilog source files are not related to any of Elphel camera projects.__  Doxverilog generated
[documentaion](https://github.com/Elphel/oc_jpegencode_vdt/tree/master/html) is
is browsable [here](https://cdn.rawgit.com/Elphel/oc_jpegencode_vdt/master/html/index.html).

Instructions below are preserved from the original (first fork) repo. With [VDT plugin](https://github.com/Elphel/vdt-plugin)
you need to install the plugin following the instructions and/or video tutorial, then clone this project and open it in VDT.
Then open any of the Verilog source files in the editor and change perspective:

Window -> Perspective -> Open Perspective -> Other... -> Verilog/VHDL

Icarus and Cocotb tools will be available in the bottom-left panel, under "Simulation".

Cocotb will be cloned from the official Github repository and installed when you first run the simulation from the IDE GUI.
Both Icarus simulation with traditional plain Verilog testbench and with Cocotb are supported. 

Below is the original [README.md](https://github.com/chiggs/oc_jpegencode) content

---------------------------------------

[![Documentation Status](https://readthedocs.org/projects/opencores-jpegencoder/badge/?version=latest)](http://opencores-jpegencoder.readthedocs.org/en/latest/)
[![Build Status](https://api.travis-ci.org/chiggs/oc_jpegencode.png?branch=master)](https://travis-ci.org/chiggs/oc_jpegencode)
[![Coverage Status](https://img.shields.io/coveralls/chiggs/oc_jpegencode.svg)](https://coveralls.io/r/chiggs/oc_jpegencode)

Fork of OpenCores jpegencode with Cocotb testbench. Uses the Python image library to send files through the encoder.

Original project page on Opencores: http://opencores.org/project,jpegencode

To run the testbench:

    # Pre-requisites
    sudo yum install -y python-imaging
    sudo yum install -y iverilog
    
    # Checkout git repositories
    git clone https://github.com/potentialventures/cocotb.git
    git clone https://github.com/chiggs/oc_jpegencode.git
    
    # Environment
    export COCOTB=`pwd`/cocotb
    
    # Run the tests...
    cd oc_jpegencode/tb
    make

[Documentation](http://opencores-jpegencoder.readthedocs.org/en/latest/) hosted on [ReadTheDocs](https://readthedocs.org/).
