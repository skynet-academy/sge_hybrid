# sge_hybrid
This is a hybrid version of grid engine forked from "Son of grid engine"
# Installing CMake last version 
wget https://github.com/Kitware/CMake/releases/download/v3.19.2/cmake-3.19.2.tar.gz
sh ./bootstrap && make && sudo make install
tar -xfvz cmake-3.19.2.tar.gz
rm cmake-3.19.2.tar.gz
# Running bootstrap.sh to compile without java
sh scripts/bootstrap.sh -no-java -no-jni
