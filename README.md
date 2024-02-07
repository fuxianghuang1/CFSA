# Coarse-to-fine sparse self-attention for vehicle re-identification - Accepted at Knowledge-Based Systems, 2023
- The paper can be accessed at [KBS2023](https://www.sciencedirect.com/science/article/abs/pii/S0950705123002769)


If you find this code useful in your research then please cite


'''
@article{huang2023coarse,

  title={Coarse-to-fine sparse self-attention for vehicle re-identification},
  
  author={Huang, Fuxiang and Lv, Xuefeng and Zhang, Lei},
  
  journal={Knowledge-Based Systems},
  
  volume={270},
  
  pages={110526},
  
  year={2023},
  
  publisher={Elsevier}
}
'''


## Abstract

Existing vehicle re-identification (Re-ID) methods usually combine global features and local features to meet the challenge of inter-class similarity and intra-class variance, but almost all existing methods rely on extra auxiliary networks to locate the vehicle parts for feature mining, which are inefficient, cost-ineffective and time-consuming. Self-attention mechanism, averaging model’s attention weights on the similar vehicle parts, can guide the model to identify more discriminative vehicle parts for identification, thus extracting expensive local features becomes unnecessary. However, the computational cost of the original self-attention mechanism is unacceptable and the attention map is less discriminative when processing high-resolution feature maps (i.e. 384*384 or larger), which limits the performance gains of the challenging vehicle Re-ID. In this paper, we propose a lightweight coarse-to-fine sparse self-attention mechanism for vehicle Re-ID. Our method decomposes the self-attention process to a coarse stage and a fine stage. In coarse stage, the pixel-level feature map is transformed to patch-level feature map and the dependencies between similar vehicle parts are captured in a global context. In fine stage, the details of vehicle parts are captured in a local context. In addition, multi-head structure is introduced to capture diverse but robust attention information. Experiments on VeRi and VERI-Wild show that our method not only outperforms recent vehicle Re-ID methods relying on expensive auxiliary networks, but also outperforms the original self-attention mechanism in accuracy with much lower computation and memory cost.




