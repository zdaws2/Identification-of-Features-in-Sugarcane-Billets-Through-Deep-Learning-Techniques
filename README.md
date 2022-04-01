# Identification-of-Features-in-Sugarcane-Billets-Through-Deep-Learning-Techniques

The following project aims to successfully collect an extensive array of data using photography with an RGB camera capturing multiple samples of sugarcane billets. Training data evaluation had to successfully derive from models through data annotations within bounding boxes and polygons. The main priority was to train a successful multi-feature classification model meeting a benchmark with an AP50 higher than 70% to produce a model that suitability identifies quality features within sugarcane billets with high confidence and accuracy. Once successful training occurred, the model's implementation within a practical system had to occur within a live sugar mills conveyor belt at Sunshine Sugars Condong Mill. Finally, to deliver statistical results through machine vision python scripts to identify Sound, Damaged, and Mutilated billets according to SRA quality guidelines. Therefore, allowing parties involved to make informed decisions based on meaningful data.

Update:

The project was successfully completed with several feature classifications, resulting in the successful creation of a multi-feature classification model for sugar cane billets. 

![image](https://user-images.githubusercontent.com/95267711/161190700-e1643667-52c2-4c7e-89c9-9ce2c6ece5a1.png)
Figure 1. Poly segmented billets, labelled with features; Broken, Pulpy, Rind-Missing, Small, Split, Sound and Squashed-Ends, respectively.

Table 1. Multi-feature classifications trained off Mask R-CNN using X101-FPN baseline, in instance segmentation for Sound, Split, Small, Broken and Rind-Missing. Training produced overall AP50 with IoU50 for each multi-feature model for bounding box and mask detections. Ticks denote active classes used in each model. 
![image](https://user-images.githubusercontent.com/95267711/161191397-ff2ebe32-a88e-4b31-ac3c-97f486310a61.png)



![image](https://user-images.githubusercontent.com/95267711/161191073-9f90e480-5009-4f0d-928b-d7d20da2f7cb.png)

Figure 2. Broken, Split and Small instance segmentation detections, with high confidence levels.

![image](https://user-images.githubusercontent.com/95267711/161191141-11c0af25-1b45-4ba0-89f5-2c7a2f396be7.png)
![image](https://user-images.githubusercontent.com/95267711/161191152-108a9e1a-3bee-4f0d-a03a-3ebbc2bd6149.png)

Figure 3. Sound, Split, Small and Broken instance segmentation detections, with high confidence levels.

![image](https://user-images.githubusercontent.com/95267711/161191193-f6e971d9-b058-4a16-999d-a497634a39b3.png)

Figure 4. There is a representation of overfitting occurring in the X101-FPN Sound, Split, Broken and Small feature classification model. At iteration 65,000, it is resulting in decreased performance, which shows an increase in losses for classes (top left), bounding box (top right), total loss (bottom right) and a decrease in Faster R-CNN accuracy (bottom left).

![image](https://user-images.githubusercontent.com/95267711/161191245-7a063e09-8ebe-402a-92ec-3ccebe9a161f.png)

Figure 5. Sound, Split, Small, Broken and Rind-Missing instance segmentation detections, with high confidence levels.
