# Automatic

Bootstrap: docker
From: nvidia/cuda:8.0-runtime-ubuntu14.04

%post

    apt-get update
    apt-get -y install build-essential
    apt-get -y install apt-utils
    apt-get -y install make
    apt-get -y install cmake
	apt-get -y install wget
    apt-get -y install flex
    apt-get -y install automake
    apt-get -y install autoconf
    apt-get -y install autotools-dev
    apt-get -y install libtool
    apt-get -y install gcc
    export TERM=xterm

    # OpenCL	

    wget -q "http://registrationcenter-download.intel.com/akdlm/irc_nas/vcp/11705/intel_sdk_for_opencl_2017_7.0.0.2511_x64.tgz"
    tar -zxvf intel_sdk_for_opencl_2017_7.0.0.2511_x64.tgz
    cd intel_sdk_for_opencl_2017_7.0.0.2511_x64/
    chmod +x install_GUI.sh
    ./install_GUI.sh -s

    wget -q "http://registrationcenter-download.intel.com/akdlm/irc_nas/9019/opencl_runtime_16.1.1_x64_ubuntu_6.4.0.25.tgz"
    tar -zxvf opencl_runtime_16.1.1_x64_ubuntu_6.4.0.25.tgz
    cd opencl_runtime_16.1.1_x64_ubuntu_6.4.0.25/
    chmod +x install.sh
    ./install.sh -s

    apt-get -y install clinfo


    # OpenMP
    apt-get -y install openmpi-bin
    apt-get -y install openmpi-doc
    apt-get -y install libopenmpi-dev
