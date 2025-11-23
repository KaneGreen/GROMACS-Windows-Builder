# GROMACS binary builds for Windows x64

[GROMACS version](https://manual.gromacs.org/current/download.html): 2025.4

## Overall
- Target OS: Microsoft Windows 10 or 11 (64-bit).
- Target CPU: x84_64 CPUs that support AVX2 instructions.
- Bundled with [FFTW (3.3.10)](https://fftw.org), [OpenBLAS (0.3.30)](https://www.openblas.net/) and [hwloc (2.12.2)](https://www.open-mpi.org/projects/hwloc/).
- Compiled with OpenMP support, but without MPI support.
- Extra force fields: [CHARMM36 (July 2022)](https://mackerell.umaryland.edu/charmm_ff.shtml#gromacs)

## CPU version
[![build_cpu](https://github.com/KaneGreen/GROMACS-Windows-Builder/actions/workflows/build_cpu.yml/badge.svg)](https://github.com/KaneGreen/GROMACS-Windows-Builder/actions/workflows/build_cpu.yml)  
Including both single (`gmx.exe`) and double precision (`gmx_d.exe`) versions.

## GPU version
[![build_cuda](https://github.com/KaneGreen/GROMACS-Windows-Builder/actions/workflows/build_cuda.yml/badge.svg)](https://github.com/KaneGreen/GROMACS-Windows-Builder/actions/workflows/build_cuda.yml)  
Single precision version only.  
Nvidia Windows driver (version 572.61 or higher) which supports Nvidia CUDA 12.8.1 or higher is required.

## Patches
The following unmerged PRs of vcpkg registry are introduced to improve the dependency versions:
* OpenBLAS: https://github.com/microsoft/vcpkg/pull/46118
* hwloc: https://github.com/microsoft/vcpkg/pull/47719
* The flag `-DBUILD_WITHOUT_LAPACK=ON` has been removed from OpenBLAS.

## For those who fork this repository
Compiling GROMACS with the MSVC toolchain is very time-consuming, so please **do not abuse GitHub Actions**.
