# Touching-Cell-Dataset


This is a dataset of touching cell images used for "A robust concave point detector based on k-variance of k-sum of chain code", which can be used to evaluate concave points detection methods. 

The image dataset consists of 24 different original 300×300 binary images, which were collected from the CellaVision blog (http://blog.cellavision.com/) and segmented by our earlier work. Each image contains a single touching-cell clump. 


![An example image](https://raw.githubusercontent.com/zxaoyou/Touching-Cell-Dataset/master/example.jpg) 


All the concave points of each image were manually labeled by domain experts and stored in a .mat file. You can read the .mat files using MATLAB load statement as follows:

C = load('001.mat','Corner');

C is a m*2 matrix, where m is the total number of all the concave points in "001.bmp". Each row vector of C is the position (x,y) of each concave point. 



If you use the dataset in your paper, please acknowledge `the CellaVision blog <http://blog.cellavision.com/>`_ (http://blog.cellavision.com/) and cite the paper::

    @article{Zheng2018,
      title={Fast and Robust Segmentation of White Blood Cell Images by Self-supervised Learning},
      author={Xin Zheng and Yong Wang and Guoyou Wang and Jianguo Liu},
      journal={Micron},
      volume={107},
      pages={55--71},
      year={2018},
      publisher={Elsevier}
      doi={https://doi.org/10.1016/j.micron.2018.01.010},
      url={https://www.sciencedirect.com/science/article/pii/S0968432817303037}
    }
