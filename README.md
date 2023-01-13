# YOLOv4 Experimental Setup

Developed as a partial requirement for the course:
CPE020 - Methods of Research

One of the main metrics used by object detection algorithms such as YOLO (You Only Look Once) and Fast R-CNN are mean average precision (mAP). It measures the average precision across all classes and all images in the test dataset. 

**Results & Discussions:**

One of the main metrics used by object detection algorithms such as YOLO (You Only Look Once) and Fast R-CNN are mean average precision (mAP). It measures the average precision across all classes and all images in the test dataset. 


<table>
  <tr>
   <td> 
   </td>
   <td><strong>Batch Size</strong>
   </td>
   <td><strong>Subdivisions</strong>
   </td>
   <td><strong>Resolution</strong>
   </td>
   <td><strong>Max Batches</strong>
   </td>
   <td><strong>Random Flag</strong>
   </td>
   <td><strong>Learning Rate</strong>
   </td>
  </tr>
  <tr>
   <td><strong>Low</strong>
   </td>
   <td>64
   </td>
   <td>16
   </td>
   <td>416x416
   </td>
   <td>6000
   </td>
   <td>0
   </td>
   <td>0.001
   </td>
  </tr>
  <tr>
   <td><strong>Mid</strong>
   </td>
   <td>64
   </td>
   <td>16
   </td>
   <td>512x512
   </td>
   <td>6000
   </td>
   <td>0
   </td>
   <td>0.001
   </td>
  </tr>
  <tr>
   <td><strong>High</strong>
   </td>
   <td>64
   </td>
   <td>16
   </td>
   <td>608x608
   </td>
   <td>6000
   </td>
   <td>0
   </td>
   <td>0.001
   </td>
  </tr>
</table>


**Table 1**

**Average Precision of the Models over different IOU Thresholds**


<table>
  <tr>
   <td rowspan="2" ><strong>Models</strong>
   </td>
   <td rowspan="2" ><strong>IOU Threshold</strong>
   </td>
   <td colspan="6" ><strong>Average Precision</strong>
   </td>
   <td rowspan="2" ><strong>Mean Average Precision</strong>
   </td>
  </tr>
  <tr>
   <td>Motorcycle
   </td>
   <td>Tricycle
   </td>
   <td>Car
   </td>
   <td>Van
   </td>
   <td>Bus
   </td>
   <td>Truck
   </td>
  </tr>
  <tr>
   <td rowspan="5" ><strong>Low</strong>
   </td>
   <td>0.30
   </td>
   <td><p style="text-align: right">
97.63</p>

   </td>
   <td><p style="text-align: right">
98.85</p>

   </td>
   <td><p style="text-align: right">
97.85</p>

   </td>
   <td><p style="text-align: right">
99.02</p>

   </td>
   <td><p style="text-align: right">
99.4</p>

   </td>
   <td><p style="text-align: right">
99.28</p>

   </td>
   <td><p style="text-align: right">
98.67</p>

   </td>
  </tr>
  <tr>
   <td>0.40
   </td>
   <td><p style="text-align: right">
97.63</p>

   </td>
   <td><p style="text-align: right">
98.85</p>

   </td>
   <td><p style="text-align: right">
97.84</p>

   </td>
   <td><p style="text-align: right">
99.02</p>

   </td>
   <td><p style="text-align: right">
98.91</p>

   </td>
   <td><p style="text-align: right">
99.28</p>

   </td>
   <td><p style="text-align: right">
98.59</p>

   </td>
  </tr>
  <tr>
   <td>0.50
   </td>
   <td><p style="text-align: right">
97.63</p>

   </td>
   <td><p style="text-align: right">
98.33</p>

   </td>
   <td><p style="text-align: right">
97.67</p>

   </td>
   <td><p style="text-align: right">
99.02</p>

   </td>
   <td><p style="text-align: right">
98.91</p>

   </td>
   <td><p style="text-align: right">
99.28</p>

   </td>
   <td><p style="text-align: right">
98.47</p>

   </td>
  </tr>
  <tr>
   <td>0.60
   </td>
   <td><p style="text-align: right">
97.13</p>

   </td>
   <td><p style="text-align: right">
98.33</p>

   </td>
   <td><p style="text-align: right">
97.2</p>

   </td>
   <td><p style="text-align: right">
98.44</p>

   </td>
   <td><p style="text-align: right">
98.91</p>

   </td>
   <td><p style="text-align: right">
96.86</p>

   </td>
   <td><p style="text-align: right">
97.81</p>

   </td>
  </tr>
  <tr>
   <td>0.70
   </td>
   <td><p style="text-align: right">
92.61</p>

   </td>
   <td><p style="text-align: right">
97.9</p>

   </td>
   <td><p style="text-align: right">
96.29</p>

   </td>
   <td><p style="text-align: right">
97.81</p>

   </td>
   <td><p style="text-align: right">
98.37</p>

   </td>
   <td><p style="text-align: right">
96.07</p>

   </td>
   <td><p style="text-align: right">
96.51</p>

   </td>
  </tr>
  <tr>
   <td rowspan="5" ><strong>Mid</strong>
   </td>
   <td>0.30
   </td>
   <td><p style="text-align: right">
97.57</p>

   </td>
   <td><p style="text-align: right">
99.31</p>

   </td>
   <td><p style="text-align: right">
96.94</p>

   </td>
   <td><p style="text-align: right">
99.11</p>

   </td>
   <td><p style="text-align: right">
99.45</p>

   </td>
   <td><p style="text-align: right">
99.2</p>

   </td>
   <td><p style="text-align: right">
98.6</p>

   </td>
  </tr>
  <tr>
   <td>0.40
   </td>
   <td><p style="text-align: right">
97.57</p>

   </td>
   <td><p style="text-align: right">
99.26</p>

   </td>
   <td><p style="text-align: right">
96.94</p>

   </td>
   <td><p style="text-align: right">
99.11</p>

   </td>
   <td><p style="text-align: right">
99.31</p>

   </td>
   <td><p style="text-align: right">
99.2</p>

   </td>
   <td><p style="text-align: right">
98.56</p>

   </td>
  </tr>
  <tr>
   <td>0.50
   </td>
   <td><p style="text-align: right">
97.57</p>

   </td>
   <td><p style="text-align: right">
99.26</p>

   </td>
   <td><p style="text-align: right">
96.41</p>

   </td>
   <td><p style="text-align: right">
99.11</p>

   </td>
   <td><p style="text-align: right">
98.91</p>

   </td>
   <td><p style="text-align: right">
98.5</p>

   </td>
   <td><p style="text-align: right">
98.29</p>

   </td>
  </tr>
  <tr>
   <td>0.60
   </td>
   <td><p style="text-align: right">
96.39</p>

   </td>
   <td><p style="text-align: right">
99.26</p>

   </td>
   <td><p style="text-align: right">
95.84</p>

   </td>
   <td><p style="text-align: right">
98.09</p>

   </td>
   <td><p style="text-align: right">
98.91</p>

   </td>
   <td><p style="text-align: right">
97.67</p>

   </td>
   <td><p style="text-align: right">
97.69</p>

   </td>
  </tr>
  <tr>
   <td>0.70
   </td>
   <td><p style="text-align: right">
92.26</p>

   </td>
   <td><p style="text-align: right">
97.55</p>

   </td>
   <td><p style="text-align: right">
94.85</p>

   </td>
   <td><p style="text-align: right">
98.07</p>

   </td>
   <td><p style="text-align: right">
98.91</p>

   </td>
   <td><p style="text-align: right">
96.99</p>

   </td>
   <td><p style="text-align: right">
96.44</p>

   </td>
  </tr>
  <tr>
   <td rowspan="5" ><strong>High</strong>
   </td>
   <td>0.30
   </td>
   <td><p style="text-align: right">
97.94</p>

   </td>
   <td><p style="text-align: right">
98.98</p>

   </td>
   <td><p style="text-align: right">
96.36</p>

   </td>
   <td><p style="text-align: right">
99.62</p>

   </td>
   <td><p style="text-align: right">
99.43</p>

   </td>
   <td><p style="text-align: right">
99.28</p>

   </td>
   <td><p style="text-align: right">
98.6</p>

   </td>
  </tr>
  <tr>
   <td>0.40
   </td>
   <td><p style="text-align: right">
97.94</p>

   </td>
   <td><p style="text-align: right">
98.98</p>

   </td>
   <td><p style="text-align: right">
96.36</p>

   </td>
   <td><p style="text-align: right">
99.42</p>

   </td>
   <td><p style="text-align: right">
98.92</p>

   </td>
   <td><p style="text-align: right">
99.28</p>

   </td>
   <td><p style="text-align: right">
98.48</p>

   </td>
  </tr>
  <tr>
   <td>0.50
   </td>
   <td><p style="text-align: right">
97.83</p>

   </td>
   <td><p style="text-align: right">
98.98</p>

   </td>
   <td><p style="text-align: right">
96.35</p>

   </td>
   <td><p style="text-align: right">
99.42</p>

   </td>
   <td><p style="text-align: right">
98.92</p>

   </td>
   <td><p style="text-align: right">
99.28</p>

   </td>
   <td><p style="text-align: right">
98.46</p>

   </td>
  </tr>
  <tr>
   <td>0.60
   </td>
   <td><p style="text-align: right">
95.66</p>

   </td>
   <td><p style="text-align: right">
98.98</p>

   </td>
   <td><p style="text-align: right">
95.83</p>

   </td>
   <td><p style="text-align: right">
98.84</p>

   </td>
   <td><p style="text-align: right">
98.92</p>

   </td>
   <td><p style="text-align: right">
97.28</p>

   </td>
   <td><p style="text-align: right">
97.58</p>

   </td>
  </tr>
  <tr>
   <td>0.70
   </td>
   <td><p style="text-align: right">
91.84</p>

   </td>
   <td><p style="text-align: right">
98.56</p>

   </td>
   <td><p style="text-align: right">
94.32</p>

   </td>
   <td><p style="text-align: right">
96.66</p>

   </td>
   <td><p style="text-align: right">
98.92</p>

   </td>
   <td><p style="text-align: right">
97.28</p>

   </td>
   <td><p style="text-align: right">
96.26</p>

   </td>
  </tr>
</table>


All models are almost identical ranging around 96% to 98% between different IOU thresholds. Looking at the table there are some slight drop in performance as the IOU threshold. This phenomenon is expected as having a higher IOU threshold requires a tighter difference in the bounding boxes. The more tight the bounding box the higher the tendency to misclassify an object. The table also shows a 4% to 5% decrease in the average precision of the motorcycle class in the 0.70 IOU threshold in all the models. This occurs because the motorcycle class consists of relatively small objects, which may be more challenging to detect compared to the larger classes. The models had a harder time to classify it properly because of the more strict IOU threshold.

**Table 2**

**Average IOU of the Models in Different IOU Threshold**


<table>
  <tr>
   <td><strong>IOU Thresholds</strong>
   </td>
   <td><strong>0.30</strong>
   </td>
   <td><strong>0.40</strong>
   </td>
   <td><strong>0.50</strong>
   </td>
   <td><strong>0.60</strong>
   </td>
   <td><strong>0.70</strong>
   </td>
  </tr>
  <tr>
   <td><strong>Low</strong>
   </td>
   <td>85.47
   </td>
   <td>85.5
   </td>
   <td>85.39
   </td>
   <td>85.16
   </td>
   <td>84.39
   </td>
  </tr>
  <tr>
   <td><strong>Mid</strong>
   </td>
   <td>84.98
   </td>
   <td>84.95
   </td>
   <td>84.87
   </td>
   <td>84.6
   </td>
   <td>83.89
   </td>
  </tr>
  <tr>
   <td><strong>High</strong>
   </td>
   <td>85.67
   </td>
   <td>85.6
   </td>
   <td>85.56
   </td>
   <td>85.18
   </td>
   <td>84.58
   </td>
  </tr>
</table>


The average IoU of a model reflects the precision of the bounding boxes it generates. A higher average IoU indicates that the model can be used at higher IoU thresholds without compromising accuracy or precision. The data indicated by table 2 shows that the average IOU of the models are excellent at around an average of 85% but we can see a decline as the IOU threshold increases.

**Table 3**

**Total Detection Count of the Models**


<table>
  <tr>
   <td>
   </td>
   <td><strong>Total Detection Count</strong>
   </td>
  </tr>
  <tr>
   <td><strong>Low</strong>
   </td>
   <td>1769
   </td>
  </tr>
  <tr>
   <td><strong>Mid</strong>
   </td>
   <td>1821
   </td>
  </tr>
  <tr>
   <td><strong>High</strong>
   </td>
   <td>1797
   </td>
  </tr>
</table>


The total detection count of the models is the count of all objects including all classes that were successfully detected by the model. This count remains consistent regardless of the IoU threshold used. Looking back at table 2 and comparing it to table 3, it shows that there is a relationship between the average IOU and total detection count. Lower average IOU results in higher detection count. This suggests that using a lower IoU threshold may result in a greater number of object detections, although it may also increase the number of false positives.

**Table 4**

**Total Detection Time of the Models in different IOU Threshold in Seconds**


<table>
  <tr>
   <td><strong>IOU Thresholds</strong>
   </td>
   <td><strong>0.30</strong>
   </td>
   <td><strong>0.40</strong>
   </td>
   <td><strong>0.50</strong>
   </td>
   <td><strong>0.60</strong>
   </td>
   <td><strong>0.70</strong>
   </td>
   <td><strong>Average</strong>
   </td>
  </tr>
  <tr>
   <td><strong>Low</strong>
   </td>
   <td>26
   </td>
   <td>28
   </td>
   <td>26
   </td>
   <td>29
   </td>
   <td>27
   </td>
   <td>27.2
   </td>
  </tr>
  <tr>
   <td><strong>Mid</strong>
   </td>
   <td>41
   </td>
   <td>38
   </td>
   <td>38
   </td>
   <td>38
   </td>
   <td>39
   </td>
   <td>38.8
   </td>
  </tr>
  <tr>
   <td><strong>High</strong>
   </td>
   <td>48
   </td>
   <td>48
   </td>
   <td>49
   </td>
   <td>48
   </td>
   <td>49
   </td>
   <td>48.4
   </td>
  </tr>
</table>


Table 4 presents the total detection time of the models at various IoU thresholds. There is roughly some slight variation in seconds over the different IOU thresholds. The last column refers to the average over those thresholds, which can be used to estimate the time it would take for the model to process a single image. To derive the estimated detection speed per image, just simply divide it by the number of images used in the test dataset which is 900 images in this case.

 **Table 5**

**Detection Speed per Image of the Models in Seconds**


<table>
  <tr>
   <td>
   </td>
   <td><strong>Average Total Detection Time over Different IOU Thresholds</strong>
   </td>
   <td><strong>Detection Speed per Image</strong>
   </td>
  </tr>
  <tr>
   <td><strong>Low</strong>
   </td>
   <td>27.2
   </td>
   <td>0.03
   </td>
  </tr>
  <tr>
   <td><strong>Mid</strong>
   </td>
   <td>38.8
   </td>
   <td>0.04
   </td>
  </tr>
  <tr>
   <td><strong>High</strong>
   </td>
   <td>48.4
   </td>
   <td>0.05
   </td>
  </tr>
</table>


Upon examining the table above, it is clear that there is a slight uptrend. Specifically, for an increase in resolution there is an increase of 0.01 second in the detection speed per image. This suggests that as the complexity of the input images increases, the object detection algorithm takes longer to process them and produce the detections.
