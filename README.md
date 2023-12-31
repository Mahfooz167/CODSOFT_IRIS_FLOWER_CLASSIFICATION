# Iris Flower Species Classification
![](https://hub.packtpub.com/wp-content/uploads/2018/03/iStock-475486224-696x490.jpg)  ![](https://storage.googleapis.com/kaggle-datasets-images/681981/1197252/1b0b365670f0fbbe87def6645e0e7cd2/dataset-card.jpg?t=2020-05-29-13-18-35) 
 
## Author: Md Mahfooz Alam Ansari
## Batch: September
## Domain: Data Science

### Aim

The aim of this project is to develop a model that can classify iris flowers into different species based on their sepal and petal measurements.

### Libraries Used

The following important libraries were used for this project:

- `numpy`
- `pandas`
- `sklearn.cluster.KMeans`
- `matplotlib.pyplot`
- `seaborn`

### Dataset

The iris dataset was loaded using seaborn's `load_dataset` function, which contains information about iris flowers, including sepal length, sepal width, petal length, petal width, and species.

### Data Exploration and Preprocessing

- The dataset was loaded using seaborn's `load_dataset` function as a DataFrame, and its first 5 rows were displayed using `df.head()`.

- The 'species' column in the DataFrame was encoded to numerical values using `pd.factorize(df['species'])`.

- Descriptive statistics for the dataset were displayed using `df.describe()`.

- Missing values in the dataset were checked using `df.isna().sum()`.

### Data Visualization

- 3D scatter plots were created to visualize the relationship between species, petal length, and petal width, as well as between species, sepal length, and sepal width using `matplotlib.pyplot` and `mpl_toolkits.mplot3d.Axes3D`.

- 2D scatter plots were created to visualize the relationship between species and sepal length, as well as between species and sepal width using `seaborn.scatterplot`.

### Applying Elbow Technique for K-Means Clustering

- The Elbow Technique was applied to determine the optimal number of clusters (K) using the sum of squared errors (SSE).

- The `KMeans` algorithm was initialized with different values of K (1 to 10), and SSE was computed for each K value.

- A plot of K values against SSE was created using `matplotlib.pyplot` to identify the "elbow point," which indicates the optimal number of clusters.

### Applying K-Means Algorithm

- The `KMeans` algorithm was applied to the dataset with the optimal number of clusters (K=3) obtained from the Elbow Technique.

- The cluster labels were predicted for each data point in the dataset using `km.fit_predict(df[['petal_length','petal_width']])`.

### Accuracy Measure

- The confusion matrix was calculated to evaluate the accuracy of the K-Means clustering.

- The confusion matrix was plotted using `matplotlib.pyplot.imshow` and `plt.text` to visualize the true and predicted labels.

For further details and code implementation, please refer to the project files and code documentation.

### Contact

If you have any questions or need further assistance, feel free to contact the author, Md Mahfooz Alam Ansari.

Thank you for using the Iris Flower Species Classification model!
