# Relational databases for handling vector data

##### Motivation: 

Nearly all geospatial problems involve manipulation of vector data. Vector data include anything that can be represented by sets of coordinate pairs. The simplest form of vector data is a single point. A line is a colletion of points linked together, and a polygon is a collection of points that connects back to the first point. Point, line and polygon data are different types of geospatial _features_.

The structure of these vector data is inherently well represented in tabular format:

|  feature type | coordinates  | 
| --- | --- | 
| point | (x<sub>1</sub>,y<sub>1</sub>)  |
| line | (x<sub>1</sub>,y<sub>1</sub>), (x<sub>2</sub>,y<sub>2</sub>), (x<sub>3</sub>,y<sub>3</sub>)  |
| polygon | (x<sub>1</sub>,y<sub>1</sub>), (x<sub>2</sub>,y<sub>2</sub>),(x<sub>3</sub>,y<sub>3</sub>), (x<sub>1</sub>,y<sub>1</sub>) | 


### Lesson content:

* dataAccess.md: instructions for how to connect to the ice2oceans cloud database for example datasets 