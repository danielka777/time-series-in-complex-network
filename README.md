
<h1>
  Инстурмент конвертирования временных рядов в сети
  <img src="https://media.giphy.com/media/KAqOh6pbJ6qTasMB2E/giphy.gif" width="100"/> 
</h1>
_Generate images from a text prompt_




## How to use it?

There are several ways to use DALL·E mini to create your own images:

* use [the official DALL·E Mini demo](https://huggingface.co/spaces/dalle-mini/dalle-mini)

* experiment with the pipeline step by step through our [`inference pipeline notebook`](tools/inference/inference_pipeline.ipynb)

  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/danielka777/time-series-in-complex-network/blob/main/Run.ipynb)

You can also use these great projects from the community:

* spin off your own app with [DALL-E Playground repository](https://github.com/saharmor/dalle-playground) (thanks [Sahar](https://twitter.com/theaievangelist))

* try [DALL·E Flow](https://github.com/jina-ai/dalle-flow) project for generating, diffusion, upscaling in a Human-in-the-Loop workflow (thanks [Han Xiao](https://github.com/hanxiao))

  [![Open In ColabFunc](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/danielka777/time-series-in-complex-network/blob/main/Functions.ipynb)

## How does it work?

Refer to [our report](https://wandb.ai/dalle-mini/dalle-mini/reports/DALL-E-mini-Generate-images-from-any-text-prompt--VmlldzoyMDE4NDAy).

## Contributing

Join the community on the [LAION Discord](https://discord.gg/xBPBXfcFHd).
Any contribution is welcome, from reporting issues to proposing fixes/improvements or testing the model with cool prompts!

## Development

### Dependencies Installation

For inference only, use `pip install git+https://github.com/borisdayma/dalle-mini.git`.

For development, clone the repo and use `pip install -e ".[dev]"`.
Before making a PR, check style with `make style`.

### Training of DALL·E mini

Use [`tools/train/train.py`](tools/train/train.py).

You can also adjust the [sweep configuration file](https://docs.wandb.ai/guides/sweeps) if you need to perform a hyperparameter search.

## FAQ

### Where to find the latest models?

Trained models are on 🤗 Model Hub:

* [VQGAN-f16-16384](https://huggingface.co/dalle-mini/vqgan_imagenet_f16_16384) for encoding/decoding images
* [DALL·E mini](https://huggingface.co/flax-community/dalle-mini) for generating images from a text prompt

### Where does the logo come from?

The "armchair in the shape of an avocado" was used by OpenAI when releasing DALL·E to illustrate the model's capabilities. Having successful predictions on this prompt represents a big milestone to us.

## Acknowledgements

* 🤗 Hugging Face for organizing [the FLAX/JAX community week](https://github.com/huggingface/transformers/tree/master/examples/research_projects/jax-projects)
* Google [TPU Research Cloud (TRC) program](https://sites.research.google/trc/) for providing computing resources
* [Weights & Biases](https://wandb.com/) for providing the infrastructure for experiment tracking and model management
