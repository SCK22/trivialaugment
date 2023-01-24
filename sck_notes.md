1. Find if they used Earlystopping #novelty
   1. did not find in the primary search that I did
   2. may be hard to prove, lets see
2. Check for all the configs that ran 1 gpu
3. setup office system with pytorch gpu and run all these 1 gpu things, dont have to worry about cost
4. Read the yaml files and see if you can make a better representation of the experiments that they did
5. There are three implementations of the augmentations,I am thinking to run same model with all the three and compare the results
   1. TrivialAugment
   2. Uniaugment
   3. RandAugment
6. Check aug_lib.py line 636, the differences between these three types of augmentations are lucid!
7. Collate info related to
    - number of datasets used
    - for each of these 
      - number of images
      - size of the images (resolution)
      - size of time images (mb)
      - time take to run a few epochs (if possible)
    - 