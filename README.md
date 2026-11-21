# GROMACS binary builds for Windows x64

[GROMACS version](https://manual.gromacs.org/current/download.html): 2026.4

## Overall
- Target OS: Microsoft Windows 10 or 11 (64-bit).
- Target CPU: x84_64 CPUs that support AVX2 instructions.
- Bundled with [FFTW (3.3.11)](https://fftw.org), [OpenBLAS (0.3.34)](https://www.openmathlib.org/OpenBLAS/) and [hwloc (2.15.0)](https://www.open-mpi.org/projects/hwloc/).
- Compiled with OpenMP support, but without MPI support.
- Extra force fields: [CHARMM36 (February 2026)](https://mackerell.umaryland.edu/charmm_ff.shtml#gromacs)

## CPU version
[![build_cpu](https://github.com/KaneGreen/GROMACS-Windows-Builder/actions/workflows/build_cpu.yml/badge.svg)](https://github.com/KaneGreen/GROMACS-Windows-Builder/actions/workflows/build_cpu.yml)  
Including both single (`gmx.exe`) and double precision (`gmx_d.exe`) versions.

## GPU version
[![build_cuda](https://github.com/KaneGreen/GROMACS-Windows-Builder/actions/workflows/build_cuda.yml/badge.svg)](https://github.com/KaneGreen/GROMACS-Windows-Builder/actions/workflows/build_cuda.yml)  
Single precision version only.  
Nvidia Windows driver (version 610.88 or higher) which supports Nvidia CUDA 13.3.1 or higher is required. **It is strongly recommended to install the latest supported GPU driver.**

## Patches
The following unmerged PRs of vcpkg registry are introduced to improve the dependency versions:
* The flag `-DBUILD_WITHOUT_LAPACK=ON` has been removed from OpenBLAS.

## For those who fork this repository
Compiling GROMACS with the MSVC toolchain is very time-consuming, so please **do not abuse GitHub Actions**.
