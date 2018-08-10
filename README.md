# CNN-models-comparison
The goal of this repository is:
- To see the comparison of famous CNN models at a glance
- To keep on track of new or improved CNN architectures
- To access their research papers and implementations on different frameworks

(This repository will be updated regularly.)

## Comparison Table
CNN model comparison table on the [ImageNet](http://www.image-net.org/) classification results, reference paper and implementations.

Model | Detail | Inpus size | Parameters | Mult-Adds | FLOPS | Depth | Top-1 Acc | Top-5 Acc | Model Reference | TensorFlow | Keras | Pytorch | Caffe | Else
-- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | --
AmoebaNet-B | (N=6, F=228) | 331x331⁵ | 155.3M⁵ | 41.1B⁵ |   |   | 83.10⁵ | 96.30⁵ | [Link](https://arxiv.org/abs/1802.01548) | - | - | - | - | -
PNASNet-5_Large | (N=4, F=216) | 331x331⁵ | 86.1M⁵ | 25.0B⁵ |   |   | 82.90⁵ | 96.20⁵ | [Link](https://arxiv.org/abs/1712.00559) | [Link](https://github.com/tensorflow/models/tree/master/research/slim) | - | - | - | -
AmoebaNet-B | (N=6, F=190) | 331x331⁵ | 86.7M⁵ | 23.1B⁵ |   |   | 82.80⁵ | 96.10⁵ | [Link](https://arxiv.org/abs/1802.01548) | - | - | - | - | -
SENet-154 |   | 320x320⁵ | 145.8M⁵ | 42.3B⁵ |   |   | 82.70⁵ | 96.20⁵ | [Link](https://arxiv.org/pdf/1709.01507.pdf) | [Link](https://github.com/kobiso/SENet-tensorflow-slim) | [Link](https://github.com/titu1994/keras-squeeze-excite-network) | [Link](https://github.com/pytorch/vision/tree/master/torchvision) | [Link](https://github.com/hujie-frank/SENet) | -
NASNet-A_Large | (N=6, F=168) | 331x331⁵ | 88.9M⁵ | 23.8B⁵ |   |   | 82.70⁵ | 96.20⁵ | [Link](https://arxiv.org/abs/1707.07012) | [Link](https://github.com/tensorflow/models/tree/master/research/slim) | [Link](https://keras.io/applications/) | [Link](https://github.com/wandering007/nasnet-pytorch) | - | -
AmoebaNet-B | (N=6, F=190) | 331x331⁵ | 84.0M⁵ | 22.3B⁵ |   |   | 82.30⁵ | 96.10⁵ | [Link](https://arxiv.org/abs/1802.01548) | - | - | - | - | -
Dual-Path-Net-131 |   | 320x320⁵ | 79.5M⁵ | 32.0B⁵ |   |   | 81.50⁵ | 95.80⁵ | [Link](https://arxiv.org/abs/1707.01629) | - | [Link](https://github.com/titu1994/Keras-DualPathNetworks) | [Link](https://github.com/Queequeg92/DualPathNet) | [Link](https://github.com/cypw/DPNs) | [Link](https://github.com/cypw/DPNs)
PolyNet |   | 331x331⁵ | 92M⁵ | 34.7B⁵ |   |   | 81.30⁵ | 95.80⁵ | [Link](https://arxiv.org/abs/1611.05725) | - | - | [Link](https://github.com/Cadene/pretrained-models.pytorch/blob/master/pretrainedmodels/models/polynet.py) | [Link](https://github.com/CUHK-MMLAB/polynet) | -
ResNeXt-101 | (64x4d) | 320x320⁵ | 83.6M⁵ | 31.5B⁵ |   |   | 80.90⁵ | 95.60⁵ | [Link](https://arxiv.org/abs/1611.05431) | [Link](https://github.com/taki0112/ResNeXt-Tensorflow) | [Link](https://github.com/titu1994/Keras-ResNeXt) | [Link](https://github.com/prlz77/ResNeXt.pytorch) | [Link](https://github.com/cypw/ResNeXt-1) | [Link](https://github.com/facebookresearch/ResNeXt)
Inception-ResNet-v2 |   | 299x299¹ | 55.8M² |   | 11.75G⁴ | 572² | 80.40¹ | 95.30¹ | [Link](http://arxiv.org/abs/1602.07261) | [Link](https://github.com/tensorflow/models/tree/master/research/slim) | [Link](https://keras.io/applications/) | - | [Link](https://github.com/twtygqyy/Inception-resnet-v2) | -
Inception-ResNet-v2+SE |   | 299X299⁴ |   |   | 11.76G⁴ |   | 80.20⁴ | 95.21⁴ | [Link](https://arxiv.org/pdf/1709.01507.pdf) | [Link](https://github.com/kobiso/SENet-tensorflow-slim) | - | [Link](https://github.com/moskomule/senet.pytorch) | [Link](https://github.com/hujie-frank/SENet) | -
Inception V4 |   | 299x299¹ | 46M¹ |   |   |   | 80.20¹ | 95.20¹ | [Link](http://arxiv.org/abs/1602.07261) | [Link](https://github.com/tensorflow/models/tree/master/research/slim) | [Link](https://github.com/kentsommer/keras-inceptionV4) | [Link](https://github.com/pytorch/vision/tree/master/torchvision) | - | -
ResNet V2 200 |   | 320x320 | 64.7M |   | 15G |   | 79.90¹ | 95.20¹ | [Link](https://arxiv.org/abs/1603.05027) | [Link](https://github.com/tensorflow/models/tree/master/research/slim) | [Link](https://github.com/raghakot/keras-resnet) | - | [Link](https://github.com/soeaver/caffe-model/tree/master/cls/resnet-v2) | -
Xception |   | 299x299² | 23M² |   |   | 126² | 79.00² | 94.50² | [Link](https://arxiv.org/abs/1610.02357) | [Link](https://github.com/kwotsin/TensorFlow-Xception) | [Link](https://keras.io/applications/) | [Link](https://github.com/tstandley/Xception-PyTorch) | [Link](https://github.com/yihui-he/Xception-caffe) | -
ResNeXt-101+CBAM | (32x4d) | 224x224³ | 49M³ |   | 7.519G³ |   | 78.93³ | 94.41³ | [Link](https://arxiv.org/pdf/1807.06521.pdf) | [Link](https://github.com/kobiso/CBAM-tensorflow) | [Link](https://github.com/kobiso/CBAM-keras) | - | - | -
ResNeXt-101+SE | (32x4d) | 224x224³ | 49M³ |   | 7.512G³ |   | 78.83³ | 94.34³ | [Link](https://arxiv.org/pdf/1709.01507.pdf) | [Link](https://github.com/taki0112/SENet-Tensorflow) | - | - | [Link](https://github.com/hujie-frank/SENet) | -
ResNet101+CBAM |   | 224x224³ | 49M³ |   | 7.581G³ |   | 78.49³ | 94.31³ | [Link](https://arxiv.org/pdf/1807.06521.pdf) | [Link](https://github.com/kobiso/CBAM-tensorflow-slim) | [Link](https://github.com/kobiso/CBAM-keras) | - | - | -
ResNeXt-101 | (32x4d) | 224x224³ | 44.2M³ |   | 7.508G³ |   | 78.46³ | 94.25³ | [Link](https://arxiv.org/abs/1611.05431) | [Link](https://github.com/taki0112/ResNeXt-Tensorflow) | [Link](https://github.com/titu1994/Keras-ResNeXt) | [Link](https://github.com/prlz77/ResNeXt.pytorch) | [Link](https://github.com/cypw/ResNeXt-1) | [Link](https://github.com/facebookresearch/ResNeXt)
ResNeXt50+SE | (32x4d) | 224x224³ | 27.6M³ |   | 3.771G³ |   | 78.09³ | 93.96³ | [Link](https://arxiv.org/pdf/1709.01507.pdf) | [Link](https://github.com/taki0112/SENet-Tensorflow) | - | - | [Link](https://github.com/hujie-frank/SENet) | -
ResNeXt50+CBAM | (32x4d) | 224x224³ | 27.6M³ |   | 3.774G³ |   | 78.08³ | 94.09³ | [Link](https://arxiv.org/pdf/1807.06521.pdf) | [Link](https://github.com/kobiso/CBAM-tensorflow) | [Link](https://github.com/kobiso/CBAM-keras) | - | - | -
Inception V3 |   | 299x299¹ | 23.8M² |   |   | 159² | 78.00¹ | 93.90¹ | [Link](http://arxiv.org/abs/1512.00567) | [Link](https://github.com/tensorflow/models/tree/master/research/slim) | [Link](https://keras.io/applications/) | [Link](https://github.com/pytorch/vision/tree/master/torchvision) | [Link](https://github.com/smichalowski/google_inception_v3_for_caffe) | -
ResNet V2 152 |   | 299x299¹ |   |   |   |   | 77.80¹ | 94.10¹ | [Link](https://arxiv.org/abs/1603.05027) | [Link](https://github.com/tensorflow/models/tree/master/research/slim) | [Link](https://github.com/raghakot/keras-resnet) | - | [Link](https://github.com/soeaver/caffe-model/tree/master/cls/resnet-v2) | -
ResNet101+SE |   | 224x224³ | 49M³ |   | 7.575G³ |   | 77.65³ | 93.81³ | [Link](https://arxiv.org/pdf/1709.01507.pdf) | [Link](https://github.com/kobiso/SENet-tensorflow-slim) | - | [Link](https://github.com/moskomule/senet.pytorch) | [Link](https://github.com/hujie-frank/SENet) | -
ResNet50+CBAM |   | 224x224³ | 28M³ |   | 3.864G³ |   | 77.34³ | 93.69³ | [Link](https://arxiv.org/pdf/1807.06521.pdf) | [Link](https://github.com/kobiso/CBAM-tensorflow-slim) | [Link](https://github.com/kobiso/CBAM-keras) | - | - | -
ResNeXt50 | (32x4d) | 224x224³ | 25M³ |   | 3.768G³ |   | 77.15³ | 94.25³ | [Link](https://arxiv.org/abs/1611.05431) | [Link](https://github.com/taki0112/ResNeXt-Tensorflow) | [Link](https://github.com/titu1994/Keras-ResNeXt) | [Link](https://github.com/prlz77/ResNeXt.pytorch) | [Link](https://github.com/cypw/ResNeXt-1) | [Link](https://github.com/facebookresearch/ResNeXt)
DenseNet201 |   | 224x224² | 20M² |   |   | 201² | 77.00² | 93.30² | [Link](https://arxiv.org/abs/1608.06993) | [Link](https://github.com/YixuanLi/densenet-tensorflow) | [Link](https://keras.io/applications/) | [Link](https://github.com/pytorch/vision/tree/master/torchvision) | [Link](https://github.com/shicai/DenseNet-Caffe) | -
ResNet V2 101 |   | 299x299¹ |   |   |   |   | 77.00¹ | 93.70¹ | [Link](https://arxiv.org/abs/1603.05027) | [Link](https://github.com/tensorflow/models/tree/master/research/slim) | [Link](https://github.com/raghakot/keras-resnet) | - | [Link](https://github.com/soeaver/caffe-model/tree/master/cls/resnet-v2) | -
ResNet50+SE |   | 224x224³ | 28M³ |   | 3.86G³ |   | 76.86³ | 93.30³ | [Link](https://arxiv.org/pdf/1709.01507.pdf) | [Link](https://github.com/kobiso/SENet-tensorflow-slim) | - | [Link](https://github.com/moskomule/senet.pytorch) | [Link](https://github.com/hujie-frank/SENet) | -
ResNet V1 152 |   | 224x224¹ | 60M |   | 11.3G⁴ | 517 | 76.80¹ | 93.20¹ | [Link](https://arxiv.org/abs/1512.03385) | [Link](https://github.com/tensorflow/models/tree/master/research/slim) | [Link](https://github.com/statech/resnet) | [Link](https://github.com/pytorch/vision/tree/master/torchvision) | [Link](https://github.com/KaimingHe/deep-residual-networks) | [Link](https://github.com/facebook/fb.resnet.torch)
ResNet V1 101 |   | 224x224¹ | 45M³ |   | 7.57G³ |   | 76.40¹ | 92.90¹ | [Link](https://arxiv.org/abs/1512.03385) | [Link](https://github.com/tensorflow/models/tree/master/research/slim) | [Link](https://github.com/statech/resnet) | [Link](https://github.com/pytorch/vision/tree/master/torchvision) | [Link](https://github.com/KaimingHe/deep-residual-networks) | [Link](https://github.com/facebook/fb.resnet.torch)
DenseNet169 |   | 224x224² | 14M² |   |   | 169² | 75.90² | 92.80² | [Link](https://arxiv.org/abs/1608.06993) | [Link](https://github.com/YixuanLi/densenet-tensorflow) | [Link](https://keras.io/applications/) | [Link](https://github.com/pytorch/vision/tree/master/torchvision) | [Link](https://github.com/shicai/DenseNet-Caffe) | -
BN-Inception+SE |   | 224x224⁴ |   |   | 2.04G⁴ |   | 75.77⁴ | 92.86⁴ | [Link](https://arxiv.org/pdf/1709.01507.pdf) | [Link](https://github.com/kobiso/SENet-tensorflow-slim) | - | - | [Link](https://github.com/hujie-frank/SENet) | -
ResNet V2 50 |   | 299x299¹ |   |   |   |   | 75.60¹ | 92.80¹ | [Link](https://arxiv.org/abs/1603.05027) | [Link](https://github.com/tensorflow/models/tree/master/research/slim) | [Link](https://github.com/raghakot/keras-resnet) | - | [Link](https://github.com/soeaver/caffe-model/tree/master/cls/resnet-v2) | -
ResNet V1 50 |   | 224x224¹ | 25.6M² |   | 3.858G³ | 168² | 75.20¹ | 92.20¹ | [Link](https://arxiv.org/abs/1512.03385) | [Link](https://github.com/tensorflow/models/tree/master/research/slim) | [Link](https://keras.io/applications/) | [Link](https://github.com/pytorch/vision/tree/master/torchvision) | [Link](https://github.com/KaimingHe/deep-residual-networks) | [Link](https://github.com/facebook/fb.resnet.torch)
WideResNet18+CBAM | widen=2.0 | 224x224³ | 45.97M³ |   | 6.697G³ |   | 75.16³ | 92.37³ | [Link](https://arxiv.org/pdf/1807.06521.pdf) | - | - | - | - | -
WideResNet18+SE | widen=2.0 | 224x224³ | 45.97M³ |   | 6.696G³ |   | 75.07³ | 92.35³ | [Link](https://arxiv.org/pdf/1709.01507.pdf) | - | - | - | [Link](https://github.com/hujie-frank/SENet) | -
MobileNet_v2 | α=1.4 | 224x224¹ | 6M |   |   |   | 74.90¹ | 92.50¹ | [Link](https://arxiv.org/abs/1801.04381) | [Link](https://github.com/tensorflow/models/tree/master/research/slim) | [Link](https://keras.io/applications/) | [Link](https://github.com/tonylins/pytorch-mobilenet-v2) | [Link](https://github.com/shicai/MobileNet-Caffe) | -
BN-Inception |   | 224x224⁴ |   |   | 2.03G⁴ |   | 74.62⁴ | 92.21⁴ | [Link](https://arxiv.org/pdf/1502.03167) | - | - | - | [Link](https://github.com/pertusa/InceptionBN-21K-for-Caffe) | -
DenseNet121 |   | 224x224² | 8M² |   |   | 121² | 74.50² | 91.80² | [Link](https://arxiv.org/abs/1608.06993) | [Link](https://github.com/YixuanLi/densenet-tensorflow) | [Link](https://keras.io/applications/) | [Link](https://github.com/pytorch/vision/tree/master/torchvision) | [Link](https://github.com/shicai/DenseNet-Caffe) | -
WideResNet18 | widen=2.0 | 224x224³ | 45.62M³ |   | 6.696G³ |   | 74.37³ | 91.80³ | [Link](https://arxiv.org/abs/1605.07146) | [Link](https://github.com/dalgu90/wrn-tensorflow) | [Link](https://github.com/titu1994/Wide-Residual-Networks) | [Link](https://github.com/xternalz/WideResNet-pytorch) | [Link](https://github.com/razorx89/caffe-wrn-generator) | -
ResNet34+CBAM |   | 224x224³ | 22M³ |   | 3.665G³ |   | 74.01³ | 91.76³ | [Link](https://arxiv.org/pdf/1807.06521.pdf) | [Link](https://github.com/kobiso/CBAM-tensorflow-slim) | [Link](https://github.com/kobiso/CBAM-keras) | - | - | -
NASNet-A_Mobile |   | 224x224¹ |   |   |   |   | 74.00¹ | 91.60¹ | [Link](https://arxiv.org/abs/1707.07012) | [Link](https://github.com/tensorflow/models/tree/master/research/slim) | [Link](https://keras.io/applications/) | [Link](https://github.com/wandering007/nasnet-pytorch) | - | -
WideResNet18+CBAM | widen=1.5 | 224x224³ | 26.08M³ |   | 3.868G³ |   | 73.90³ | 91.57³ | [Link](https://arxiv.org/pdf/1807.06521.pdf) | - | - | - | - | -
Inception V2 |   | 224x224¹ |   |   |   |   | 73.90¹ | 91.80¹ | [Link](http://arxiv.org/abs/1502.03167) | [Link](https://github.com/tensorflow/models/tree/master/research/slim) | - | [Link](https://github.com/pytorch/vision/tree/master/torchvision) | - | -
ResNet34+SE |   | 224x224³ | 22M³ |   | 3.664G³ |   | 73.87³ | 91.65³ | [Link](https://arxiv.org/pdf/1709.01507.pdf) | [Link](https://github.com/kobiso/SENet-tensorflow-slim) | - | [Link](https://github.com/moskomule/senet.pytorch) | [Link](https://github.com/hujie-frank/SENet) | -
WideResNet18+SE | widen=1.5 | 224x224³ | 26.07M³ |   | 3.867G³ |   | 73.79³ | 91.53³ | [Link](https://arxiv.org/pdf/1709.01507.pdf) | - | - | - | [Link](https://github.com/hujie-frank/SENet) | -
ResNet34 |   | 224x224³ | 21.8M³ |   | 3.664G³ |   | 73.31³ | 91.40³ | [Link](https://arxiv.org/abs/1512.03385) | [Link](https://github.com/tensorflow/models/tree/master/research/slim) | - | [Link](https://github.com/pytorch/vision/tree/master/torchvision) | [Link](https://github.com/KaimingHe/deep-residual-networks) | [Link](https://github.com/facebook/fb.resnet.torch)
WideResNet18 | widen=1.5 | 224x224³ | 25.88M³ |   | 3.866G³ |   | 73.15³ | 91.12³ | [Link](https://arxiv.org/abs/1605.07146) | [Link](https://github.com/dalgu90/wrn-tensorflow) | [Link](https://github.com/titu1994/Wide-Residual-Networks) | [Link](https://github.com/xternalz/WideResNet-pytorch) | [Link](https://github.com/razorx89/caffe-wrn-generator) | -
MobileNet_v2 | α=1.0 | 224x224¹ | 3.47M |   |   |   | 71.90¹ | 91.00¹ | [Link](https://arxiv.org/abs/1801.04381) | [Link](https://github.com/tensorflow/models/tree/master/research/slim) | [Link](https://keras.io/applications/) | [Link](https://github.com/tonylins/pytorch-mobilenet-v2) | [Link](https://github.com/shicai/MobileNet-Caffe) | -
VGG 16 |   | 224x224¹ | 138M² |   | 15.47⁴ | 23² | 71.50¹ | 89.80¹ | [Link](http://arxiv.org/abs/1409.1556.pdf) | [Link](https://github.com/tensorflow/models/tree/master/research/slim) | [Link](https://keras.io/applications/) | [Link](https://github.com/pytorch/vision/tree/master/torchvision) | [Link](https://github.com/davidgengenbach/vgg-caffe) | -
VGG 19 |   | 224x224¹ | 143M² |   |   | 26² | 71.10¹ | 89.80¹ | [Link](http://arxiv.org/abs/1409.1556.pdf) | [Link](https://github.com/tensorflow/models/tree/master/research/slim) | [Link](https://keras.io/applications/) | [Link](https://github.com/pytorch/vision/tree/master/torchvision) | [Link](https://github.com/davidgengenbach/vgg-caffe) | -
MobileNet_v1+CBAM | α=1.0 | 224x224³ | 5.07M³ |   | 0.576G³ |   | 70.99³ | 90.01³ | [Link](https://arxiv.org/pdf/1807.06521.pdf) | - | [Link](https://github.com/kobiso/CBAM-keras) | - | - | -
MobileNet_v1 | α=1.0 | 224x224¹ |   |   |   |   | 70.90¹ | 89.90¹ | [Link](https://arxiv.org/pdf/1704.04861.pdf) | [Link](https://github.com/tensorflow/models/tree/master/research/slim) | [Link](https://keras.io/applications/) | [Link](https://github.com/marvis/pytorch-mobilenet) | [Link](https://github.com/shicai/MobileNet-Caffe) | -
ResNet18+CBAM |   | 224x224³ | 11.8M³ |   | 1.815G³ |   | 70.73³ | 89.91³ | [Link](https://arxiv.org/pdf/1807.06521.pdf) | [Link](https://github.com/kobiso/CBAM-tensorflow-slim) | [Link](https://github.com/kobiso/CBAM-keras) | - | - | -
ResNet18+SE |   | 224x224³ | 11.8M³ |   | 1.814G³ |   | 70.59³ | 89.78³ | [Link](https://arxiv.org/pdf/1709.01507.pdf) | [Link](https://github.com/kobiso/SENet-tensorflow-slim) | - | [Link](https://github.com/moskomule/senet.pytorch) | [Link](https://github.com/hujie-frank/SENet) | -
ResNet18 |   | 224x224³ | 11.7M³ |   | 1.814G³ |   | 70.40³ | 89.45³ | [Link](https://arxiv.org/abs/1512.03385) | [Link](https://github.com/tensorflow/models/tree/master/research/slim) | - | [Link](https://github.com/pytorch/vision/tree/master/torchvision) | [Link](https://github.com/KaimingHe/deep-residual-networks) | [Link](https://github.com/facebook/fb.resnet.torch)
MobileNet_v1+SE | α=1.0 | 224x224³ | 5.07M³ |   | 0.570G³ |   | 70.03³ | 89.37³ | [Link](https://arxiv.org/pdf/1709.01507.pdf) | - | - | - | [Link](https://github.com/hujie-frank/SENet) | -
Inception V1 |   | 224x224¹ |   |   |   |   | 69.80¹ | 89.60¹ | [Link](http://arxiv.org/abs/1409.4842v1) | [Link](https://github.com/tensorflow/models/tree/master/research/slim) | [Link](https://gist.github.com/joelouismarino/a2ede9ab3928f999575423b9887abd14) | [Link](https://github.com/pytorch/vision/tree/master/torchvision) | - | -
MobileNet_v1 | α=1.0 | 224x224³ | 4.23M³ |   | 0.569G³ |   | 68.61³ | 88.49³ | [Link](https://arxiv.org/pdf/1704.04861.pdf) | [Link](https://github.com/tensorflow/models/tree/master/research/slim) | [Link](https://keras.io/applications/) | [Link](https://github.com/marvis/pytorch-mobilenet) | [Link](https://github.com/shicai/MobileNet-Caffe) | -
MobileNet_v1+CBAM | α=0.7 | 224x224³ | 2.71M³ |   | 0.289G³ |   | 68.49³ | 88.52³ | [Link](https://arxiv.org/pdf/1807.06521.pdf) | - | [Link](https://github.com/kobiso/CBAM-keras) | - | - | -
ShuffleNet+SE | 1x(g=3) | 224x224⁴ | 2.4M⁴ |   | 0.142G⁴ |   | 68.30⁴ | 88.30⁴ | [Link](https://arxiv.org/pdf/1709.01507.pdf) | - | - | - | [Link](https://github.com/hujie-frank/SENet) | -
MobileNet_v1+SE | α=0.7 | 224x224³ | 2.71M³ |   | 0.283G³ |   | 67.50³ | 87.51³ | [Link](https://arxiv.org/pdf/1709.01507.pdf) | - | - | - | [Link](https://github.com/hujie-frank/SENet) | -
ShuffleNet | 1x(g=3) | 224x224⁴ | 1.8M⁴ |   | 0.14G⁴ |   | 66.10⁴ | 86.40⁴ | [Link](https://arxiv.org/pdf/1707.01083) | [Link](https://github.com/MG2033/ShuffleNet) | [Link](https://github.com/scheckmedia/keras-shufflenet) | [Link](https://github.com/jaxony/ShuffleNet) | [Link](https://github.com/farmingyard/ShuffleNet) | -
MobileNet_v1 | α=0.7 | 224x224³ | 2.3M³ |   | 0.283G³ |   | 65.14³ | 86.31³ | [Link](https://arxiv.org/pdf/1704.04861.pdf) | [Link](https://github.com/tensorflow/models/tree/master/research/slim) | [Link](https://keras.io/applications/) | [Link](https://github.com/marvis/pytorch-mobilenet) | [Link](https://github.com/shicai/MobileNet-Caffe) | -
MobileNet_v1 | α=0.5 | 160x160¹ |   |   |   |   | 59.10¹ | 81.90¹ | [Link](https://arxiv.org/pdf/1704.04861.pdf) | [Link](https://github.com/tensorflow/models/tree/master/research/slim) | [Link](https://keras.io/applications/) | [Link](https://github.com/marvis/pytorch-mobilenet) | [Link](https://github.com/shicai/MobileNet-Caffe) | -
MobileNet_v1 | α=0.25 | 128x128¹ |   |   |   |   | 41.50¹ | 66.30¹ | [Link](https://arxiv.org/pdf/1704.04861.pdf) | [Link](https://github.com/tensorflow/models/tree/master/research/slim) | [Link](https://keras.io/applications/) | [Link](https://github.com/marvis/pytorch-mobilenet) | [Link](https://github.com/shicai/MobileNet-Caffe) | -

- **Mult-Adds**: The number of multiply-add operations
- **FLOPS**: The floating point operations

### Value References
Superscript numbers on each value indicate the reference number of each value from.
1. [TF-Slim](https://github.com/tensorflow/models/tree/master/research/slim)
2. [Keras: Applications](https://keras.io/applications/)
3. [CBAM: Convolutional Block Attention Module](https://arxiv.org/pdf/1807.06521.pdf)
4. [Squeeze-and-Excitation Networks](https://arxiv.org/pdf/1709.01507.pdf)
5. [Progressive Neural Architecture Search](https://arxiv.org/pdf/1712.00559.pdf)
6. [Residual Attention Network for Image Classification](https://arxiv.org/pdf/1704.06904.pdf)

## Related Resources
Check the other good resources about CNN models
- [Caffe-model](https://github.com/soeaver/caffe-model)
- [TensorNets](https://github.com/taehoonlee/tensornets)
- [DeepDetect : Open Source Deep Learning Server & API](https://github.com/jolibrain/deepdetect#deepdetect--open-source-deep-learning-server--api)
- [Pretrained models for Pytorch](https://github.com/Cadene/pretrained-models.pytorch)
- [Netscope CNN Analyzer](https://dgschwend.github.io/netscope/quickstart.html)
- [Memory consumption and FLOP count](https://github.com/albanie/convnet-burden)

## Author
Byung Soo Ko / kobiso62@gmail.com
