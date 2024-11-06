# Download the Poky Source code using this git repository 

$ git clone git://git.yoctoproject.org/poky

# Prepare the build environment, Poky provides you a script 'oe-init-build-env', which should be used to setup the build environment

$ source poky/oe-init-build-env [build_directory]
# after that we can see "conf" file and open that file usin this command
$ vi conf/local.conf

# and modify configuration as per our software and hardware requirments
# so, in my case i am developing "beaglebone-yocto" build images 
edit  
and comment "#MACHINE= qemu_x86"
# and it will be modifies as per our requrments.
# back to our build directory. and, build Images using commant:
$ bitbake cor-image-minimal.
