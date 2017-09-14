# Image for GPU testing 
# Ubuntu 14.04 - Running on Krueger
# OpenCL
# 12/09/2017


# Header

Bootstrap: debootstrap
OSVersion: trusty
MirrorURL: http://us.archive.ubuntu.com/ubuntu/

# Sections

%runscript

exec echo Hello "S@"
exec echo $'OS Version - Ubuntu 14.04\n'

%post

    # General
    apt-get update
    apt-get -y install build-essential
    apt-get -y install git
    apt-get -y install cmake
    apt-get -y install g++
    apt-get -y install vim 
    apt-get -y install wget
    	
    #Seismic Unix
    
    mkdir -p ~/cwp/43R1
	cd ~/cwp/43R1
	wget ftp://ftp.cwp.mines.edu/pub/cwpcodes/cwp_su_all_43R1.tgz
	tar -zxvf cwp_su_all_43R1.tgz
	echo "export CWPROOT=~/cwp/43R1" >> ~/.bashrc
	echo "export PATH=$PATH:~/cwp/43R1/bin" >> ~/.bashrc
	source ~/.bashrc
	cd $CWPROOT/src
	make install
	sudo apt-get install libx11-dev
	sudo apt-get install libxt-dev
	sudo apt-get install gfortran
	make finstall
	make xtinstall
	make sfinstall 

	
    #OpenCL
    apt-get install ocl-icd-opencl-dev
    
    #apt	-get -y install ocl-icd-opencl-dev
    
    # OpenMPI
    apt-get -y install libopenmpi-dev
    apt-get -y install libopenmpi1.6
    apt-get -y install openmpi-bin
    apt-get -y install openmpi-common
    apt-get -y install openmpi-doc

