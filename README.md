# LRZebra
Given a Zebra image, identifies whether it is right or left flank using Pre-trained ResNet34
Project serves as a simple intoduction to Transfer Learning. It uses pretrained ResNet34 model and uses pytorch framework.
Currently the test accuracy is around ~97%. 
Initially, the model suffered with high loss during training and low accuracy during test ~95%, later I have identified the issue is with covariate shift. Randomizing training data helped overcome the problem.

Various approches have been trained and tested in the process. 

