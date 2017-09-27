Bootstrap: docker
From: nvidia/cuda:8.0-runtime-ubuntu14.04

%post

    apt-get update
    apt-get -y install build-essential
    apt-get -y install make
    apt-get -y install cmake
	apt-get -y install wget
    apt-get -y --ignore-missing install flex
    apt-get -y --ignore-missing install automake
    apt-get -y --ignore-missing install autoconf
    apt-get -y --ignore-missing install autotools-dev
    apt-get -y --ignore-missing install libtool
 
    apt-get -y install nvidia-opencl-dev
    apt-get -y install linux-headers-$(uname -r)
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

