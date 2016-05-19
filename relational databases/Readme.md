# Relational databases for handling vector data

##### Motivation: 

Nearly all geospatial problems involve manipulation of vector data. Vector data include anything that can be represented by sets of coordinate pairs. The simplest form of vector data is a single point:
(x<sub>1</sub>,y<sub>1</sub>)

A line is a colletion of points linked together:

(x<sub>1</sub>,y<sub>1</sub>)
(x<sub>2</sub>,y<sub>2</sub>)
(x<sub>3</sub>,y<sub>3</sub>)

And a polygon is a collection of points that connects back to the first point, forming a closed feature:

(x<sub>1</sub>,y<sub>1</sub>)
(x<sub>2</sub>,y<sub>2</sub>)
(x<sub>3</sub>,y<sub>3</sub>)
(x<sub>1</sub>,y<sub>1</sub>)

Point, line and polygon data are different types of geospatial _features_.

The structure of vector data is inherently well represented in tabular format, especially when we start attaching some additional information to the features:

|  feature type | coordinates | attributes | 
| --- | --- | ---|
| point | (x<sub>1</sub>,y<sub>1</sub>) | location |
| line | (x<sub>1</sub>,y<sub>1</sub>), (x<sub>2</sub>,y<sub>2</sub>), (x<sub>3</sub>,y<sub>3</sub>) | river |
| polygon | (x<sub>1</sub>,y<sub>1</sub>), (x<sub>2</sub>,y<sub>2</sub>),(x<sub>3</sub>,y<sub>3</sub>), (x<sub>1</sub>,y<sub>1</sub>) | glacier| 

### Lesson content:

* dataAccess.md: instructions for how to connect to the ice2oceans cloud database for example datasets 