# crossref_funder_data_utility

How to use:
- Edit the config file to enter the target file
- Include full file path if file is not in the same folder
- Make sure backslashes are used in the full path
- Inlcude the encoding of the file
- If you do not want a visualization, leave the neo4j parameters blank in the config file
- Fill out neo4j database link and key. Results can then be seen in the database
- Once configured, open the jupyter notebook file and ensure all dependencies are setup
- To run navigate to "cell", and then "run all"
- Statistics results are in the notebook
- Output csv is in the funders.csv file

Note:
- Please ensure encoding is accurate
- Only use .bib, .ris or .csv files
- Ensure the following columns are present in the input. Case Sensitive:
  - title
  - author
  - date
  - doi
  
Code references:
  - Python file write. (n.d.). Retrieved April 7, 2023, from https://www.w3schools.com/python/python_file_write.asp 
  - pandas.DataFrame.to_csv - pandas 2.0.0 documentation. (n.d.). Retrieved April 7, 2023, from https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.to_csv.html 
  - Swagger UI. (n.d.). Retrieved April 7, 2023, from https://api.crossref.org/swagger-ui/index.html 
