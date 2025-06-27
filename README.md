# Scalable-Graph-Based-Data-Processing-Pipeline

This project implements a **Scalable Graph Based Data Processing Pipeline** using the NYC Yellow Taxi Trip dataset. It enables dynamic analysis of urban mobility patterns by streaming taxi trip data, storing it as a graph, and running powerful graph algorithms. Such analytics can help city planners and transportation providers optimize traffic flow, identify hotspots, and improve resource allocation in near real time.

---

## 🚀 Features

- **Graph Database**: Neo4j with Graph Data Science (GDS) plugin  
- **Real-Time Streaming**: Apache Kafka for trip data ingestion  
- **Orchestration**: Kubernetes (via Minikube) with Helm charts  
- **Automated Integration**: Kafka Connect for Neo4j ingestion  
- **Built-in Analytics**: PageRank and BFS algorithms  
- **Python API**: Interface for custom graph queries and testing  

---

## ⚙️ Architecture Overview

### 🔧 Components

- **Neo4j**: Stores trip data as graph structures (locations, trips)  
- **Kafka**: Streams preprocessed trip records  
- **Kafka Connect**: Ingests Kafka topics into Neo4j using Cypher  
- **Kubernetes**: Manages and scales the deployment  
- **Python Interface**: Executes graph algorithms and tests  

### 🔄 Flow

1. Trip data is streamed to Kafka.  
2. Kafka Connect ingests the data into Neo4j as nodes and edges.  
3. Neo4j runs graph algorithms (PageRank, BFS).  
4. Results are queried or analyzed via the Python interface.  

---

## 📈 Results

- Processed millions of taxi trips with near real-time throughput  
- Identified key locations (hubs) using PageRank  
- Computed shortest paths with BFS efficiently  
- Kubernetes ensured zero downtime and easy scaling  

---

## 🎯 Conclusion

The pipeline provides a robust, scalable, and real-time graph analytics system for transportation data. It efficiently combines streaming, graph storage, and analytics technologies to generate actionable insights with minimal latency.

---

## 🔮 Future Work
 
- Add real-time visualization dashboards  
- Integrate external data sources for enriched analysis  
- Implement security features (authentication, encryption)  

---
