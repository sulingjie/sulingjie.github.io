---
permalink: /
title: "Su Lingjie"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
<p style="text-align:justify; text-justify:inter-ideograph;">
My name is Su Lingjie(苏凌杰), a second-year master's student at the State Key Laboratory of Intelligent Manufacturing Equipment and Technology at Huazhong University of Science and Technology (HUST), under the supervision of <a href="https://mse.hust.edu.cn/info/1142/1340.htm">Prof. Wenlong Li</a>. I previously earned my bachlor's degree from the School of Mechanical Science and Engineering at HUST. My research focuses on point cloud registration, surface reconstruction, and mesh denoising. These research topics enhance the ability of robots to perceive and understand their surroundings, providing high-quality data for robotic inspection and measurement. <br><br>



<strong>Algorithm Theory</strong>: The mathematical theory in my research includs optimization theory, statistics (especially Gaussian Mixture Model and EM algorithm), matrix theory, iterative solution methods and preconditioning of linear functions, and bilateral filtering method. <br><br>

<strong>Algorithm Application</strong>: These designed algorithms can be used for robot pose estimation, localization of parts, evaluation of machining quality, and visualization.

</p>

You can find my CV [here](../assets/CV.pdf).

Publications
======

<p style="text-align:justify; text-justify:inter-ideograph;">
1. <strong>L. Su</strong>, W. Xu, and W. Li, “Robust point cloud registration in robotic inspection with locally consistent gaussian mixture model,” <i>IEEE Trans. Instrum. Meas.</i>, 2024, Under Review.  <br><br>

2. <strong>L. Su</strong> et al., “An adaptive anisotropic bilateral filtering method for mesh data in scale space,” <i>Meas. Sci. Technol.</i>, vol 35, no. 6, 2024, <a href="https://iopscience.iop.org/article/10.1088/1361-6501/ad317e">doi: 10.1088/1361-6501/ad317e</a>
   
</p>


Research Experience
======

1.Point Cloud Reconstruction and Multi-view Registration
--------
<p style="text-align:justify; text-justify:inter-ideograph;">
In the point cloud measurement process, the 3D sensor needs to be positioned at various locations due to the limited working range or the large size of the measured parts, such as a car body. This project focuses on how to integrete the point clouds from different perspetives through the following procedures. (1) Estabilishing binocular imaging model and calibrating the internal and external parameters of the stereo cameras. (2) Reconstructing the centers of marked points, including elliptic fitting, polar constraints and triangulation. Matching marked points under different perspectives with spatial invariant characteristics and registering point clouds coarsly. (3) Constructing the objective function of minimizing the mean square error of corresponding points in overlapping areas. Solving the optimization problem with gradient decent method and graph optimization method
</p>

<p align="center">
    <img src="../images/multi_reg.png" alt="measurement scene" style="width: 100%;">
</p>

2.Probability-based Point Cloud Registration
--------
<p style="text-align:justify; text-justify:inter-ideograph;">
In the area of robotic inspection, achieving accurate pairwise point cloud registration between scanned and model data is essential. However, noise and outliers generated in robotic scanned data can compromise registration accuracy. To mitigate this problem, this project proposes a probability-based registration method utilizing Gaussian Mixture Model (GMM) with local consistency constraint. This method converts the registration problem into a model-fitting one, constraining the similarity of posterior distributions between neighboring points to enhance correspondence robustness. I employ the Expectation Maximization algorithm iteratively to find the optimal rotation matrix and translation vector while obtaining GMM parameters. Both E-step and M-step have closed-form solutions. Extensive simulation and actual experiments confirm the method's robustness and accuracy. <br><br>
Now I am currently attempting to extend this method to multi-view registration to simultaneously estimate the accurate poses of multiple point clouds.
</p>

<p style="float: left; width: 55%;">
    <img src="../images/reg_GMM.png" alt="registration with GMM" style="width: 100%;">
</p>
<p style="float: left; width: 45%;">
    <img src="../images/reg_blade.gif" alt="blade registration gif" style="width: 100%;"> 
</p>

<br />

3.Anosotropic Bilateral Mesh Filtering
--------
<p style="text-align:justify; text-justify:inter-ideograph;">
Three-dimensional mesh data of parts, such as blades and engine bodies, have been widely used in industrial fields. Due to the different kinds of noise during mesh acquisition and machining deficiency of parts, the mesh quality is often insufficient for subsequent operations. Therefore, mesh denoising is a necessary and critical procedure to improve mesh quality. This project proposed an adaptive anisotropic bilateral filtering method for mesh data in scale space. Firstly, the mesh is decomposed into a smooth base with low frequency and a height vector field with high frequency based on scale space theory. The denoising of the vertex spatial field is transformed into the denoising of the height vector field, focusing on high-frequency information. Secondly, the bilateral filter scheme with the anisotropic Gaussian kernel is proposed to denoise the height vector field, removing noise mixed with features. The parameters in the bilateral filter scheme are chosen adaptively by maximizing the designed probability density function. This method can achieve mesh denoising as well as preserving geometry features.
</p>

<p align="center">
    <img src="../images/mesh_denoise.png" alt="mesh denoising" style="width: 70%;">
</p>

4.Implicit B-spline Surface Reconstruction
--------

<p style="text-align:justify; text-justify:inter-ideograph;">
For better visualization and analysis, surface function are required to be reconstructed from point cloud data. Implict B-spline (IBS) function is a widely-used and convenient format for representing surfaces. This project focuses on estimating the IBS surface with point cloud data. Firstly, I generate internal data and external data by moving the original data along the normals. These added data can gaurantee the orientation of the surface. Next, I represent the implict B-spline surface fitting as a least square problem. Finally, we incorporate a global tension constraint to control the smoothness and solve the least squares problem. Now, I am working on improving local accuracy in high-curvature areas.
</p>

<p align="center">
    <img src="../images/surface.png" alt="surface reconstruction" style="width: 70%;">
</p>

<br />

5.Software development for architectural point cloud
--------

<p style="text-align:justify; text-justify:inter-ideograph;">
We have developed two softwares for processing architectural point cloud based on QT framework and MicroStation platform. The following functions are included. (1) Data formate transformation: support for various formats, including ifc, obj, las, and pcd. (2) Preprocessing of architecture point cloud: including down-sampling, registration, and filtering. (3) construction progess estimation. (4) component extration, including I-beam, angle steel, and tubes, and parameter calcuclation.
</p>


Volunteering and Teaching
======

1.Volunteer for high-school student tours at HUST
--------

<p style="float: left; width: 50%;">
    <img src="../images/volunteer.png" alt="volunteer image" style="width: 95%;">
</p>
<p style="text-align:justify; text-justify:inter-ideograph;">
I once volunteered to guide high school students visiting Huazhong University of Science and Technology (HUST). My main responsibilities included leading them on campus tours, providing information about the university, and sharing details about our school's development and research achievements. <br>
</p>

<br />

2.Teaching assistent in experimental class for exchange students
--------

<p style="float: left; width: 50%;">
    <img src="../images/teaching_assistant.png" alt="volunteer image" style="width: 95%;">
</p>
<p style="text-align:justify; text-justify:inter-ideograph;">
I once served as a teaching assistant for a robotics measurement course during the summer exchange program (Global HUST) at Huazhong University of Science and Technology. My responsibilities included explaining the principles and operational procedures of robotic control, the imaging theory and usage of 3D scanners, and the algorithm of point cloud registration to eight exchange students from France, as well as guiding them in completing robotic measurement experiments.
</p>

