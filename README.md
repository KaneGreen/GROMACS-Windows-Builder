# GROMACS binary builds for Windows x64

GROMACS version: 2024.4

## Overall
- Target OS: Windows 10 or 11 (64-bit)
- Target CPU: CPUs that support AVX2 instructions
- Bundled with FFTW (3.3.10) and OpenBLAS (latest: currently 0.3.28).
- Compiled with OpenMP support, but without MPI support.

## CPU version
[![build_cpu](https://github.com/KaneGreen/GROMACS-Windows-Builder/actions/workflows/build_cpu.yml/badge.svg)](https://github.com/KaneGreen/GROMACS-Windows-Builder/actions/workflows/build_cpu.yml)  
Including both single (`gmx.exe`) and double precision (`gmx_d.exe`) versions.

## GPU version
[![build_cuda](https://github.com/KaneGreen/GROMACS-Windows-Builder/actions/workflows/build_cuda.yml/badge.svg)](https://github.com/KaneGreen/GROMACS-Windows-Builder/actions/workflows/build_cuda.yml)  
Single precision version only. Requires Nvidia CUDA 12.4.1 or higher.
