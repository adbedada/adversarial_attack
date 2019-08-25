# [Black-box Adversarial ML Attack on Modulation Classification](https://arxiv.org/pdf/1908.00635.pdf) 


#### Key Point

The paper discusses the reesult of a Carlini & Wegner (C-W) adversarial attack to test the robustness of SoTA modulatioon classfiers.

Two types of attack settings: 

- White-box: Attacks based on the assumption that the adversary has complete knowledge (hyperparameters, test data, etc.) of the deployed model.
- Black-box: Attacks based on no knowledge of the deployed ML model. Adversary can only act as  standard user and query the system for a response.
  
FGSM (Fast Gradient Sign Method) is an adversarial sample crafting algorithm where the adversarial perturbation is calculated by taking a gradient step in the direction of the sign of the gradient of test example.
