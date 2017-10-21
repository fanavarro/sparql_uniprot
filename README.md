# sparql_uniprot
Python application to retrieve information from uniprot through its sparql endpoint interface. It includes a galaxy wrapper.

## Usage
The python script receives all the arguments in the following order:
```
proteinId
proteinName
geneName
organismName
diseaseAnnotation
domainName
similarityAnnotation
locationAnnotation
functionAnnotation
pharmaceuticalAnnotation
outputFile
```
All params must be provided. If you want to leave a param in blank, an empty string ("") must be specified for the param. For example, to look for protein names whose name includes "insulin" in humans and store the results in the file "output.txt":
```
python sparql_uniprot.py "" "insulin" "" "homo sapiens" "" "" "" "" "" "" "output.txt"
```

## More info
This was a project for the Master Degree in Bioinformatics at the University of Murcia (Spain). The documentation of the project was writen in latex and all the files (including the pdf) are under "report" folder. It includes information about the script and how we implemented the galaxy wrapper.
