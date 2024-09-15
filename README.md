# Data-Analysis-On-MTTQ-Bank-Transfer
# Basic data visualizations 
This is an analysis of the transfers made to support the Northen Vietnam recover from the last typhoon. Tools used in this including python and its basic Data Analysis packages. Pytrends and Selenium was used to scrape Google trends for trending terms.

If you need the csv files for transactions or trending term, please refer to this link: [Link to csv files](https://drive.google.com/drive/folders/17kDjbjckM-YWd0TZlYC37YchBdiz84jl?usp=sharing)

# Text clustering on Bank Transfer notes
This is a visualization of applying text clustering techniques to find the relationships between notes in the bank transfer file. If you want to see the outputs/graphs, please refer to this colab link: https://drive.google.com/file/d/1JzW9LCCYRhHtvhaXvb19ajeAx8ulZv3n/view?usp=sharing . The outputs are too large to upload here

Data preprocess steps including:
1. Remove special characters and number
2. Use the library underthesea to tokenize vietnamese words
3. Convert to text embeddings. In this project, I experimented with 2 types of text embeddings: TFIDF and Dang Van Tuan Vietnamese embeddings
4. Reduce the dimensions to 3 with PCA
5. Visualize the words in 3D space with plotly
6. Pick the approprite n-cluster for K-means
7. Train K-means on TFIDF embeddings and visualize the result
