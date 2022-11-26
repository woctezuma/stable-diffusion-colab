# Stable-Diffusion-Colab

The goal of this repository is to provide a Colab notebook to run the text-to-image ["Stable Diffusion"][huggingface-latest-weights] model [1].

# Usage

-   Run [`stable_diffusion.ipynb`][colab-notebook-stable-diffusion].
[![Open In Colab][colab-badge]][colab-notebook-stable-diffusion]

## Schedulers

A scheduler [2] can be chosen among:
- PNDM, which is the default scheduler in [🤗's D🧨iffusers][huggingface-blogpost] for Stable Diffusion [at 512 resolution][huggingface-sd2-resolution-512],
- DDIM, which is the default scheduler for Stable Diffusion [at 768 resolution][huggingface-sd2-resolution-768],
- K-LMS, which is the scheduler suggested by [DreamStudio][dreamstudio-demo].
- Euler, which is the scheduler used in [🤗's example][huggingface-sd2-examples] for Stable Diffusion 2.

## Parameters

Typically, parameters are set with the following ranges in mind:
- `num_images` (default: `4`), between `1` and `4`,
- `guidance_scale` (default: `9`), between `0` and `20`,
- `num_inference_steps` (default: `25`), between `10` and `150`.

# Results

<img alt="Astronaut on Mars" src="https://github.com/woctezuma/stable-diffusion-colab/wiki/img/astronaut_3.jpg" width="256"> <img alt="Astronaut on Mars" src="https://github.com/woctezuma/stable-diffusion-colab/wiki/img/astronaut_1.jpg" width="256"> <img alt="Astronaut on Mars" src="https://github.com/woctezuma/stable-diffusion-colab/wiki/img/astronaut_2.jpg" width="256">

<sub>
Different results obtained with the text prompt: "a photo of an astronaut riding a horse on mars".
</sub>

<img alt="Pikachu in Paris" src="https://github.com/woctezuma/stable-diffusion-colab/wiki/img/pikachu_3.jpg" width="256"> <img alt="Pikachu in Paris" src="https://github.com/woctezuma/stable-diffusion-colab/wiki/img/pikachu_1.jpg" width="256"> <img alt="Pikachu in Paris" src="https://github.com/woctezuma/stable-diffusion-colab/wiki/img/pikachu_2.jpg" width="256">

<sub>
Different results obtained with the text prompt: "a pikachu fine dining with a view to the Eiffel Tower".
</sub>

# References

[1] Rombach, Robin, et al. [*High-resolution image synthesis with latent diffusion models*][stable-diffusion-paper]. CVPR 2022.
([models][huggingface-models] & [demo][huggingface-demo])

[2] Karras, Tero, et al. [*Elucidating the Design Space of Diffusion-Based Generative Models*][sampler-schedule-paper]. NeurIPS 2022. ([code][edm-implementation])

[stable-diffusion-paper]: <https://openaccess.thecvf.com/content/CVPR2022/html/Rombach_High-Resolution_Image_Synthesis_With_Latent_Diffusion_Models_CVPR_2022_paper.html>
[sampler-schedule-paper]: <https://arxiv.org/abs/2206.00364>

[huggingface-blogpost]: <https://huggingface.co/blog/stable_diffusion>
[huggingface-models]: <https://huggingface.co/CompVis/stable-diffusion>
[huggingface-latest-weights]: <https://huggingface.co/stabilityai/stable-diffusion-2>
[huggingface-sd2-resolution-512]: <https://huggingface.co/stabilityai/stable-diffusion-2-base>
[huggingface-sd2-resolution-768]: <https://huggingface.co/stabilityai/stable-diffusion-2>
[huggingface-sd2-examples]: <https://huggingface.co/stabilityai/stable-diffusion-2#examples>
[huggingface-demo]: <https://huggingface.co/spaces/stabilityai/stable-diffusion>
[dreamstudio-demo]: <http://beta.dreamstudio.ai>
[edm-implementation]: <https://github.com/NVlabs/edm>

[colab-notebook-stable-diffusion]: <https://colab.research.google.com/github/woctezuma/stable-diffusion-colab/blob/main/stable_diffusion.ipynb>
[colab-badge]: <https://colab.research.google.com/assets/colab-badge.svg>
