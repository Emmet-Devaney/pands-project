## Iris Dataset Analysis
This repository is an analysis of the Iris Dataset by R. A. Fisher.

## Libraries

- pandas
- matplotlib
- seaborn

# 1.  About This Repository 
As I am still a beginning my coding journey, I had decided to display this project in a Jupyter notebook as that is an easier format for me.

**The files that this Repository contains:**

* **README.md**
    - A summary and conclusion of the statistical and visual analysis of the Iris Dataset

* **Iris.csv**
    - This file contains the dataset in question

* **Iris-Dataset-Analysis.ipynb**
    - A statistical and visual investigation using pandas, matplotlib, and seaborn.



# 2. The Dataset
The data set contains 3 classes of iris plant, with 50 samples per class. I found that one class is linearly separable from the other 2; the latter were not distinctly separable from each other.

**The Variables:**
-	sepal length in cm
-	sepal width in cm
-	petal length in cm
-	petal width in cm
-	species: -- Iris Setosa -- Iris Versicolour -- Iris Virginica.

This dataset had been used by Ronald Fisher in 1936, published as The Use of Multiple Measurements in Taxonomic Problems, to show how, using statistics, you may distinguish the differences between species of iris with just the petal and sepal measurements. This is now referred to as “Linear Discriminant Analysis” (What is LDA?).

# 3. The Analysis of Data

For this project, I will be using pandas to read the dataset and a combination of matplotlib and seaborn to perform a statistical investigation and illustrate patterns present.

![Iris Table Types](/pands/pands-project/Image%20Files/Iris%20Table%20Types.png)

# 4. Displaying the Statistics

The describe function in pandas shows the basic statistics e.g means, standard deviations, medians, etc.

![Iris Mean +](/pands/pands-project/Image%20Files/Iris%20Mean%20+.png)

# 5. Data Visualisation

Below I have included visualisations of the data to better understand the differences and correlations between the variables measured:

**Histograms:**

(Note to self, figure out how to add imhgaes to this file)

![Histograms](/pands/pands-project/Image%20Files/Histogram%20Tables.png)

**Scatterplots**

![Scatterplots](/pands/pands-project/Image%20Files/Scatterplot%20Tables.png)

From the images, we can note that the “Iris-Setosa” species is noticeably different, especially highlighted in the “Petal Measurement”. There does appear to be a difference between the other two species, but the difference is not as stark as the “Setosa”.

# 6. Correlations

Using the Pandas correlation function, we may be able to discern a distinction between the variables measured.

![Overall Width & Length](/pands/pands-project/Image%20Files/Overall%20Width%20+%20Length.png)

Here we can note:

* It appears that Petal Length and Width have a very strong correlation, as they both become larger together (r = 0.96~).
* The same cannot be said for the Sepal Length and Width which have a very weak correlation (r = -0.1~).
* It appears that there is a strong correlation for the Petal Width and Length in regard to the Sepal Length, which may indicate that they grow larger together (r= 0.81~ and r = 0.87~ respectively).
* I would say there is a weak correlation for Petal Width and Length in regards to Sepal Width (r = -0.35~ and 0.42~).

A good way to visualise this information is through a heatmap:

![Heatmap](/pands/pands-project/Image%20Files/Heatmap.png)

# 7. Conclusions

My conclusions based on the data are below:
*	There is a distinct difference in size between the Iris Setosa and the other Iris Species:
	If an iris’ data is presented without the species, and the dimensions of the sepals are short and wide with short and narrow petals, it is likely that the species is Setosa.
*	An observation can be drawn that the size of the petal dimensions carries more importance in identification than the sepal dimensions (at least for differentiating between the Versicolour and the Virginica):
	For the remaining two species, Versicolour and Virginica, the sepal dimensions are somewhat similar while the petal dimensions differ by length vs width accordingly.


# 8. References
Fisher,R. A.. (1988). Iris. UCI Machine Learning Repository. https://doi.org/10.24432/C56C76.

Kumar, R. (2018) * Seaborn Plot to Visualise Itis Dataset.* Kaggle Notebook. https://www.kaggle.com/rakesh6184/seaborn-plot-to-visualize-iris-data

Mendis, A. (2019) Data Visualization in Python: Matplotlib vs Seaborn. KDnuggets. https://www.kdnuggets.com/2019/04/data-visualization-python-matplotlib-seaborn.html

# 9. Further Links:

iris.csv file: https://github.com/aswintechguy/Machine-Learning-Projects/blob/efe051137e869c76f83c75a685f5f16310186c24/Iris%20dataset%20analysis%20-%20Classification/Iris.csv

pandas.DataFrame.to_string: https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.to_string.html

How to create a seaborn correlation heatmap in Python?: https://www.geeksforgeeks.org/how-to-create-a-seaborn-correlation-heatmap-in-python/

What is LDA?: https://www.ibm.com/topics/linear-discriminant-analysis#:~:text=Linear%20discriminant%20analysis%20(LDA)%20is,helps%20optimize%20machine%20learning%20models.
