This code repository is related to the publication "A comparative study of estimating articulatory movements from phoneme sequences and acoustic features", ICASSP 2020 

LINK: https://ieeexplore.ieee.org/document/9053852

Packages Requirement:

Torch

matplotlib==2.1.0

tensorflow

numpy==1.13.3

inflect==0.2.5

librosa==0.6.0

scipy==1.0.0

tensorboardX==1.1

Unidecode==1.0.22

pillow

## Training
 `python train.py --output_directory=outdir --log_directory=logdir`


## Training using a pre-trained model
Training using a pre-trained model can lead to faster convergence and we have used this technique to fine-tune the base model. 

 `python train.py --output_directory=outdir --log_directory=logdir -c model.pt --warm_start`
 
 ## Acknowledgements
This implementation uses code from the following repos: [NVIDIA-tacotron2](https://github.com/NVIDIA/tacotron2)
