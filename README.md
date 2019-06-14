# Neural Networks Quantization

## Linear Quantization

### Quantization-Aware Training
- [PACT: Parameterized Clipping Activation for Quantized Neural Networks](https://arxiv.org/abs/1805.06085)
  - ![equation](http://www.sciweavers.org/tex2img.php?eq=y%20%3D%20%5Cittext%7BPACT%7D%28x%29%20%3D%20%5Cbegin%7Bcases%7D%0A0%20%2C%20%26%5Ctext%7B%24x%3C0%24%7D%5C%5C%0Ax%20%2C%20%26%5Ctext%7B%240%20%5Cleq%20x%20%3C%20%5Calpha%24%7D%5C%5C%0A%5Calpha%20%2C%20%26%20%5Ctext%7B%24%5Calpha%20%5Cleq%20x%24%7D%0A%5Cend%7Bcases%7D%0A&bc=White&fc=Black&im=png&fs=12&ff=txfonts&edit=0)

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





