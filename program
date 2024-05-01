import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Load the real estate dataset
data = pd.read_csv('"D://Sentamil/real_estate_data.csv")

# Display the first few rows of the dataset to understand its structure
print(data.head())

# Scatter plot to visualize property prices
plt.figure(figsize=(10, 6))
sns.scatterplot(x='SquareFeet', y='Price', data=data)
plt.title('Scatter Plot of Property Prices')
plt.xlabel('Square Feet')
plt.ylabel('Price')
plt.show()

# Box plot to visualize property prices by property type
plt.figure(figsize=(10, 6))
sns.boxplot(x='PropertyType', y='Price', data=data)
plt.title('Box Plot of Property Prices by Property Type')
plt.xlabel('Property Type')
plt.ylabel('Price')
plt.show()

# Heatmap to visualize property prices by geographic location
plt.figure(figsize=(10, 6))
sns.heatmap(data.pivot_table(index='Latitude', columns='Longitude', values='Price'), cmap='YlGnBu')
plt.title('Heatmap of Property Prices by Geographic Location')
plt.xlabel('Longitude')
plt.ylabel('Latitude')
plt.show()

# Count plot for distribution of property types
plt.figure(figsize=(8, 8))
sns.set(style="whitegrid")
sns.countplot(x='PropertyType', data=data, palette='pastel')
plt.title('Distribution of Property Types')
plt.xlabel('Property Type')
plt.ylabel('Count')
plt.show()

# Bar chart for average property prices by property type
plt.figure(figsize=(10, 6))
sns.barplot(x='PropertyType', y='Price', data=data, palette='pastel', estimator=pd.np.mean)
plt.title('Average Property Prices by Property Type')
plt.xlabel('Property Type')
plt.ylabel('Average Price')
plt.xticks(rotation=45)
plt.show()

# Line chart for housing market trends over the years
plt.figure(figsize=(10, 6))
sns.lineplot(x='YearBuilt', y='Price', data=data, estimator=pd.np.mean, color='green')
plt.title('Housing Market Trends Over the Years')
plt.xlabel('Year Built')
plt.ylabel('Average Price')
plt.grid(True)
plt.show()
