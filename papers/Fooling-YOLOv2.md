
# [Fooling Automated Survelliance Cameras  Adversarial patches to attack person detection](https://arxiv.org/pdf/1904.08653.pdf)


 #### Key Points
The paper demonestrates how a "patch" can be applied to an object can mislead object detectors and classifiers.

The patch:

- 40x40 cm
- printable
- can lower accuracy
- can hide a person
- optimized using Adam algorithm
- targets YOLOv2 object detector
- Randomly transformation ( rotated 20degree, random scale up and down, random noise)

The end goal of the patch is minimise a total loss created by:
    
  1) non-printability score:- a factor colors that can bre represented by a common printer
  2) the total variation: with smooth color transition
  3) maximum objectnesss score
