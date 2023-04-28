# crossref_funder_data_utility

## Structure
There are two files to be aware of when running the code. First is the .ipnyb jupyter notebook file. This is the file that contains the python code. It is also where the code will be run and the statistics results displayed. The second file to keep in mind in the config file. This is where users can enter their target dataset without modifying the code itself.

## Setup
Follow these steps to set up the code

1. Install required libraries in your jupyter notebook environment. This includes:
  - Response
  - Rispy
  - Bibtexparser
  - Pandas
  - Neo4j
  - Numpy
These libraries can be installed using pip install or conda install.
2. Ensure config file and ipnyb file are in the same folder.
3. Find path to dataset and enter this into the config file. This is in the form C:... for Windows machines. If your dataset is in the same folder as your code, the path can be omitted and just the name of the file can be used. Also ensure the dataset conforms to these requirements:
 - has "title", "doi", "author" and "date" columns, case sensitive.
 - is in .csv, .ris or .bib format.
4. Enter the encoding of the file.
5. Enter Neo4j database information. Leave blank to omit the visualization

Note on Neo4j: If you would like to learn how to set up a Neo4j database for viewing visualizations, access this link: https://neo4j.com/docs/getting-started/ 

## Running the code

1. Open ipnyb file in jupyter notebook.
2. Navigate to run and select run all.

This will execute the code in its entirity. Note that the Neo4j portion will be skipped if details have not been entered. Statistical results can be viewed in the notebook itself by scrolling down. A csv file with the funding data will also be generated in the same folder the code is in. Some sample data has been provided in the "Data" folder to allow you to test the code.

Data Sources:
- Clarke, Caitlin; Lischwe Mueller, Natalie; Joshi, Manasi Ballal; Fu, Yuanxi; Schneider, Jodi (2022): The Inclusion Network of 27 Review Articles Published between 2013-2018 Investigating the Relationship Between Physical Activity and Depressive Symptoms. University of Illinois at Urbana-Champaign. https://doi.org/10.13012/B2IDB-4614455_V2 
- Fu, Yuanxi; Hsiao, Tzu-Kun; Joshi, Manasi Ballal (2022): The Salt Controversy Systematic Review Reports and Primary Study Reports Network Dataset . University of Illinois at Urbana-Champaign. https://doi.org/10.13012/B2IDB-6128763_V2 

  
Code references:
  - Python file write. (n.d.). Retrieved April 7, 2023, from https://www.w3schools.com/python/python_file_write.asp 
  - pandas.DataFrame.to_csv - pandas 2.0.0 documentation. (n.d.). Retrieved April 7, 2023, from https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.to_csv.html 
  - Swagger UI. (n.d.). Retrieved April 7, 2023, from https://api.crossref.org/swagger-ui/index.html 
