# Point-Cloud-Classification-ad-Segmentation
Point clouds, 3D data representations, are efficiently harnessed by PointNet models, bypassing size-inflating transformations. This example demonstrates PointNet's prowess in shape segmentation, simplifying tasks like object classification and part segmentation in computer vision.


## **Introduction**

Classification, detection and segmentation of unordered 3D point sets i.e. point clouds
is a core problem in computer vision. This example implements the seminal point cloud
deep learning paper [PointNet (Qi et al., 2017)](https://arxiv.org/abs/1612.00593). For a
detailed intoduction on PointNet see [this blog
post](https://medium.com/@luis_gonzales/an-in-depth-look-at-pointnet-111d7efdaa1a).

### **What are Point Clouds?**

A point cloud is a set of data points in space. The points may represent a 3D shape or object.

![](https://upload.wikimedia.org/wikipedia/commons/thumb/c/c0/Extract_Video_Beit_Ghazaleh_Orthophoto_Survey_AG%26P_2017.gif/440px-Extract_Video_Beit_Ghazaleh_Orthophoto_Survey_AG%26P_2017.gif)
