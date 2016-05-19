# Relational databases for handling vector data

##### Motivation: 

Nearly all geospatial problems involve manipulation of vector data. Vector data include anything that can be represented by sets of coordinate pairs:

The simplest form of vector data is a single point:
(x<sub>1</sub>,y<sub>1</sub>, <data>)

A line is a colletion of points linked together:

(x<sub>1</sub>,y<sub>1</sub>, <data>)
(x<sub>2</sub>,y<sub>2</sub>, <data>)
(x<sub>3</sub>,y<sub>3</sub>, <data>)

And a polygon is a collection of points that connects back to the first point, forming a closed feature:

(x<sub>1</sub>,y<sub>1</sub>, <data>)
(x<sub>2</sub>,y<sub>2</sub>, <data>)
(x<sub>3</sub>,y<sub>3</sub>, <data>)
(x<sub>1</sub>,y<sub>1</sub>, <data>)

| x | y | z | 
| --- | --- | ---|
1 | 2 | 3 


The structure of vector data is inherently well represented in tabular format:


 
### Lesson content:

* dataAccess.md: instructions for how to connect to the ice2oceans cloud database for example datasets 