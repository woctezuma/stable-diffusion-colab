# Stable-Diffusion-Colab

The goal of this repository is to provide a Colab notebook to run the text-to-image ["Stable Diffusion"][huggingface-latest-weights] model [1].

# Usage

-   Run [`stable_diffusion.ipynb`][colab-notebook-stable-diffusion].
[![Open In Colab][colab-badge]][colab-notebook-stable-diffusion]

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

[stable-diffusion-paper]: <https://openaccess.thecvf.com/content/CVPR2022/html/Rombach_High-Resolution_Image_Synthesis_With_Latent_Diffusion_Models_CVPR_2022_paper.html>

[huggingface-models]: <https://huggingface.co/CompVis/stable-diffusion>
[huggingface-latest-weights]: <https://huggingface.co/CompVis/stable-diffusion-v1-4>
[huggingface-demo]: <https://huggingface.co/spaces/stabilityai/stable-diffusion>

[colab-notebook-stable-diffusion]: <https://colab.research.google.com/github/woctezuma/stable-diffusion-colab/blob/main/stable_diffusion.ipynb>
[colab-badge]: <https://colab.research.google.com/assets/colab-badge.svg>
