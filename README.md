oc_jpegencode
=============
This repository is for of a fork - it is taken from [https://github.com/chiggs/oc_jpegencode](https://github.com/chiggs/oc_jpegencode),
just added Eclipse/[VDT](https://github.com/Elphel/vdt-plugin) project files so it can be imported into IDE and run there.

__These Verilog source files are not related to any of Elphel camera projects.__

Instructions below are preserved from the original (first fork) repo. With [VDT plugin](https://github.com/Elphel/vdt-plugin) you need
to install the plugin following the instructions and/or video tutorial, then clone this project and open it in VDT. Cocotb
will be cloned and installed when you first run the simulation from the IDE GUI. Both Icarus simulation with traditional plain
Verilog testbench and with Cocotb are supported. 

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
