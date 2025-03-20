# RDF-Based Image Classification and Visualization with ConceptNet

## Overview
This project integrates **YOLOv8**, **ConceptNet**, and **Blazegraph RDF store** to classify objects in images and link them to semantic concepts. It allows visualization and querying of RDF data using **SPARQL**.

## Features
- **Object detection** using YOLOv8.
- **Concept linking** with ConceptNet API.
- **RDF generation** and storage in Blazegraph.
- **SPARQL querying** for structured data retrieval.
- **Graph visualization** of RDF relationships.

## Installation

### Prerequisites
Ensure you have the following installed
- **Python 3.8+**
- **pip** (Python package manager)
- **Git**
- **Blazegraph** (RDF database)

### 1: Clone the Repository
```sh
git clone https://github.com/Siloya/SemanticImageClassification-YOLO-RDF-ConceptNet-SPARQL.git
cd SemanticImageClassification-YOLO-RDF-ConceptNet-SPARQL
```
### 2: install Dependencies
```sh
pip install -r requirements.txt
```
### 3: Start Blazegraph
```sh
java -server -Xmx4g -jar blazegraph.jar
```
### 4: Start the Flask Server
```sh
python app.py
```
## Usage

### 1. Upload an Image
- Open [http://127.0.0.1:5000](http://127.0.0.1:5000) in your browser.
- Click **"Choose Image"** and upload an image.
- The system detects objects, links them to **ConceptNet**, and stores **RDF data** in **Blazegraph**.

### 2. Query RDF Data
- Use the **SPARQL Query** section in the web interface.
- Run SPARQL queries to explore **RDF relationships**.

### 3. Visualize RDF Graph
- After processing an image, the **RDF graph visualization** will be displayed automatically.


