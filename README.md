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

![Orthophoto Survey GIF](https://upload.wikimedia.org/wikipedia/commons/thumb/c/c0/Extract_Video_Beit_Ghazaleh_Orthophoto_Survey_AG%26P_2017.gif/440px-Extract_Video_Beit_Ghazaleh_Orthophoto_Survey_AG%26P_2017.gif)

## Structuring the dataset

We generate the following in-memory data structures from the Airplane point clouds and
their labels:

- `point_clouds` is a list of `np.array` objects that represent the point cloud data in
the form of x, y and z coordinates. Axis 0 represents the number of points in the
point cloud, while axis 1 represents the coordinates. `all_labels` is the list
that represents the label of each coordinate as a string (needed mainly for
visualization purposes).
- `test_point_clouds` is in the same format as `point_clouds`, but doesn't have
corresponding the labels of the point clouds.
- `all_labels` is a list of `np.array` objects that represent the point cloud labels
for each coordinate, corresponding to the `point_clouds` list.
- `point_cloud_labels` is a list of `np.array` objects that represent the point cloud
labels for each coordinate in one-hot encoded form, corresponding to the `point_clouds`
list.


### Setup 

!pip install trimesh

## Point cloud classification
Introduction
Classification, detection and segmentation of unordered 3D point sets i.e. point clouds is a core problem in computer vision. This example implements the seminal point cloud deep learning paper PointNet (Qi et al., 2017). For a detailed intoduction on PointNet see this blog post.

What are Point Clouds?
A point cloud is a set of data points in space. The points may represent a 3D shape or object.

## Point Cloud Segmentation 
Introduction
A "point cloud" is an important type of data structure for storing geometric shape data. Due to its irregular format, it's often transformed into regular 3D voxel grids or collections of images before being used in deep learning applications, a step which makes the data unnecessarily large. The PointNet family of models solves this problem by directly consuming point clouds, respecting the permutation-invariance property of the point data. The PointNet family of models provides a simple, unified architecture for applications ranging from object classification, part segmentation, to scene semantic parsing.

In this example, we demonstrate the implementation of the PointNet architecture for shape segmentation.

References
PointNet: Deep Learning on Point Sets for 3D Classification and Segmentation
Point cloud classification with PointNet
Spatial Transformer Networks
