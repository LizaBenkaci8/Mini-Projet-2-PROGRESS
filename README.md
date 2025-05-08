# PROGRES 2024 - Mini-Projet 2: Movie and Actor Data API

## Description

This project allows users to interact with movie and actor data from the Internet Movie Database (IMDB) through a Python web API and a user-friendly interface. It utilizes the Bottle framework to provide a RESTful API and a simple web interface to search for movies and actors, calculate collaboration distances between actors, and more.

## Features

- Retrieve a list of movies and actors.
- Search for specific movies or actors by name.
- Retrieve detailed information about movies and actors.
- Calculate collaboration distances between actors who have worked together in movies.
- Interactive web interface for easy search and navigation.

## Technologies Used

- Python
- Bottle (web framework)
- IMDB datasets
- Requests
- GZip (for handling compressed datasets)
- JSON (for data interchange)

## Setup
## Download the IMDB Datasets

To get started, download the following datasets from IMDB:

- [title.principals.tsv.gz](https://datasets.imdbws.com/title.principals.tsv.gz)
- [name.basics.tsv.gz](https://datasets.imdbws.com/name.basics.tsv.gz)
- [title.basics.tsv.gz](https://datasets.imdbws.com/title.basics.tsv.gz)
## Running the Application

    ### Start the API Server:

    To start the API server, run the following command:
```bash
python runn.py

The API will be available at http://localhost:8080.

    ### Start the Web Interface:

To start the web interface, run:
```bash
python runn2.py

    The web interface will be available at http://localhost:8081.
## API Endpoints

    GET /movies/{id}: Retrieve a movie by its ID.

    GET /movies: Retrieve a list of movies with optional pagination and sorting.

    GET /actors/{id}: Retrieve an actor by their ID.

    GET /actors: Retrieve a list of actors with optional pagination and sorting.

    GET /actors/{id}/costars: Retrieve a list of co-actors who worked in the same movies.

    GET /search/actors/{searchString}: Search for actors by name substring.

    GET /search/movies/{searchString}: Search for movies by title substring with optional filtering.

### Prerequisites

Before running the project, ensure you have Python installed on your system. You will also need to install the following libraries:

```bash
pip install bottle requests pytest
