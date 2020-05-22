# segment-correction-net
Paper ibrahim et al, cvpr 2020 - Mostafa S Ibrahim, Arash Vahdat, Mani Ranjbar, William G Macready

* [Slides - with Intro / Math derivations](https://docs.google.com/presentation/d/1kGIuZ8c07k8mUvd-pDpWxPVQmcNEXpBDNDZZl-VM5dU/edit?usp=sharing)

* Code: Still trying to get permission from the Company, Dwave
  * Our code is based on this deeplabv3+ [repo](https://github.com/tensorflow/models/tree/master/research/deeplab). Our changes mainly: 
  * Extention to their loss function with extra Cross Entropy calls for the self-correction modules
  * A small cnn network for merging logits
  * A small cnn to encode the bbounding box and inject in the decoder at some scale (Deeplab uses 2 scales)
  * Several scripts to prepare the data to be saved/loaded from the ancilary model
