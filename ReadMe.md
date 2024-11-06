# DLFuzz implementation

DLFuzz is an adversarial input generator presented in this paper : https://arxiv.org/pdf/1808.09413

Adversarial inputs are generated for a DNN composed of 5 fully connected layers and trained on the MNIST dataset.

This model achieved 95% accuracy on the test dataset. 
We only generate an adversarial input from a well classified input.

This implementation of DLFuzz generated 121 adversarial inputs out of 5000 images from the test set.
Each adversarial input has an L2 distance with the original input bounded by 0.002

## Examples

![capture 1](images/capture_1.png)
***Left** is adversarial input recognised as 9, **right** is original input recognized as 4*

![capture 2](images/capture_2.png)
***Left** is adversarial input recognised as 7, **right** is original input recognized as 9*

## Next

Next step would be to generate adversarials inputs for a Convolutionnal Neural Network which could achieve much higher accuracy than the DNN used here.