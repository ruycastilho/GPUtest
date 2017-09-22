# Image for GPU testing 
# Ubuntu 14.04 - Running on Jason
# 21/09/2017

# Header

Bootstrap: debootstrap
OSVersion: trusty
MirrorURL: http://us.archive.ubuntu.com/ubuntu/

# Sections
    
%post
    apt-get update
    apt-get -y install software-properties-common
    add-apt-repository universe 
    apt-get -y install build-essential  
	apt-get -y --ignore-missing install curl
	apt-get -y --ignore-missing install cmake
	apt-get -y --ignore-missing install make
	apt-get -y --ignore-missing install ftp
	apt-get -y --ignore-missing install fuse
	apt-get -y --ignore-missing install g++
	apt-get -y --ignore-missing install gcc
	apt-get -y --ignore-missing install gcc-4.8
	apt-get -y --ignore-missing install gcc-4.8-base:amd64
	apt-get -y --ignore-missing install gcc-4.9-base:amd64
	
    apt-get -y --ignore-missing install linux-headers-$(uname -r)
    
	apt-get -y --ignore-missing install nvidia-375
	apt-get -y --ignore-missing install nvidia-375-dev
	apt-get -y --ignore-missing install nvidia-machine-learning-repo-ubuntu1404
	apt-get -y --ignore-missing install nvidia-modprobe
	apt-get -y --ignore-missing install nvidia-opencl-icd-375
	apt-get -y --ignore-missing install nvidia-prime
	apt-get -y --ignore-missing install nvidia-profiler
	apt-get -y --ignore-missing install nvidia-visual-profiler
	apt-get -y --ignore-missing install nvidia-settings
	
	apt-get -y --ignore-missing install opencl-headers
	apt-get -y --ignore-missing install opencv-doc
	apt-get -y --ignore-missing install python-opencv
	apt-get -y --ignore-missing install libopencv-calib3d-dev:amd64
	apt-get -y --ignore-missing install libopencv-calib3d2.4:amd64
	apt-get -y --ignore-missing install libopencv-contrib2.4:amd64
	apt-get -y --ignore-missing install libopencv-core-dev:amd64
	apt-get -y --ignore-missing install libopencv-core2.4:amd64
	apt-get -y --ignore-missing install libopencv-features2d-dev:amd64
	apt-get -y --ignore-missing install libopencv-features2d2.4:amd64
	apt-get -y --ignore-missing install libopencv-flann-dev:amd64ls
	apt-get -y --ignore-missing install libopencv-flann2.4:amd64
	apt-get -y --ignore-missing install libopencv-highgui-dev:amd64
	apt-get -y --ignore-missing install libopencv-highgui2.4:amd64
	apt-get -y --ignore-missing install libopencv-imgproc-dev:amd64
	apt-get -y --ignore-missing install libopencv-imgproc2.4:amd64
	apt-get -y --ignore-missing install libopencv-legacy-dev:amd64
	apt-get -y --ignore-missing install libopencv-legacy2.4:amd64
	apt-get -y --ignore-missing install libopencv-ml-dev:amd64
	apt-get -y --ignore-missing install libopencv-ml2.4:amd64
	apt-get -y --ignore-missing install libopencv-objdetect-dev:amd64
	apt-get -y --ignore-missing install libopencv-objdetect2.4:amd64
	apt-get -y --ignore-missing install libopencv-ocl-dev:amd64
	apt-get -y --ignore-missing install libopencv-ocl2.4:amd64
	apt-get -y --ignore-missing install libopencv-photo2.4:amd64
	apt-get -y --ignore-missing install libopencv-video-dev:amd64
	apt-get -y --ignore-missing install libopencv-video2.4:amd64
	apt-get -y --ignore-missing install ocl-icd-libopencl1:amd64
    apt-get -y --ignore-missing install ocl-icd-opencl-dev

	apt-get -y --ignore-missing install python
	apt-get -y --ignore-missing install python-apt
	apt-get -y --ignore-missing install python-apt-common
    apt-get -y --ignore-missing install wget
    apt-get -y --ignore-missing install flex
    apt-get -y --ignore-missing install automake
    apt-get -y --ignore-missing install autoconf
    apt-get -y --ignore-missing install autotools-dev
    apt-get -y --ignore-missing install libtool
    apt-get -y --ignore-missing install git  

    apt-get -y --ignore-missing install python2.7
	apt-get -y --ignore-missing install python2.7-dev
	apt-get -y --ignore-missing install python2.7-minimal
	apt-get -y --ignore-missing install python3
	apt-get -y --ignore-missing install python3-apport
	apt-get -y --ignore-missing install python3-apt
	apt-get -y --ignore-missing install python-pip
	apt-get -y --ignore-missing install python3-pip
	apt-get -y --ignore-missing install vim
	apt-get -y --ignore-missing install vim-common
	apt-get -y --ignore-missing install vim-runtime
	apt-get -y --ignore-missing install vim-tiny
    
	apt-get -y --ignore-missing install libopenmpi1.6
	
	apt-get -y --ignore-missing install libpython-dev:amd64
	apt-get -y --ignore-missing install libpython-stdlib:amd64
	apt-get -y --ignore-missing install libpython2.7:amd64
	apt-get -y --ignore-missing install libpython2.7-dev:amd64
	apt-get -y --ignore-missing install libpython2.7-minimal:amd64
	apt-get -y --ignore-missing install libpython2.7-stdlib:amd64
	apt-get -y --ignore-missing install libpython3-dev:amd64
	apt-get -y --ignore-missing install libpython3-stdlib:amd64
	apt-get -y --ignore-missing install libpython3.4:amd64
	apt-get -y --ignore-missing install libpython3.4-dev:amd64
	apt-get -y --ignore-missing install libpython3.4-minimal:amd64
	apt-get -y --ignore-missing install libpython3.4-stdlib:amd64


