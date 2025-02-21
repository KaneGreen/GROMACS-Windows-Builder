# GROMACS binary builds for Windows x64

GROMACS version: 2025.0

## Overall
- Target OS: Microsoft Windows 10 or 11 (64-bit).
- Target CPU: CPUs that support AVX2 instructions.
- Bundled with [FFTW (3.3.10)](https://fftw.org), [OpenBLAS (0.3.28)](https://www.openblas.net/) and [hwloc](https://www.open-mpi.org/projects/hwloc/).
- Compiled with OpenMP support, but without MPI support.
- Extra force fields: [CHARMM36 (July 2022)](https://mackerell.umaryland.edu/charmm_ff.shtml#gromacs)

## CPU version
[![build_cpu](https://github.com/KaneGreen/GROMACS-Windows-Builder/actions/workflows/build_cpu.yml/badge.svg)](https://github.com/KaneGreen/GROMACS-Windows-Builder/actions/workflows/build_cpu.yml)  
Including both single (`gmx.exe`) and double precision (`gmx_d.exe`) versions.

## GPU version
[![build_cuda](https://github.com/KaneGreen/GROMACS-Windows-Builder/actions/workflows/build_cuda.yml/badge.svg)](https://github.com/KaneGreen/GROMACS-Windows-Builder/actions/workflows/build_cuda.yml)  
Single precision version only. Nvidia Windows driver (version 561.17 or higher) which supports Nvidia CUDA 12.6.3 or higher are required.
