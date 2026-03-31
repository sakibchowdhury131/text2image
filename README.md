# text2image

A Google Colab experiment implementing a text-to-image generation model using a Transformer encoder and a CNN decoder. The model is trained on the `lambdalabs/pokemon-blip-captions` dataset from Hugging Face, which pairs Pokémon images with natural-language captions.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sakibchowdhury131/text2image/blob/main/text_image.ipynb)

## Features

- Loads the `lambdalabs/pokemon-blip-captions` dataset via the Hugging Face `datasets` library
- Implements a Transformer-based text encoder
- CNN-based image decoder that generates images conditioned on text embeddings
- Trained end-to-end with PyTorch and PyTorch Lightning

## Tech Stack

- Python 3
- PyTorch
- PyTorch Lightning
- [Hugging Face `datasets`](https://huggingface.co/docs/datasets/)
- NumPy
- Google Colab

## Project Structure

| File | Description |
|---|---|
| `text_image.ipynb` | Main Colab notebook: dataset loading, model definition, training loop |

## Requirements

```
torch
pytorch-lightning
datasets
numpy
```

## Usage

1. Open `text_image.ipynb` in Google Colab using the badge above.
2. Run all cells in order.
3. A Hugging Face access token may be required for the dataset; update `use_auth_token` in the dataset loading cell.

## License

MIT
