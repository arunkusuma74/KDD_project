# Project Title :
NASA | Nearest Earth Objects

# Team Members List :

1.Arun Kusuma

2.Anusha Bethini

3.Pavan Kumar Kovi

# Project Introduction:
The dataset at hand focuses on Nearest Earth Objects (NEOs), which are celestial bodies that closely approach Earth. NASA has compiled observations of these objects from 1910 to 2024, resulting in a comprehensive dataset of 338,199 records. Some of these NEOs pose significant threats to Earth and are classified by NASA as "is_hazardous." This project aims to predict whether an NEO is hazardous or not using various attributes of the dataset.

The purpose of this project is to identify which characteristics are the most accurate predictors of a NEO's potential hazard. This predictive modelling challenge will use supervised learning approaches, specifically classification models, to classify NEOs as hazardous or non-hazardous. The project will involve selecting and optimising machine learning models to attain the highest potential categorisation accuracy.

# Research Question:

Which physical and orbital characteristics of Near-Earth Objects (NEOs) are the most significant predictors of their potential hazard, and how can machine learning models be optimized to accurately classify NEOs as hazardous or non-hazardous?

# Relevant Domain Information :
Nearest Earth Objects (NEOs) are asteroids and comets with orbits that bring them close to Earth's orbit .
Understanding NEOs is crucial for assessing potential collision threats and planning space missions .
This field combines astronomy, planetary science, and data analytics to study the dynamics of these celestial bodies.

[_NASA - Near Earth Object Program_](https://www.nasa.gov/mission_pages/asteroids/main/index.html) - This NASA webpage provides information about NEOs, including their monitoring, detection, and the risks they pose to Earth.

[_NASA Center for Near-Earth Object Studies_](https://cneos.jpl.nasa.gov/) - The Center for Near Earth Objects Studies(CNEOS) maintains a continuous watch for asteroids and comets that could approach Earth, providing data and predictions about NEOs.

# Data Source and Description:
[_Kaggle NASA | Nearest Earth Objects_](https://www.kaggle.com/datasets/ivansher/nasa-nearest-earth-objects-1910-2024)

The dataset originates from NASA's observations of Nearest Earth Objects spanning from 1910 to 2024. It includes the following attributes:

1. neo_id: Unique Identifier for each Asteroid
2. name: Name given by NASA
3. absolute_magnitude: Describes intrinsic luminosity
4. estimated_diameter_min: Minimum Estimated Diameter in Kilometres
5. estimated_diameter_max: Maximum Estimated Diameter in Kilometres
6. orbiting_body: Planet that the asteroid orbits
7. relative_velocity: Velocity Relative to Earth in Kmph
8. miss_distance: Distance in Kilometres missed
9. is_hazardous: Boolean feature that indicates whether the asteroid is harmful or not
  The goal is to use these features to predict the "is_hazardous" attribute

# Data Understanding and EDA:

### 1. Distribution of Absolute Maginitude
Interpretation: This graph illustrates how absolute magnitudes are spread out among NEOs. This shows that there are more non-dangerous NEOs present and they have a wider range of brightness. Dangerous Near-Earth Objects, while not as frequent, tend to occur at greater intensities. The overlap in brightness between hazardous and non-hazardous objects is pronounced, showing that absolute magnitude is not enough to predict an object's hazard status. This visualization highlights the importance of additional features or advanced models to accurately distinguish celestial objects as either dangerous or harmless.

### 2. Correlation Heatmap
Interpretation: The correlation heatmap shows the connection among different attributes of the dataset. High associations between data like relative_velocity and miss_distance could suggest possible connections that could aid in predicting an object's level of threat. For instance, a significant correlation between relative_velocity and is_hazardous might suggest that quicker NEOs are more prone to posing a threat. This visualization underscores the significance of comprehending how features interact, aiding in selecting features for better hazard prediction.

### 3. Scatter Plot of Diameter vs Miss Distance
Interpretation: This scatter plot shows how close NEOs come to Earth in relation to their estimated maximum diameter size. There seems to be no obvious, straightforward connection between the size of a NEO and its proximity to Earth. Dangerous NEOs are scattered throughout the area, coming in different sizes and distances. This indicates that, although size may play a role, it is not the sole indicator of danger. Understanding the interaction of these properties will enhance your comprehension of why a NEO is considered dangerous.

### 4. Boxplot of Relative Velocity by Hazardous Status
Interpretation: The boxplot shows how relative velocity is distributed among hazardous and non-hazardous NEOs. Dangerous NEOs generally display a wider variety of speeds and a higher average velocity compared to non-dangerous NEOs. This demonstrates that the velocity relative to other objects could be an important consideration in determining the level of danger associated with an object. Outliers within dangerous NEOs could indicate extreme instances of high speeds, which may have a significant impact on hazard evaluation.

### 5. Countplot of Orbiting Bodies
Interpretation: The boxplot shows how relative velocity is distributed among hazardous and non-hazardous NEOs. Dangerous NEOs typically exhibit a wider range of speeds and a higher median speed compared to non-dangerous ones. This indicates that the speed of the object compared to another may play an important role in determining its level of threat. Outliers in dangerous NEOs could indicate extreme instances with exceptionally high speeds that may be crucial for evaluating hazards.

### 6. Distribution of Estimated Diameter (Min) by Hazardous Status
Interpretation: The data visualization shows the anticipated sizes of astronomical objects classified as either non-hazardous or hazardous. The data is greatly skewed towards smaller objects, with most of them having diameters around 0 km and frequencies exceeding 1.9 million for the smallest size category. Typically, harmless items appear to be more common, particularly in smaller size categories. Although the x-axis stretches for 35 km, objects that exceed 5 km in size are uncommon and only noticeable at very low frequencies.

### 7. Distribution of Estimated Diameter (Max) by Hazardous Status
Interpretation: This graph displays the estimated maximum diameters distribution of celestial objects classified as either dangerous or non-hazardous. The information skews towards smaller objects, with the tiniest category, mostly made up of non-dangerous items, having the highest frequency at nearly two million. Although the x-axis goes up to 80 km, objects over 20 km are very rare and can only be detected at extremely low frequencies. In general, non-dangerous items are much more common, while dangerous items are slightly more common in larger size categories compared to the previous "min diameter" data.

Further details will be appended to Deliverable 2 and Deliverable 3.
