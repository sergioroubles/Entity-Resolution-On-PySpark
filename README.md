# Entity-Resolution-On-PySpark

This repository contains an integral development of an Entity Resolution algorithm on PySpark. It is organised as follows:

- The jupyter-notebook **Pivote.ipynb** contains the main `code` of the algorithm, along with some displayed results and explainations.
> WARNING: Original Data base and sensible displays have been removed from the project, as it contained a real set of names and personal information about the patients. This code is only for displaying purposes.
- The directory ***/articulos*** contains a certain amount of literature articles on which this project is based. Check for more information.
- The directory ***/codigos*** contains 3 jupyter-notebooks, each of them exploring different aspects of the project
- The directory ***/errores*** contains simple information about the amount and form of the duplicates found on the database.
- The directory ***/resources*** contains a set of media resources used to explain the results of the project.

## Entity Resolution 
To see more about the Entity Resolution problem, check the following [link](https://www.sciencedirect.com/topics/computer-science/entity-resolution "link").

## The algorithm
# Core idea

![plot](/resources/dia_pivote_final1.png)

# Explanation

1. This is an example on the original data base:

![plot](/resources/pivote1_listainicial.png)

The goal is to resolve the maximum number of duplicates, avoiding the quadratic cost of comparing the whole data base, and making the algorithm scalable at the same time. To do that, we use the method of *Pivote* or Pivoting, (check [a relative link](./Pivote.ipynb), which prioritises some fields over others in a sequential way. 


2. This is an example on the pivoting method approach. It groups entities based on one preferred feel. As you can see in the image, it will suceeed at comparing every pair of matching entities, except for the ones that differ in the column you are pivoting over. Therefore, it will have to be applied twice to cover por all duplicates.

![plot](/resources/pivote2_bloques.png)

3. The results of applying a two-fold pivoting on two different fields from the database are as follows:

![plot](/resources/tabladoble.png)

4. These is a graphic representation that shows the importance of chosing the right approach:

![plot](/resources/comparaciones.png)





