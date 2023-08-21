# Multi-Latent Compositing from batch selection

![workflow image](https://raw.githubusercontent.com/cathodeDreams/ComfyUI-Workflows/main/Multi-Latent%20Compositing%20from%20batches/compositing.png)

### Overview

This workflow utilizes Multi-Latent Compositing but allows for a selection of what latents to composite from a batch. 

Mute the Preview node at the end, and save image nodes if using with a full upscale path, and press Queue Prompt to generate a set of two batches to composite together. 

Make your selections in the Latent Selector nodes, only one selection per node, and unmute the preview image node.

Note that settings relating to the composition itself must be entered based on what you wish to do with the image.

### Requires these custom nodes:

[ComfyUI_Dave_CustomNode](https://github.com/Davemane42/ComfyUI_Dave_CustomNode)

[ComfyUI-Impact-Pack](https://github.com/ltdrdata/ComfyUI-Impact-Pack)

[ComfyUI-Custom-Scripts](https://github.com/pythongosssss/ComfyUI-Custom-Scripts)

[ComfyUI-Image-Selector](https://github.com/SLAPaper/ComfyUI-Image-Selector)

[rgthree-comfy](https://github.com/rgthree/rgthree-comfy)