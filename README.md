# Project Title

*GmE 205 Laboratory 1 — Spatial Data Inspection*

The main objective of this laboratory activity is to teach students how to create and use a Python script that reads and inspects a CSV dataset containing spatial coordinate data. The script checks the quality of the data, validates longitude and latitude values, calculates the bounding box, saves a summary in JSON format, and generates a scatter plot of the valid coordinate points.


# Objectives

The objectives of this laboratory are to:

- Configure Python in VS Code using a virtual environment.
- Initialize and manage a GitHub repository.
- Practice Git commands such as commit, push, and pull.
- Read and inspect a CSV file using Python and Pandas.
- Check missing and invalid coordinate values.
- Calculate the bounding box of valid coordinates.
- Save data inspection results as a JSON file.
- Generate a scatter plot of valid coordinates.
- Apply computational thinking concepts using abstraction, representation, responsibility, and scale.


# Tools and Technologies

The following tools were used:

- *Python 3.x*
- *Visual Studio Code*
- *Git*
- *GitHub*
- *Pandas*
- *Matplotlib*

# How to set up the virtual environment

1. Open the project folder (gme205-lab1) in VS Code.
2. Open the terminal (Terminal -> New Terminal) and create the virtual environment:
    py -m venv .venv 
    .\.venv\Scripts\activate 
3. Confirm the terminal prompt shows (.venv).
4. Select the interpreter inside .venv via Ctrl + Shift + P -> Python: Select Interpreter.
5. Install the required packages:
    pip install --upgrade pip
    pip install pandas matplotlib
    pip freeze > requirements.txt

## Reflection

# Abstraction

I chose to inspect the basic information, missing values, coordinate validity, and bounding box because these are important for understanding whether the dataset is usable.

# Representation

I assume that the CSV file contains lon and lat columns, that longitude values range from -180 to 180, and latitude values range from -90 to 90.

# Responsibility

The script should automatically check missing values, required columns, invalid coordinates, and generate the summary and visualization, while a human should review whether the data makes sense for its actual purpose.

# Scale
A very large dataset may require more memory and processing time, especially when loading the entire CSV and creating a scatter plot.