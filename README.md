# Stable-Diffusion-Colab

The goal of this repository is to provide a Colab notebook to run the text-to-image ["Stable Diffusion"][huggingface-latest-weights] model [1].

# Usage

-   Run [`stable_diffusion.ipynb`][colab-notebook-stable-diffusion].
[![Open In Colab][colab-badge]][colab-notebook-stable-diffusion]

## Safety Check

To remove the safety check, switch `remove_safety` to `True`:
```python
remove_safety = True
```

## Schedulers

A scheduler [2] can be chosen among:
- PNDM, which is the default scheduler in [🤗's D🧨iffusers][huggingface-blogpost] for Stable Diffusion,
- DDIM,
- K-LMS, which is the scheduler suggested by [DreamStudio][dreamstudio-demo].

## Parameters

Typically, parameters are set with the following ranges in mind:
- `num_images` (default: `1`), between `1` and `4`,
- `guidance_scale` (default: `7.5`), between `0` and `20`,
- `num_inference_steps` (default: `50`), between `10` and `150`.

# Results

<img alt="Astronaut on Mars" src="https://github.com/woctezuma/stable-diffusion-colab/wiki/img/astronaut_3.jpg" width="256"> <img alt="Astronaut on Mars" src="https://github.com/woctezuma/stable-diffusion-colab/wiki/img/astronaut_1.jpg" width="256"> <img alt="Astronaut on Mars" src="https://github.com/woctezuma/stable-diffusion-colab/wiki/img/astronaut_2.jpg" width="256">

<sub>
Different results obtained with the text prompt: "a photo of an astronaut riding a horse on mars".
</sub>

# Misuse and Malicious Use 

To be able to run the notebook, a "HuggingFace🤗 Hub token" is mandatory.
This token is personal!

In order to obtain such token, you need to accept a "CreativeML OpenRAIL-M license", which explicitly states that:
> You cannot use the model to deliberately produce nor share illegal or harmful outputs or content.

Moreover, as for the DALL·E model, you are asked to abide to the following statement:
> Do not create or disseminate images that create hostile or alienating environments for people.
> This includes images that people would find disturbing, distressing, or offensive; or content that propagates stereotypes.

# References

[1] Rombach, Robin, et al. [*High-resolution image synthesis with latent diffusion models*][stable-diffusion-paper]. CVPR 2022.
([models][huggingface-models] & [demo][huggingface-demo])

[2] Karras, Tero, et al. [*Elucidating the Design Space of Diffusion-Based Generative Models*][sampler-schedule-paper]. NeurIPS 2022. ([code][edm-implementation])

[stable-diffusion-paper]: <https://openaccess.thecvf.com/content/CVPR2022/html/Rombach_High-Resolution_Image_Synthesis_With_Latent_Diffusion_Models_CVPR_2022_paper.html>
[sampler-schedule-paper]: <https://arxiv.org/abs/2206.00364>

[huggingface-blogpost]: <https://huggingface.co/blog/stable_diffusion>
[huggingface-models]: <https://huggingface.co/CompVis/stable-diffusion>
[huggingface-latest-weights]: <https://huggingface.co/CompVis/stable-diffusion-v1-4>
[huggingface-demo]: <https://huggingface.co/spaces/stabilityai/stable-diffusion>
[dreamstudio-demo]: <http://beta.dreamstudio.ai>
[edm-implementation]: <https://github.com/NVlabs/edm>

[colab-notebook-stable-diffusion]: <https://colab.research.google.com/github/woctezuma/stable-diffusion-colab/blob/main/stable_diffusion.ipynb>
[colab-badge]: <https://colab.research.google.com/assets/colab-badge.svg>
