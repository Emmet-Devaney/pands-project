## Iris Dataset Analysis
This repository is an analysis of the Iris Dataset by R. A. Fisher.

## Libraries

- pandas
- matplotlib
- seaborn

1. # About This Repository 
As I am still a beginning my coding journey, I had decided to display this project in a Jupyter notebook as that is an easier format for me.

**The files that this Repository contains:**

* **README.md**
    - A summary and conclusion of the statistical and visual analysis of the Iris Dataset

* **Iris.csv**
    - This file contains the dataset in question

* **Iris-Dataset-Analysis.ipynb**
    - A statistical and visual investigation using pandas, matplotlib, and seaborn.



2. # The Dataset
The data set contains 3 classes of iris plant, with 50 samples per class. I found that one class is linearly separable from the other 2; the latter were not distinctly separable from each other.

**The Variables:**
-	sepal length in cm
-	sepal width in cm
-	petal length in cm
-	petal width in cm
-	species: -- Iris Setosa -- Iris Versicolour -- Iris Virginica.

This dataset had been used by Ronald Fisher in 1936, published as The Use of Multiple Measurements in Taxonomic Problems, to show how, using statistics, you may distinguish the differences between species of iris with just the petal and sepal measurements. This is now referred to as “Linear Discriminant Analysis”.

3. # The Analysis of Data

For this project, I will be using pandas to read the dataset and a combination of matplotlib and seaborn to perform a statistical investigation and illustrate patterns present.

<class 'pandas.core.frame.DataFrame'>
RangeIndex: 150 entries, 0 to 149
Data columns (total 5 columns):
 #   Column         Non-Null Count  Dtype  
---  ------         --------------  -----  
 0   SepalLengthCm  150 non-null    float64
 1   SepalWidthCm   150 non-null    float64
 2   PetalLengthCm  150 non-null    float64
 3   PetalWidthCm   150 non-null    float64
 4   Species        150 non-null    object 
dtypes: float64(4), object(1)

Species
Iris-setosa        50
Iris-versicolor    50
Iris-virginica     50
Name: count, dtype: int64

4. # Displaying the Statistics

The describe function in pandas shows the basic statistics e.g means, standard deviations, medians, etc.

	SepalLengthCm	SepalWidthCm	PetalLengthCm	PetalWidthCm
count	150.000000	150.000000	150.000000	150.000000
mean	5.843333	3.054000	3.758667	1.198667
std	0.828066	0.433594	1.764420	0.763161
min	4.300000	2.000000	1.000000	0.100000
25%	5.100000	2.800000	1.600000	0.300000
50%	5.800000	3.000000	4.350000	1.300000
75%	6.400000	3.300000	5.100000	1.800000
max	7.900000	4.400000	6.900000	2.500000

5. # Data Visualisation

Below I have included visualisations of the data to better understand the differences and correlations between the variables measured:

**Histograms:**

(Note to self, figure out how to add imhgaes to this file)

**Scatterplots**

(Same as above)

From the images, we can note that the “Iris-Setosa” species is noticeably different, especially highlighted in the “Petal Measurement”. There does appear to be a difference between the other two species, but the difference is not as stark as the “Setosa”.

6. # Correlations

Using the Pandas correlation function, we may be able to discern a distinction between the variables measured.

Here we can note:

* It appears that Petal Length and Width have a very strong correlation, as they both become larger together (r = 0.96~).
* The same cannot be said for the Sepal Length and Width which have a very weak correlation (r = -0.1~).
* It appears that there is a strong correlation for the Petal Width and Length in regard to the Sepal Length, which may indicate that they grow larger together (r= 0.81~ and r = 0.87~ respectively).
* I would say there is a weak correlation for Petal Width and Length in regards to Sepal Width (r = -0.35~ and 0.42~).

A good way to visualise this information is through a heatmap:

(Heatmap image)

7. # Conclusions

... Due to finish

8. # References

9. # Further Links:

... Add with conclusion

