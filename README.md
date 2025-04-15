# Stable Diffusion SANA-Sprint - Colab

The goal of this repository is to provide a Colab notebook to run the text-to-image [Stable Diffusion SANA-Sprint][huggingface-latest-weights] model.

## Usage

-   Run [`stable_diffusion.ipynb`][colab-notebook-stable-diffusion].
[![Open In Colab][colab-badge]][colab-notebook-stable-diffusion]

## Results

<img alt="Astronaut on Mars" src="https://github.com/woctezuma/stable-diffusion-colab/wiki/img/astronaut_3xl.jpg" width="256"> <img alt="Astronaut on Mars" src="https://github.com/woctezuma/stable-diffusion-colab/wiki/img/astronaut_1xl.jpg" width="256"> <img alt="Astronaut on Mars" src="https://github.com/woctezuma/stable-diffusion-colab/wiki/img/astronaut_2xl.jpg" width="256">

<sub>
Different results obtained with the text prompt: "a photo of an astronaut riding a horse on Mars" using Stable Diffusion XL.
</sub>

---

<img alt="Pikachu in Paris" src="https://github.com/woctezuma/stable-diffusion-colab/wiki/img/pikachu_3xl.jpg" width="256"> <img alt="Pikachu in Paris" src="https://github.com/woctezuma/stable-diffusion-colab/wiki/img/pikachu_1xl.jpg" width="256"> <img alt="Pikachu in Paris" src="https://github.com/woctezuma/stable-diffusion-colab/wiki/img/pikachu_2xl.jpg" width="256">

<sub>
Different results obtained with the text prompt: "a photo of Pikachu fine dining with a view to the Eiffel Tower" using Stable Diffusion XL.
</sub>

---

<img alt="Astronaut on Mars" src="https://github.com/woctezuma/stable-diffusion-colab/wiki/img/astronaut_3xlb.jpg" width="256"> <img alt="Astronaut on Mars" src="https://github.com/woctezuma/stable-diffusion-colab/wiki/img/astronaut_1xlb.jpg" width="256"> <img alt="Astronaut on Mars" src="https://github.com/woctezuma/stable-diffusion-colab/wiki/img/astronaut_2xlb.jpg" width="256">

<sub>
Different results obtained with the text prompt: "a photo of an astronaut riding a horse on Mars" using SANA-Sprint.
</sub>

---

<img alt="Pikachu in Paris" src="https://github.com/woctezuma/stable-diffusion-colab/wiki/img/pikachu_3xlb.jpg" width="256"> <img alt="Pikachu in Paris" src="https://github.com/woctezuma/stable-diffusion-colab/wiki/img/pikachu_1xlb.jpg" width="256"> <img alt="Pikachu in Paris" src="https://github.com/woctezuma/stable-diffusion-colab/wiki/img/pikachu_2xlb.jpg" width="256">

<sub>
Different results obtained with the text prompt: "a photo of Pikachu fine dining with a view to the Eiffel Tower" using SANA-Sprint.
</sub>

## References

[1] Rombach, Robin, et al. [*High-resolution image synthesis with latent diffusion models*][stable-diffusion-paper]. CVPR 2022.
([models][huggingface-models] & [demo][huggingface-demo])

[2] Karras, Tero, et al. [*Elucidating the Design Space of Diffusion-Based Generative Models*][sampler-schedule-paper]. NeurIPS 2022. ([code][edm-implementation])

[3] Luo, Simian, et al. [*Latent Consistency Models: Synthesizing HR Images with Few-Step Inference.*][lcm-paper] arXiv 2023. ([code][lcm-github])

[4] Luo, Simian, et al. [*LCM-LoRA: A Universal Stable-Diffusion Acceleration Module.*][lcm-lora-paper] arXiv 2023.

[stable-diffusion-paper]: <https://openaccess.thecvf.com/content/CVPR2022/html/Rombach_High-Resolution_Image_Synthesis_With_Latent_Diffusion_Models_CVPR_2022_paper.html>
[sampler-schedule-paper]: <https://arxiv.org/abs/2206.00364>
[lcm-paper]: <https://arxiv.org/abs/2310.04378>
[lcm-lora-paper]: <https://arxiv.org/abs/2311.05556>

[huggingface-blogpost]: <https://huggingface.co/blog/stable_diffusion>
[huggingface-lcm-blogpost]: <https://huggingface.co/blog/lcm_lora>
[huggingface-models]: <https://huggingface.co/CompVis/stable-diffusion>
[huggingface-latest-weights]: <https://huggingface.co/Efficient-Large-Model/Sana_Sprint_0.6B_1024px>
[huggingface-sd2-resolution-512]: <https://huggingface.co/stabilityai/stable-diffusion-2-1-base>
[huggingface-sd2-resolution-768]: <https://huggingface.co/stabilityai/stable-diffusion-2-1>
[huggingface-sd2-examples]: <https://huggingface.co/stabilityai/stable-diffusion-2#examples>
[huggingface-sd21-examples]: <https://huggingface.co/stabilityai/stable-diffusion-2-1#examples>
[huggingface-demo]: <https://huggingface.co/spaces/stabilityai/stable-diffusion>
[dreamstudio-demo]: <http://beta.dreamstudio.ai>
[edm-implementation]: <https://github.com/NVlabs/edm>
[lcm-github]: <https://github.com/luosiallen/latent-consistency-model>

[colab-notebook-stable-diffusion]: <https://colab.research.google.com/github/woctezuma/stable-diffusion-colab/blob/main/stable_diffusion.ipynb>
[colab-badge]: <https://colab.research.google.com/assets/colab-badge.svg>
