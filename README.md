# Parsing Raw Text Files

This program extracts data from semi structured html file. The html file consists of data from the Monash unit handbook.
Each unit has the following data:
* Unit code
* Pre-requisite units for the unit
* Prohibitions (The units which can not be taken in order to study the unit)
* Synopsis of the unit
* Requirements for the unit
* Outcomes of the unit
* Chief Examiners which will be examining the unit.

The RE library was used to extract all the reqiured elements from the html file.
The extracted elements are then printed inside the appropriate xml and json tags.

The json library is then used to format and indent the json file appropriately.

* The raw data is in html format. So, the data which we need is enclosed between some tags. To extract this data we have used Regular Expressions.
* The initial regex finds the entire block of data we need and the secondary regex filters out the unwanted tags, leaving us with only the clean data.


# Text PreProcessing 

* Main motive of this task is to convert extracted data into formatted data. The textual information or data is converted into its numerical representation.
* The dataset consists of information of units offered at Monash University.
* The data provided per unit includes:
1.Unit Code
2.Synopsis
3.Outcomes
* The task is to extract the information about each unit and generate a vector-space model.
