
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

	# Cuda 8.0
    apt-get -y install linux-headers-generic
    cd /tmp
	wget -nv "https://developer.nvidia.com/compute/cuda/8.0/Prod2/local_installers/cuda-repo-ubuntu1404-8-0-local-ga2_8.0.61-1_amd64-deb"
    dpkg -i cuda-repo-ubuntu1404-8-0-local-ga2_8.0.61-1_amd64-deb
	apt-key add /var/cuda-repo-8-0-local-ga2/7fa2af80.pub
                    
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

    # Cuda

	apt-get update
	apt-get -y install cuda
    export PATH=/usr/local/cuda-9.0/bin:$PATH
    export LD_LIBRARY_PATH=/usr/local/cuda-9.0/lib64:$LD_LIBRARY_PATH
    export LD_LIBRARY_PATH=/usr/lib63/nvidia:$LD_LIBRARY_PATH

	apt-get -y --ignore-missing install libcuda0-375
	apt-get -y --ignore-missing install cuda-command-line-tools-9-0
	apt-get -y --ignore-missing install cuda-core-9-0
	apt-get -y --ignore-missing install cuda-cublas-9-0
	apt-get -y --ignore-missing install cuda-cublas-dev-9-0
	apt-get -y --ignore-missing install cuda-cudart-9-0
	apt-get -y --ignore-missing install cuda-cudart-dev-9-0
	apt-get -y --ignore-missing install cuda-cufft-9-0
	apt-get -y --ignore-missing install cuda-cufft-dev-9-0
	apt-get -y --ignore-missing install cuda-curand-9-0
	apt-get -y --ignore-missing install cuda-curand-dev-9-0
	apt-get -y --ignore-missing install cuda-cusolver-9-0
	apt-get -y --ignore-missing install cuda-cusolver-dev-9-0
	apt-get -y --ignore-missing install cuda-cusparse-9-0
	apt-get -y --ignore-missing install cuda-cusparse-dev-9-0
	apt-get -y --ignore-missing install cuda-demo-suite-9-0
	apt-get -y --ignore-missing install cuda-documentation-9-0
	apt-get -y --ignore-missing install cuda-driver-dev-9-0
	apt-get -y --ignore-missing install cuda-drivers
	apt-get -y --ignore-missing install cuda-license-9-0
	apt-get -y --ignore-missing install cuda-misc-headers-9-0
	apt-get -y --ignore-missing install cuda-npp-9-0
	apt-get -y --ignore-missing install cuda-npp-dev-9-0
	apt-get -y --ignore-missing install cuda-nvgraph-9-0
	apt-get -y --ignore-missing install cuda-nvgraph-dev-9-0
	apt-get -y --ignore-missing install cuda-nvml-dev-9-0
	apt-get -y --ignore-missing install cuda-nvrtc-9-0
	apt-get -y --ignore-missing install cuda-nvrtc-dev-9-0
	apt-get -y --ignore-missing install cuda-runtime-9-0
	apt-get -y --ignore-missing install cuda-samples-9-0
	apt-get -y --ignore-missing install cuda-toolkit-9-0
	apt-get -y --ignore-missing install cuda-visual-tools-9-0  
    
