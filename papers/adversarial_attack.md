
# [Adversarial Patch](https://arxiv.org/pdf/1712.09665.pdf)

Brown et al, 2017

#### The Patch

- Salient to a neural network
- Scene-independent
- Doesn’t require knowledge of image being attacked
- Patch can be easily distributed across the internet
- Uses Large perturbation 

#### Attack:
- Replace part of image with new patch
- Takes any shape 
- Is trained on a variety of images
- Goes through random translation, scaling and rotation in each image
- Optimizing using  gradient descent

#### Experiment
- Two white box, a black box and a control patch
- White box attack jointly trains a single patch across five ImageNet models (inception3, resnet50, exception, VGG16 and VGG19)
- Attack is evaluated by averaging the win rate across all 5 models
- Patches are rescaled and inserted on a random location
- Size of patch for black box has to be larger than others
- Transferability to physical world by printing generated patch 

#### Result
-  When a photo of a tabletop with a banana and a notebook is passed through VGG16, the network reports class ’banana’ with 97% confidence. If we physically place a sticker targeted to the class "toaster" on the table (bottom photograph),
the photograph is classified as a toaster with 99% confidence.

#### Conclusion
-  Can generate a universal, robust, targeted patch that fools classifiers regardless of
the scale or location of the patch
- Does not require knowledge of the other items in the scene
that it is attacking
- The attack works in the real world, and can be disguised as an innocuous sticker.
- The attack could be created offline, and then broadly shared