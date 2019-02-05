# ConvNet
## How Convolutional Nerual Networks Work
### Fully connected layer
* Input:32x32x3
* Output:10
* Weights:3072(32x32x3)x10
### Convolutional layer
* Input:Keep the structure of the image 32x32x3
* Output:28x28x1
* Weights:small filters like 5x5x3
<br>Convolution is a looser definition in there.

## ConvNet
* ConvNet is a sequence of convolutional layers, interspersed with activation functions.
* The filters of the earlier layers usually represent low-level features. Things kind of like edges.
* Mid-level features get more complex features. Things kind of like corners and blobs.
* At high-level features get more resemble concepts than blobs.

### Output Size
* output_size=(N-F)/stride+1
<br>
N : dimension of input<br>
F : filter size

### Common to zero pad the border
* we can get the same output size of input size.
* provide the activation maps sizes shrinking and features losing quickly.

### 1x1 convolution layer
* 32x32x64 through 32 1x1(x32) convolution layer to become 32x32x32

## Pooling layer
* downsample 224x224x3 to 112x112x3
* max-pooling, average-pooling
* just look as a region and next a region

