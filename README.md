# 🚀 CUDA Programming – Parallel Systems

This repository contains my personal notes, code examples, and practical exercises for learning parallel programming using NVIDIA CUDA.

The exercises are implemented in C/C++ with CUDA and executed in Google Colab.

## 📚 Topics Covered

- Introduction to CUDA programming
- CPU vs GPU execution
- CUDA kernels
- Threads, blocks, and grids
- CUDA memory management
- Vector addition
- Shared memory and synchronization
- Matrix operations
- Parallel reduction
- Atomic operations

## 🛠️ Technologies

- CUDA C/C++
- NVIDIA CUDA Toolkit
- Google Colab
- Jupyter Notebook
- nvcc4jupyter

## ⚙️ Getting Started

1. Open the notebook in Google Colab.
2. Navigate to `Runtime → Change runtime type`.
3. Select a GPU accelerator.
4. Install the required extension:

   ```python
   !pip install -q nvcc4jupyter
   ```

5. Load the CUDA extension:

   ```python
   %load_ext nvcc4jupyter
   ```

6. Run CUDA code using:

   ```cpp
   %%cuda

   #include <stdio.h>

   __global__ void hello() {
       printf("Hello from GPU!\n");
   }

   int main() {
       hello<<<1, 1>>>();
       cudaDeviceSynchronize();
       return 0;
   }
   ```

## 🎯 Project Goal

The goal of this repository is to develop a deeper understanding of GPU architecture, parallel algorithms, memory management, and performance optimization using NVIDIA CUDA.

The repository will be updated as I progress through new concepts and exercises.

## 📌 Status

🚧 Work in Progress – Learning CUDA.
