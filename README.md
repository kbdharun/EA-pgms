# EAI Programs

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kbdharun/EA-pgms)

This repository contains the Python programs that I worked in Explainable AI class.

## Index

- Logistic Regression Programs
  - [Iris dataset](LR/LR-Iris.ipynb)
  - [Red Wine Dataset](LR/Red_Wine_EA.ipynb)
  - [NYC Taxi Fare Prediction](LR/nyc-taxi-fare-prediction.ipynb)
- LIME (Local Interpretable Model-Agnostic Explanations)
  - [Red Wine Dataset](LIME/Red_Wine_EA.ipynb)
- 2D Projection
  - [Iris Dataset](2d-Projection/2d-proj.ipynb)

## Prerequisites

Python and packages in `requirements.txt` file installed.

> [!NOTE]
> You can install all the packages in the file using the command `pip install -r requirements.txt`.

### Working with Conda

If you are using `conda` to manage your environments, you can create a new environment for this repository with the command `conda create -n eai` and activate it with the command `conda activate eai`.

> [!TIP]
> For faster environment solving in Conda, I would suggesting using the `libmamba` solver. You can set it as the default solver using the command `conda config --set solver libmamba`.

Then, you can install all the required packages using the command `conda install --file requirements.txt`.

### Container Image

Alternatively, you can use the [container image](https://github.com/kbdharun/EA-pgms/pkgs/container/eai-image) I created with all the packages preinstalled.

You can install it in [Distrobox](https://github.com/89luca89/distrobox) with the command `distrobox create -i ghcr.io/kbdharun/eai-image:latest -n eai` and use it with the command `distrobox enter eai`.

Additionally, you can verify the authenticity of the container image using [`cosign`](https://github.com/sigstore/cosign) (download the `cosign.pub` file from [here](https://github.com/kbdharun/EA-pgms/blob/main/cosign.pub) and execute the following command):

```zsh
cosign verify --key cosign.pub ghcr.io/kbdharun/eai-image:latest
```
