# LRZebra
Given a Zebra image, identifies whether it is right or left flank using Pre-trained ResNet34
Project serves as a simple intoduction to Transfer Learning. It uses pretrained ResNet34 model and uses pytorch framework.
Currently the test accuracy is around ~97%. 
Initially, the model suffered with high loss during training and low accuracy during test ~95%, later I have identified the issue is with covariate shift. Randomizing training data helped overcome the problem.

### Dataset
The dataset has been picked up from archives of stripe spotter. Pre processing has been done to get remove all the background noice and get images with only zebra. This has been done using pretrained instance segmentation model from Detectron2. The images have been converted to gray to easen up the training process.

Link to processed dataset: https://drive.google.com/open?id=1dPgAlcMbMxOhm08w-sQLYhsLzNKA39r8 
