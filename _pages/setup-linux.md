---
layout: page
title: CIS 565 - Setup instructions for your Windows PC
description: >
  This page provides instructions for setting up your Windows PC for CIS 565
hide_description: true
permalink: /setup-linux/
---

## Setup your Linux Computer

Follow this guide to setup your personal Linux computer.

This guide assumes that you have root access to your computer.

0. **Install basic C/C++ compilation tools** (gcc, g++, make etc.) installed. For Debian/Ubuntu, we recommend the `build-essential` package.
1. Install **`git`** using package manager. Example `sudo apt install git` on Debian/Ubuntu.
    * After installation, follow the [**First Time Git Setup**](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup) Guide if this is the first time you are using Git.
2. Install [**CUDA 11**](https://developer.nvidia.com/cuda-downloads). You can either use the downloaded version or your package manager. Install the NVIDIA Driver if it is newer than the installed version. Make sure you also install Nsight.
3. Install **CMake** (`sudo apt install cmake` on Debian/Ubuntu).
4. Install **glfw** and **glew** (`apt install libglfw3-dev libglew-dev` on Debian/Ubuntu).
5. (_Recommended_) Nsight is a debugging and profiling tool shipped with CUDA. We recommend adding the CUDA executables to your `PATH` using `export PATH=/usr/local/cuda/bin/:${PATH}`. Note that using the `export` command is a temporary change through the life of the terminal. For permanent change, add it to your shell configuration file, e.g. `~/.bashrc` on Ubuntu). You can run then run Nsight by typing `nsight` in your terminal.

[Back to Setup](/setup/)