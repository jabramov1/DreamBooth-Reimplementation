---
configs:
- config_name: default
  data_files:
  - split: train
    path: "dataset/backpack/*.jpg"
- config_name: backpack
  data_files:
  - split: train
    path: "dataset/backpack/*.jpg"
- config_name: backpack_dog
  data_files:
  - split: train
    path: "dataset/backpack_dog/*.jpg"
- config_name: bear_plushie
  data_files:
  - split: train
    path: "dataset/bear_plushie/*.jpg"
- config_name: berry_bowl
  data_files:
  - split: train
    path: "dataset/berry_bowl/*.jpg"
- config_name: can
  data_files:
  - split: train
    path: "dataset/can/*.jpg"
- config_name: candle
  data_files:
  - split: train
    path: "dataset/candle/*.jpg"
- config_name: cat
  data_files:
  - split: train
    path: "dataset/cat/*.jpg"
- config_name: cat2
  data_files:
  - split: train
    path: "dataset/cat2/*.jpg"
- config_name: clock
  data_files:
  - split: train
    path: "dataset/clock/*.jpg"
- config_name: colorful_sneaker
  data_files:
  - split: train
    path: "dataset/colorful_sneaker/*.jpg"
- config_name: dog
  data_files:
  - split: train
    path: "dataset/dog/*.jpg"
- config_name: dog2
  data_files:
  - split: train
    path: "dataset/dog2/*.jpg"
- config_name: dog3
  data_files:
  - split: train
    path: "dataset/dog3/*.jpg"
- config_name: dog5
  data_files:
  - split: train
    path: "dataset/dog5/*.jpg"
- config_name: dog6
  data_files:
  - split: train
    path: "dataset/dog6/*.jpg"
- config_name: dog7
  data_files:
  - split: train
    path: "dataset/dog7/*.jpg"
- config_name: dog8
  data_files:
  - split: train
    path: "dataset/dog8/*.jpg"
- config_name: duck_toy
  data_files:
  - split: train
    path: "dataset/duck_toy/*.jpg"
- config_name: fancy_boot
  data_files:
  - split: train
    path: "dataset/fancy_boot/*.jpg"
- config_name: grey_sloth_plushie
  data_files:
  - split: train
    path: "dataset/grey_sloth_plushie/*.jpg"
- config_name: monster_toy
  data_files:
  - split: train
    path: "dataset/monster_toy/*.jpg"
- config_name: pink_sunglasses
  data_files:
  - split: train
    path: "dataset/pink_sunglasses/*.jpg"
- config_name: poop_emoji
  data_files:
  - split: train
    path: "dataset/poop_emoji/*.jpg"
- config_name: rc_car
  data_files:
  - split: train
    path: "dataset/rc_car/*.jpg"
- config_name: red_cartoon
  data_files:
  - split: train
    path: "dataset/red_cartoon/*.jpg"
- config_name: robot_toy
  data_files:
  - split: train
    path: "dataset/robot_toy/*.jpg"
- config_name: shiny_sneaker
  data_files:
  - split: train
    path: "dataset/shiny_sneaker/*.jpg"
- config_name: teapot
  data_files:
  - split: train
    path: "dataset/teapot/*.jpg"
- config_name: vase
  data_files:
  - split: train
    path: "dataset/vase/*.jpg"
- config_name: wolf_plushie
  data_files:
  - split: train
    path: "dataset/wolf_plushie/*.jpg"
license: cc-by-4.0
---
# Dataset Card for "dreambooth"

## Dataset of the Google paper DreamBooth: Fine Tuning Text-to-Image Diffusion Models for Subject-Driven Generation

The dataset includes 30 subjects of 15 different classes. 9 out of these subjects are live subjects (dogs and cats) and 21 are objects. The dataset contains a variable number of images per subject (4-6). Images of the subjects are usually captured in different conditions, environments and under different angles.

We include a file dataset/prompts\_and\_classes.txt which contains all of the prompts used in the paper for live subjects and objects, as well as the class name used for the subjects.

The images have either been captured by the paper authors, or sourced from www.unsplash.com

The dataset/references\_and\_licenses.txt file contains a list of all the reference links to the images in www.unsplash.com - and attribution to the photographer, along with the license of the image.

### [project page](https://dreambooth.github.io/) | [arxiv](https://arxiv.org/abs/2208.12242)

## Academic Citation

If you use this work please cite:
```
@inproceedings{ruiz2023dreambooth,
  title={Dreambooth: Fine tuning text-to-image diffusion models for subject-driven generation},
  author={Ruiz, Nataniel and Li, Yuanzhen and Jampani, Varun and Pritch, Yael and Rubinstein, Michael and Aberman, Kfir},
  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
  year={2023}
}
```

## Disclaimer

This is not an officially supported Google product.