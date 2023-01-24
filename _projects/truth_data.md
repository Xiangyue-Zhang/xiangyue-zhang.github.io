---
layout: page
title: Truth Data Acquisition Method
description: Research on an AI-based Low-cost Truth Data Acquisition Method in Crowd Intelligence Sensing Network
img: assets/img/truth_data/truth_data.png
importance: 2
category: college
link: true
new_page: true
---
<b>1. Brief introduction of the project</b>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/truth_data/truth_data.png" title="Industrial sensing and prediction via sparse MCS." class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <b>Industrial sensing and prediction via sparse MCS.</b>
</div>
&emsp; &emsp; <b>1.1</b> With the rapid development of Web2.0, Industry4.0 and corresponding technologies, social media has become a powerful tool for industrial manufacturing by promoting the effectiveness of communication, collaboration, decision-making and other aspects. As a new data sensing paradigm, mobile crowd sensing (MCS) [1] - [3] can recruit a large number of users with mobile devices to collect social data in the target sensing area. Therefore, by using MCS, we can obtain sufficient social data and further analyze it to understand and use the obtained insights to help producers, suppliers and customers to carry out industrial manufacturing. 
<br>&emsp; &emsp; For example, considering a large factory, we can use MCS to collect the fine-grained environmental information of the whole factory, and then upload and share the sensing data to social media, so as to further analyze these data for the safety monitoring of industrial manufacturing. 
<br>&emsp; &emsp;  Traditional MCS recruits a large number of users in all target sensing fields to provide high-quality sensing services. However, we cannot ignore the fact that recruiting more users means greater costs. Even though all users are recruited, we still cannot guarantee full coverage due to the uncertainty of mobility. Therefore, especially in large-scale and fine-grained industrial manufacturing systems, the data perceived by MCS is incomplete, random (even sparse), which leads to poor performance of cognitive analysis from data. [4] The important problem is that we can't know the accuracy of the data provided by users. 
<br>
&emsp; &emsp; <b>1.2</b> We plan to propose a low-cost AI based method for obtaining authentic data, and establish a group-aware intelligent trust cooperation network system. First of all, we use the cooperation of 3D laser and UAV to collect the data of the Internet of Things as the reference truth value of the weather. Secondly, we divided the Changsha area into regions and randomly selected the truth value from the regions. 
<br>
&emsp;&emsp;  According to the comparison between the user uploaded data and our reference truth value, we proposed an active and verifiable trust evaluation method to evaluate the credibility of the recruited users. Thirdly, we use AI neural network to build the model of the time series data before the region, and predict and fill the sparse MCS from the perspective of time and space. 
<br>&emsp; &emsp; Finally, we use the model trained by AI neural network to predict each region, and compare the predicted results with the data collected by users as true values, while reducing the use of 3D laser and UAV. Regularly compare the models predicted by 3D laser and UAV with AI neural network, and correct the models within a certain time. This can greatly reduce the cost in industry and achieve a low-cost AI-based access to real image data in swarm intelligence sensing networks.
<br>
<b>2. Research purpose</b>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/truth_data/truth_data2.png" title="Flowchart of industrial sensing and prediction system." class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <b>Flowchart of industrial sensing and prediction system.</b>
</div>
<br>&emsp;&emsp;This project aims to study an AI-based low-cost truth data acquisition method in the crowd-sensing network. By establishing a rigorous credibility evaluation model for recruited users, using AI deep learning neural network to process time-series data, from space Predict the data in the time and time dimensions, so as to complete the filling of the MCS, thereby significantly reducing the analysis time of each user's credibility, achieving the situation that all regions are covered by users with high credibility, and significantly reducing the cost of industrial data collection. Specific goals include:
<br>
&emsp;&emsp;(1) Establish an AI-based sparse MCS filling model.
<br>
&emsp;&emsp;(2) Establish an algorithm model for evaluating the credibility of user-collected data.
<br>
&emsp;&emsp;(3) Establish an AI-based group perception intelligent trust collaboration network system.
<br>
<b>3. Research content</b>
<br>
<b>3.1 Establish an AI-based sparse MCS filling model.</b>
<br>
&emsp;&emsp;Mobile canopy sensing (MCS) is a powerful perception paradigm that provides sufficient social data for cognitive analysis in industrial sensing and industrial manufacturing. Considering the perception cost, sparse MCS, as a variant, only perceives the data of a few sub-regions, and then infers the data of the unperceived sub-regions according to the spatio-temporal relationship of the sensed data. Existing works usually assume that the sensory data is linearly spatio-temporally correlated, which does not work well in real-world nonlinear systems, resulting in lower accuracy for data inference. Moreover, in many cases, users not only need to infer current data, but are also interested in predicting the near future, which can provide more information for users' decision-making. In response to these problems, we plan to propose an AI deep learning deep learning industrial sensing prediction scheme based on sparse MCS, which consists of two parts: matrix completion and future prediction. Our goal is to achieve high-precision predictions of future moments under the assumption that historical data is sparse. In order to make full use of sparse data for prediction, a deep matrix factorization method is first proposed, which can preserve nonlinear spatio-temporal relationships and perform high-precision matrix completion.
<br>
<b>3.2 Establish an algorithm model for evaluating the credibility of user-collected data.</b>
&emsp;&emsp;For example, random collection of 3D laser and UAV data in selected areas after user data collection can provide baseline data for trust assessment. We passed the 3D laser and drone through some covered nodes and got accurate data. Establish a trust evaluation mechanism, and the data center evaluates the user's trust score by calculating the matching degree between the baseline data and the data provided by the user. Trust Evaluation provides three ways to update the trust score: Increment Score (IS), Decrease Score (DS) and Timeout Penalty (TP). For example, the data collected by user 1 matches the baseline data provided by 3D laser and UAV, so in this round of evaluation, user 1 is considered as a trustworthy user, IS improves the trust of user 1 Score. On the contrary, user No. 2's data differs too much from the baseline data, so its trust score is lowered through DS. In addition, TP evaluates the user's activity according to the interval between adjacent collection times. The larger the interval, the less activity and the lower the trust score. After multiple rounds of updates, trusted and untrusted users can be distinguished. In this way, users with low trust or inactivity can be filtered out, and users with high trust can be covered in all regions, significantly reducing the cost of industrial data collection. [4]
<br>
<b>3.3 Establish an AI-based group perception intelligent trust collaboration network system.</b>
<br>
The industrial sensing and forecasting problem is formally described in sparse MCS, and the goal is to recover the current sensing map and predict the near future from the sparse sensing data. [5] Compared with traditional methods, we plan to use multi-layer neural network so that the non-linearity of the matrix can be better exploited. To further capture and exploit spatiotemporal correlations for prediction, we plan to propose a component that learns nonlinear temporal relationships and a component that learns spatial correlations. Then we will evaluate the proposed method on some real datasets and some concrete industrial sensing tasks. According to this method, it can be judged whether it is effective in terms of recovery and prediction accuracy of sparse data. We use the model trained by the AI ​​neural network to predict each area, and compare the prediction results with the data collected by users as the baseline data, while reducing the use of industrial sensor data. Regularly compare the true industrial sensor data with the model predicted by the AI neural network, and correct the model within a certain period of time. And based on this, the credibility of the user can be quickly judged in a short period of time.
<br>
<b>Reference</b>
<br>
[1] J. Xiong, R. Ma, L. Chen, Y. Tian, Q. Li, X. Liu, and Z. Yao, “A
personalized privacy protection framework for mobile crowdsensing in
IIoT,” IEEE Trans. Ind. Informat., vol. 16, no. 6, pp. 4231–4241, Jun. 2020.
<br>
[2] L. Wang, Z. Yu, D. Yang, H. Ma, and H. Sheng, “Efficiently targeted
billboard advertising using crowdsensing vehicle trajectory data,” IEEE
Trans. Ind. Informat., vol. 16, no. 2, pp. 1058–1066, Feb. 2020.
<br>
[3] M. Xiao, J.Wu, L. Huang, R. Cheng, and Y.Wang, “Online task assignment
for crowdsensing in predictable mobile social networks,” IEEE Trans.
Mobile Comput., vol. 16, no. 8, pp. 2306–2320, Aug. 2017.
<br>
[4]Guo J ,  Liu A ,  Ota K , et al. ITCN: An Intelligent Trust Collaboration Network System in IoT[J]. IEEE Transactions on Network Science and Engineering, 2021, PP(99):1-1.
<br>
[5]Wang E ,  Zhang M ,  Cheng X , et al. Deep Learning-Enabled Sparse Industrial CrowdSensing and Prediction[J]. IEEE Transactions on Industrial Informatics, 2020, PP(99):1-1.

