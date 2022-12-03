# Bored Ape Diffusion

Diffusion model for unconditional image generation of [Bored Apes](https://opensea.io/collection/boredapeyachtclub)

## Example
![example](https://user-images.githubusercontent.com/59410571/205454220-eb365897-7239-4feb-8826-4203ac651c6c.png)

## Usage

```python
from diffusers import DDPMPipeline

pipeline = DDPMPipeline.from_pretrained('daspartho/bored-ape-diffusion')
image = pipeline().images[0]
image
```

## Training
The model is trained on [this dataset](https://huggingface.co/datasets/daspartho/bored-ape) of 10000 Bored Ape images I've uploaded on HuggingFace Hub.

Notebook for training the model is available [here](https://github.com/daspartho/bored-ape-diffusion/blob/main/main.ipynb).

The trained [Model](https://huggingface.co/daspartho/bored-ape-diffusion) is uploaded on HuggingFace Hub.

## Acknowledgement

Special thanks to the awesome [Diffusion Models class](https://github.com/huggingface/diffusion-models-class) by Jonathan Whitaker and the HuggingFace team.
