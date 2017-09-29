# MANUAL

Bootstrap: debootstrap
OSVersion: trusty  
MirrorURL: http://us.archive.ubuntu.com/ubuntu/

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
    apt-get -y install dkms
    apt-get -y install linux-headers-generic

    # Cuda 8.0
    echo $'blacklist nouveau\noptions nouveau modeset=0' > /etc/modprobe.d/blacklist-nouveau.conf
    update-initramfs -u
	wget -nv "https://developer.nvidia.com/compute/cuda/8.0/Prod2/local_installers/cuda_8.0.61_375.26_linux-run"
    sh cuda_8.0.61_375.26_linux.run
    export PATH=/usr/local/cuda-8.0/bin:$PATH
    export LD_LIBRARY_PATH=/usr/local/cuda-8.0/lib64:$LD_LIBRARY_PATH
    export LD_LIBRARY_PATH=/usr/lib64/nvidia:$LD_LIBRARY_PATH

                
	# OpenCL
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
