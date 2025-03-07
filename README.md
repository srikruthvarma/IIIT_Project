
# Atlas Game Graph Analysis

This project focuses on analyzing a graph created from country names and cities, following the Atlas game rules. The graph is analyzed based on centrality, density, diameter, and communities detected using different algorithms.

## Steps in the Notebook

### 1. Install Required Libraries
Install the required libraries for network analysis and visualization:
```bash
!pip install networkx matplotlib requests scipy
```

### 2. Import Libraries
The necessary Python libraries, such as `networkx` for graph analysis, `requests` for fetching data, and `matplotlib` for visualization, are imported.

### 3. Fetch Country Names
We use the REST API from `https://restcountries.com` to fetch country names, and they are combined with a list of pre-defined major cities.

### 4. Create the Graph
The project creates a directed graph based on the Atlas game rules, where a country or city's last letter connects to the next place's first letter.

### 5. Visualize the Graph
The graph is visualized using NetworkX and Matplotlib, making it easier to interpret the relationships between different countries and cities.

### 6. Graph Analysis
We perform various graph analysis tasks, including:
- **Degree Centrality**: Measures the importance of nodes based on their connections.
- **Graph Density**: Measures how close the graph is to being complete.
- **Graph Diameter**: The longest shortest path in a graph.

### 7. Community Detection
We detect communities in the graph using:
- **Girvan-Newman Algorithm**: Detects communities by removing high-betweenness edges.
- **Label Propagation Algorithm**: A heuristic algorithm to find communities in an undirected graph.

### 8. Modularity Calculation
Modularity is calculated to evaluate the quality of the communities detected in the graph.

### 9. Graph Analysis Tasks
Analysis of individual graphs for countries and cities is performed using various centrality and community detection measures.

## Usage
1. Clone the repository and run the notebook in a Jupyter environment.
2. Install the required libraries as mentioned in step 1.
3. Follow the steps in the notebook to fetch data, build the graph, and analyze it.

## Requirements
- Python 3.x
- Jupyter Notebook
- NetworkX
- Matplotlib
- Requests

## Author
Developed as part of the Atlas Graph Analysis project.
