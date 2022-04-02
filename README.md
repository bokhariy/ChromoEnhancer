# ChromoEnhancer
ChromoNet enhance poor quality karyograms so that it would be easier to analyze them with less error.


## Instructions:
For using the our trained model:
  1. Download and install [CycleGAN](https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix)
  2. Download the weights from the Dropbox [link](https://www.dropbox.com/sh/df7d925gu6xkoqj/AAAvm97vmkmrCwTu__yMnnBXa?dl=0)
  3. Make a directory inside CycleGAN 'checkpoints' directory and name it 'chrom_images'
  4. Put the weights downloaded at CycleGAN `checkpoints/chrom_images` directory
  5. Make a directory inside CycleGAN 'datasets' directory and name it 'chrom_images'
  6. Put the images of the chromosme pair at CycleGAN  `checkpoints/datasets` directory
  7. Run the follwing command `python test.py --dataroot datasets/chrom_images/ --name chrom_images --gpu_ids 0 --input_nc 1 --output_nc 1 --norm batch --netG unet_256 --model cycle_gan`
