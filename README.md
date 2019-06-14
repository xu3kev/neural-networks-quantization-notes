# Neural Networks Quantization

## Linear Quantization

### Quantization-Aware Training
- [PACT: Parameterized Clipping Activation for Quantized Neural Networks](https://arxiv.org/abs/1805.06085)
  - Relu-α where α is learnable parameter with L2 regularization
  
- [Accurate and Efficient 2-bit Quantized Neural Networks](https://www.sysml.cc/doc/2019/168.pdf)
  - PACT quantization aware training
  - Statistic-Aware Weight Binning
  - full precision for shortcut connections in resnet
  
- [Fully Quantized Network for Object Detection](http://openaccess.thecvf.com/content_CVPR_2019/papers/Li_Fully_Quantized_Network_for_Object_Detection_CVPR_2019_paper.pdf)
  - 4bits quantization
  - Freeze BN statistic
  - clamped activation from calibration statistic
  - channel-wise quantization scale

- [Simultaneously Optimizing Weight and Quantizer of Ternary Neural Network using Truncated Gaussian Approximation](http://openaccess.thecvf.com/content_CVPR_2019/papers/He_Simultaneously_Optimizing_Weight_and_Quantizer_of_Ternary_Neural_Network_Using_CVPR_2019_paper.pdf)


## Non-Uniform Quantization:
- [LQ-Nets: Learned Quantization for Highly Accurate and Compact Deep Neural Networks](https://arxiv.org/abs/1807.10029)
- [Quantization Networks](http://openaccess.thecvf.com/content_CVPR_2019/papers/Yang_Quantization_Networks_CVPR_2019_paper.pdf)



## Quantization Support in Libraries
- TensorRT
  - Per channel weight scale
  - Calibration: minimize KL Divergence
- Tensorflow lite
  - Per channel  weight scale
  - Calibration: min max??
- TVM
  - Per channel weight scale
  - Calibration: minimize MSE
