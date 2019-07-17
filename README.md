# Robust 3D Face Alignment with Efficient Fully Convolutional Neural Networks - Pytorch
Accepted in: The 10th International Conference on Image and Graphics(ICIG2019)-Oral

## Note
In 'Demo.py' file, you will find how to run these codes.
In 'FaceSwap/Demo2.py' file, you will find how to run face swap code.

## Abstract
In this paper proposes a novel and efficient end-to-end 3D face alignment framework.We build an efficient and stable network model through Depthwise Separable Convolution
and Densely Connected Convolutional,named MobDenseNet. Simultaneously,different loss functions are used to constrain 3D parameters based on 3D Morphable Model (3DMM) and 3D vertices

### The framework of ours proposes method
![](https://github.com/LeiJiangJNU/R3FA/blob/master/figures/framework01.png)

### MobDenseNet Structure
<img src="https://github.com/LeiJiangJNU/R3FA/blob/master/figures/MobDenseNet.png" width="600">

### Layer3 Structure-DenseBlock
<img src="https://github.com/LeiJiangJNU/R3FA/blob/master/figures/layer3.png" width="600">


## Training

![](https://github.com/hli1221/imagefusion_densefuse/blob/master/figures/train.png)

We train our network using MS-COCO(T.-Y. Lin, M. Maire, S. Belongie, J. Hays, P. Perona, D. Ramanan, P. Dollar, and C. L. Zitnick. Microsoft coco: Common objects in context. In ECCV, 2014. 3-5.) as input images which contains 80000 images and all resize to 256×256 and RGB images are transformed to gray ones. Learning rate is 1×10^(-4). The batch size and epochs are 2 and 4, respectively. Our method is implemented with GTX 1080Ti and 64GB RAM.


## Experimental results

### Infrared and visible images('street')
![](https://github.com/hli1221/imagefusion_densefuse/blob/master/figures/fused_street.png)

### Infrared and visible images(RGB)
Database:  
Hwang S, Park J, Kim N, et al. Multispectral pedestrian detection: Benchmark dataset and baseline[C]//Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. 2015: 1037-1045.  

![](https://github.com/hli1221/imagefusion_densefuse/blob/master/figures/ivrgb_results.png)

### Multi-focus images(RGB)
![](https://github.com/hli1221/imagefusion_densefuse/blob/master/figures/fused_color.png)

If you have any question about this code, feel free to reach me(hui_li_jnu@163.com, lihui@stu.jiangnan.edu.cn)


# Citation

For paper:

 *H. Li, X. J. Wu, “DenseFuse: A Fusion Approach to Infrared and Visible Images,” IEEE Trans. Image Process., vol. 28, no. 5, pp. 2614–2623, May. 2019.*

For code:
```
@misc{li2018IVimagefusion_densefuse,
    author = {Hui Li},
    title = {CODE: DenseFuse_A Fusion Approach to Infrared and Visible Images},
    year = {2018},
    publisher = {GitHub},
    journal = {GitHub repository},
    howpublished = {\url{https://github.com/hli1221/imagefusion_densefuse}}
  }
```
