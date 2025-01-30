# 🏗️ Data Analysis & Visualization Project  

## 📜 Overview  
This project covers **perception experiment analysis, astronomical object visualization, Montana population trends, and air quality data exploration** using **R and Tableau**. It applies **distribution analysis, scatter plots, time series visualization, and logarithmic scaling** to uncover insights.  

## 🎯 Problem Explanation  

### **1. Perception Experiment Analysis**
📌 Dataset: **PerceptionExperiment.csv**  
- **Error Analysis (Over/Underestimation):**  
  - Compute `Error = Response - TrueValue`.  
  - **Boxplot or histogram** to analyze error trends.  
- **Absolute Error Distribution:**  
  - **Univariate scatterplot** to compare errors across different visualization methods.  
- **Display Order Effects (Subjects 56-73):**  
  - **Comparison of Displays 1 & 2** to determine learning effects.  
- **Erroneous Stimulus Identification:**  
  - **Outlier detection visualization** for anomalous responses.  

📊 **Tools Used:** R, Tableau  

### **2. Messier Astronomical Object Visualization**
📌 Dataset: **Messier Objects Data**  
- **Messier Number vs. Object Properties:**  
  - Explore patterns in **brightness, distance, or type**.  
- **Distance Distribution by Kind:**  
  - **Boxplot or density plot** sorted logically.  
- **Distance vs. Apparent Magnitude:**  
  - **Scatter plot with inverse brightness scale**.  
- **Augmented Scatter Plot:**  
  - Adjust **point size** based on **angular size** of objects.  

📊 **Tools Used:** R, Tableau  

### **3. Montana Population Growth**
📌 Dataset: **Montana Population Data**  
- **Logarithmic Scale Visualization:**  
  - **Population doubling trends since 1890**.  
  - **Percentage rate of change over time**.  
  - **Years with >15% population growth**.  
- **Graph choices:**  
  - **Logarithmic line plot** for population growth.  
  - **Log-ratio transformation** for percentage changes.  

📊 **Tools Used:** R, Tableau  

### **4. New York Air Quality Analysis**
📌 Dataset: **Built-in R dataset (May–Sept)**  
- **Wind vs. Solar Radiation Scatterplot:**  
  - **Trendline for relationship analysis**.  
- **Distributions of Wind & Solar Radiation:**  
  - **Violin plot, boxplot, or faceted histograms**.  
- **Multiple Variable Comparison:**  
  - **Data pivoting for streamlined visualization**.  
- **(Extra Credit) QQ Plot:**  
  - **Wind vs. Solar Radiation distribution comparison**.  

📊 **Tools Used:** R, Tableau  

## 🚀 Technologies Used  
- **R (ggplot2, dplyr, tidyr)** – Data transformation & visualization.  
- **Tableau** – Interactive charts & geospatial analysis.  

## 📊 Example Output  

### **1. Perception Experiment Analysis**
📉 **Stacked Bar Graph of Response Errors**
- To graph the story whether subjects have provided Overestimated or Underestimated responses, grouped Error values would be the choice here - using count. Furthermore, using stacked bar chart to emphasize the sub-categories proportional distribution across tests. The sub-categories are 'Accurately observed', 'Overestimated', and 'Underestimated'. Formulas for both Error and
 Status are shown above, very simple logic.
- From the graph, Volume and Slope tests have least Underestimated responses - 51 and 96 counts, respectively. Correspondingly, both also have highest Overestimated counts.
- On the other hand, Color Value and Length - Non-Aligned tests have highest Underestimated responses. Correspondingly, both have lowest Underestimated counts - 72 and 133 counts, respectively.
- Finally, Vertical Distance - Aligned test has the highest Accuractly observed responses with 234 counts - 42.4% within the test sample. This aligns with Muzner's material where position on common-scale is the most effective encoding method
![Perception Error](https://github.com/pngo1997/Images/blob/main/VS%203%20-%20Stacked%20bar%20graph%20perception.png)  

---

### **2. Messier Object Distances**
🌌 **Distance Distribution by Kind**  
- From the graph, there is somewhat a light positive linear relationship between Messier Object Number and Apparent Magnitude, the higher the order of Messier Object Number corresponding to higher the values of Apparent Magnitude.
- To visualize the story of the higher the number the fainter the object is in the sky, sequential color palette for Apparent Magnitude will deliver that message. The higher up in Apparent Magnitude and further distance, the object- circle will have lighter color indicates less clearly visible.
- Using log base 10 due to nature of the data- with magnitude.
![Messier Distances](https://github.com/pngo1997/Images/blob/main/VS%203%20-%20Scatterplot%20messier%20object.png)  

---

### **3. Montana Population Growth**
📈 **Log-Scale Population Growth Since 1890**  
- Montana population grew from log2 (17) to log2 (19), which means that the population has doubled twice since 1890.
![Montana Log Growth](https://github.com/pngo1997/Images/blob/main/VS%203%20-%20Population%20Growth.png)  

---

### **4. New York Air Quality**
🌞 **Wind vs. Solar Radiation Scatterplot**  
- Since the objective is to visualize and compare the distributions of two variable Wind and Solar R., Q-Q plot would be the best choice here. Typically for Q-Q plot, we are looking for a 45 degree straight slope depicts normal distribution. From the graph, Q-Q plot has a more wavy pattern and the points deviate from the straight line indicate that the two attributes do not have normal distribution.
![Wind vs Solar](https://github.com/pngo1997/Images/blob/main/VS%203%20-%20Wind%20vs%20Solar.png)  
