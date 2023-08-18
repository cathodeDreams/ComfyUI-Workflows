# txt>img

![workflow image](https://github.com/cathodeDreams/ComfyUI-Workflows/blob/main/txt%20to%20img/txt%20to%20img.png)

### Overview

This is what I use for txt>img generation. It generates 4 images in a batch and then upscales a selection from that batch. The upscale is an iterative latent upscale x2, split into two, followed by a pixel scale x2 using 4x-ultrasharp. The upscales utilize the Controlnet tile model.

### Requires these custom nodes:

[ComfyUI-Impact-Pack](https://github.com/ltdrdata/ComfyUI-Impact-Pack)

[ComfyUI-Custom-Scripts](https://github.com/pythongosssss/ComfyUI-Custom-Scripts)

[ComfyUI-Image-Selector](https://github.com/SLAPaper/ComfyUI-Image-Selector)

[rgthree-comfy](https://github.com/rgthree/rgthree-comfy)

### Instructions for Use

1. Input your choice of checkpoint and lora in their respective nodes in Group A.
2. Click New Fixed Random in the Seed node in Group A.
3. Mute the two Save Image nodes in Group E.
4. Click Queue Prompt to generate a batch of 4 image previews in Group B.
5. Use the Latent Selector node in Group B to input a choice of images to upscale. Select 1, 2, 3, and/or 4, separated by commas.
6. Unmute either one or both of the Save Image nodes in Group E.
7. Note the Image Selector node in Group D. If your initial choice was more than one image, you will need to make further selections. For example, if you chose 1, 3 and want to fully upscale both images, the Image Selector node should be 1, 2. Otherwise, just type 2 there and generate again after 1.
8. Click Queue Prompt to upscale your selection(s).