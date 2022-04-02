# Entity-Resolution-On-PySpark

This repository contains an integral development of an Entity Resolution algorithm on PySpark. It is organised as follows:

- The jupyter-notebook **Pivote.ipynb** contains the main `code` of the algorithm, along with some displayed results and explainations.
> WARNING: Original Data base and sensible displays have been removed from the project, as it contained a real set of names and personal information about the patients. This code is only for displaying purposes.
- The directory ***/articulos*** contains a certain amount of literature articles on which this project is based. Check for more information.
- The directory ***/codigos*** contains 3 jupyter-notebooks, each of them exploring different aspects of the project
- The directory ***/errores*** contains simple information about the amount and form of the duplicates found on the database.
- The directory ***/resources*** contains a set of media resources used to explain the results of the project.

## Entity Resolution 
>The problem of duplicate detection in **large databases** is a vital process that appears in diverse and both academical and industry enviroments, its formal study being known as Entity Resolution. All throughout this project, framed in a research in collaboration with the Oftalmology department of the Hospital Clínico de Madrid, we will tackle the problem that involves the presence of numberous duplicates in a pacient database. To this aim, the problem will be thouroughly discussed, the theoretical underlying mathematical theory will be developped, and a particular solution to the problem will be presented and studied with the help of Spark. The analysis of the results will yield to several conclusions concerning the **optimal strategies to face the duplicate detection problem in structured databases in a scalable approach.**

This is an example on the original data base:
![plot](/resources/pivote1_listainicial.png)

This is an example on what we want to achieve:
![plot](/resources/pivote2_bloques.png)

The goal is to resolve the maximum number of duplicates, avoiding the quadratic cost of comparing the whole data base, and making the algorithm scalable at the same time.

To see more about the Entity Resolution problem, check the following [link](https://www.sciencedirect.com/topics/computer-science/entity-resolution "link").

