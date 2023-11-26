# neural_style_transfer

Running
run in cmd

py .\model.py --content "images/content/city.jpg" --style "images/style/art.jpg"

or edit the variables

set the path to the content image and style image in the file.

# path to images
CONTENT_IMG_PATH = "images/content/planets.jpg"
STYLE_IMG_PATH = "images/style/art.jpg"

# image will save every epoch under
# save/IMG_SAVE_NAME-{n}.png
IMG_SAVE_NAME = "mountain-greatwave"
You can alter the weights in the style_weight, content_weight, and total_variation_weight

style_weight = 1e-2  # default: 1e-2
content_weight = 1e4  # default: 1e4
total_variation_weight = 30  # default: 30
