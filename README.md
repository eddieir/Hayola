![drawn_example1](https://user-images.githubusercontent.com/23243761/68202115-5fa70e00-ffc3-11e9-96b6-8bfaf116795d.jpg)


![Screenshot_2019-11-05 Scaffold](https://user-images.githubusercontent.com/23243761/68202209-86654480-ffc3-11e9-93fb-1278cd6373cc.png)


Welcome to Hayola. Hayola is a deep learning model that takes hand-drawn web mockups and converts them into working HTML code. It uses an image captioning architecture to generate its HTML markup from hand-drawn website wireframes.


Note: This project is defiend by Python3, It will not work by Python2

Example Usage

Download the data and pretrained weights:



Converting an example drawn image into HTML code, using pretrained weights:

cd src

python convert_single_image.py --png_path ../examples/drawn_example1.png \
      --output_folder ./generated_html \
      --model_json_file ../bin/model_json.json \
      --model_weights_file ../bin/weights.h5

General Usage

Converting a single image into HTML code, using weights:

cd src

python convert_single_image.py --png_path {path/to/img.png} \
      --output_folder {folder/to/output/html} \
      --model_json_file {path/to/model/json_file.json} \
      --model_weights_file {path/to/model/weights.h5}

Converting a batch of images in a folder to HTML:

cd src

python convert_batch_of_images.py --pngs_path {path/to/folder/with/pngs} \
      --output_folder {folder/to/output/html} \
      --model_json_file {path/to/model/json_file.json} \
      --model_weights_file {path/to/model/weights.h5}


