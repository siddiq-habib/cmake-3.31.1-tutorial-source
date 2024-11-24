This directory contains source code examples for the CMake Tutorial.
Each step has its own subdirectory containing code that may be used as a
starting point. The tutorial examples are progressive so that each step
provides the complete solution for the previous step.

####################################################################
#Config/Build can be done as follows from the root Folder

#Example 1: with libary MathFunctions

cmake -S ./Step2 -B ./build/Step2 -DUSE_MYMATH=ON
make -C ./build/Step2

#Exectuion of binary for the above build generation
./build/Step2/Tutorial 10

#Expected result
The square root of 10 is 3.16228

======================================================================
#Example 2: with mathlib library

cmake -S ./Step2 -B ./build/Step2 -DUSE_MYMATH=OFF
make -C ./build/Step2

#Exectuion of binary for the above build generation
./build/Step2/Tutorial 10

#Expected result
Computing sqrt of 10 to be 5.5
Computing sqrt of 10 to be 3.65909
Computing sqrt of 10 to be 3.19601
Computing sqrt of 10 to be 3.16246
Computing sqrt of 10 to be 3.16228
Computing sqrt of 10 to be 3.16228
Computing sqrt of 10 to be 3.16228
Computing sqrt of 10 to be 3.16228
Computing sqrt of 10 to be 3.16228
Computing sqrt of 10 to be 3.16228
The square root of 10 is 3.16228
####################################################################
