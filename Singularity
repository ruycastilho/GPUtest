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
    apt-get -y install atool

    # Cuda 8.0
    wget -q "http://us.download.nvidia.com/XFree86/Linux-x86_64/384.90/NVIDIA-Linux-x86_64-384.90.run"
    echo $'blacklist vga16fb\nblacklist nouveau\noptions nouveau modeset=0' > /etc/modprobe.d/blacklist-nouveau.conf
    service lightdm stop
    apt-get -y --purge remove nvidia-*
    service gdm stop
    apt-get -y --purge remove xserver-xorg-video-nouveau-lts-quantal
    #reboot
    ./NVIDIA-Linux-x86_64-384.90.run
    nvidia-xconfig
    service gdm start
    CUDA_REPO_PKG=cuda-repo-ubuntu1404-8-0-local-ga2_8.0.61-1_amd64.deb
    wget -q "https://developer.nvidia.com/compute/cuda/8.0/Prod2/local_installers/cuda-repo-ubuntu1404-8-0-local-ga2_8.0.61-1_amd64-deb" -O /tmp/${CUDA_REPO_PKG}
    dpkg -i /tmp/${CUDA_REPO_PKG} 
    rm -f /tmp/${CUDA_REPO_PKG} 
 
    ML_REPO_PKG=nvidia-machine-learning-repo-ubuntu1404_4.0-2_amd64.deb 
    wget -q http://developer.download.nvidia.com/compute/machine-learning/repos/ubuntu1404/
 x86_64/${ML_REPO_PKG} -O /tmp/${ML_REPO_PKG} 
    dpkg -i /tmp/${ML_REPO_PKG} 
    rm -f /tmp/${ML_REPO_PKG} 
  
    apt-get update
    apt-get -y install digits cuda


#    update-initramfs -u
#	wget -nv "https://developer.nvidia.com/compute/cuda/8.0/Prod2/local_installers/cuda_8.0.61_375.26_linux-run"
#    sh cuda_8.0.61_375.26_linux-run
#    export PATH=/usr/local/cuda-8.0/bin:$PATH
#    export LD_LIBRARY_PATH=/usr/local/cuda-8.0/lib64:$LD_LIBRARY_PATH
#    export LD_LIBRARY_PATH=/usr/lib64/nvidia:$LD_LIBRARY_PATH

                
	# OpenCL
   
    wget -q "http://registrationcenter-download.intel.    com/akdlm/irc_nas/vcp/11705/intel_sdk_for_opencl_2017_7.0.0.2511_x64.tgz"
    aunpack intel_sdk_for_opencl_2017_7.0.0.2511_x64.tgz
    cd intel_sdk_for_opencl_2017_7.0.0.2511_x64/
    ./install_GUI.sh

    wget -q "http://registrationcenter-download.intel.com/akdlm/irc_nas/9019/opencl_runtime_16.1.1_x64_ubuntu_6.4.0.25.tgz"
    aunpack opencl_runtime_16.1.1_x64_ubuntu_6.4.0.25.tgz
    cd opencl_runtime_16.1.1_x64_ubuntu_6.4.0.25/
    ./install.sh
    #apt-get -y install opencl-headers
    #apt-get -y install ocl-icd-libopencl1:amd64
    #apt-get -y install oc l-icd-opencl-dev
    #apt-get -y install clinfo
    #apt-get -y install nvidia-opencl-icd-375
