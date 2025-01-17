
<div align="center">
    <br>
    <img src="https://github.com/Djdefrag/QualityScaler/blob/main/logo.png" width="175"> </a> 
    <br><br> QualityScaler - image/video deeplearning upscaling for any GPU <br><br>
    <a href="https://github.com/Djdefrag/QualityScaler/releases">
         <img src="https://user-images.githubusercontent.com/86362423/162710522-c40c4f39-a6b9-48bc-84bc-1c6b78319f01.png" width="200">
    </a>
</div>
<br>
<div align="center">
    <img src="https://user-images.githubusercontent.com/32263112/189052979-d3dc5682-61bd-4cb1-a15e-af591f78519d.jpg"> </a> 
</div>

## Credits.

BSRGAN - https://github.com/cszn/BSRGAN | https://arxiv.org/abs/2103.14006

RealSR_JPEG - https://github.com/jixiaozhong/RealSR | https://arxiv.org/pdf/2005.01996.pdf

## How is made.

QualityScaler is completely written in Python, from backend to frontend. External packages are:
- [ ] AI  -> Pytorch-directml
- [ ] GUI -> Tkinter / Tkdnd / Sv_ttk
- [ ] Image/video -> OpenCV / Moviepy
- [ ] Packaging   -> Pyinstaller
- [ ] Miscellaneous -> Pywin32 / Win32mica / Image_slicer

## Installation.

1) download the QualityScaler release .zip
2) unzip using 7zip or similar
3) execute QualityScaler.exe in the directory

## Requirements
- [ ] Windows 11 / Windows 10
- [ ] RAM >= 8Gb
- [ ] Directx12 compatible GPU:
    - [ ] any AMD >= Radeon HD 7000 series
    - [ ] any Intel HD Integrated >= 4th-gen core
    - [ ] any NVIDIA >=  GTX 600 series
- [ ] CPU [works without GPU, but is very slow]

## Features.

- [x] Easy to use GUI
- [x] Image/list of images upscale
- [x] Video upscale
- [x] Drag&drop files [image/multiple images/video]
- [x] Automatic image tiling and merging to avoid gpu VRAM limitation
- [x] Resize image/video before upscaling
- [x] Cpu and Gpu backend
- [x] Compatible images - png, jpeg, bmp, webp, tif  
- [x] Compatible video  - mp4, wemb, gif, mkv, flv, avi, mov, qt 

## Next steps.

- [x] Support for Nvidia RTX 3k and 2k with cuda 11
- [x] New Fused model (that combines the best of both models)
- [x] New GUI with Windows 11 style
- [ ] Include audio for upscaled video
- [x] Switch to Pytorch-directml to support all Directx12 compatible gpu (AMD, Intel, Nvidia)
- [ ] Update libraries 
    - [ ] Python 3.10 (expecting ~10% more performance) 
    - [ ] Python 3.11 (expecting ~30% more performance, now in beta)

## Known bugs.
- [x] Windows10 - the app starts with white colored navbar instead of dark
- [x] Upscaling multiple images doesn't free GPU Vram, so the it is very likely that the process will fail when the gpu memory fills up
- [ ] Filenames with non-latin symbols (for example kangy, cyrillic etc.) not supported - [Temp solution] rename files like "image" or "video"

## Some Example.

- BSRGAN examples

![test](https://user-images.githubusercontent.com/32263112/166690007-f1601487-7b94-4f2c-b4e2-436bc189a26e.png)

![Bsrgan x4](https://user-images.githubusercontent.com/32263112/168884625-c869baee-4cca-4a33-bdad-b65d9c29889d.png)

![example](https://user-images.githubusercontent.com/32263112/171657072-0a746274-46e9-4641-b16c-a9f6f612624b.png)




