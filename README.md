

![FaceTag](explain.jpg)



## Steps on how to run:

  1. Download [miniconda3](https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh) and install.

    ```bash
    chmod 755 Miniconda3-latest-Linux-x86_64.sh
    ./Miniconda3-latest-Linux-x86_64.sh
    ```

  2. Install conda evn and required pip library packages and go the environment.

  ```bash
  conda env create -f environment.yml
  pip install -r requirement.txt
  conda activate CV
  ```

  3. (Optional) If want to train on own image, follow the instrution from [***Facenet***](https://github.com/davidsandberg/facenet).

  4. Run the test on single image.

  ```bash
  python image.py --img_filename [PATH OF TEST IMAG] --save_filename [NAME TO SAVE RESULT]
  ```
  5. Run the real time video.

  ```bash
  python video.py --video_link [0(WEB CAM) or 1(USB CAM) ]
  ```
