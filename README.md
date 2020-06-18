## [Semi-Supervised Semantic Image Segmentation With Self-Correcting Networks. Mostafa S. Ibrahim, Arash Vahdat, Mani Ranjbar, William G. Macready.  IEEE Computer Vision and Pattern Recognition 2020](http://openaccess.thecvf.com/content_CVPR_2020/papers/Ibrahim_Semi-Supervised_Semantic_Image_Segmentation_With_Self-Correcting_Networks_CVPR_2020_paper.pdf)

## Contents
0. [Code](#code)
0. [Model](#model)
0. [Links](#links)
0. [Citation](#citation)

## Code
* I am still trying to get permission from the Company, Dwave
* Our code is based on this deeplabv3+ [repo](https://github.com/tensorflow/models/tree/master/research/deeplab). Our changes mainly: 
* Extention to their loss function with extra Cross Entropy calls for the self-correction modules
* A small cnn network for merging logits
* A small cnn to encode the bbounding box and inject in the decoder at some scale (Deeplab uses 2 scales)
* Several scripts to prepare the data to be saved/loaded from the ancilary model

## Model

<img src="https://github.com/mostafa-saad/segment-correction-net/blob/master/img/data.png" alt="Figure 1" height="400" >


<img src="https://github.com/mostafa-saad/segment-correction-net/blob/master/img/final.jpg" alt="Figure 1" height="400" >

## Links
* 15-min video presentation in [English](https://www.youtube.com/watch?v=lRA1KnkFibs) / [Arabic](https://www.youtube.com/watch?v=FlzUMWKkoHk)
* For detailed [Slides](https://docs.google.com/presentation/d/1kGIuZ8c07k8mUvd-pDpWxPVQmcNEXpBDNDZZl-VM5dU/edit?usp=sharing) / [Slides pdf](https://github.com/mostafa-saad/segment-correction-net/blob/master/img/slides.pdf)

## Citation
    @inproceedings{msibrahiCVPR20segmentcorrectionnet,
      author    = {Mostafa S. Ibrahim and Arash Vahdat and Mani Ranjbar and William G. Macready},
      title     = {Semi-Supervised Semantic Image Segmentation With Self-Correcting Networks.},
      booktitle = {2020 IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},
      year      = {2020}
    }

