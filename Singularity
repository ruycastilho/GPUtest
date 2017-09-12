# Image for GPU testing 
# Ubuntu 14.04 - Running on Krueger
# OpenCL
# /09/2017


# Header

Bootstrap: docker
From: ubuntu:14.04

# Sections

%runscript

exec echo Hello "S@"
exec echo $'OS Version - Ubuntu 14.04\n'

%post

    # General
    sudo apt-get update
    apt-get -y install build-essential
    apt-get -y install git
    apt-get -y install cmake
    apt-get -y install g++
    apt-get -y install vim 
    apt-get -y install python3-pip
    
    #OpenCL
    
    #apt-get -y install ocl-icd-opencl-dev
    
    # OpenMPI
    apt-get -y install libopenmpi-dev
    apt-get -y install libopenmpi1.6
    apt-get -y install openmpi-bin
    apt-get -y install openmpi-common
    apt-get -y install openmpi-doc

