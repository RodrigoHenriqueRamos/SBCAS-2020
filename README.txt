To run the code we used in the paper, just open and run the "cancerData_preprocessing.ipynb" with Jupyter Notebook.
All the dependencies are in the first cell.
The images output are commented, the data generate by the code are saved in the same folder of the input.

- About the folders that we used to organize the input
* CancerData:
	The "Data Mutations Extended" is the original file downloaded from CBioPortal.
	The .maf files will be generate after the preprocessing routine.

* CompMethodDriverMutationIdentification
	Each folder stores the result of each Driver Method. Code for theses methods are not available. 

* mapperData
	The three .csv files combine the "Data Mutations Extended" with "Clinical Data" for de BRCA's studys (download from CBioPortal).
	The code used to create these files are not available.
	The "cancerData_preprocessing.ipynb" will output the mapper graph in 3 different ways:
		* edgeListCSV: useful for using with NetworkX and/or Cytoscape
		* gml: store the gene id within each node. A mapper node area a set of genes.
		* html: A visual representation of the graph
