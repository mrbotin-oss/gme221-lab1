# GmE 221 – Laboratory Exercise 1

## Overview
This laboratory sets up a spatial analysis environment using Python and PostGIS 
and performs a parcel–landuse overlay analysis.

## Environment Setup
- Python 3.x
- PostgreSQL with PostGIS
- GeoPandas, SQLAlchemy, psycopg2

## How to Run
1. Activate the virtual environment
2. Run `main.py` to test the database connection
3. Run `overlay.py` to compute landuse percentages

## Outputs
- PostGIS table: `parcel_landuse_percentage`
- Visualization in QGIS

## Reflection - Database Connection Milestone
- Finishing this part of our Laboratory Exercise, this connection allow Python to act as an interface between GIS algorithms that we did in PostGIS. 
- The main.py translate spatial intent into computational executions.

## Reflection - Overlay Analysis Milestone
- After checking the given code and running the script, the result gives us a new table of our created script which is to compute landuse percentage.

## Reflection - Interpreting Algorithm Output
- Analysing the given result, landuse percentages make sense given the parcel shape. The value of the parcels depends on the covered percentage of landuse that is why some have high or low values. 
- If we don't consider the  other factors like CRS, geomtery quality, and scale then our interpretation of our result can be misleading or incorrect, because spatial relationships such as distances and area of our study and its topology may be distorted or inaccurately represented. 