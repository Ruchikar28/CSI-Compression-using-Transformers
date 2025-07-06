### CSI-Compression-using-Transformers**

The objective of this project is to efficiently compress *Channel State Information (CSI)* in massive MIMO systems for next-generation 5G/6G wireless networks. Since CSI is a high-dimensional matrix, transmitting it directly from user devices to base stations results in substantial feedback overhead. To overcome this challenge, I proposed a compression framework utilizing Axial Transformers and advanced attention mechanisms, aiming to reduce the feedback data while preserving key information for accurate channel estimation. 

I studied the *Swin CF architecture* to understand the correct implementation of various blocks like MLP, Patch Merging and Patch division and techniques that enhance the efficiency and accuracy of the compression process and implemented them for axial transformers. Axial transformers focus on calculating attention along spatial and frequency axes in a highly efficient manner.  Also, I added a Window-based Axial Attention block, which localizes the attention computation within windows, reducing computational complexity while maintaining performance. 

The model was trained on various compression ratios of 1/4, 1/16 and 1/64. The code for training on 1/4 compression ratio is given here. The performance was evaluated using key metrics such as NMSE (Normalized Mean Squared Error), FLOPs (Floating Point Operations) and parameter count. 

The best performance was achieved for  1/4 compression ratio, where the model reached an NMSE of -15.4dB with 4.87M parameters and 20.18M FLOPs.  This project gives a deep understanding of how deep learning techniques can be applied to solve critical problems in 6G wireless communication systems.
