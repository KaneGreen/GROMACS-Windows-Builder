# GROMACS binary build for Windows x64

## Overall
- Target OS: Windows 10 or 11 (64-bit)
- Target CPU: CPUs that support AVX2 instructions
- Bundled with FFTW (3.3.10) and OpenBLAS (latest: currently 0.3.28).
- Compiled With OpenMP support, but without MPI support.

## CPU version
Includes both single (gmx.exe) and double (gmx_d.exe) precision versions.

## GPU version
Single precision version only. Requires Nvidia CUDA 12.4.1.
