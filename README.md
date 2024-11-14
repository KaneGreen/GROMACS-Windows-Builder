# GROMACS binary build for Windows x64

## Overall
- Target OS: Windows 10 or 11 (64-bit)
- Target CPU: CPUs that support AVX2
- Bundled: FFTW (3.3.10) and OpenBLAS (lastest: currently 0.3.28)
- No MPI and no OpenMP.

## CPU version
Includes both single (gmx.exe) and double (gmx_d.exe) precision versions.

## GPU version
Single precision version only. Requires Nvidia CUDA 12.4.1.
