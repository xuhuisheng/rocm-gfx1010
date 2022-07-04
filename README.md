
# ROCm with gfx1010

This repo upload some archieves for ROCm with gfx1010.

## ROCm-5.2.0

|OS            |linux|Python|ROCm |GPU     |
|--------------|-----|------|-----|--------|
|Ubuntu-20.04.4|5.13 |3.8.10|5.2.0|RX5700XT|

<https://github.com/xuhuisheng/rocm-gfx1010/releases/tag/rocm520>

Install ROCm First <https://docs.amd.com/bundle/ROCm-Installation-Guide-v5.2/page/Overview_of_ROCm_Installation_Methods.html>

|component  |version   |size   |link|
|-----------|----------|-------|----|
|rocblas    |2.44.0    |9.0M   |<https://github.com/xuhuisheng/rocm-gfx1010/releases/download/rocm520/rocblas_2.44.0.50200-65_amd64.deb>|
|rocfft     |1.0.17    |69M    |<https://github.com/xuhuisheng/rocm-gfx1010/releases/download/rocm520/rocfft_1.0.17.50200-65_amd64.deb>|
|rocrand    |2.10.9    |9.1M   |<https://github.com/xuhuisheng/rocm-gfx1010/releases/download/rocm520/rocrand_2.10.9.50200-65_amd64.deb>|
|rocsparse  |2.2.0     |8.9M   |<https://github.com/xuhuisheng/rocm-gfx1010/releases/download/rocm520/rocsparse_2.2.0.50200-65_amd64.deb>|
|rccl       |2.11.4    |9.8M   |<https://github.com/xuhuisheng/rocm-gfx1010/releases/download/rocm520/rccl_2.11.4.50200-65_amd64.deb>|
|pytorch    |1.12.0    |145.14M|<https://github.com/xuhuisheng/rocm-gfx1010/releases/download/rocm520/torch-1.12.0a0+git67ece03-cp38-cp38-linux_x86_64.whl>
|torchvision|0.13.0    |18.47M |<https://github.com/xuhuisheng/rocm-gfx1010/releases/download/rocm520/torchvision-0.13.0a0+da3794e-cp38-cp38-linux_x86_64.whl>
|tensorflow |2.9.2     |300.22M|<https://github.com/xuhuisheng/rocm-gfx1010/releases/download/rocm520/tf_nightly_rocm-2.9.2-cp38-cp38-linux_x86_64.whl>|

1. Install ROCm-5.2.0
2. `sudo dpkg -i rocblas_2.44.0.50200-65_amd64.deb`
2. `sudo dpkg -i rocfft_1.0.17.50200-65_amd64.deb`
2. `sudo dpkg -i rocrand_2.10.9.50200-65_amd64.deb`
2. `sudo dpkg -i rocsparse_2.2.0.50200-65_amd64.deb`
2. `sudo dpkg -i rccl_2.11.4.50200-65_amd64.deb`
3. `pip3 install torch-1.12.0a0+git67ece03-cp38-cp38-linux_x86_64.whl`
4. `pip3 install torchvision-0.13.0a0+da3794e-cp38-cp38-linux_x86_64.whl`
5. `pip3 install tf_nightly_rocm-2.9.2-cp38-cp38-linux_x86_64.whl`

PS: You may need `export LD_LIBRARY_PATH=/opt/rocm/lib` to resolve cannot find libmiopen.so error.

