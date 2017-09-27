
Bootstrap: debootstrap
OSVersion: trusty  
MirrorURL: http://us.archive.ubuntu.com/ubuntu/

%post

    apt-get update
    apt-get -y install build-essential
    apt-get -y install make
    apt-get -y install cmake
	apt-get -y install wget
    apt-get -y install flex
    apt-get -y install automake
    apt-get -y install autoconf
    apt-get -y install autotools-dev
    apt-get -y install libtool

	# Cuda 8.0

    apt-get -y install linux-headers-generic
	wget -q "https://developer.nvidia.com/compute/cuda/8.0/Prod2/local_installers/cuda-repo-ubuntu1404-8-0-local-ga2_8.0.61-1_amd64-deb"   
	dpkg -i cuda-repo-ubuntu1404-8-0-local-ga2_8.0.61-1_amd64.deb
	apt-key add /var/cuda-repo-<version>/7fa2af80.pub
	apt-get update
	apt-get -y install cuda

	apt-get -y --ignore-missing install libcuda1-375
	apt-get -y --ignore-missing install cuda-8-0
	apt-get -y --ignore-missing install cuda-command-line-tools-8-0
	apt-get -y --ignore-missing install cuda-core-8-0
	apt-get -y --ignore-missing install cuda-cublas-8-0
	apt-get -y --ignore-missing install cuda-cublas-dev-8-0
	apt-get -y --ignore-missing install cuda-cudart-8-0
	apt-get -y --ignore-missing install cuda-cudart-dev-8-0
	apt-get -y --ignore-missing install cuda-cufft-8-0
	apt-get -y --ignore-missing install cuda-cufft-dev-8-0
	apt-get -y --ignore-missing install cuda-curand-8-0
	apt-get -y --ignore-missing install cuda-curand-dev-8-0
	apt-get -y --ignore-missing install cuda-cusolver-8-0
	apt-get -y --ignore-missing install cuda-cusolver-dev-8-0
	apt-get -y --ignore-missing install cuda-cusparse-8-0
	apt-get -y --ignore-missing install cuda-cusparse-dev-8-0
	apt-get -y --ignore-missing install cuda-demo-suite-8-0
	apt-get -y --ignore-missing install cuda-documentation-8-0
	apt-get -y --ignore-missing install cuda-driver-dev-8-0
	apt-get -y --ignore-missing install cuda-drivers
	apt-get -y --ignore-missing install cuda-license-8-0
	apt-get -y --ignore-missing install cuda-misc-headers-8-0
	apt-get -y --ignore-missing install cuda-npp-8-0
	apt-get -y --ignore-missing install cuda-npp-dev-8-0
	apt-get -y --ignore-missing install cuda-nvgraph-8-0
	apt-get -y --ignore-missing install cuda-nvgraph-dev-8-0
	apt-get -y --ignore-missing install cuda-nvml-dev-8-0
	apt-get -y --ignore-missing install cuda-nvrtc-8-0
	apt-get -y --ignore-missing install cuda-nvrtc-dev-8-0
	apt-get -y --ignore-missing install cuda-repo-ubuntu1404
	apt-get -y --ignore-missing install cuda-runtime-8-0
	apt-get -y --ignore-missing install cuda-samples-8-0
	apt-get -y --ignore-missing install cuda-toolkit-8-0
	apt-get -y --ignore-missing install cuda-visual-tools-8-0  

	export PATH=/usr/local/cuda-8.0/bin${PATH:+:${PATH}}
	export LD_LIBRARY_PATH=/usr/local/cuda-8.0/lib64\
                         ${LD_LIBRARY_PATH:+:${LD_LIBRARY_PATH}}

	# OpenCL

    apt-get -y install nvidia-opencl-dev
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

