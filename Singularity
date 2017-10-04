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

    # OpenCL	
	apt-get -y install opencl-headers
	apt-get -y install opencv-doc
	apt-get -y install python-opencv
	apt-get -y install libopencv-calib3d-dev:amd64
	apt-get -y install libopencv-calib3d2.4:amd64
	apt-get -y install libopencv-contrib2.4:amd64
	apt-get -y install libopencv-core-dev:amd64
	apt-get -y install libopencv-core2.4:amd64
	apt-get -y install libopencv-features2d-dev:amd64
	apt-get -y install libopencv-features2d2.4:amd64
	apt-get -y install libopencv-highgui-dev:amd64
	apt-get -y install libopencv-highgui2.4:amd64
	apt-get -y install libopencv-imgproc-dev:amd64
	apt-get -y install libopencv-imgproc2.4:amd64
	apt-get -y install libopencv-legacy-dev:amd64
	apt-get -y install libopencv-legacy2.4:amd64
	apt-get -y install libopencv-ml-dev:amd64
	apt-get -y install libopencv-ml2.4:amd64
	apt-get -y install libopencv-objdetect-dev:amd64
	apt-get -y install libopencv-objdetect2.4:amd64
	apt-get -y install libopencv-ocl-dev:amd64
	apt-get -y install libopencv-ocl2.4:amd64
	apt-get -y install libopencv-photo2.4:amd64
	apt-get -y install libopencv-video-dev:amd64
	apt-get -y install libopencv-video2.4:amd64
	apt-get -y install ocl-icd-libopencl1:amd64
    apt-get -y install ocl-icd-opencl-dev
    apt-get -y install clinfo
    apt-get -y install nvidia-opencl-icd-375

    # Nvidia
#    wget -q "http://us.download.nvidia.com/XFree86/Linux-x86_64/375.26/NVIDIA-Linux-x86_64-375.26.run"
#    chmod 777 NVIDIA-Linux-x86_64-375.26.run
#    ./NVIDIA-Linux-x86_64-375.26.run    
#    apt-get update
#    apt-get upgrade


    # OpenMP
    #apt-get update
    apt-get -y install openmpi-bin
    apt-get -y install openmpi-doc
    apt-get -y install libopenmpi-dev
