# neural_style_transfer
Neural Style Transfer is a technique that takes two images, a content image and a style image, and blends them together so the content image is in the style of the style image.

## Running

run in cmd

`py .\dashtoon.ipynb --content "2615123.jpg" --style "bOvf94dPRxWu0u3QsPjF_tree.jpg"

or edit the variables

set the path to the content image and style image in the file.

```py
# path to images
CONTENT_IMG_PATH = "2615123.jpg"
STYLE_IMG_PATH = "bOvf94dPRxWu0u3QsPjF_tree.jpg"

# image will save every epoch under
# save/IMG_SAVE_NAME-{n}.png
IMG_SAVE_NAME = "output.png"
```

You can alter the weights in the style_weight, content_weight, and total_variation_weight

```py
style_weight = 1e-2  # default: 1e-2
content_weight = 1e4  # default: 1e4
total_variation_weight = 30  # default: 30
```

## Examples

Running for around 10 epochs(1000 steps) tends to yield the best results. With certain images it may be better to run more or less epochs as well as editing the weights to generate a better image.
