# sge_hybrid
This is a hybrid version of grid engine forked from "Son of grid engine"
# Installing CMake last version 
wget https://github.com/Kitware/CMake/releases/download/v3.19.2/cmake-3.19.2.tar.gz
sh ./bootstrap && make && sudo make install
tar -xfvz cmake-3.19.2.tar.gz
rm cmake-3.19.2.tar.gz
# Running bootstrap.sh to compile without java
sh scripts/bootstrap.sh -no-java -no-jni

# Recommendations
## change the following variable in the file version.c in the directory: /opt/sge/source/libs/gdi/
file	 : /opt/sge/source/libs/gdi/version.c
//const char GDI_VERSION[] = GIT_REPO_VERSION;
const char GDI_VERSION[] = "r20.556adb4";

# setting the root directory the SGE_ROOT=/opt/sge

export SGE_ROOT=/opt/sge
