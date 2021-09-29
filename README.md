># UAV Path Planning in 3D Unstructured Environment
> ## Author: Yogeshkarna Govindaraj
### Introduction 
This repository contains implementation of UAV 3D Path planning algorithms. The global path planning algorithm based on Simulated Annealing (SA) and local path planning algorithms I-PRM and A*. For Lazy-Theta* the recent implementation by [1] is used by modifying the dataset. 

The original pointcloud files of datasets are too large for github repository, The `.pcd` files can be downloaded into `dataset` folder from below link.
>### Link to Pointcloud Datasets
>https://hochschulebonnrheinsieg-my.sharepoint.com/:f:/g/personal/yogeshkarna_govindaraj_365h-brs_de/EuGETRMeFsNHuxAuSCPIrnUBsj4sKXes7GBqepAkbaC8Uw?e=f24C6K

### Installation
The project is developed in `anaconda` environment. The `requirements.yml` file contans all the dependencies required to run all path planning programs contained in `src` folder. 
```python
conda env update -n my_env --file requirements.yml
```
The above command creates a new anaconda environment named `my_env` consisting of all the dependencies required to run the path planners.

### Repository structure
`dataset` folder contains `octomap` files of all three datasets used for testing the local path planning algorithms. The `src` folder contains three `.ipynb` files where `SA` implements the global path planning solution, `A-star` and `I-PRM` files implements the respective local path planning algorithm. 

All these programs are standalone containing program explanation within. For Lazy-Theta* an method proposed by [1]  is used, which can be found in the link below.
>#### Link to Lazy-Theta* Implementation
>https://sites.google.com/view/lazythetastaronline/autonomous-exploration?authuser=0

References 
1. Faria, M., Ferreira, A. S., Pérez-Leon, H., Maza, I., & Viguria, A. (2019). Autonomous 3D Exploration of Large Structures Using an UAV Equipped with a 2D LIDAR. Sensors, 19(22), 4849. [DOI 10.3390/s19224849](https://www.google.com/url?q=https%3A%2F%2Fdoi.org%2F10.3390%2Fs19224849&sa=D&sntz=1&usg=AFQjCNF3oU0jNOzBtJkwHxJRxMP0D6iZZA)

