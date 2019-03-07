eip 3

what is convolution
we have a function and we are converting that to image
divide imge into many functions

output resolution

1x1 convolution is pointwise --> reduce the channels

idea of receptive field - see the object fully
we have image of 10x10, we add 3x3, receptive field is now 3x3 - global receptive field

---

my receptive field should be the size of the image - we are talking aobut the object which are very large
size of the image = size of the object ^

for small object this chain is breaking

the size of the obiject is nearly as the size of the imgage
network will start learning edges and texture with pattern 

--- 

checkboard issue (mosquito net)
we are covering some pixels more than others

---
we have kernal of 3x3 - then local receptive field is 3x3
Q. how do we make this to 5x5 local receptive field
A. adding padding diretly to kernal and not image - 3x3 dilated convolution (dilation of 1.. for 5x5)
this is specifically \used for image segmentation ^
---

5x5 - kernal is 3x3 - output is 3x3
5x5 - kernal is 3x3 - output is 7x7 - 

ground truth?
---
problem that we trying to slve
5x5x3 > 15x15x3

A. 
5x5x3 | (1x1x3)x27 (adding ) | 5x5x27 (output)
5x5x27 | (5x5x9)x3

using pixel shuffle algorithm
---
depthwise convolution

--- 
grouped convolutions
---
dropout - training on more images
it will make sure you can change questionin your book
sideeffect of dropoout

---
A3
1. epoch do not matter
18000 is the limit

image augmentation
small image

negative for image dropout

2. yolo

3.



