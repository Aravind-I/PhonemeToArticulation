This code repository is related to the publication "A comparative study of estimating articulatory movements from phoneme sequences and acoustic features", ICASSP 2020 

LINK: https://ieeexplore.ieee.org/document/9053852

## Packages Requirement:
1. Torch
2. matplotlib==2.1.0
3. tensorflow
4. numpy==1.13.3
5. inflect==0.2.5
6. librosa==0.6.0
7. scipy==1.0.0
8. tensorboardX==1.1
9. Unidecode==1.0.22
10. pillow

## Training
 `python train.py --output_directory=outdir --log_directory=logdir`


## Training using a pre-trained model
Training using a pre-trained model can lead to faster convergence and we have used this technique to fine-tune the base model. 

 `python train.py --output_directory=outdir --log_directory=logdir -c model.pt --warm_start`
 
 ## Acknowledgements
This implementation uses code from the following repo: [NVIDIA-tacotron2](https://github.com/NVIDIA/tacotron2)
