# Project - LinNet
---
## Abstract
Networks with residual units, such as ResNet had proven its use in various domain of AI such as image classification. However, the commonly used models, such as ResNetV2, BiT ensure some degree of "shorter pathes" between two layers, but it is restricted due to the construction of the residual connection with identity/downscale of the original inputs. In this project, the alternative version of ResNet, a LinNet is proposed for purpose of generalizing not only residual, but all the possible connections between the layers.

## LinNet - Main Ideas
---
Residual units are usually expressed in general form:

$y_l = h(x_l) + F(x_l, W_l),$

$x_l + 1 = f(y_l),$

Most of the models commonly use $h$ as an identity function, or downscale of the original input by convolution.

However, LinNet Model Uses a huge accumulation layer, or network to imitate this residual connection, and furthermore generalize the connection between layers.

How LinNet Works
---
<image scr = "img1.png"> </image>
