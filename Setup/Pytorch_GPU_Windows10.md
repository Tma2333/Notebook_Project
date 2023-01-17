# Setup
Written 2023/1/17
## 1. (Optional) Install MSVC C++ build tool
This is only necessary to build from source. This is also necessary for Tensorflow setup. 

You can download the Free VS community version in here: https://visualstudio.microsoft.com/vs/community/

Select the appropriate components, or just select **Desktop development with C++**. You can always come back for more components. 

![alt text](https://raw.githubusercontent.com/Tma2333/Notebook_Project/main/Setup/imgs/msvs_install_0.png)

**Restart after installing the MSVC**

## 2. Install CUDA Toolkit 
You can find all version of CUDA in CUDA Toolkit Archive here: https://developer.nvidia.com/cuda-toolkit-archive

Find the corresponding version you want to install with Pytorch. 

Here is an example for CUDA 11.6

![alt text](https://raw.githubusercontent.com/Tma2333/Notebook_Project/main/Setup/imgs/cuda_install_11_6.png)

Follow the instruction in installer. Choose the Express. 

![alt text](https://raw.githubusercontent.com/Tma2333/Notebook_Project/main/Setup/imgs/cuda_install_11_6_installer_0.png)

You need cuDNN if you want to compile from source. 
## 3. Install Anaconda

Install Anacodna here: https://www.anaconda.com/ and follow the instruction.

## 4. Install Pytorch

You can find install command here: https://pytorch.org/get-started/locally/

## 5. Verify

```
import torch

>>> torch.cuda.is_available()
True

>>> torch.cuda.device_count()
1

>>> torch.cuda.current_device()
0

>>> torch.cuda.device(0)
<torch.cuda.device at 0x243764c97c0>

>>> torch.cuda.get_device_name(0)
'NVIDIA GeForce RTX 4090'
```
