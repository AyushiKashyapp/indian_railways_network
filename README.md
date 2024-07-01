# Indian Railways Network

The Indian Railways network is the fourth largest railway network. This project aims to implement the Indian Railways Network as a Knowledge Graph.

The dataset used in this project can be found here: [Indian Railways](https://www.kaggle.com/datasets/sripaadsrinivasan/indian-railways-dataset)

Find teh project question bank here [QuestionBank](https://github.com/AyushiKashyapp/indian_railways_network/blob/main/QuestionBank.md)

The files train and stations are available in GeoJSON format.

# IndianRailways_Triples.ipynb

In this Python notebook, we process the GeoJSON files and extract information about the stations and trains in the form of triples. In performs broadly in three steps:

- A function designed to load and process a GeoJSON file, filtering out invalid LineString geometries and converting the valid ones into a GeoDataFrame.
- A function designed to construct a directed graph representing the Indian Railways network using the networkx library, and then converts the graph data into RDF-like triples.
- Exporting the triples as an excel file named: train_station_triples.

# Neo4jGraphCreation.ipynb

Generating a Neo4j Knowledge Graph using the extracted triples. A knowledge graph created using the triples extracted in the previous parts of the project, sources from the trains and stations JSON files later converted to triples and extracted as an excel file.

# File VisualiseKG.ipynb

Visualising Knowledge Graph using pyvis.network by reading the triples extracted in previous steps of the project.

The graph is later exported as an HTML file named: "indian_railways.html"

# Graph Snippet

![WhatsApp Image 2024-06-28 at 00 58 13_2ddf627d](https://github.com/AyushiKashyapp/indian_railways_network/assets/147310638/3884529b-ba45-433c-9d24-f0893e966027)
