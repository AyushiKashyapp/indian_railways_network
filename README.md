# Indian Railways Network

The Indian Railways network is the fourth largest railway network. This project aims to implement the Indian Railways Network as a Knowledge Graph.

The dataset used in this project can be found here: [Indian Railways](https://www.kaggle.com/datasets/sripaadsrinivasan/indian-railways-dataset)

The files train and stations are available in GeoJSON format.

# IndianRailways_Triples.ipynb

In this Python notebook, we process the GeoJSON files and extract information about the stations and trains in the form of triples. In performs broadly in three steps:

- A function designed to load and process a GeoJSON file, filtering out invalid LineString geometries and converting the valid ones into a GeoDataFrame.
- A function designed to construct a directed graph representing the Indian Railways network using the networkx library, and then converts the graph data into RDF-like triples.
- Exporting the triples as an excel file named: train_station_triples.

