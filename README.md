CUDA Installation:
!apt-get update
!apt-get install -y build-essential
!apt-get install -y nvidia-cuda-toolkit

sudo apt update
sudo apt install -y nvidia-cuda-toolkit

!nvcc -arch=sm_75 -o matmull matmull.cu
!./matmull

!nvcc -o vector_add vector_add.cu
!nvcc -arch=sm_75 -o vector_add vector_add.cu
!./vector_add

Terminal Command:
sudo apt update
sudo apt install g++
gedit filename.cpp
g++ -fopenmp filename.cpp -o filename
./filename
