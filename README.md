# Android Studio 	ools/base - Native Windows ARM64 Port

This repository contains the patch and modified Bazel toolchain configuration files required to build **Android Studio** natively on **Windows 11 ARM64** (Snapdragon X Elite, Snapdragon X Plus, and other ARM64 Windows platforms).

## Upstream Target
- **Upstream Tag / Branch**: studio-rabbit1-release (	ools/base)
- **Base Commit**: 4a5d2ec9

## Modifications Overview
- Added Windows ARM64 platform constraints and @platforms//os:windows + @platforms//cpu:arm64 toolchain mappings.
- Configured native MSVC ARM64 toolchains and cross-compilation flags in platform_specific.bazelrc and platforms/BUILD.
- Patched Bazel toolchain module dependencies (zlmod/toolchains.MODULE.bazel) for ARM64 Windows execution.

## Application
To apply the changes directly onto upstream AOSP 	ools/base:
`ash
git apply 0001-windows-arm64-port.patch
`
