# Project 9: Conduct a market research study using Python
You work at La poule qui chante (The Singing Hen), a French agri-food company. It wishes to expand internationally; no particular country or continent has been chosen yet. All countries are conceivable.

## Objectives:
Market research for exportation of poultry
1. Propose an initial analysis of country groupings that we can target for exporting our chickens. We will then deepen the market study.
2. Test hierarchical agglomerative clustering, with a dendrogram as a visualization. 
3. Then you can use the k-means method to refine the analysis and compare the results of the two clustering methods. 
4. Don't hesitate to take the time to analyse the centroids of your classes. 
5. You can also perform a PCA (Principal Component Analysis) to visualize the results of your analysis, understand the groups, the links between variables, the links between individuals.

## Data Preprocessing
- Imported 2 csv data files (population 2000-2018 and DisponibilitéAlimentaire 2017).

<img width="1314" alt="a" src="https://github.com/user-attachments/assets/82da49bd-b1b7-490d-a9c0-9eef3755cc3b" />

- Studied the data values, checked the columns and rows for duplicates.
- Filled missing data with zero.
- Merge the 2 csv files.

<img width="1316" alt="aa" src="https://github.com/user-attachments/assets/85cdf90a-0ac3-432a-87b4-4d3796e99088" />

## Exploratory Data Analysis (EDA)
- Looked at the distribution of data.

<img width="1032" alt="aap" src="https://github.com/user-attachments/assets/47a108a5-0217-473b-a8c2-e56db0021ba2" />

- Checked for outliers, normality, correlation coefficient, and caluclated zscores.

<img width="737" alt="aaaap" src="https://github.com/user-attachments/assets/57af2dd1-8423-4bf2-a724-1ab436ce440a" />

<img width="1304" alt="aaaaap" src="https://github.com/user-attachments/assets/27341d8d-50b0-42a2-bf29-5160dc53f4df" />

<img width="889" alt="aaaaaaap" src="https://github.com/user-attachments/assets/25fe8f4e-e6c2-461e-b8b5-562cbd0a1083" />

## Data Analysis
### Propose an initial analysis of country groupings that could be targeted for exporting chickens.
- Test hierarchical agglomerative clustering, with a dendrogram as visualization.
<img width="1090" alt="aaa1" src="https://github.com/user-attachments/assets/56829e66-5018-481a-9d03-0ee48044e390" />

<img width="994" alt="aaa111" src="https://github.com/user-attachments/assets/0615cafd-9150-44a3-9bdf-1b93d08bb256" />

<img width="1312" alt="aac" src="https://github.com/user-attachments/assets/0f906514-05d0-4ecb-a563-897a3d915d28" />

<img width="1228" alt="aaac" src="https://github.com/user-attachments/assets/01586aed-f81b-417e-862e-4d04f76092be" />

- Use the K-Means method to refine the analysis and compare the results of the two clustering methods; analyze the centroids of the clusters.

<img width="767" alt="aaaac" src="https://github.com/user-attachments/assets/05ad848b-1d14-4ef8-9c18-bac5d1fde19d" />

<img width="955" alt="aaaaac" src="https://github.com/user-attachments/assets/558c3ed0-e3f2-4fd4-b92d-48f0b49c9e9c" />

<img width="1312" alt="aaaaaaac" src="https://github.com/user-attachments/assets/0cbf5404-6180-4873-8e65-94f762b57bdd" />

<img width="920" alt="aaaaaac" src="https://github.com/user-attachments/assets/33384611-d2e3-418f-a376-978dd9f6f7ae" />

### Deepen the market study.
- Perform a PCA (Principal Component Analysis) to visualize the analysis results.
  
<img width="785" alt="aaa" src="https://github.com/user-attachments/assets/68fff54a-6d6a-4947-b74f-daab196bf57a" />
<img width="692" alt="aaaa" src="https://github.com/user-attachments/assets/38bd131b-1d2c-4bee-a9e0-ead6e089333e" />

- Understand the groups, the relationships between the variables, and the relationships between the individuals.

<img width="1186" alt="aaaaa" src="https://github.com/user-attachments/assets/d85160f9-33a6-4374-900f-f06eabc7528d" />

<img width="1043" alt="aaaa11" src="https://github.com/user-attachments/assets/d128e629-2c66-4139-aac6-4eeea5be01a9" />

## Insights 
Understanding the links between variables and Principal Component Analysis (PCA):
Understanding the Links Between Variables:
The x-axis represents the first principal component (F1), while the y-axis represents F2. The principal components can be viewed as "new variables" that synthesize existing variables.
Principal Component 1 (F1):
F1 explains a large portion of the total variance in the dataset, approximately 35.3%.
The initial variables such as domestic availability, losses, and population are positively correlated with F1, with domestic availability being the most strongly correlated.
Domestic availability indicates the food availability of 'poultry meat' within the country. This variable is the most strongly correlated with F1 and contributes positively to F1.
Losses represent food waste coming from 'poultry meat'. It is positively correlated with F1.
Population is a set of the habitats of a country. It is positively correlated with F1.
What is interesting in the interpretation of the F1 axis is that all these variables are united by the notion of the availability of 'poultry meat' within a country.
Principal Component 2 (F2):
F2 also explains a significant portion of the total variance in the dataset, roughly 21%.
The initial variables such as import quantity, export quantity, stock variations, and protein availability in quantity ( g/person/day ) are negatively correlated with F2, with the last variable being the most strongly correlated.
Import quantity is the amount of 'poultry meat' imported by a country. This variable is negatively correlated with F2.
Export quantity is the amount of 'poultry meat' exported by a country. It is negatively correlated with F2.
Stock variations measure the difference between domestic availability, production, and imports, adding the exports. This variable is negatively correlated with F2.
Protein availability in quantity ( g/person/day ) measures the protein availability in grams per person per day from 'poultry meat'. It is negatively correlated with F2 and is also the most strongly correlated.
What is interesting in the interpretation of the F2 axis is that all these variables are united by the notion of the quality of 'poultry meat' within a country.
In summarizing variables into new dimensions F1 and F2, sometimes even F3 and F4, the principal components can be viewed as new variables and new columns of our data table.

## Recommendations

# Project 9 in French
## Mission:
1. Proposer une première analyse des groupements de pays que l’on peut cibler pour exporter des poulets :
- Pré-traitement des données (la preparation, le nettoyage et l’analyse exploratoire des données),
- Tester la Classification Ascendante Hiérarchique (CAH), avec un dendrogramme comme visualisation,
- Utiliser la méthode des K-Means, afin d’affiner l’analyse et comparer les résultats des deux méthodes de clustering, analyser les centroïdes des classes.
2. Approfondir l'étude de marché :
- Réaliser une Analyse Composantes Principale (ACP) afin de visualiser les résultats d'analyse,
- Comprendre les groupes, les liens entre les variables, les liens entre les individus.
